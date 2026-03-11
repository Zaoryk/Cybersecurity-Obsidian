La clase anterior fue un pinceleado, hoy es mas detallado
# Protocolos, Modelos y Características de Redes

## 1. Conceptos Fundamentales de Comunicación en Redes

La comunicación en redes de datos consiste en el intercambio de información entre dispositivos conectados mediante un medio físico o lógico. Para que esta comunicación sea posible se requieren varios elementos fundamentales.

### Elementos de la comunicación

- **Emisor (Tx)**  
  Dispositivo que envía la información.

- **Receptor (Rx)**  
  Dispositivo que recibe la información.

- **Mensaje**  
  Información que se transmite entre los dispositivos.

- **Medio de transmisión**  
  Canal físico o inalámbrico por el cual viajan los datos.

- **Protocolo**  
  Conjunto de reglas que define cómo se realiza la comunicación.

- **Ruido externo**
  Interferencias que afectan la transmisión de la señal.

- **Atenuación**
  Pérdida de potencia de la señal a medida que viaja por el medio.

---

# 2. Protocolos de Red

## Definición de Protocolo

Un **protocolo** es una descripción formal de reglas y convenciones que determinan cómo los dispositivos de red intercambian información.

Los protocolos definen:

- formato de los mensajes
- sincronización de la comunicación
- secuencia de transmisión
- control de errores
- control de flujo
- tiempos de espera

Los protocolos **no especifican cómo implementar la función**, sino **qué función debe cumplirse**, lo que los hace independientes de la tecnología utilizada.

---

## Necesidad de los protocolos

Para que dos dispositivos se comuniquen correctamente deben acordar varios aspectos.

### Aspectos definidos por los protocolos

**1. Direccionamiento**

Permite identificar a los dispositivos en una red.

Ejemplos:

- Dirección MAC
- Dirección IP
- Correo electrónico
- Número telefónico
- RUT

---

**2. Método de acceso al medio**

Determina cómo los dispositivos acceden al medio de transmisión.

Problema típico:

Si dos dispositivos transmiten simultáneamente se produce una **colisión**.

Para evitarlo se utilizan mecanismos como:

- turnos
- detección de portadora
- temporizadores aleatorios

---

**3. Control de flujo**

Permite que un dispositivo receptor controle la velocidad con que recibe datos.

Ejemplo:

Si el emisor envía datos demasiado rápido, el receptor puede solicitar:

- reducción de velocidad
- confirmación de recepción (ACK)

---

**4. Tiempos de espera**

Permite detectar fallas en la comunicación.

Si no se recibe respuesta dentro de cierto tiempo, el sistema asume que el dispositivo no está disponible.

Ejemplos de mensajes:

- keepalive
- hello
- acknowledgement (ACK)

---

# 3. Modelos de Protocolos

Para simplificar el diseño de redes, los protocolos se organizan en **capas** dentro de un modelo estructurado.

## Ventajas del modelo por capas

- Permite dividir problemas complejos en partes pequeñas
- Facilita el diseño de protocolos
- Permite modificar una capa sin afectar las demás
- Establece un lenguaje común entre fabricantes
- Facilita el aprendizaje

Cada capa utiliza los servicios de la capa inferior para realizar su función.

---

# 4. Conmutación de Paquetes

Las redes modernas utilizan el principio de **conmutación de paquetes**.

## Proceso de transmisión

1. La información se digitaliza en bits.
2. Los datos se dividen en paquetes.
3. Cada paquete recibe información adicional llamada **encabezado (header)**.
4. Los paquetes se transmiten a través de la red.
5. En el destino se eliminan los encabezados.
6. Se reconstruye la información original.

---

## Segmentación

Proceso de dividir el flujo de datos en unidades llamadas **PDU (Protocol Data Unit)**.

---

## Encapsulamiento

Cada capa del modelo agrega su propio encabezado al paquete.

Esto permite que cada paquete contenga información suficiente para:

- identificar origen
- identificar destino
- indicar tipo de datos
- controlar errores

---

# 5. Modelo TCP/IP

## Introducción

El modelo **TCP/IP** es el estándar técnico de Internet.

Fue desarrollado por el **Departamento de Defensa de Estados Unidos (DoD)**.

Su diseño buscaba una red capaz de seguir funcionando incluso bajo ataques o fallas graves.

---

## Capas del modelo TCP/IP

El modelo TCP/IP posee **4 capas principales**:

### 1. Capa de Aplicación
Proporciona servicios a las aplicaciones de usuario.

Ejemplos de protocolos:

- HTTP
- FTP
- SMTP
- DNS

---

### 2. Capa de Transporte

Responsable de:

- segmentar datos
- controlar errores
- garantizar entrega

Protocolos principales:

**TCP**

- orientado a conexión
- confiable
- retransmite paquetes perdidos

**UDP**

- no orientado a conexión
- rápido
- no garantiza entrega

---

### 3. Capa de Internet

