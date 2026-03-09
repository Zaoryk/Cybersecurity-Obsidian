# Gestión de la Ciberseguridad
## Sistemas de Gestión de Seguridad de la Información (SGSI)

---

# Contenidos del Módulo

## Bloque 1: SGSI
- Conceptos fundamentales
- Marcos normativos
- Metodologías de gestión de seguridad de la información

## Bloque 2: Amenazas y Vulnerabilidades
- Identificación de amenazas en el ciberespacio
- Uso de bases de datos de vulnerabilidades
- Reconocimiento de riesgos actuales

---

# Sistema de Gestión de Seguridad de la Información (SGSI)

## Definición
Un **SGSI** es un conjunto de:

- Políticas
- Procedimientos
- Controles
- Procesos

Diseñados para **proteger los activos de información de una organización**.

### Objetivo
Garantizar:

- **Confidencialidad**
- **Integridad**
- **Disponibilidad**

frente a **riesgos internos y externos**.

### Importante
Un **SGSI no es un producto tecnológico**, sino un **marco de gestión continuo** que integra:

- Personas
- Procesos
- Tecnología

---

# Tríada CIA (CID)

Los pilares de la seguridad de la información.

## Confidencialidad
La información solo debe ser accesible para **personas autorizadas**.

Métodos de protección:
- Cifrado
- Control de acceso
- Clasificación de datos

## Integridad
La información debe ser:

- Exacta
- Completa
- Sin modificaciones no autorizadas

Métodos de protección:
- Hashing
- Firmas digitales
- Auditorías

## Disponibilidad
Los sistemas y datos deben estar **accesibles cuando se necesiten**.

Métodos de protección:
- Redundancia
- Backups
- Planes de continuidad

---

# Componentes Clave de un SGSI

## Políticas de Seguridad
Declaraciones formales que establecen las **reglas y directrices de seguridad** en la organización.

## Análisis de Riesgos
Proceso de:

- Identificar riesgos
- Evaluar impacto
- Priorizar controles

sobre los **activos de información**.

## Controles de Seguridad
Medidas implementadas para **mitigar riesgos**.

Tipos de controles:

- Técnicos
- Organizativos
- Físicos

## Auditoría y Revisión
Evaluaciones periódicas para:

- Verificar cumplimiento
- Comprobar efectividad del SGSI

---

# Normas y Estándares

## ISO/IEC 27001
Es el **estándar internacional más reconocido** para implementar un SGSI.

Define requisitos para:

- Establecer
- Implementar
- Mantener
- Mejorar continuamente

un sistema de gestión de seguridad de la información.

### Estructura de Alto Nivel (HLS)
Sigue el **Anexo SL**, permitiendo integración con:

- ISO 9001 (gestión de calidad)
- ISO 22301 (continuidad del negocio)

### Anexo A
Incluye **93 controles de seguridad**, organizados en 4 dominios:

- Organizativos
- Personas
- Físicos
- Tecnológicos

---

# Ciclo PDCA en SGSI

El SGSI usa el modelo de mejora continua **PDCA (Plan-Do-Check-Act)**.

## Plan
Definir:

- Alcance
- Políticas
- Riesgos
- Controles

## Do
Implementar los controles definidos.

## Check
Monitorizar y auditar el sistema.

## Act
Corregir fallos y mejorar continuamente.

---

# Otros Marcos de Seguridad

## NIST Cybersecurity Framework
Marco del **NIST (EE.UU.)**.

Organiza la ciberseguridad en 5 funciones:

1. Identificar
2. Proteger
3. Detectar
4. Responder
5. Recuperar

Usado frecuentemente en **infraestructuras críticas**.

## COBIT 2019
Marco de **gobernanza de TI**.

Conecta:

- Objetivos de negocio
- Controles de seguridad

Facilita la **alineación estratégica del SGSI con la empresa**.

## ENS (España)
**Esquema Nacional de Seguridad** obligatorio en administraciones públicas españolas.

Clasifica sistemas según impacto:

- Básico
- Medio
- Alto

---

# Comparación de Marcos

## ISO 27001
- Ámbito: Internacional
- Certificable: Sí
- Enfoque: Gestión de riesgos
- Sector: Cualquier organización

## NIST CSF
- Ámbito: Internacional (EE.UU.)
- Certificable: No
- Enfoque: Funciones de ciberseguridad
- Sector: Infraestructuras críticas

---

# Amenazas en el Ciberespacio

## Definición
Una **amenaza** es cualquier evento con potencial de **causar daño a los activos de información**.

Las amenazas evolucionan constantemente por factores:

- Económicos
- Políticos
- Geopolíticos

---

# Tipos de Amenazas

## Malware y Ransomware
Software malicioso diseñado para:

- Dañar sistemas
- Robar información
- Cifrar datos

**Ransomware:** cifra archivos y exige rescate.

En 2023 representó **24% de incidentes globales**.

## Phishing e Ingeniería Social
Manipulación psicológica para:

