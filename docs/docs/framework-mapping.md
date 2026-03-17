# Mapeo Detallado de Frameworks

> Documento técnico: relación entre cada pregunta de ShieldScan y los controles específicos de NIST CSF 2.0, ISO 27001:2022 y COBIT 2019.

## Metodología de Mapeo

Cada pregunta del assessment fue diseñada para evaluar uno o más controles específicos de los tres frameworks. La selección de controles prioriza aquellos con mayor impacto en la supervivencia operativa de una PyME argentina.

### Criterios de selección de controles

1. **Relevancia para PyME**: Se priorizaron controles implementables sin grandes presupuestos ni equipos dedicados
2. **Impacto en supervivencia**: Los controles de peso 3 son aquellos cuya ausencia pone en riesgo la continuidad del negocio
3. **Verificabilidad**: Cada control puede evaluarse con una pregunta de Sí/Parcial/No sin ambigüedad
4. **Cumplimiento local**: Se incluyen controles que satisfacen requisitos de la Ley 25.326 y Disposición AAIP 47/2018

## Control de Accesos → NIST PR.AA / ISO A.5-A.8 / COBIT DSS05

| Pregunta | Control evaluado | NIST CSF 2.0 | ISO 27001:2022 | COBIT 2019 | Ley 25.326 |
|----------|-----------------|--------------|----------------|------------|------------|
| a1 - Contraseñas únicas | Gestión de credenciales | PR.AA-01 Identities and credentials are managed | A.5.17 Authentication information | DSS05.04 Manage user identity | — |
| a2 - MFA activo | Autenticación multifactor | PR.AA-03 Authentication is performed | A.8.5 Secure authentication | DSS05.04 Manage user identity | Art. 9 (medidas de seguridad) |
| a3 - Revocación de accesos | Ciclo de vida de identidad | PR.AA-05 Access permissions managed | A.5.18 Access rights | DSS05.04 Manage user identity | Art. 9 |
| a4 - Mínimo privilegio | Control de privilegios | PR.AA-06 Least privilege applied | A.8.3 Access restriction | DSS05.04 Manage user identity | — |

## Copias de Seguridad → NIST PR.DS, RC.RP / ISO A.8.13, A.5.29-30 / COBIT DSS04

| Pregunta | Control evaluado | NIST CSF 2.0 | ISO 27001:2022 | COBIT 2019 | Ley 25.326 |
|----------|-----------------|--------------|----------------|------------|------------|
| b1 - Backups automáticos | Protección de datos en reposo | PR.DS-01 Data-at-rest protected | A.8.13 Information backup | DSS04.07 Manage backup arrangements | Art. 9 |
| b2 - Backups externos | Resiliencia y recuperación | RC.RP-02 Recovery performed | A.8.13 Information backup | DSS04.07 Manage backup arrangements | — |
| b3 - Pruebas de restore | Validación de recuperación | RC.RP-04 Integrity of backups verified | A.5.29 ICT readiness for BC | DSS04.08 Post-resumption review | — |
| b4 - Anti-ransomware | Aislamiento de backups | RC.RP-03 Recovery activities communicated | A.5.30 ICT readiness for BC | DSS04.07 Manage backup arrangements | — |

## Seguridad de Red → NIST PR.IR, DE.CM / ISO A.8.20-23 / COBIT DSS05

| Pregunta | Control evaluado | NIST CSF 2.0 | ISO 27001:2022 | COBIT 2019 | Ley 25.326 |
|----------|-----------------|--------------|----------------|------------|------------|
| r1 - Firewall activo | Protección de red | PR.IR-01 Networks protected | A.8.20 Network security | DSS05.02 Manage network security | Art. 9 |
| r2 - Redes separadas | Segmentación | PR.IR-01 Networks protected | A.8.22 Segregation in networks | DSS05.02 Manage network security | — |
| r3 - VPN remoto | Acceso seguro remoto | PR.IR-01 Networks protected | A.8.20 Network security | DSS05.02 Manage network security | — |
| r4 - Dispositivos actualizados | Gestión de configuración | PR.PS-01 Configuration management | A.8.9 Configuration management | DSS05.03 Manage endpoint security | — |

## Actualizaciones → NIST ID.RA, PR.PS / ISO A.8.7-9 / COBIT DSS05, BAI06

| Pregunta | Control evaluado | NIST CSF 2.0 | ISO 27001:2022 | COBIT 2019 | Ley 25.326 |
|----------|-----------------|--------------|----------------|------------|------------|
| p1 - Updates automáticos | Gestión de parches | PR.PS-01 Configuration management | A.8.8 Management of tech vulnerabilities | BAI06.01 Evaluate and prioritize changes | — |
| p2 - Antivirus/EDR | Protección contra malware | PR.PS-02 Software maintained | A.8.7 Protection against malware | DSS05.01 Protect against malware | Art. 9 |
| p3 - Apps actualizadas | Vulnerabilidades en software | PR.PS-01 Configuration management | A.8.8 Management of tech vulnerabilities | BAI06.01 Evaluate and prioritize changes | — |
| p4 - Responsable de parches | Roles y responsabilidades | GV.RR-02 Roles established | A.8.8 Management of tech vulnerabilities | DSS03.01 Identify and classify problems | — |

## Protección de Datos → NIST PR.DS, GV.PO / ISO A.5.33-34, A.8.10-12 / COBIT APO01, DSS05

| Pregunta | Control evaluado | NIST CSF 2.0 | ISO 27001:2022 | COBIT 2019 | Ley 25.326 |
|----------|-----------------|--------------|----------------|------------|------------|
| d1 - Mapeo de datos | Inventario de activos de información | ID.AM-07 Data inventoried | A.5.33 Protection of records | APO01.06 Define data management | **Art. 5, 6** |
| d2 - Política de privacidad | Políticas de protección | GV.PO-01 Policy established | A.5.34 Privacy and PII protection | DSS06.06 Secure information assets | **Art. 6, 11** |
| d3 - Cifrado | Protección criptográfica | PR.DS-01 Data-at-rest protected | A.8.10 Information deletion / A.8.12 Data leak prevention | DSS05.06 Manage sensitive documents | **Art. 9** |
| d4 - Plan de brecha | Respuesta a incidentes | RS.MA-01 Incident managed | A.5.26 Response to info security incidents | DSS02.01 Define incident classification | **Art. 12** |

## Concientización → NIST PR.AT / ISO A.6.3 / COBIT APO07

| Pregunta | Control evaluado | NIST CSF 2.0 | ISO 27001:2022 | COBIT 2019 | Ley 25.326 |
|----------|-----------------|--------------|----------------|------------|------------|
| c1 - Capacitación phishing | Formación en seguridad | PR.AT-01 Awareness provided | A.6.3 Information security awareness | APO07.03 Maintain skills and competencies | — |
| c2 - Política documentada | Gobernanza de seguridad | GV.PO-01 Policy established | A.5.1 Policies for info security | APO01.03 Maintain enablers of mgmt system | Art. 9 (Disp. 47/2018) |
| c3 - Respuesta a incidentes | Comunicación de incidentes | RS.CO-02 Incidents reported | A.6.8 Info security event reporting | DSS02.01 Define incident classification | — |
| c4 - BYOD | Control de activos | PR.AA-06 Physical access managed | A.8.1 User endpoint devices | DSS05.03 Manage endpoint security | — |

---

> Las referencias a artículos de la Ley 25.326 se incluyen donde la pregunta evalúa directa
