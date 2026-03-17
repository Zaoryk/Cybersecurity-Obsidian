# Caso Empresa — EPTA Chile SpA

## 1. Ficha de la Empresa

### Nombre
- EPTA Chile SpA (Filial)

### Rubro
- Refrigeración comercial e industrial

### Sectores atendidos
- Retail (supermercados, tiendas de conveniencia)
- Ho.Re.Ca (Hoteles, Restaurantes y Catering)
- Food & Beverage (producción y distribución de alimentos y bebidas)

### Servicios principales
- diseño e instalación de sistemas de refrigeración
- mantenimiento técnico
- monitoreo de equipos
- soporte a clientes comerciales

---

## 2. Contexto Tecnológico

La empresa depende fuertemente de infraestructura tecnológica para:

- operación de sistemas de refrigeración conectados
- gestión de inventario y ERP
- comunicación entre sucursales
- atención al cliente
- soporte técnico remoto

Esto implica una alta dependencia de:

- redes (LAN, WAN, WiFi)
- sistemas cloud o centralizados
- dispositivos IoT
- plataformas de comunicación

---

# 3. Problemáticas Identificadas

## 3.1 Problemas de Conectividad Interna

### Red LAN / WiFi inestable

#### Problema
- zonas con baja cobertura o señal débil
- interrupciones en acceso a sistemas críticos

#### Impacto
- dificultad para acceder a ERP
- retrasos en inventarios
- problemas en comunicación interna

#### Posibles causas
- mala distribución de access points
- interferencias electromagnéticas
- infraestructura de red obsoleta
- falta de segmentación de red

#### Complejidad
- media-alta (requiere rediseño de red física y lógica)

---

## 3.2 Conectividad entre Sucursales

### VPN lenta o poco segura

#### Problema
- acceso remoto ineficiente para técnicos
- caídas frecuentes en la conexión

#### Impacto
- retraso en reportes técnicos
- baja productividad
- riesgo de pérdida de información

#### Posibles causas
- ancho de banda insuficiente
- mala configuración de VPN
- uso de protocolos antiguos
- falta de redundancia

#### Complejidad
- alta (involucra redes WAN y seguridad)

---

## 3.3 Telecomunicaciones con Clientes

### Falta de canales integrados

#### Problema
- múltiples canales sin integración (teléfono, correo, WhatsApp)

#### Impacto
- pérdida de solicitudes
- duplicación de casos
- mala experiencia del cliente

#### Posibles causas
- ausencia de sistema CRM
- falta de automatización
- procesos manuales

#### Complejidad
- media (requiere integración de sistemas y procesos)

---

## 3.4 Seguridad y Monitoreo

### Riesgos en IoT y refrigeración conectada

#### Problema
- dispositivos conectados vulnerables a ataques

#### Impacto
- interrupción de operación
- manipulación de equipos
- pérdida de datos

#### Posibles causas
- falta de segmentación de red
- dispositivos sin actualizaciones
- credenciales débiles
- ausencia de monitoreo continuo

#### Complejidad
- alta (ciberseguridad + IoT)

---

## 3.5 Innovación y Tecnología

### Falta de integración tecnológica

#### Problema
- no se utilizan tecnologías modernas (IoT, Cloud, IA)

#### Impacto
- mantenimiento reactivo en vez de predictivo
- menor competitividad
- procesos ineficientes

#### Posibles causas
- falta de estrategia digital
- baja inversión tecnológica
- desconocimiento de soluciones disponibles

#### Complejidad
- media-alta (transformación digital)

---

# 4. Análisis de Causas (Enfoque Sistémico)

Los problemas identificados no son aislados, sino interdependientes.

## Causas raíz principales

### Infraestructura tecnológica limitada
- redes deficientes
- hardware obsoleto

### Falta de integración de sistemas
- sistemas aislados (silos)
- ausencia de plataformas centralizadas

### Baja madurez digital
- escasa adopción de cloud
- falta de automatización

### Deficiencias en ciberseguridad
- IoT sin protección adecuada
- falta de monitoreo activo

---

# 5. Alcance Tecnológico

Las soluciones potenciales involucran múltiples áreas:

## Redes
- rediseño LAN/WiFi
- implementación de SD-WAN
- optimización de VPN

## Cloud Computing
- migración a servicios cloud
- centralización de sistemas

## Ciberseguridad
- segmentación de red
- gestión de identidades
- monitoreo de amenazas

## IoT
- sensores inteligentes
- monitoreo en tiempo real

## Inteligencia Artificial
- mantenimiento predictivo
- análisis de datos operacionales

---

# 6. Complejidad del Problema

Nivel global: **ALTO**

Razones:
- múltiples sistemas interdependientes
- impacto en operación crítica
- necesidad de transformación digital
- integración de tecnologías avanzadas

---

# 7. Foco de Investigación (Propuesto)

## Opción 1 — Infraestructura de Red
Optimizar:
- conectividad interna
- estabilidad WiFi
- acceso a sistemas críticos

## Opción 2 — Conectividad y Acceso Remoto
Mejorar:
- VPN
- acceso de técnicos
- disponibilidad de sistemas

