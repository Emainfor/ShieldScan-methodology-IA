<p align="center">
  <p align="center">
 <img src="https://github.com/user-attachments/assets/21eb807a-306d-4eb5-906b-8ef54d8f5d48" alt="CiberShield" width="700"/>

<h1 align="center">ShieldScan</h1>
<h3 align="center">Motor de Diagnóstico de Ciberseguridad con IA para PyMEs Argentinas</h3>

<p align="center">
  <a href="https://cibershield.io"><img src="https://img.shields.io/badge/Web-cibershield.io-00aaff?style=flat-square&logo=google-chrome&logoColor=white" alt="Website"/></a>
  <img src="https://img.shields.io/badge/NIST_CSF-2.0-0066cc?style=flat-square" alt="NIST CSF 2.0"/>
  <img src="https://img.shields.io/badge/ISO-27001:2022-0066cc?style=flat-square" alt="ISO 27001"/>
  <img src="https://img.shields.io/badge/COBIT-2019-0066cc?style=flat-square" alt="COBIT 2019"/>
  <img src="https://img.shields.io/badge/Ley-25.326-D4AF37?style=flat-square" alt="Ley 25.326"/>
  <img src="https://img.shields.io/badge/Security_Headers-A-10b981?style=flat-square" alt="Security Headers A"/>
  <img src="https://img.shields.io/badge/Trackers-0-10b981?style=flat-square" alt="Zero Trackers"/>
  <img src="https://img.shields.io/badge/AAIP-Registrado-D4AF37?style=flat-square" alt="AAIP Registrado"/>
</p>

<p align="center">
  <b>24 preguntas · 6 dominios · Score 0–100 · Análisis ejecutivo con IA</b><br/>
  <sub>Gratuito · Sin registro · 5 minutos · <a href="https://cibershield.io/#assessment">Hacé el diagnóstico →</a></sub>
</p>

---

## Qué es ShieldScan

ShieldScan es el motor de assessment automatizado de **CiberShield**, diseñado para evaluar la madurez de ciberseguridad de pequeñas y medianas empresas argentinas.

Combina un cuestionario de autoevaluación ponderado con análisis ejecutivo generado por inteligencia artificial, calibrado por **sector**, **tamaño de empresa** y **región geográfica**.

El assessment evalúa 6 dominios críticos de seguridad mapeados directamente a controles de **NIST CSF 2.0**, **ISO 27001:2022** y **COBIT 2019**, adaptados a la realidad operativa y al marco legal argentino (**Ley 25.326**).

### Características Técnicas

| Parámetro | Valor |
|-----------|-------|
| Preguntas | 24 en 6 dominios |
| Escala de respuesta | Sí (1.0) · Parcial (0.5) · No (0.0) |
| Pesos | 1–3 por pregunta (criticidad) |
| Score | 0–100 (promedio ponderado) |
| Motor IA | Anthropic Claude con system prompt sectorial |
| Privacidad | Cero trackers de terceros |
| Cumplimiento | Ley 25.326 · AAIP Registrado |
| Duración | < 5 minutos |

---

## Dominios Evaluados

```
┌─────────────────────────┬─────────────────────────┬─────────────────────────┐
│  🔑 Control de Accesos  │  💾 Copias de Seguridad │  🌐 Seguridad de Red   │
│  Contraseñas, MFA,      │  Backups automáticos,   │  Firewall, WiFi,       │
│  revocación, privilegio │  externos, restore,     │  VPN, actualización    │
│  mínimo                 │  anti-ransomware        │  de dispositivos       │
│  Peso máximo: 9         │  Peso máximo: 10        │  Peso máximo: 7        │
├─────────────────────────┼─────────────────────────┼─────────────────────────┤
│  🔄 Actualizaciones     │  📋 Protección de Datos │  👥 Concientización    │
│  Parches OS, antivirus/ │  Mapeo datos, política  │  Phishing, política    │
│  EDR, apps de negocio,  │  privacidad, cifrado,   │  documentada, BYOD,    │
│  responsable definido   │  plan de brecha         │  respuesta a incid.    │
│  Peso máximo: 8         │  Peso máximo: 9         │  Peso máximo: 6        │
└─────────────────────────┴─────────────────────────┴─────────────────────────┘
```

