# Redes de Datos — Comandos IOS (Packet Tracer)

## 1. Modos del IOS (Cisco)

| Modo                     | Prompt            | Función principal                          |
|--------------------------|-------------------|--------------------------------------------|
| User EXEC                | `>`               | Comandos básicos de monitoreo              |
| Privileged EXEC          | `#`               | Acceso completo a comandos                 |
| Global Configuration     | `(config)#`       | Configuración general del dispositivo      |
| Interface Configuration  | `(config-if)#`    | Configuración de interfaces                |
| Line Configuration       | `(config-line)#`  | Configuración de acceso (console, vty)     |

---

## 2. Comandos Básicos de Navegación

| Comando         | Función |
|-----------------|--------|
| enable          | Entra a modo privilegiado (`#`) |
| disable         | Sale a modo usuario (`>`) |
| configure terminal | Entra a modo configuración global |
| exit            | Retrocede un nivel |
| end             | Vuelve directamente a modo privilegiado |
| ?               | Ayuda contextual |
| Tab             | Autocompleta comandos |

---

## 3. Configuración Inicial del Router/Switch

| Comando                         | Función |
|--------------------------------|--------|
| hostname NOMBRE                | Cambia nombre del dispositivo |
| no ip domain-lookup            | Evita búsquedas DNS incorrectas |
| enable secret PASSWORD         | Contraseña modo privilegiado |
| service password-encryption    | Encripta contraseñas |

---

## 4. Configuración de Interfaces

| Comando                        | Función |
|--------------------------------|--------|
| interface fa0/0                | Entra a interfaz específica |
| ip address IP MASCARA          | Asigna dirección IP |
| no shutdown                    | Activa la interfaz |
| shutdown                       | Desactiva la interfaz |
| description TEXTO              | Agrega descripción |

---

## 5. Verificación (Show Commands)

| Comando                 | Función |
|------------------------|--------|
| show running-config     | Muestra configuración actual |
| show startup-config     | Configuración guardada |
| show ip interface brief| Estado de interfaces |
| show ip route           | Tabla de rutas |
| show version            | Información del dispositivo |

---

## 6. Guardar Configuración

| Comando                    | Función |
|----------------------------|--------|
| copy running-config startup-config | Guarda configuración |
| write memory               | Guarda configuración (atajo) |

---

## 7. Configuración de Contraseñas

### Consola

| Comando |
|--------|
| line console 0 |
| password PASSWORD |
| login |

---

### Acceso remoto (Telnet/SSH)

| Comando |
|--------|
| line vty 0 4 |
| password PASSWORD |
| login |

---

## 8. Configuración de Switch

### VLAN Básica

| Comando |
|--------|
| vlan 10 |
| name Ventas |

---

### Asignar VLAN a puerto

| Comando |
|--------|
| interface fa0/1 |
| switchport mode access |
| switchport access vlan 10 |

---

## 9. Direccionamiento IP

### Conceptos clave

| Concepto     | Explicación |
|--------------|------------|
| IP           | Identificador único de dispositivo |
| Máscara      | Define red y host |
| Gateway      | Puerta de salida de la red |

---

## 10. Comandos de Conectividad

| Comando        | Función |
|----------------|--------|
| ping IP        | Verifica conectividad |
| traceroute IP  | Muestra ruta hacia destino |

---

## 11. Tabla de Flujo Básico de Configuración

| Paso | Acción |
|------|-------|
| 1 | enable |
| 2 | configure terminal |
| 3 | hostname |
| 4 | configurar interfaces |
| 5 | asignar IP |
| 6 | no shutdown |
| 7 | guardar configuración |

---

## 12. Cómo Funciona Todo (Resumen Técnico)

### Flujo de funcionamiento

1. Dispositivo recibe datos
2. Usa IP para identificar destino
3. Consulta tabla de rutas
4. Envía paquetes por interfaz correcta
5. Switch usa MAC para entregar en LAN

---

## 13. Conceptos Clave para Pruebas

- Router → capa 3 (IP)
- Switch → capa 2 (MAC)
- VLAN → segmentación de red
- IP → identificación lógica
- MAC → identificación física

---

## 14. Errores Comunes

| Error | Causa |
|------|------|
| No hay conexión | falta `no shutdown` |
| IP incorrecta | mala máscara |
| No responde ping | gateway mal configurado |
| No guarda config | no usar `copy run start` |

