# Red Team CTF: Proyecto Final especialización en Ciberseguridad en Entornos de las Tecnologías de la Información  – Simulación de Compromiso en Infraestructura NASA

## Descripción General

Este proyecto corresponde al trabajo final de mi especialización en ciberseguridad. Consiste en una máquina tipo CTF con enfoque Red Team que simula un escenario realista donde un atacante externo busca comprometer un servidor de la NASA. Este servidor contiene información altamente confidencial vinculada a investigaciones científicas clasificadas y de ética cuestionable.

El propósito principal es poner en práctica técnicas de intrusión, persistencia y escalada de privilegios dentro de un entorno corporativo crítico, replicando un ataque organizado en una infraestructura sensible.

---

## Objetivos del Simulacro

- Realizar reconocimiento y explotación de servicios abiertos (FTP, HTTP, SSH).
- Obtener acceso inicial y moverse lateralmente dentro del sistema.
- Escalar privilegios desde el usuario `www-data` hasta `root`.
- Identificar archivos sensibles y recolectar múltiples flags ocultas.
- Completar el compromiso total de un entorno crítico simulado.

---

## Técnicas y Habilidades Aplicadas

- **Enumeración activa:** Uso de herramientas como Nmap y FFUF, además del análisis de metadatos.
- **Explotación de servicios mal configurados:** Acceso anónimo en FTP y paneles web vulnerables.
- **Cracking de archivos protegidos:** Uso de `fcrackzip`, `hashcat` y `john`.
- **Inyección SQL y subida de archivos maliciosos:** Para obtener shells remotas.
- **Escalada de privilegios:** Aprovechando usuarios con permisos sudo sin contraseña y binarios inseguros.
- **Análisis de archivos ofuscados:** Detección mediante Magic Numbers, base64 y extensiones falsas.

---

## Servicios y Vulnerabilidades Simuladas

| Servicio | Vulnerabilidad Simulada                          |
| -------- | ----------------------------------------------- |
| FTP      | Acceso anónimo y fuga de archivos sensibles     |
| HTTP     | Fuzzing de directorios, análisis de metadata y subida de reverse shells |
| MySQL    | Inyección SQL para obtención de credenciales    |
| SSH      | Claves expuestas que permiten acceso sin contraseña |
| Sistema  | Usuarios con permisos sudo sin contraseña y archivos `shadow` accesibles |
| Archivos | Manipulación de extensiones y compresión para ocultar datos |

Si deseas explotar la maquina por ti mismo en el siguiente link la puedes descargar : https://drive.google.com/drive/folders/1YFV19nsgo-IdN9ijlZt3_00LJmI0o9Lj?usp=drive_link