Responsable del direccionamiento lógico y del enrutamiento.

Protocolo principal:

- IP

---

### 4. Capa de Acceso a Red

Define cómo los datos se transmiten físicamente.

Incluye tecnologías como:

- Ethernet
- WiFi

---

# 6. Modelo OSI

## Introducción

El modelo **OSI (Open Systems Interconnection)** fue creado por la organización **ISO** en los años 80.

Su objetivo fue establecer un estándar universal para la comunicación entre sistemas de diferentes fabricantes.

El modelo OSI posee **7 capas**.

---

## Capas del modelo OSI

### 7. Aplicación

Proporciona servicios de red a los programas del usuario.

Dispositivos:

- computadores
- servidores
- smartphones
- tablets

---

### 6. Presentación

Se encarga de la representación de los datos.

Funciones:

- conversión de formatos
- compresión
- cifrado

Ejemplos de formatos:

- PDF
- JPG
- MP3

---

### 5. Sesión

Administra las sesiones de comunicación entre aplicaciones.

Funciones:

- iniciar sesiones
- mantener sesiones
- finalizar sesiones

---

### 4. Transporte

Responsable de la comunicación entre aplicaciones.

Funciones:

- segmentación de datos
- reensamblaje
- control de errores
- control de flujo

Identifica aplicaciones mediante **números de puerto**.

---

### 3. Red

Encargada del **direccionamiento lógico y del enrutamiento**.

Determina la mejor ruta entre origen y destino.

---

### 2. Enlace de datos

Controla la transmisión dentro de una red local.

Funciones:

- direccionamiento MAC
- detección de errores
- control de acceso al medio

---

### 1. Física

Transmite bits a través del medio físico.

Ejemplos de medios:

- cables de cobre
- fibra óptica
- señales inalámbricas

---

# 7. Redes de Medio Común

Las primeras redes Ethernet utilizaban un **medio compartido**.

Todos los dispositivos estaban conectados al mismo cable.

Si un equipo transmitía, **todos recibían la señal**.

Esto generaba problemas como:

- colisiones
- saturación del canal

---

# 8. CSMA/CD

Mecanismo usado para manejar colisiones en redes Ethernet antiguas.

## Funcionamiento

1. **Carrier Sense**
   El dispositivo verifica si el medio está ocupado.

2. **Multiple Access**
   Varios dispositivos pueden acceder al mismo medio.

3. **Collision Detection**
   Si ocurre una colisión, se detecta la interferencia.

4. **Señal de congestión (Jam)**
   Se notifica a todos los nodos.

5. **Temporizadores aleatorios**
   Cada equipo espera un tiempo antes de retransmitir.

Actualmente este mecanismo casi no se usa debido al uso de switches y full-duplex.

---

# 9. Conmutación

La conmutación consiste en establecer rutas específicas para el tráfico de datos.

Ventajas:

- mayor seguridad
- mejor uso del ancho de banda
- menor congestión

Tipos principales:

- conmutación de circuitos
- conmutación de paquetes

---

# 10. Conmutación de Circuitos

Se establece un canal dedicado entre emisor y receptor.

Fases:

1. Establecimiento del circuito
2. Transmisión de datos
3. Liberación del circuito

Ejemplo clásico:

- red telefónica tradicional

Problema principal:

El canal queda ocupado aunque no se transmitan datos.

---

# 11. Conmutación de Paquetes

La información se divide en paquetes que viajan independientemente.

Ventajas:

- uso eficiente del ancho de banda
- multiplexación

Desventajas:

- mayor latencia
- variabilidad (jitter)

---

# 12. Conexiones Orientadas y No Orientadas

## Orientadas a conexión

Garantizan la entrega de los datos.

Ejemplo:

TCP

Usos:

- páginas web
- correo electrónico
- transferencia de archivos

---

## No orientadas a conexión

No garantizan entrega ni orden.

Ejemplo:

UDP

Usos:

- streaming
- VoIP
- videojuegos en línea

---

# 13. Tabla CAM

La **tabla CAM (Content Addressable Memory)** se utiliza en los switches.

Relaciona:

Dirección MAC ↔ Puerto del switch

Puede llenarse de dos formas:

- dinámica (automática)
- estática (configurada por administrador)

---

# 14. Proceso de Reenvío del Switch

Cuando un switch recibe una trama:

### Si no conoce la MAC destino

Realiza **inundación (flooding)** enviando la trama a todos los puertos.

---

### Cuando aprende las MAC

El switch puede:

- **Copiar (unicast)** → enviar solo al puerto correcto
- **Multicast** → enviar a un grupo
- **Filtrar** → descartar tráfico innecesario

---

# 15. Evolución de las Redes Ethernet

Década de 1990:

- Los **hubs** comienzan a desaparecer.
- Son reemplazados por **switches**.

También se reemplaza:

Half-duplex → Full-duplex

Esto elimina prácticamente las colisiones en redes modernas.