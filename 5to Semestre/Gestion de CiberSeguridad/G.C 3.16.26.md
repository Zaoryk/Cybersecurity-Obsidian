# Amenazas y Vulnerabilidades en el Ciberespacio

## 1. Importancia de Identificar Amenazas
Identificar amenazas y vulnerabilidades es una actividad crítica dentro de la gestión de ciberseguridad.

### ¿Por qué es importante?
- Cada día se descubren miles de nuevas vulnerabilidades en sistemas informáticos.
- Las organizaciones que no monitorean fuentes de inteligencia de amenazas quedan expuestas a ataques conocidos.
- Detectar vulnerabilidades tempranamente reduce:
  - el tiempo de exposición
  - el impacto de incidentes de seguridad
  - el costo de recuperación

### Datos relevantes
- Más de **29.000 vulnerabilidades CVE registradas**.
- Aproximadamente **72% de las empresas sufrieron al menos un incidente de seguridad en el último año**.

### Conceptos clave
- **Amenaza:** cualquier evento potencial que pueda comprometer un sistema.
- **Vulnerabilidad:** debilidad en un sistema que puede ser explotada.
- **Riesgo:** probabilidad de que una amenaza explote una vulnerabilidad.

---

# 2. Bases de Datos de Inteligencia de Amenazas

Las organizaciones utilizan repositorios de seguridad para identificar vulnerabilidades conocidas.

## CVE / NVD
- **CVE (Common Vulnerabilities and Exposures)**: catálogo global de vulnerabilidades conocidas.
- **NVD (National Vulnerability Database)**: base de datos mantenida por NIST que incluye información técnica, impacto y mitigaciones.

Importancia:
- estandariza la identificación de vulnerabilidades
- permite priorizar parches de seguridad

---

## MITRE ATT&CK
Framework que documenta **tácticas, técnicas y procedimientos (TTPs)** usados por atacantes reales.

Uso principal:
- análisis de comportamiento de atacantes
- simulación de ataques
- detección de amenazas avanzadas

---

## OWASP
**Open Web Application Security Project**

Proyecto internacional enfocado en seguridad de aplicaciones web.

Recurso más importante:
- **OWASP Top 10** (lista de vulnerabilidades web más críticas).

---

## CISA KEV
Catálogo de **Known Exploited Vulnerabilities** mantenido por la Agencia de Ciberseguridad de EE.UU.

Ventaja:
- prioriza vulnerabilidades **activamente explotadas en el mundo real**.

---

# 3. Malware (Software Malicioso)

El malware es uno de los vectores de ataque más comunes en el ciberespacio.

## Definición
Software diseñado para:
- infiltrarse en sistemas
- dañar dispositivos
- robar información
- obtener acceso no autorizado

---

## Tipos principales de malware

### Ransomware
- Cifra archivos del sistema.
- Exige un rescate para recuperar los datos.

Ejemplos conocidos:
- LockBit
- ALPHV
- Cl0p

Impacto:
- paralización de operaciones
- pérdidas económicas
- daño reputacional

---

### Troyanos (Trojans)
Malware que se disfraza como software legítimo.

Funciones comunes:
- robo de credenciales
- acceso remoto
- instalación de otros malware

Ejemplos:
- Emotet
- QakBot

---

### Spyware
Software que espía la actividad del usuario.

Puede recolectar:
- contraseñas
- historial de navegación
- datos personales

---

### Adware
Software que muestra publicidad invasiva.

Riesgos:
- ralentización del sistema
- posible instalación de malware adicional.

---

### Worms (Gusanos)
Malware capaz de **propagarse automáticamente por redes**.

Ejemplo histórico:
- WannaCry

---

### Rootkits
Malware diseñado para **ocultar la presencia de otros programas maliciosos** dentro del sistema operativo.

Son difíciles de detectar y eliminar.

---

## Distribución aproximada de malware

- Ransomware → 24%
- Troyanos → 22%
- Spyware → 18%
- Adware → 14%
- Worms → 12%
- Rootkits → 10%

Los **ransomware y troyanos representan casi la mitad de los incidentes detectados**.

---

# 4. Phishing e Ingeniería Social

La ingeniería social explota el **factor humano** en lugar de vulnerabilidades técnicas.

### Importancia
Más del **36% de las brechas de seguridad comienzan con phishing**.

---

## Tipos de phishing

### Spear Phishing
Ataque dirigido y personalizado a una persona específica.

Objetivos comunes:
- empleados con acceso privilegiado
- administradores de sistemas

---

### Whaling
Variante del spear phishing dirigida a **altos ejecutivos**.

Ejemplos:
- CEO
- CFO
- directores financieros

