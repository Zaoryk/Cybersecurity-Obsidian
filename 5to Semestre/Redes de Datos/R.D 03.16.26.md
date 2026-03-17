# Redes de Datos — Características y Tamaños de una Red

## 1. Concepto de Red de Datos

Una **red de datos** es un conjunto de dispositivos interconectados que pueden comunicarse entre sí para intercambiar información y compartir recursos.

Estos dispositivos pueden incluir:

- computadores
- servidores
- teléfonos
- impresoras
- dispositivos IoT
- sistemas industriales

Las redes permiten que la información viaje de un punto a otro utilizando **protocolos de comunicación** que definen cómo se transmiten, reciben y procesan los datos.

### Funciones principales de una red
- intercambio de información
- acceso a recursos compartidos
- comunicación entre usuarios
- acceso a servicios en internet
- centralización de datos

### Ejemplo práctico
En una empresa, los empleados pueden:

- acceder a archivos en un servidor central
- imprimir documentos en una impresora compartida
- utilizar aplicaciones alojadas en servidores internos
- conectarse a internet mediante la red corporativa.

---

# 2. Componentes de una Red

Una red se compone de diferentes elementos que permiten su funcionamiento.

## Dispositivos finales (End Devices)

Son los dispositivos que utilizan los usuarios para enviar o recibir información.

Ejemplos:

- computadores
- laptops
- smartphones
- tablets
- impresoras de red
- cámaras IP

Estos dispositivos generan o consumen datos dentro de la red.

---

## Dispositivos intermediarios

Son equipos que gestionan el tráfico de red y permiten que los datos lleguen a su destino.

Ejemplos:

### Router
- conecta redes diferentes
- determina la mejor ruta para enviar datos
- permite acceso a internet.

### Switch
- conecta dispositivos dentro de una misma red local
- envía datos únicamente al dispositivo destino.

### Access Point
- permite conectar dispositivos inalámbricos a la red.

### Firewall
- filtra tráfico de red para proteger sistemas.

---

## Medios de transmisión

Son los canales por donde viajan los datos.

Tipos principales:

### Cableado
- cable Ethernet
- fibra óptica
- cable coaxial

### Inalámbrico
- WiFi
- Bluetooth
- redes celulares (4G, 5G)

---

# 3. Características Fundamentales de una Red

Las redes modernas deben cumplir con ciertas características para garantizar su funcionamiento eficiente.

---

## 3.1 Tolerancia a fallos

La **tolerancia a fallos** es la capacidad de una red para continuar funcionando incluso cuando uno de sus componentes falla.

Esto se logra mediante:

- redundancia de enlaces
- múltiples rutas de comunicación
- servidores duplicados
- sistemas de respaldo

### Ejemplo
Si un enlace de red falla, el sistema puede redirigir el tráfico por otro camino.

### Importancia
Evita interrupciones del servicio y garantiza disponibilidad.

---

## 3.2 Escalabilidad

La **escalabilidad** es la capacidad de una red para crecer sin afectar significativamente su rendimiento.

Una red escalable permite:

- agregar nuevos dispositivos
- aumentar el número de usuarios
- expandir infraestructura

sin necesidad de rediseñar completamente la red.

### Ejemplo
Una empresa que pasa de 50 a 500 empleados debe poder ampliar su red fácilmente.

---

## 3.3 Calidad de servicio (QoS)

La **Quality of Service (QoS)** es la capacidad de priorizar ciertos tipos de tráfico en la red.

Esto es importante para aplicaciones sensibles a la latencia como:

- videollamadas
- VoIP
- streaming
- juegos online

QoS permite:

- reducir retrasos
- evitar pérdida de paquetes
- mantener calidad de transmisión.

---

## 3.4 Seguridad

La seguridad en redes protege los sistemas contra accesos no autorizados y ataques.

Incluye:

- autenticación de usuarios
- cifrado de datos
- firewalls
- detección de intrusos
- segmentación de red.

La seguridad es fundamental porque las redes transportan información sensible.

---

# 4. Tipos de Redes Según su Tamaño

Las redes pueden clasificarse según su **alcance geográfico**.

---