## Opción 3 — Transformación Digital
Implementar:
- IoT
- cloud
- IA para mantenimiento predictivo

## Opción 4 — Experiencia del Cliente
Desarrollar:
- sistema CRM integrado
- omnicanalidad
- automatización de atención

## Opción 5 — Ciberseguridad
Fortalecer:
- seguridad en IoT
- monitoreo de red
- control de accesos

---

# 8. Recomendación Estratégica

Foco sugerido:

**"Optimización de infraestructura de red y adopción de tecnologías cloud para habilitar mantenimiento predictivo y mejorar la conectividad operacional."**

Justificación:
- aborda múltiples problemas simultáneamente
- mejora eficiencia operativa
- habilita innovación futura
- reduce riesgos de seguridad

---
# Como solucionar???

# 1. Soluciones de Conectividad Interna (LAN / WiFi)  
  
## Problema  
Red inestable y zonas con baja señal.  
  
## Soluciones  
  
### Rediseño de red WiFi (Site Survey)  
- realizar estudio de cobertura (heatmap)  
- identificar zonas muertas  
- redistribuir access points  
  
### Implementación de WiFi empresarial  
- uso de Access Points gestionados (controlador central)  
- estándares modernos (WiFi 6 / 6E)  
  
### Segmentación de red (VLANs)  
- separar tráfico:  
- administrativo  
- IoT (refrigeración)  
- invitados  
  
### Mejora de infraestructura cableada  
- uso de switches gestionables (Layer 2/3)  
- cableado estructurado certificado (Cat6 o superior)

# 2. Soluciones de Conectividad entre Sucursales  
  
## Problema  
VPN lenta, inestable o insegura.  
  
## Soluciones  
  
### Implementación de SD-WAN  
- optimiza tráfico entre sucursales  
- prioriza aplicaciones críticas  
- balanceo de carga entre enlaces  
  
### Modernización de VPN  
- uso de protocolos seguros:  
- IPsec  
- SSL VPN  
- autenticación multifactor (MFA)  
  
### Redundancia de enlaces  
- múltiples proveedores de internet (ISP)  
- failover automático  
  
### Uso de servicios Cloud  
- migrar sistemas a nube para acceso centralizado  
- reducir dependencia de VPN tradicional

## Problema  
Canales de comunicación no integrados.  
  
## Soluciones  
  
### Implementación de CRM omnicanal  
- integración de:  
- teléfono  
- correo  
- WhatsApp  
- chat web  
  
### Sistema de tickets  
- centraliza solicitudes de clientes  
- evita duplicaciones  
- seguimiento en tiempo real  
  
### Automatización (Chatbots)  
- respuestas automáticas  
- clasificación de solicitudes  
  
### Integración con ERP  
- vincular solicitudes con:  
- órdenes de servicio  
- historial de clientes

# 4. Soluciones de Seguridad e IoT  
  
## Problema  
Riesgos en dispositivos conectados (refrigeración).  
  
## Soluciones  
  
### Segmentación de red para IoT  
- red independiente para dispositivos  
- aislamiento de sistemas críticos  
  
### Implementación de Zero Trust  
- verificación continua de dispositivos y usuarios  
- acceso mínimo necesario  
  
### Gestión de dispositivos IoT  
- actualización de firmware  
- credenciales seguras  
- inventario de dispositivos  
  
### Monitoreo de seguridad (SIEM)  
- detección de anomalías  
- alertas en tiempo real  
  
### Firewalls de nueva generación (NGFW)  
- inspección profunda de tráfico  
- control de aplicaciones

# 5. Soluciones de Innovación Tecnológica
## Problema  
Falta de uso de tecnologías modernas.  
  
## Soluciones  
  
### Implementación de IoT inteligente  
- sensores en equipos de refrigeración  
- monitoreo en tiempo real:  
- temperatura  
- consumo energético  
- estado operativo  
  
### Mantenimiento predictivo con IA  
- análisis de datos históricos  
- detección de fallas antes de ocurrir  
  
### Migración a Cloud  
- sistemas ERP en la nube  
- almacenamiento centralizado  
- acceso remoto seguro  
  
### Analítica de datos (Big Data)  
- optimización de operaciones  
- toma de decisiones basada en datos

# 6. Priorización de Implementación  
  
## Corto Plazo  
- optimización WiFi  
- mejora VPN  
- implementación de CRM básico  
  
## Mediano Plazo  
- SD-WAN  
- segmentación de red  
- monitoreo de seguridad  
  
## Largo Plazo  
- IoT + IA  
- migración completa a cloud  
- automatización avanzada  
  
---  
  
# 7. Arquitectura Recomendada  
  
## Modelo híbrido  
- infraestructura local + cloud  
  
Incluye:  
- red segmentada (VLANs)  
- acceso remoto seguro  
- servicios cloud centralizados  
- monitoreo continuo  
  
---  
  
# 8. Impacto Esperado  
  
## Operacional  
- mayor eficiencia  
- menor tiempo de respuesta  
  
## Técnico  
- alta disponibilidad  
- mejor rendimiento  
  
## Seguridad  
- menor riesgo de ciberataques  
  
## Negocio  
- mejor experiencia del cliente  
- mayor competitividad  
  
---