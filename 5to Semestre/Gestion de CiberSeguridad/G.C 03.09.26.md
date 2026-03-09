# Gestión de Ciberseguridad

## Fechas de Pruebas
- **30.03** — 15% — 1era Prueba Sumativa (Selección Múltiple)
- **27.04** — 30% — 2nda Prueba Sumativa (Informe taller)
- **25.05** — 30% — 3era Prueba Sumativa (Informe taller)
- **08.06 – 22.06** — 25% — 4ta Prueba Sumativa (Presentación)

### Examen
- **No obligatorio**

---

## Seguridad de la Información

### Modelo CID
**CID = Confidencialidad, Integridad, Disponibilidad**

- **Confidencialidad**  
  Restringe el acceso a la información únicamente a personal autorizado.  
  Se implementa comúnmente mediante **cifrado**.

- **Integridad**  
  Garantiza que los datos sean **exactos y no hayan sido alterados sin autorización**.

- **Disponibilidad**  
  Asegura que los sistemas y datos estén **accesibles y operativos cuando se necesiten**.

---

## Criptografía y Estándares

### AES-GCM
**AES-GCM (Advanced Encryption Standard – Galois/Counter Mode)**

- Algoritmo de **cifrado simétrico**
- Proporciona:
  - **Confidencialidad**
  - **Integridad de los datos**
- Usos comunes:
  - **TLS**
  - **VPNs**
  - Seguridad de datos en **.NET**

---

### FIPS
**FIPS (Federal Information Processing Standards)**

- Estándares definidos por **NIST (National Institute of Standards and Technology)** de EE. UU.
- Aplicados a **seguridad informática y criptografía**
- Garantizan validación de:
  - **Módulos criptográficos**
  - Algoritmos de cifrado (**AES**, **SHA**)
  - **Protocolos de seguridad**

---

## Entropía y Seguridad de Contraseñas

- **NIST recomienda:**  
  **112 bits de entropía** para seguridad criptográfica.

Notas relacionadas:

- `(0-9)`
- `E = log(2)10 ≈ 3,5`
- `SAS`

*(Notas matemáticas posiblemente relacionadas con cálculo de entropía)*

---

## Seguridad de Contraseñas

### Salt
- Datos **aleatorios** añadidos a una contraseña **antes de aplicar hashing**.
- Previene ataques como:
  - **Rainbow tables**
  - **Fuerza bruta precomputada**

### Pepper
- **Cadena secreta y aleatoria** añadida a la contraseña antes del hashing.
- Diferencia clave:
  - **No se almacena en la base de datos**
  - Se guarda **separadamente** (ej: en el servidor o HSM).

### Nonce
**Nonce = Number Used Once**

- Valor **aleatorio o arbitrario**
- Diseñado para **usarse una sola vez**
- Utilizado en:
  - **Protocolos criptográficos**
  - **Autenticación**
  - **Prevención de ataques de repetición (replay attacks)**