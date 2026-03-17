# Changelog

Todos los cambios notables de ShieldScan se documentan en este archivo.

El formato está basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.1.0/).

## [1.0.0] — 2026-03-12

### Lanzamiento Inicial

#### Assessment Engine
- 24 preguntas en 6 dominios de seguridad
- Sistema de scoring ponderado (pesos 1-3)
- Escala de madurez de 4 niveles (Inicial / En Desarrollo / Gestionado / Optimizado)
- Mapeo completo a NIST CSF 2.0, ISO 27001:2022 y COBIT 2019

#### Análisis con IA
- Integración con Anthropic Claude Haiku 4.5
- System prompt con inteligencia sectorial para 10 industrias
- Calibración por 5 regiones argentinas y 5 tamaños de empresa
- Prompt Injection Shield con detección de 7 categorías de ataque

#### Seguridad
- HTTPS/TLS con HSTS preload
- Content Security Policy estricta (SecurityHeaders.com: A)
- Cero trackers de terceros (sin Google Analytics, sin reCAPTCHA)
- Honeypot + timestamp anti-bot (reemplazo de reCAPTCHA)
- Rate limiting por IP (15 req/h IA, 10 req/h formularios)
- Sanitización de inputs + textContent para outputs

#### Cumplimiento Legal
- Consentimiento informado con checkbox obligatorio
- Política de Privacidad (5 páginas, 11 secciones)
- Términos y Condiciones
- Registro ante AAIP como responsable de base de datos
- Inscripción de base de datos privada presentada
- IPs hasheadas con SHA-256 (sin PII cruda)

#### Infraestructura
- Lead capture automatizado con JSON storage
- Panel administrativo con filtros y estadísticas
- Email HTML al admin con badges por tipo de contacto
- Email de resultados al cliente con análisis completo
- Email de confirmación automática con timeline de servicio
- Página de contacto con sesión gratuita + cotización

---

> Cada entrada refleja cambios en la metodología y capacidades de la plataforma, no en el código fuente.
