# Tratamiento de Datos — Transparencia

> Este documento detalla las prácticas de CiberShield respecto al manejo de datos recopilados a través de ShieldScan, en cumplimiento con la Ley 25.326 de Protección de Datos Personales.

## 1. Qué datos recopilamos

| Dato | Tipo | Obligatorio | Almacenamiento |
|------|------|:-----------:|----------------|
| Nombre de empresa | Identificatorio | No | Texto plano en JSON |
| Sector de actividad | Demográfico | No | Texto plano en JSON |
| Cantidad de empleados | Demográfico | No | Texto plano en JSON |
| Provincia | Geográfico | No | Texto plano en JSON |
| 24 respuestas del cuestionario | Assessment | Sí (para generar score) | Valores: yes/partial/no |
| Score calculado (0–100) | Resultado | Generado automáticamente | Número entero |
| Nivel de madurez | Resultado | Generado automáticamente | Texto (4 niveles) |
| Scores por dominio (6) | Resultado | Generado automáticamente | Números enteros |
| Dominios débiles | Resultado | Generado automáticamente | Lista de nombres |
| IP del visitante | Técnico | Automático | **Hasheada con SHA-256** (no se almacena la IP real) |
| User Agent | Técnico | Automático | Texto (truncado a 200 caracteres) |
| Timestamp | Técnico | Automático | Fecha y hora ISO 8601 |
| Consentimiento | Legal | Sí | Accepted: true/false + timestamp + versión |

### Lo que NO recopilamos
- Nombres de personas individuales
- Emails personales (solo si se opta por recibir resultados)
- Datos financieros, de salud o sensibles (Art. 8 Ley 25.326)
- Contraseñas o credenciales
- Acceso a sistemas del respondente
- Cookies de tracking de terceros

## 2. Quién accede a los datos

| Rol | Persona | Acceso | Método |
|-----|---------|--------|--------|
| Administrador único | Emanuel Pereyra (Fundador) | Total | Panel privado con autenticación (cs-admin/) |
| Motor de IA | Anthropic Claude (API) | Solo datos agregados | Recibe: empresa, sector, score, dominios débiles. **No recibe respuestas individuales ni IP** |

Ningún otro empleado, socio, proveedor o tercero tiene acceso a los datos individuales de los assessments.

## 3. Para qué se usan los datos

| Finalidad | Descripción | Base Legal |
|-----------|-------------|-----------|
| **Generar el diagnóstico** | Calcular scores, nivel de madurez y recomendaciones | Consentimiento (Art. 5) |
| **Análisis con IA** | Producir el análisis ejecutivo personalizado | Consentimiento (Art. 5) |
| **Contacto posterior** | Ofrecer servicios de consultoría basados en los resultados | Consentimiento (Art. 5) |
| **Envío de resultados** | Enviar el informe por email si el usuario lo solicita | Consentimiento explícito |
| **Mejora del servicio** | Optimizar las preguntas, pesos y recomendaciones del assessment | Interés legítimo |

## 4. Agregación anónima para estadísticas

Los datos de todos los assessments se agregan de forma **anónima** (sin identificar empresas individuales) para:

- Construir **estadísticas sectoriales** de madurez en ciberseguridad PyME en Argentina
- Generar **informes regionales** por provincia sobre el estado de seguridad
- Identificar **tendencias nacionales** en dominios débiles (ej: "el 73% de las PyMEs no tiene MFA")
- Producir **contenido educativo** basado en datos reales del mercado argentino

### Cómo se anonimiza

| Dato original | Dato agregado | Ejemplo |
|---------------|---------------|---------|
| "Distribuidora López" | No se incluye | — |
| Sector: "Agro" | Conteo por sector | "35% de assessments son del sector Agro" |
| Provincia: "Santa Fe" | Conteo por provincia | "Score promedio en Santa Fe: 42/100" |
| Score: 38 | Promedio/distribución | "Score promedio nacional: 47/100" |
| Dominio débil: "Control de Accesos" | Frecuencia | "68% tiene debilidades en Control de Accesos" |

**Ninguna empresa individual puede ser identificada a partir de los datos agregados.**

## Retención y eliminación

| Tipo de dato | Período de retención | Método de eliminación |
|-------------|---------------------|----------------------|
| Datos individuales del assessment | 12 meses | Eliminación segura del archivo JSON |
| Datos agregados/estadísticos | Indefinido (anónimos) | No aplica — no son datos personales |
| Logs de seguridad | 30 días | Rotación automática |

## Derechos del titular (ARCO)

Conforme a los Artículos 14 y 16 de la Ley 25.326:

| Derecho | Plazo | Cómo ejercerlo |
|---------|-------|----------------|
| **Acceso** | 10 días hábiles | Email a contacto@cibershield.io con asunto "Derecho de Acceso" |
| **Rectificación** | 5 días hábiles | Email con datos a corregir |
| **Cancelación** | 5 días hábiles | Email solicitando eliminación |
| **Oposición** | 5 días hábiles | Email con motivo de oposición |

## Responsable

| Campo | Dato |
|-------|------|
| Responsable | Emanuel Pereyra |
| CUIT | 20-33120188-0 |
| Registro AAIP | RL-2026-25503147-APN-DNPDP#AAIP |
| Domicilio | Libertad 750, Arroyo Seco, Santa Fe, Argentina |
| Email | contacto@cibershield.io |
| Organismo de control | [AAIP — Agencia de Acceso a la Información Pública](https://www.argentina.gob.ar/aaip) |

---

> Última actualización: Marzo 2026 · Versión 1.0
