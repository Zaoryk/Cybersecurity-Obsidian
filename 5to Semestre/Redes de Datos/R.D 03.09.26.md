Profesor: Eduardo Hernán Zúñiga González

# Redes de Datos

## 1. Fundamentos de Comunicación y Protocolos

- **Protocolo:** Descripción formal de reglas y convenciones que rigen la comunicación entre dispositivos. Determinan el formato, sincronización, secuencia y control de errores.
    
- **Elementos Clave:** Emisor (Tx), Receptor (Rx), Mensaje y Medio .
    
- **Aspectos Definidos:** Direccionamiento (MAC, IP), método de acceso al medio, control de flujo y tiempos de espera (keepalive/ack) .
    

## 2. Modelos de Referencia: OSI vs. TCP/IP

Los modelos dividen la comunicación en capas para facilitar el diseño, aprendizaje y compatibilidad.

Modelo OSI (7 Capas)

1. **Aplicación (7):** Interfaz para aplicaciones de red (HTTP, DNS).
    
2. **Presentación (6):** Formato de datos (PDF, MP3, JPG), compresión y cifrado .
    
3. **Sesión (5):** Administra el inicio y fin de diálogos.
    
4. **Transporte (4):** Segmentación y reensamblaje. Usa **números de puerto**.
    
5. **Red (3):** Determinación de rutas y direccionamiento lógico (**IP**). Dispositivos: Routers .
    
6. **Enlace de Datos (2):** Comunicación local mediante direcciones **MAC**. Dispositivos: Switch .
    
7. **Física (1):** Transmisión de bits por el medio físico. Dispositivos: Hubs, módems.
    

Modelo TCP/IP (4 Capas)

- **Aplicación:** Equivale a las capas 5, 6 y 7 de OSI.
    
- **Transporte:** Segmentos (TCP) o Datagramas (UDP).
    
- **Internet:** Paquetes IP.
    
- **Acceso a la Red:** Tramas y bits.
    

## 3. Conceptos de Transmisión y Conmutación

- **Segmentación:** Dividir el flujo de datos en PDU (Protocol Data Unit).
    
- **Encapsulamiento:** Proceso donde cada capa agrega un encabezado (header) con información de control.
    
- **Tipos de Conmutación:**
    
    - **De Circuitos:** Camino dedicado y fijo (ej. telefonía antigua). Ineficiente para datos por no poder multiplexar .
        
    - **De Paquetes:** La información se divide en paquetes que pueden seguir rutas distintas. Permite **multiplexación** .
        
- **Modos de Comunicación:**
    
    - **Unicast:** De uno a uno.
        
    - **Multicast:** De uno a un grupo.
        
    - **Broadcast:** De uno a todos.
        

## 4. Funcionamiento del Switch y Tabla CAM

- **Tabla CAM (o MAC):** Base de datos que relaciona direcciones MAC con interfaces físicas del switch.
    
- **Procesos del Switch:**
    
    1. **Inundación (Flooding):** Si la MAC destino es desconocida, envía la trama por todos los puertos.
        
    2. **Aprendizaje:** Registra la MAC origen de las tramas entrantes en la tabla.
        
    3. **Filtrado/Reenvío:** Una vez conocida la MAC, envía solo al puerto correspondiente (Unicast).
        
- **Aging Time:** Las entradas dinámicas expiran por defecto tras 300 segundos.
    

## 5. Acceso al Medio y Multiplexación

- **CSMA/CD:** Mecanismo para detectar y manejar colisiones en redes Ethernet de medio común .
    
- **Multiplexación:** Técnica para transmitir varias señales por un solo medio.
    
    - **FDM (Frecuencia):** Divide el espectro en canales (ej. WiFi, Radio).
        
    - **TDM (Tiempo):** Divide el uso del medio en ranuras temporales (ej. Ethernet, Telefonía digital).
        

6. Tamaños y Clasificación de Redes

- **PAN:** Área personal (~10 mts), ej. Bluetooth.
- **LAN:** Área local (hasta 1 km), ej. Red de oficina o SOHO.
- **MAN:** Área metropolitana (una ciudad), ej. MetroEthernet.
- **WAN:** Área amplia (distancias superiores), conecta sucursales a través de un ISP.

---