## 4.1 PAN — Personal Area Network

Una **PAN** es una red personal de corto alcance.

### Características
- alcance aproximado de 1 a 10 metros
- conecta dispositivos personales
- generalmente inalámbrica.

### Tecnologías comunes
- Bluetooth
- NFC
- USB

### Ejemplo
Un teléfono conectado a audífonos Bluetooth.

---

## 4.2 LAN — Local Area Network

Una **LAN** es una red que conecta dispositivos dentro de un área limitada.

### Características
- alta velocidad de transmisión
- baja latencia
- controlada por una sola organización.

### Ejemplos
- redes domésticas
- redes de oficinas
- redes escolares

### Tecnologías usadas
- Ethernet
- WiFi.

---

## 4.3 MAN — Metropolitan Area Network

Una **MAN** conecta múltiples redes dentro de una ciudad.

### Características
- mayor alcance que una LAN
- utilizada por proveedores de telecomunicaciones
- conecta campus o edificios distribuidos.

### Ejemplo
La red de fibra óptica de una ciudad.

---

## 4.4 WAN — Wide Area Network

Una **WAN** es una red que conecta dispositivos en grandes distancias geográficas.

### Características
- cubre países o continentes
- utiliza infraestructura de telecomunicaciones.

### Ejemplo más grande
Internet.

Las WAN utilizan tecnologías como:

- enlaces satelitales
- fibra óptica submarina
- redes celulares
- MPLS.

---

# 5. Redes Empresariales

Las empresas implementan redes según sus necesidades operativas.

---

## Redes pequeñas (SOHO)

SOHO significa **Small Office / Home Office**.

### Características
- hasta 10–15 dispositivos
- infraestructura simple
- un router conectado a internet
- conexión WiFi y Ethernet.

### Uso común
- pequeñas empresas
- oficinas domésticas.

---

## Redes de campus

Utilizadas por organizaciones grandes.

### Características
- múltiples edificios
- miles de dispositivos
- segmentación por departamentos
- servidores internos.

Ejemplos:
- universidades
- hospitales
- grandes empresas.

---

## Redes empresariales distribuidas

Organizaciones con múltiples sedes geográficas.

### Características
- sucursales conectadas mediante WAN
- centros de datos centrales
- uso de VPN corporativas.

---

# 6. Centros de Datos

Un **data center** es una instalación que alberga infraestructura crítica de TI.

Incluye:

- servidores
- almacenamiento
- redes
- sistemas de respaldo energético.

Los centros de datos permiten que organizaciones ejecuten:

- aplicaciones empresariales
- sistemas financieros
- servicios en la nube
- plataformas digitales.

---

# 7. Virtualización y Redes Modernas

Las redes modernas utilizan virtualización para mejorar eficiencia.

## Virtualización de servidores
Permite ejecutar múltiples sistemas operativos en un mismo hardware.

## Redes definidas por software (SDN)
Permiten administrar la red mediante software.

Beneficios:

- mayor flexibilidad
- automatización
- control centralizado.

---

# 8. Conceptos Clave

## Latencia
Tiempo que tarda un paquete de datos en viajar desde origen a destino.

## Ancho de banda
Cantidad máxima de datos que pueden transmitirse en un enlace.

## Paquete de datos
Unidad básica de información transmitida en una red.

## Protocolo de red
Conjunto de reglas que define cómo se comunican los dispositivos.

Ejemplos:
- TCP
- IP
- HTTP
- FTP.

---

# Idea Clave

Las redes modernas permiten conectar millones de dispositivos y servicios a nivel global.

Su diseño debe considerar:

- **rendimiento**
- **seguridad**
- **escalabilidad**
- **confiabilidad**

para garantizar comunicaciones eficientes en la era digital.

---

# Comandos de Cisco Packet Tracer

Modo Usuario > 
Modo Privilegiado #
Modo Configuracion Global (config)#

- Switch> Enable - Modo Priviliegado
- Switch# Disable Modo Usuario
- Switch# Configure terminal
- Switch(Config)# Hostname sw-502
- sw-502(config)# exit
- sw-502#show mac-address-table

PC
- C:\> Ping