Objetivo:
- transferencias fraudulentas
- acceso a datos estratégicos

---

### Vishing
Phishing mediante **llamadas telefónicas**.

---

### Smishing
Phishing mediante **mensajes SMS**.

---

# 5. Vulnerabilidades en Aplicaciones Web (OWASP Top 10)

Las aplicaciones web son uno de los principales objetivos de ataques.

## 1. Broken Access Control
- controles de acceso mal configurados
- usuarios pueden realizar acciones fuera de sus permisos

Ejemplo:
- acceder a datos de otros usuarios.

---

## 2. Cryptographic Failures
Errores en la protección criptográfica.

Ejemplos:
- uso de cifrado débil
- contraseñas almacenadas en texto plano
- transmisión de datos sin HTTPS

---

## 3. Injection
Inyección de código malicioso.

Tipos comunes:
- SQL Injection
- Cross-Site Scripting (XSS)
- LDAP Injection

Impacto:
- robo o modificación de bases de datos.

---

## 4. Security Misconfiguration
Configuraciones incorrectas en servidores o aplicaciones.

Ejemplos:
- servicios innecesarios activos
- credenciales por defecto
- exposición de mensajes de error sensibles

---

## 5. Vulnerable and Outdated Components
Uso de software desactualizado.

Ejemplo real:
- vulnerabilidad **Log4Shell (2021)**.

---

# 6. Ataques de Red

Los ataques de red buscan interceptar, manipular o interrumpir comunicaciones.

---

## Man-in-the-Middle (MitM)
El atacante intercepta la comunicación entre dos partes.

Situaciones comunes:
- redes WiFi públicas
- conexiones sin cifrado

Riesgos:
- robo de credenciales
- modificación de datos transmitidos.

---

## Ataques DDoS (Distributed Denial of Service)

Consisten en inundar un servidor con tráfico para hacerlo inaccesible.

Características:
- uso de botnets
- ataques volumétricos superiores a **1 Tbps**

Consecuencias:
- caída de servicios
- pérdida de ingresos.

---

## DNS Spoofing
Manipulación de registros DNS para redirigir usuarios a sitios maliciosos.

Objetivo:
- robo de credenciales
- distribución de malware.

---

# 7. Amenazas Persistentes Avanzadas (APT)

Las **APT (Advanced Persistent Threats)** son campañas de ataque sofisticadas y prolongadas.

Características:
- altamente organizadas
- generalmente patrocinadas por estados
- permanecen ocultas durante meses o años.

---

## Ejemplos de grupos APT

### APT28 (Fancy Bear)
- vinculado a inteligencia militar rusa.
- ataques a gobiernos y organizaciones políticas.

---

### APT41 (Double Dragon)
- grupo chino con actividades de espionaje y cibercrimen.

Sectores atacados:
- salud
- telecomunicaciones
- tecnología.

---

### Lazarus Group
- asociado a Corea del Norte.

Actividades:
- robo a bancos
- ataques a exchanges de criptomonedas
- espionaje industrial.

---

# 8. Ataques a la Cadena de Suministro

Ocurren cuando un atacante compromete un proveedor de software o servicios.

Impacto:
- miles de organizaciones afectadas simultáneamente.

---

## Ejemplos reales

### SolarWinds (2020)
- actualización comprometida.
- afectó a **18.000 organizaciones**.

---

### Kaseya VSA (2021)
- vulnerabilidad zero-day explotada por ransomware REvil.

---

### 3CX (2023)
- software VoIP comprometido para distribuir malware.

---

# 9. Conceptos Clave para Estudio

### Vector de ataque
Método utilizado para comprometer un sistema.

Ejemplos:
- phishing
- malware
- vulnerabilidades web.

---

### Zero-Day
Vulnerabilidad desconocida para el fabricante y sin parche disponible.

---

### Patch Management
Proceso de actualización de software para corregir vulnerabilidades.

---

### Defensa en Profundidad
Estrategia que utiliza múltiples capas de seguridad:

- firewall
- antivirus
- autenticación multifactor
- monitoreo de red
- cifrado de datos

---

# 10. Buenas Prácticas de Ciberseguridad

- mantener sistemas actualizados
- implementar autenticación multifactor
- usar cifrado de datos
- capacitar a los usuarios contra phishing
- monitorear logs y tráfico de red
- realizar auditorías de seguridad periódicas

---

# Idea Clave

La ciberseguridad moderna depende de tres pilares:

1. **Prevención** (parches, configuraciones seguras)
2. **Detección** (monitoreo, análisis de amenazas)
3. **Respuesta** (planes de incidentes y recuperación)