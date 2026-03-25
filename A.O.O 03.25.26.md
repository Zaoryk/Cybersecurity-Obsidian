# Redes de Datos — Configuración + Seguridad (Resumen Integrado)

## 1. Configuración de Dispositivos (Router/Switch)

### Flujo básico

| Paso | Comando |
|------|--------|
| 1 | enable |
| 2 | configure terminal |
| 3 | hostname NOMBRE |
| 4 | interface fa0/0 |
| 5 | ip address IP MASCARA |
| 6 | no shutdown |
| 7 | exit |
| 8 | copy running-config startup-config |

---

## 2. Configuración de Interfaces

| Comando | Función |
|--------|--------|
| interface fa0/0 | Selecciona interfaz |
| ip address X.X.X.X X.X.X.X | Asigna IP |
| no shutdown | Activa interfaz |
| shutdown | Desactiva interfaz |

---

## 3. Verificación de Red

| Comando | Función |
|--------|--------|
| show ip interface brief | Estado interfaces |
| show running-config | Configuración actual |
| show ip route | Tabla de rutas |
| ping IP | Verifica conectividad |
| traceroute IP | Ruta de paquetes |

---

## 4. VLAN (Segmentación de Red)

### Crear VLAN

| Comando |
|--------|
| vlan 10 |
| name Ventas |

---

### Asignar VLAN

| Comando |
|--------|
| interface fa0/1 |
| switchport mode access |
| switchport access vlan 10 |

---

## 5. Seguridad en Redes

### Conceptos

| Concepto | Definición |
|----------|-----------|
| Amenaza | Posible ataque |
| Vulnerabilidad | Debilidad |
| Riesgo | Probabilidad de explotación |

---

## 6. Triada CID

| Elemento | Función |
|----------|--------|
| Confidencialidad | Solo acceso autorizado |
| Integridad | Datos no alterados |
| Disponibilidad | Acceso continuo |

---

## 7. Tipos de Ataques

| Ataque | Descripción |
|-------|------------|
| Malware | Software malicioso |
| Phishing | Engaño al usuario |
| DDoS | Saturación de red |
| MitM | Intercepción |
| Ransomware | Secuestro de datos |

---

## 8. Vulnerabilidades Comunes

| Vulnerabilidad | Ejemplo |
|---------------|--------|
| Mala configuración | puertos abiertos |
| Software desactualizado | sin parches |
| Contraseñas débiles | fácil acceso |
| Inyección | SQL, XSS |

---

## 9. Seguridad en Dispositivos Cisco

### Contraseñas

| Comando |
|--------|
| enable secret PASSWORD |
| line console 0 |
| password PASSWORD |
| login |

---

### Acceso remoto

| Comando |
|--------|
| line vty 0 4 |
| password PASSWORD |
| login |

---

## 10. Buenas Prácticas de Seguridad

- usar contraseñas seguras
- actualizar sistemas
- segmentar red (VLAN)
- usar firewall
- monitorear red

---

## 11. Criptografía Básica

| Concepto | Función |
|----------|--------|
| AES | cifrado simétrico |
| Hash | integridad |
| Salt | aleatoriedad en contraseñas |
| Pepper | secreto adicional |
| Nonce | uso único |

---

## 12. Flujo de Comunicación en Red

1. Dispositivo envía datos
2. Se encapsulan en paquetes
3. Se asigna IP destino
4. Router decide ruta
5. Switch entrega por MAC

---

## 13. Resolución de Problemas

| Problema | Solución |
|----------|--------|
| No hay red | revisar IP |
| No hay conexión | no shutdown |
| No responde ping | gateway |
| VLAN incorrecta | revisar asignación |
