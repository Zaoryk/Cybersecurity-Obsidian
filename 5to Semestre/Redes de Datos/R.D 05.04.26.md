| **Categoría**               | **Comando**                      | **Descripción**                                                      |
| --------------------------- | -------------------------------- | -------------------------------------------------------------------- |
| **Seguridad de Acceso**     | `enable secret [clave]`          | Configura contraseña con hash MD5 para modo privilegiado.            |
|                             | `password [clave]`               | Define la contraseña de línea (Consola o VTY).                       |
|                             | `login`                          | Habilita la solicitud de contraseña en la línea.                     |
|                             | `username [user] secret [clave]` | Crea un usuario local con contraseña cifrada.                        |
|                             | `login local`                    | Indica a las líneas que usen la base de datos de usuarios local.     |
| **Cifrado General**         | `service password-encryption`    | Cifra todas las contraseñas de texto plano en la configuración.      |
| **Mensajes de Aviso**       | `banner motd #[mensaje]#`        | Configura el mensaje de advertencia legal al acceder.                |
| **Configuración de Líneas** | `line console 0`                 | Entra a la configuración del puerto de consola física.               |
|                             | `line vty 0 4` (o `0 15`)        | Entra a la configuración de acceso remoto (Telnet/SSH).              |
|                             | `logging synchronous`            | Sincroniza mensajes de consola para no interrumpir la escritura.     |
| **Gestión de DNS**          | `no ip domain-lookup`            | Desactiva la búsqueda DNS (evita bloqueos por errores de escritura). |
|                             | `ip name-server [IP]`            | Define la dirección de un servidor DNS.                              |
| **Interfaces y IP**         | `interface [tipo/número]`        | Entra al modo de configuración de una interfaz específica.           |
|                             | `ip address [IP] [Máscara]`      | Asigna dirección IP y máscara de subred.                             |
|                             | `description [texto]`            | Agrega una etiqueta descriptiva a la interfaz.                       |
|                             | `no shutdown`                    | Enciende la interfaz (por defecto están apagadas en routers).        |
|                             | `ip default-gateway [IP]`        | Define la puerta de enlace en un Switch.                             |
| **Verificación**            | `show ip interface brief`        | Muestra resumen de estado y direcciones IP de interfaces.            |
|                             | `show running-config`            | Muestra la configuración actual en RAM.                              |
|                             | `show ip route`                  | Muestra la tabla de enrutamiento.                                    |
| **Mantenimiento**           | `write` o `copy run start`       | Guarda la configuración actual en la NVRAM.                          |
|                             | `reload`                         | Reinicia el equipo.                                                  |
|                             | `erase startup-config`           | Borra la configuración de respaldo (inicio).                         |