---

## Mapeo a Frameworks

Cada dominio se alinea con controles específicos de tres frameworks internacionales:

| Dominio | NIST CSF 2.0 | ISO 27001:2022 | COBIT 2019 |
|---------|-------------|----------------|------------|
| **Control de Accesos** | PR.AA-01 a AA-06 | A.5.15-17, A.8.2-8.5 | DSS05.04-05, APO13.01 |
| **Copias de Seguridad** | PR.DS, RC.RP-01 a RP-06 | A.8.13, A.5.29-30 | DSS04.07-08, BAI09.03 |
| **Seguridad de Red** | PR.IR-01, DE.CM | A.8.20-23 | DSS05.02-03, DSS05.07 |
| **Actualizaciones** | ID.RA, PR.PS-01 | A.8.7-9 | DSS05.01, BAI06.01 |
| **Protección de Datos** | PR.DS, GV.PO, ID.AM | A.5.33-34, A.8.10-12 | APO01.06, DSS05.06 |
| **Concientización** | PR.AT-01/02, GV.RR | A.6.3, A.5.4, A.6.8 | APO07.03-04, DSS05.01 |

> **Ley 25.326** — Abordada específicamente en el dominio "Protección de Datos" (preguntas d1-d4), evaluando mapeo de datos personales, políticas de privacidad, cifrado y respuesta ante brechas, conforme a los Artículos 5, 6, 9 y 12 y la Disposición AAIP 47/2018.

---

## Matriz de Preguntas

### Dominio 1 — Control de Accesos
| ID | Pregunta | Peso | NIST | ISO | COBIT |
|----|----------|:----:|------|-----|-------|
| a1 | ¿Contraseñas únicas por sistema? | 2 | PR.AA-01 | A.5.17 | DSS05.04 |
| a2 | ¿MFA en correo y sistemas críticos? | **3** | PR.AA-03 | A.8.5 | DSS05.04 |
| a3 | ¿Proceso formal de revocación de accesos? | 2 | PR.AA-05 | A.5.18 | DSS05.04 |
| a4 | ¿Principio de mínimo privilegio? | 2 | PR.AA-06 | A.8.3 | DSS05.04 |

### Dominio 2 — Copias de Seguridad
| ID | Pregunta | Peso | NIST | ISO | COBIT |
|----|----------|:----:|------|-----|-------|
| b1 | ¿Backups automáticos y periódicos? | **3** | PR.DS-01 | A.8.13 | DSS04.07 |
| b2 | ¿Backups en ubicación separada? | **3** | RC.RP-02 | A.8.13 | DSS04.07 |
| b3 | ¿Pruebas de restauración? | 2 | RC.RP-04 | A.5.29 | DSS04.08 |
| b4 | ¿Backups anti-ransomware (offline/inmutable)? | 2 | RC.RP-03 | A.5.30 | DSS04.07 |

### Dominio 3 — Seguridad de Red
| ID | Pregunta | Peso | NIST | ISO | COBIT |
|----|----------|:----:|------|-----|-------|
| r1 | ¿Firewall activo y configurado? | 2 | PR.IR-01 | A.8.20 | DSS05.02 |
| r2 | ¿Wi-Fi empleados separada de visitantes? | 2 | PR.IR-01 | A.8.22 | DSS05.02 |
| r3 | ¿VPN para trabajo remoto? | 2 | PR.IR-01 | A.8.20 | DSS05.02 |
| r4 | ¿Routers y dispositivos de red actualizados? | 1 | PR.PS-01 | A.8.9 | DSS05.03 |

### Dominio 4 — Actualizaciones
| ID | Pregunta | Peso | NIST | ISO | COBIT |
|----|----------|:----:|------|-----|-------|
| p1 | ¿Updates automáticos de SO? | 2 | PR.PS-01 | A.8.8 | BAI06.01 |
| p2 | ¿Antivirus/EDR activo y actualizado? | **3** | PR.PS-02 | A.8.7 | DSS05.01 |
| p3 | ¿Apps de negocio actualizadas? | 2 | PR.PS-01 | A.8.8 | BAI06.01 |
| p4 | ¿Responsable de verificar parches? | 1 | GV.RR-02 | A.8.8 | DSS03.01 |