- Robar credenciales
- Obtener acceso a sistemas

Es el **vector de ataque más común**.

## Ataques DoS / DDoS
Ataques que saturan recursos para volver **inaccesible un servicio**.

DDoS:
- Ataques distribuidos
- Pueden generar tráfico de **terabits por segundo**.

---

# Amenazas Avanzadas

## APT (Advanced Persistent Threat)
Campañas de ataque sofisticadas y prolongadas.

Características:

- Patrocinadas por estados o grupos organizados
- Alto nivel de sigilo
- Objetivos de alto valor

Fases comunes:

- Reconocimiento previo
- Uso de exploits **zero-day**
- Movimiento lateral dentro de la red

## Insider Threat (Amenaza Interna)
Proviene de:

- Empleados
- Ex empleados
- Colaboradores

Puede ser:

- Maliciosa (espionaje, sabotaje)
- Accidental (errores humanos)

Según **Ponemon Institute**, el **60% de brechas incluye componente interno**.

Métodos de detección:

- UEBA (User and Entity Behavior Analytics)
- Gestión de privilegios

---

# Vulnerabilidades

## Definición
Una **vulnerabilidad** es una debilidad en:

- Sistemas
- Aplicaciones
- Procesos
- Controles

que puede ser explotada por una amenaza.

Diferencia clave:

- **Amenaza → externa**
- **Vulnerabilidad → debilidad interna del sistema**

---

# Tipos de Vulnerabilidades

## Técnicas
Errores en software o configuración:

- Buffer overflow
- Inyección SQL
- Credenciales por defecto
- Fallos de programación

## De Proceso
Problemas en procedimientos:

- Falta de gestión de parches
- Procesos de acceso deficientes
- Backups no verificados

## Humanas
Factores humanos:

- Falta de formación
- Contraseñas débiles
- Uso indebido de dispositivos

---

# Bases de Datos de Vulnerabilidades

## NVD / CVE
Bases de datos globales de vulnerabilidades.

Formato de identificación:

CVE-YYYY-NNNNN

Incluyen:

- Descripción
- Severidad
- Puntuación **CVSS**

## OWASP Top 10
Lista de las **10 vulnerabilidades más críticas en aplicaciones web**.

Utilizada para:

- Desarrollo seguro
- Auditorías
- Pentesting

## MITRE ATT&CK
Base de conocimiento de:

- Tácticas
- Técnicas
- Procedimientos (TTP)

Usada para **analizar ataques reales y fortalecer defensas**.

---

# OWASP Top 10 (Ejemplos)

## Broken Access Control
Usuarios acceden a recursos **fuera de sus permisos**.

## Cryptographic Failures
Exposición de datos sensibles por:

- Cifrado incorrecto
- Ausencia de cifrado

## Injection
Entrada de datos maliciosos en comandos o consultas:

- SQL Injection
- NoSQL Injection
- OS Injection

---

# CVSS (Common Vulnerability Scoring System)

Sistema que asigna **puntuación de severidad a vulnerabilidades (0–10)**.

## Baja (0.0 – 3.9)
Impacto limitado y difícil explotación.

## Media (4.0 – 6.9)
Explotable en ciertas condiciones.

## Alta (7.0 – 8.9)
Explotación probable con impacto significativo.

## Crítica (9.0 – 10)
Explotación sencilla y consecuencias graves.

Un **CVE con CVSS ≥ 9** debe tratarse como **prioridad inmediata**.

### Métricas evaluadas

- Vector de ataque (red, local, físico)
- Complejidad del ataque
- Privilegios requeridos
- Impacto en CIA

---

# Relación Amenaza – Vulnerabilidad – Incidente

Flujo del riesgo:

Activo → Vulnerabilidad → Amenaza → Riesgo → Incidente

Los **controles del SGSI** buscan:

- Reducir probabilidad
- Reducir impacto

de explotación de vulnerabilidades.

---

# Inteligencia de Amenazas (CTI)

Los SOC/CERT utilizan plataformas de **Cyber Threat Intelligence**.

## VirusTotal
Analiza:

- Archivos
- URLs

contra más de **70 motores antivirus**.

Permite detectar **IOC (Indicadores de Compromiso)**.

## Shodan
Motor de búsqueda para **dispositivos conectados a internet**.

Permite identificar:

- Servicios expuestos
- Sistemas vulnerables

## MISP / OpenCTI
Plataformas para **compartir inteligencia de amenazas**.

Intercambian:

- IOC
- TTP
- Campañas de ataque

mediante estándares **STIX/TAXII**.

---

# Gestión de Vulnerabilidades

Proceso continuo dentro del SGSI.

## Descubrir
Inventario y escaneo de sistemas.

## Priorizar
Uso de:

- CVSS
- Contexto de negocio

## Remediar
Aplicar:

- Parches
- Configuraciones seguras
- Mitigaciones

## Verificar
Re-testing y validación de la corrección.

La priorización basada en **CVSS + impacto en negocio** optimiza los recursos de seguridad.