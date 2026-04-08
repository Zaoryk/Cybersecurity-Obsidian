# Redes de Datos — Sistema Binario, Direccionamiento IP y Medios Guiados

## 1. Sistema Binario

### Definición
Sistema numérico base 2 utilizado en redes y computación.

### Características
- Solo usa: 0 y 1
- Cada dígito = bit
- 8 bits = 1 byte

---

## 2. Conversión Binario ↔ Decimal

### Tabla de valores

| Potencia | Valor |
|----------|------|
| 2⁷ | 128 |
| 2⁶ | 64 |
| 2⁵ | 32 |
| 2⁴ | 16 |
| 2³ | 8 |
| 2² | 4 |
| 2¹ | 2 |
| 2⁰ | 1 |

---

### Ejemplo

| Binario | Cálculo | Decimal |
|--------|--------|--------|
| 11000000 | 128+64 | 192 |
| 10101000 | 128+32+8 | 168 |

---

## 3. Dirección IP (IPv4)

### Definición
Identificador único de un dispositivo en una red.

### Estructura

| Parte | Descripción |
|------|------------|
| Red | identifica la red |
| Host | identifica dispositivo |

---

### Formato

- 32 bits (4 octetos)
- Ejemplo: 192.168.1.1

---

## 4. Clases de IP

| Clase | Rango | Uso |
|------|------|----|
| A | 1.0.0.0 – 126.0.0.0 | redes grandes |
| B | 128.0.0.0 – 191.255.0.0 | medianas |
| C | 192.0.0.0 – 223.255.255.0 | pequeñas |

---

## 5. Máscara de Subred

### Definición
Define qué parte de la IP es red y host.

---

### Ejemplos

| Máscara | Binario | Hosts |
|--------|--------|------|
| 255.0.0.0 | /8 | 16M |
| 255.255.0.0 | /16 | 65K |
| 255.255.255.0 | /24 | 254 |

---

## 6. Conceptos Clave IP

| Concepto | Explicación |
|----------|------------|
| IP | dirección lógica |
| MAC | dirección física |
| Gateway | salida de red |
| Broadcast | envío a todos |

---

## 7. Medios Guiados (Cableados)

### Definición
Medios físicos que transportan señales.

---

## 8. Tipos de Medios

### Par Trenzado

| Tipo | Características |
|------|---------------|
| UTP | sin blindaje |
| STP | con blindaje |

---

### Categorías

| Categoría | Velocidad |
|-----------|----------|
| Cat5 | 100 Mbps |
| Cat5e | 1 Gbps |
| Cat6 | 10 Gbps |

---

### Ventajas
- bajo costo
- fácil instalación

### Desventajas
- interferencias
- menor distancia

---

## 9. Cable Coaxial

### Características

| Elemento | Función |
|----------|--------|
| núcleo | transmite señal |
| blindaje | evita interferencias |

---

### Ventajas
- buena protección
- mayor alcance que UTP

### Desventajas
- más costoso
- menos flexible

---

## 10. Fibra Óptica (comparación necesaria)

| Tipo | Características |
|------|---------------|
| Monomodo | larga distancia |
| Multimodo | corta distancia |

---

### Ventajas
- alta velocidad
- inmune a interferencias
- gran distancia

### Desventajas
- alto costo
- instalación compleja

---

## 11. Comparación de Medios

| Medio | Velocidad | Interferencia | Costo | Distancia |
|------|----------|--------------|------|----------|
| UTP | media | alta | bajo | corta |
| Coaxial | media | media | medio | media |
| Fibra | alta | baja | alto | larga |

---

## 12. Funcionamiento en Red

### Flujo

1. Datos → binario
2. Encapsulación en paquetes
3. Transmisión por medio físico
4. Recepción y decodificación

---

## 13. Errores Comunes

| Error | Causa |
|------|------|
| IP incorrecta | mala configuración |
| red no conecta | máscara incorrecta |
| interferencia | mal cableado |
| baja velocidad | cable inadecuado |

---

## 14. Idea Clave

Todo en redes se basa en:

- binario → representación de datos
- IP → identificación
- medios → transmisión

Sin estos tres elementos no existe comunicación en red.