### Dominio 5 — Protección de Datos
| ID | Pregunta | Peso | NIST | ISO | COBIT |
|----|----------|:----:|------|-----|-------|
| d1 | ¿Mapeo de datos personales almacenados? | **3** | ID.AM-07 | A.5.33 | APO01.06 |
| d2 | ¿Política de privacidad y aviso Ley 25.326? | 2 | GV.PO-01 | A.5.34 | DSS06.06 |
| d3 | ¿Datos sensibles cifrados (reposo y tránsito)? | 2 | PR.DS-01 | A.8.10 | DSS05.06 |
| d4 | ¿Plan de respuesta ante brecha de datos? | 2 | RS.MA-01 | A.5.26 | DSS02.01 |

### Dominio 6 — Concientización
| ID | Pregunta | Peso | NIST | ISO | COBIT |
|----|----------|:----:|------|-----|-------|
| c1 | ¿Capacitación anti-phishing al personal? | 2 | PR.AT-01 | A.6.3 | APO07.03 |
| c2 | ¿Política de seguridad documentada? | 1 | GV.PO-01 | A.5.1 | APO01.03 |
| c3 | ¿Saben qué hacer ante un compromiso? | 2 | RS.CO-02 | A.6.8 | DSS02.01 |
| c4 | ¿Políticas BYOD para dispositivos personales? | 1 | PR.AA-06 | A.8.1 | DSS05.03 |

> **Peso 3 (Crítico)** se asigna a: MFA (a2), backups automáticos (b1), backups externos (b2), antivirus/EDR (p2), y mapeo de datos (d1). Si una empresa responde "No" en las 5, está en **riesgo crítico inmediato**.

---

## Motor de Scoring

### Cálculo por Dominio

```
Score_Dominio = REDONDEAR( SUMA(Valor_i × Peso_i) / SUMA(Peso_i) × 100 )
```

Donde `Valor`: Sí = 1.0 | Parcial = 0.5 | No = 0.0

### Score Global

```
Score_Global = REDONDEAR( (ACC + BKP + RED + PAR + DAT + PER) / 6 )
```

### Escala de Madurez

| Score | Nivel | Perfil de Riesgo | Acción |
|:-----:|-------|------------------|--------|
| 🔴 0–30 | **INICIAL** | Crítico — riesgos activos explotables | Esta semana |
| 🟡 31–55 | **EN DESARROLLO** | Alto — brechas significativas | Este mes |
| 🟢 56–75 | **GESTIONADO** | Medio — requiere formalización | Este trimestre |
| 🔵 76–100 | **OPTIMIZADO** | Bajo — mejora continua | Continuo |

---

## Análisis con Inteligencia Artificial

El assessment genera un análisis ejecutivo personalizado usando IA, calibrado por:

- **10 verticales de industria**: Salud, Fintech, SaaS/Tecnología, E-commerce/Retail, Agro/AgTech/Manufactura, Servicios Profesionales, Logística, Educación/EdTech, Gastronomía/Turismo, PyME General
- **5 regiones argentinas**: CABA/GBA, Córdoba/Rosario/Santa Fe, Mendoza/Tucumán/NOA, Patagonia, Interior
- **5 niveles de tamaño**: 1–5, 6–20, 21–50, 51–100, 100+ empleados

Cada combinación produce un diagnóstico ejecutivo único en lenguaje de negocio, no técnico.

### Protección Anti-Manipulación

El motor incluye un **Prompt Injection Shield** que detecta y bloquea 7 categorías de ataque antes de que lleguen al modelo de IA:

