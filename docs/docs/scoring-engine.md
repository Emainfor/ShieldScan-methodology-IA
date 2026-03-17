# Motor de Scoring — Documentación Técnica

## Modelo de Evaluación

ShieldScan utiliza un modelo de **scoring ponderado por criticidad** donde cada pregunta tiene un peso (1–3) que refleja su impacto real en la seguridad operativa de una PyME.

### Fórmula de Cálculo

#### Score por Dominio

```
Score_Dominio = REDONDEAR( SUMA(Valor_respuesta × Peso) / SUMA(Pesos) × 100 )
```

**Valores de respuesta:**
| Respuesta | Valor | Interpretación |
|-----------|:-----:|----------------|
| Sí | 1.0 | Control implementado y funcionando |
| Parcial | 0.5 | Control existe pero incompleto o inconsistente |
| No | 0.0 | Control ausente o no funcional |

#### Score Global

```
Score_Global = REDONDEAR( (ACC + BKP + RED + PAR + DAT + PER) / 6 )
```

Media aritmética de los 6 dominios. No se aplica ponderación adicional entre dominios — cada uno tiene el mismo peso en el score global.

### Distribución de Pesos por Dominio

| Dominio | Preguntas | Peso Máximo | % del Score Ideal |
|---------|:---------:|:-----------:|:-----------------:|
| Control de Accesos | 4 | 9 | 18.4% |
| Copias de Seguridad | 4 | 10 | 20.4% |
| Seguridad de Red | 4 | 7 | 14.3% |
| Actualizaciones | 4 | 8 | 16.3% |
| Protección de Datos | 4 | 9 | 18.4% |
| Concientización | 4 | 6 | 12.2% |
| **Total** | **24** | **49** | **100%** |

### Justificación de Pesos Críticos (Peso 3)

| ID | Pregunta | Por qué peso 3 |
|----|----------|----------------|
| a2 | MFA activo | El 80% de las brechas involucran credenciales comprometidas. MFA es la defensa más efectiva con menor costo |
| b1 | Backups automáticos | Sin backups, un ransomware puede destruir toda la información del negocio irreversiblemente |
| b2 | Backups externos | Backups locales se encriptan junto con el resto. Solo los externos sobreviven un ataque |
| p2 | Antivirus/EDR | Primera línea de defensa contra malware. Sin esto, cualquier amenaza entra sin resistencia |
| d1 | Mapeo de datos | No podés proteger lo que no sabés que tenés. Es el requisito base de la Ley 25.326 |

### Escala de Madurez

| Score | Nivel | Clasificación | Indicador de Riesgo |
|:-----:|-------|---------------|---------------------|
| 0–30 | **INICIAL** | Controles mínimos o inexistentes | El 60% de las PyMEs en este nivel que sufren un incidente cierran en 6 meses |
| 31–55 | **EN DESARROLLO** | Controles básicos sin consistencia | Vulnerabilidades conocidas sin mitigar. Un atacante con herramientas básicas puede comprometer |
| 56–75 | **GESTIONADO** | Controles implementados, mejorables | Postura defendible pero sin formalización. Riesgo de regresión sin procesos documentados |
| 76–100 | **OPTIMIZADO** | Postura sólida para contexto PyME | Riesgo residual bajo. Foco en mejora continua y adaptación a nuevas amenazas |

---

## Ejemplo de Cálculo

**Empresa:** Acopio San Martín — Agro — 25 empleados — Santa Fe

**Dominio: Control de Accesos (peso máximo: 9)**

| Pregunta | Respuesta | Valor | Peso | Valor × Peso |
|----------|-----------|:-----:|:----:|:------------:|
| a1 - Contraseñas únicas | Parcial | 0.5 | 2 | 1.0 |
| a2 - MFA activo | No | 0.0 | 3 | 0.0 |
| a3 - Revocación de accesos | No | 0.0 | 2 | 0.0 |
| a4 - Mínimo privilegio | Parcial | 0.5 | 2 | 1.0 |
| | | | **SUMA: 9** | **SUMA: 2.0** |

```
Score_ACC = REDONDEAR( 2.0 / 9 × 100 ) = 22
```

> Score 22 en Control de Accesos = **Nivel Inicial** en este dominio.