| Categoría | Qué detecta |
|-----------|-------------|
| Inyección directa | Intentos de sobreescribir instrucciones (ES/EN) |
| Escape de delimitadores | Uso de tokens de rol como `[SYSTEM]`, `Human:` |
| Solicitudes maliciosas | Pedidos de generar código dañino o acceder a sistemas |
| Densidad de caracteres | Prompts con exceso de caracteres especiales |
| Longitud anormal | Prompts que exceden el largo esperado del assessment |
| Extracción de instrucciones | Intentos de revelar el system prompt |
| Manipulación de rol | Intentos de cambiar la personalidad del modelo |

---

## Seguridad de la Plataforma

CiberShield implementa en su propia infraestructura los mismos controles que recomienda a sus clientes:

| Control | Implementación | Verificable |
|---------|---------------|:-----------:|
| HTTPS/TLS | HSTS con preload, max-age 1 año | ✅ |
| Content Security Policy | Estricta, sin scripts externos | ✅ [SecurityHeaders.com](https://securityheaders.com/?q=https%3A%2F%2Fcibershield.io%2F&followRedirects=on) |
| Zero Trackers | Sin Google Analytics, sin reCAPTCHA, sin Meta Pixel | ✅ |
| Anti-Bot | Honeypot + timestamp server-side | ✅ |
| Rate Limiting | 15 req/h (IA), 10 req/h (formularios) | ✅ |
| Sanitización | HTML encoding + truncado en todos los inputs | ✅ |
| Seguridad de output | Solo `textContent` (nunca `innerHTML`) | ✅ |
| Hashing de IPs | SHA-256, sin PII cruda en almacenamiento | ✅ |
| Registro AAIP | `RL-2026-25503147-APN-DNPDP#AAIP` | ✅ [Registro Público](https://www.argentina.gob.ar/aaip/datospersonales/reclama) |

---

## Tratamiento de Datos

| Aspecto | Detalle |
|---------|---------|
| **Qué datos se recopilan** | Nombre de empresa, sector, cantidad de empleados, provincia, respuestas del cuestionario (24), score calculado, nivel de madurez, IP hasheada (SHA-256), user agent |
| **Quién los ve** | Únicamente Emanuel Pereyra (fundador y único administrador de CiberShield) a través de un panel privado con autenticación |
| **Para qué se usan** | Generar el diagnóstico de seguridad, análisis con IA, contacto posterior para ofrecer servicios de consultoría |
| **Agregación anónima** | Los datos se agregan de forma anónima (sin identificar empresas individuales) para construir estadísticas sectoriales y regionales de madurez en ciberseguridad PyME en Argentina |
| **Retención** | 12 meses desde la recolección, luego eliminación segura |
| **Base legal** | Consentimiento informado (Art. 5 Ley 25.326) con checkbox obligatorio previo al assessment |
| **Derechos ARCO** | Acceso, rectificación, cancelación y oposición via contacto@cibershield.io |

---

## Sobre CiberShield

**CiberShield** es una consultoría de ciberseguridad especializada en PyMEs argentinas, fundada por **Emanuel Pereyra**, Técnico en Seguridad Informática con título oficial del Ministerio de Educación.

- 🛡 Partner oficial de seguridad de **Humand** (Y Combinator · USD 66M Serie A)
- 🎓 Disertante en **UCEL Rosario** sobre seguridad en sistemas blockchain
- 📋 Responsable inscripto ante la **AAIP** (Agencia de Acceso a la Información Pública)
- 🔒 Calificación **A** en SecurityHeaders.com
- 🚫 **Cero trackers** de terceros en su plataforma

### Contacto

| Canal | Enlace |
|-------|--------|
| Web | [cibershield.io](https://cibershield.io) |
| Email | contacto@cibershield.io |
| WhatsApp | [+54 3402 529216](https://wa.me/+543402529216) |
| LinkedIn | [Emanuel Pereyra](https://linkedin.com/in/emanuel-pereyra1-arg) |

---

<p align="center">
  <sub>© 2026 CiberShield · Emanuel Pereyra · CUIT 20-33120188-0</sub><br/>
  <sub>AAIP RL-2026-25503147-APN-DNPDP#AAIP</sub><br/>
  <sub><i>Blindamos tu información. Auditamos tu seguridad.</i></sub>
</p>

---

> **Nota:** Este repositorio documenta la metodología de ShieldScan con fines de transparencia y posiciona
<h1 align="center">ShieldScan</h1>
<h3 align="center">Motor de Diagnóstico de Ciberseguridad con IA para PyMEs Argentinas</h3>

<p align="center">
  <a href="https://cibershield.io"><img src="https://img.shields.io/badge/Web-cibershield.io-00aaff?style=flat-square&logo=google-chrome&logoColor=white" alt="Website"/></a>
  <img src="https://img.shields.io/badge/NIST_CSF-2.0-0066cc?style=flat-square" alt="NIST CSF 2.0"/>
  <img src="https://img.shields.io/badge/ISO-27001:2022-0066cc?style=flat-square" alt="ISO 27001"/>
  <img src="https://img.shields.io/badge/COBIT-2019-0066cc?style=flat-square" alt="COBIT 2019"/>
  <img src="https://img.shields.io/badge/Ley-25.326-D4AF37?style=flat-square" alt="Ley 25.326"/>
  <img src="https://img.shields.io/badge/Security_Headers-A-10b981?style=flat-square" alt="Security Headers A"/>
  <img src="https://img.shields.io/badge/Trackers-0-10b981?style=flat-square" alt="Zero Trackers"/>
  <img src="https://img.shields.io/badge/AAIP-Registrado-D4AF37?style=flat-square" alt="AAIP Registrado"/>
</p>

<p align="center">
  <b>24 preguntas · 6 dominios · Score 0–100 · Análisis ejecutivo con IA</b><br/>
  <sub>Gratuito · Sin registro · 5 minutos · <a href="https://cibershield.io/#assessment">Hacé el diagnóstico →</a></sub>
</p>

---

## Qué es ShieldScan

ShieldScan es el motor de assessment automatizado de **CiberShield**, diseñado para evaluar la madurez de ciberseguridad de pequeñas y medianas empresas argentinas.

Combina un cuestionario de autoevaluación ponderado con análisis ejecutivo generado por inteligencia artificial, calibrado por **sector**, **tamaño de empresa** y **región geográfica**.

El assessment evalúa 6 dominios críticos de seguridad mapeados directamente a controles de **NIST CSF 2.0**, **ISO 27001:2022** y **COBIT 2019**, adaptados a la realidad operativa y al marco legal argentino (**Ley 25.326**).

### Características Técnicas

| Parámetro | Valor |
|-----------|-------|
| Preguntas | 24 en 6 dominios |
| Escala de respuesta | Sí (1.0) · Parcial (0.5) · No (0.0) |
| Pesos | 1–3 por pregunta (criticidad) |
| Score | 0–100 (promedio ponderado) |
| Motor IA | Anthropic Claude con system prompt sectorial |
| Privacidad | Cero trackers de terceros |
| Cumplimiento | Ley 25.326 · AAIP Registrado |
| Duración | < 5 minutos |

---

## Dominios Evaluados

```
┌─────────────────────────┬─────────────────────────┬─────────────────────────┐
│  🔑 Control de Accesos  │  💾 Copias de Seguridad │  🌐 Seguridad de Red   │
│  Contraseñas, MFA,      │  Backups automáticos,   │  Firewall, WiFi,       │
│  revocación, privilegio │  externos, restore,     │  VPN, actualización    │
│  mínimo                 │  anti-ransomware        │  de dispositivos       │
│  Peso máximo: 9         │  Peso máximo: 10        │  Peso máximo: 7        │
├─────────────────────────┼─────────────────────────┼─────────────────────────┤
│  🔄 Actualizaciones     │  📋 Protección de Datos │  👥 Concientización    │
│  Parches OS, antivirus/ │  Mapeo datos, política  │  Phishing, política    │
│  EDR, apps de negocio,  │  privacidad, cifrado,   │  documentada, BYOD,    │
│  responsable definido   │  plan de brecha         │  respuesta a incid.    │
│  Peso máximo: 8         │  Peso máximo: 9         │  Peso máximo: 6        │
└─────────────────────────┴─────────────────────────┴─────────────────────────┘
```

---

## Mapeo a Frameworks

Cada dominio se alinea con controles específicos de tres frameworks internacionales:

| Dominio | NIST CSF 2.0 | ISO 27001:2022 | COBIT 2019 |
|---------|-------------|----------------|------------|
| **Control de Accesos** | PR.AA-01 a AA-06 | A.5.15-17, A.8.2-8.5 | DSS05.04-05, APO13.01 |
| **Copias de Seguridad** | PR.DS, RC.RP-01 a RP-06 | A.8.13, A.5.29-30 | DSS04.07-08, BAI09.03 |
| **Seguridad de Red** | PR.IR-01, DE.CM | A.8.20-23 | DSS05.02-03, DSS05.07 |
| **Actualizaciones** | ID.RA, PR.PS-01 | A.8.7-9 | DSS05.01, BAI06.01 |
| **Protección de Datos** | PR.DS, GV.PO, ID.AM | A.5.33-34, A.8.10-12 | APO01.06, DSS05.06 |
| **Concientización** | PR.AT-01/02, GV.RR | A.6.3, A.5.4, A.6.8 | APO07.03-04, DSS05.01 |

> **Ley 25.326** — Abordada específicamente en el dominio "Protección de Datos" (preguntas d1-d4), evaluando mapeo de datos personales, políticas de privacidad, cifrado y respuesta ante brechas, conforme a los Artículos 5, 6, 9 y 12 y la Disposición AAIP 47/2018.

---

## Matriz de Preguntas

### Dominio 1 — Control de Accesos
| ID | Pregunta | Peso | NIST | ISO | COBIT |
|----|----------|:----:|------|-----|-------|
| a1 | ¿Contraseñas únicas por sistema? | 2 | PR.AA-01 | A.5.17 | DSS05.04 |
| a2 | ¿MFA en correo y sistemas críticos? | **3** | PR.AA-03 | A.8.5 | DSS05.04 |
| a3 | ¿Proceso formal de revocación de accesos? | 2 | PR.AA-05 | A.5.18 | DSS05.04 |
| a4 | ¿Principio de mínimo privilegio? | 2 | PR.AA-06 | A.8.3 | DSS05.04 |

### Dominio 2 — Copias de Seguridad
| ID | Pregunta | Peso | NIST | ISO | COBIT |
|----|----------|:----:|------|-----|-------|
| b1 | ¿Backups automáticos y periódicos? | **3** | PR.DS-01 | A.8.13 | DSS04.07 |
| b2 | ¿Backups en ubicación separada? | **3** | RC.RP-02 | A.8.13 | DSS04.07 |
| b3 | ¿Pruebas de restauración? | 2 | RC.RP-04 | A.5.29 | DSS04.08 |
| b4 | ¿Backups anti-ransomware (offline/inmutable)? | 2 | RC.RP-03 | A.5.30 | DSS04.07 |

### Dominio 3 — Seguridad de Red
| ID | Pregunta | Peso | NIST | ISO | COBIT |
|----|----------|:----:|------|-----|-------|
| r1 | ¿Firewall activo y configurado? | 2 | PR.IR-01 | A.8.20 | DSS05.02 |
| r2 | ¿Wi-Fi empleados separada de visitantes? | 2 | PR.IR-01 | A.8.22 | DSS05.02 |
| r3 | ¿VPN para trabajo remoto? | 2 | PR.IR-01 | A.8.20 | DSS05.02 |
| r4 | ¿Routers y dispositivos de red actualizados? | 1 | PR.PS-01 | A.8.9 | DSS05.03 |

### Dominio 4 — Actualizaciones
| ID | Pregunta | Peso | NIST | ISO | COBIT |
|----|----------|:----:|------|-----|-------|
| p1 | ¿Updates automáticos de SO? | 2 | PR.PS-01 | A.8.8 | BAI06.01 |
| p2 | ¿Antivirus/EDR activo y actualizado? | **3** | PR.PS-02 | A.8.7 | DSS05.01 |
| p3 | ¿Apps de negocio actualizadas? | 2 | PR.PS-01 | A.8.8 | BAI06.01 |
| p4 | ¿Responsable de verificar parches? | 1 | GV.RR-02 | A.8.8 | DSS03.01 |

### Dominio 5 — Protección de Datos
| ID | Pregunta | Peso | NIST | ISO | COBIT |
|----|----------|:----:|------|-----|-------|
| d1 | ¿Mapeo de datos personales almacenados? | **3** | ID.AM-07 | A.5.33 | APO01.06 |
| d2 | ¿Política de privacidad y aviso Ley 25.326? | 2 | GV.PO-01 | A.5.34 | DSS06.06 |
| d3 | ¿Datos sensibles cifrados (reposo y tránsito)? | 2 | PR.DS-01 | A.8.10 | DSS05.06 |
| d4 | ¿Plan de respuesta ante brecha de datos? | 2 | RS.MA-01 | A.5.26 | DSS02.01 |

### Dominio 6 — Concientización
| ID | Pregunta | Peso | NIST | ISO | COBIT |
|----|----------|:----:|------|-----|-------|
| c1 | ¿Capacitación anti-phishing al personal? | 2 | PR.AT-01 | A.6.3 | APO07.03 |
| c2 | ¿Política de seguridad documentada? | 1 | GV.PO-01 | A.5.1 | APO01.03 |
| c3 | ¿Saben qué hacer ante un compromiso? | 2 | RS.CO-02 | A.6.8 | DSS02.01 |
| c4 | ¿Políticas BYOD para dispositivos personales? | 1 | PR.AA-06 | A.8.1 | DSS05.03 |

> **Peso 3 (Crítico)** se asigna a: MFA (a2), backups automáticos (b1), backups externos (b2), antivirus/EDR (p2), y mapeo de datos (d1). Si una empresa responde "No" en las 5, está en **riesgo crítico inmediato**.

---

## Motor de Scoring

### Cálculo por Dominio

```
Score_Dominio = REDONDEAR( SUMA(Valor_i × Peso_i) / SUMA(Peso_i) × 100 )
```

Donde `Valor`: Sí = 1.0 | Parcial = 0.5 | No = 0.0

### Score Global

```
Score_Global = REDONDEAR( (ACC + BKP + RED + PAR + DAT + PER) / 6 )
```

### Escala de Madurez

| Score | Nivel | Perfil de Riesgo | Acción |
|:-----:|-------|------------------|--------|
| 🔴 0–30 | **INICIAL** | Crítico — riesgos activos explotables | Esta semana |
| 🟡 31–55 | **EN DESARROLLO** | Alto — brechas significativas | Este mes |
| 🟢 56–75 | **GESTIONADO** | Medio — requiere formalización | Este trimestre |
| 🔵 76–100 | **OPTIMIZADO** | Bajo — mejora continua | Continuo |

---

## Análisis con Inteligencia Artificial

El assessment genera un análisis ejecutivo personalizado usando IA, calibrado por:

- **10 verticales de industria**: Salud, Fintech, SaaS/Tecnología, E-commerce/Retail, Agro/AgTech/Manufactura, Servicios Profesionales, Logística, Educación/EdTech, Gastronomía/Turismo, PyME General
- **5 regiones argentinas**: CABA/GBA, Córdoba/Rosario/Santa Fe, Mendoza/Tucumán/NOA, Patagonia, Interior
- **5 niveles de tamaño**: 1–5, 6–20, 21–50, 51–100, 100+ empleados

Cada combinación produce un diagnóstico ejecutivo único en lenguaje de negocio, no técnico.

### Protección Anti-Manipulación

El motor incluye un **Prompt Injection Shield** que detecta y bloquea 7 categorías de ataque antes de que lleguen al modelo de IA:

| Categoría | Qué detecta |
|-----------|-------------|
| Inyección directa | Intentos de sobreescribir instrucciones (ES/EN) |
| Escape de delimitadores | Uso de tokens de rol como `[SYSTEM]`, `Human:` |
| Solicitudes maliciosas | Pedidos de generar código dañino o acceder a sistemas |
| Densidad de caracteres | Prompts con exceso de caracteres especiales |
| Longitud anormal | Prompts que exceden el largo esperado del assessment |
| Extracción de instrucciones | Intentos de revelar el system prompt |
| Manipulación de rol | Intentos de cambiar la personalidad del modelo |

---

## Seguridad de la Plataforma

CiberShield implementa en su propia infraestructura los mismos controles que recomienda a sus clientes:

| Control | Implementación | Verificable |
|---------|---------------|:-----------:|
| HTTPS/TLS | HSTS con preload, max-age 1 año | ✅ |
| Content Security Policy | Estricta, sin scripts externos | ✅ [SecurityHeaders.com](https://securityheaders.com/?q=https%3A%2F%2Fcibershield.io%2F&followRedirects=on) |
| Zero Trackers | Sin Google Analytics, sin reCAPTCHA, sin Meta Pixel | ✅ |
| Anti-Bot | Honeypot + timestamp server-side | ✅ |
| Rate Limiting | 15 req/h (IA), 10 req/h (formularios) | ✅ |
| Sanitización | HTML encoding + truncado en todos los inputs | ✅ |
| Seguridad de output | Solo `textContent` (nunca `innerHTML`) | ✅ |
| Hashing de IPs | SHA-256, sin PII cruda en almacenamiento | ✅ |
| Registro AAIP | `RL-2026-25503147-APN-DNPDP#AAIP` | ✅ [Registro Público](https://www.argentina.gob.ar/aaip/datospersonales/reclama) |

---

## Tratamiento de Datos

| Aspecto | Detalle |
|---------|---------|
| **Qué datos se recopilan** | Nombre de empresa, sector, cantidad de empleados, provincia, respuestas del cuestionario (24), score calculado, nivel de madurez, IP hasheada (SHA-256), user agent |
| **Quién los ve** | Únicamente Emanuel Pereyra (fundador y único administrador de CiberShield) a través de un panel privado con autenticación |
| **Para qué se usan** | Generar el diagnóstico de seguridad, análisis con IA, contacto posterior para ofrecer servicios de consultoría |
| **Agregación anónima** | Los datos se agregan de forma anónima (sin identificar empresas individuales) para construir estadísticas sectoriales y regionales de madurez en ciberseguridad PyME en Argentina |
| **Retención** | 12 meses desde la recolección, luego eliminación segura |
| **Base legal** | Consentimiento informado (Art. 5 Ley 25.326) con checkbox obligatorio previo al assessment |
| **Derechos ARCO** | Acceso, rectificación, cancelación y oposición via contacto@cibershield.io |

---

## Sobre CiberShield

**CiberShield** es una consultoría de ciberseguridad especializada en PyMEs argentinas, fundada por **Emanuel Pereyra**, Técnico en Seguridad Informática con título oficial del Ministerio de Educación.

- 🛡 Partner oficial de seguridad de **Humand** (Y Combinator · USD 66M Serie A)
- 🎓 Disertante en **UCEL Rosario** sobre seguridad en sistemas blockchain
- 📋 Responsable inscripto ante la **AAIP** (Agencia de Acceso a la Información Pública)
- 🔒 Calificación **A** en SecurityHeaders.com
- 🚫 **Cero trackers** de terceros en su plataforma

### Contacto

| Canal | Enlace |
|-------|--------|
| Web | [cibershield.io](https://cibershield.io) |
| Email | contacto@cibershield.io |
| WhatsApp | [+54 3402 529216](https://wa.me/+543402529216) |
| LinkedIn | [Emanuel Pereyra](https://linkedin.com/in/emanuel-pereyra1-arg) |

---

<p align="center">
  <sub>© 2026 CiberShield · Emanuel Pereyra · CUIT 20-33120188-0</sub><br/>
  <sub>AAIP RL-2026-25503147-APN-DNPDP#AAIP</sub><br/>
  <sub><i>Blindamos tu información. Auditamos tu seguridad.</i></sub>
</p>

---

> **Nota:** Este repositorio documenta la metodología de ShieldScan con fines de transparencia y posicionamiento profesional. Las referencias a NIST CSF, ISO 27001 y COBIT se usan con fines de alineamiento y no implican certificación. El código fuente, system prompts y configuraciones de seguridad de la implementación son propiedad privada de CiberShield y no se publican en este repositorio.
