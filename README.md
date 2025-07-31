#  Red Team CTF: Proyecto Final – Simulación de Compromiso en Infraestructura NASA

##  Descripción General

Este proyecto es una máquina tipo CTF de enfoque Red Team, desarrollada como parte del proyecto final de mi especialización en ciberseguridad. Simula un entorno realista en el que un atacante externo intenta comprometer un servidor de la NASA, el cual alberga archivos confidenciales vinculados a investigaciones científicas clasificadas y de dudosa ética.

El propósito del escenario es evaluar técnicas de intrusión, persistencia y escalada de privilegios dentro de un entorno corporativo crítico, siguiendo una estructura ofensiva organizada.

---

##  Objetivos del Simulacro

- Realizar reconocimiento y explotación de servicios públicos (FTP, HTTP, SSH).
- Obtener acceso inicial y moverse lateralmente dentro del sistema.
- Escalar privilegios desde `www-data` hasta el usuario `root`.
- Identificar archivos sensibles y recolectar múltiples flags ocultas.
- Simular un compromiso completo de un entorno crítico realista.

---

##  Habilidades y Técnicas Aplicadas

- **Enumeración activa** con Nmap, FFUF y análisis de metadatos.
- **Explotación de servicios mal configurados** como FTP abierto y paneles web vulnerables.
- **Cracking de archivos protegidos** con herramientas como `fcrackzip`, `hashcat` y `john`.
- **Inyección SQL y subida de archivos maliciosos** para obtener shells remotas.
- **Escalada de privilegios** a través de usuarios mal configurados y binarios con permisos de sudo.
- **Análisis de archivos ofuscados** (Magic Numbers, base64, extensiones falsas).

---

##  Servicios y Vulnerabilidades Simuladas

| Servicio | Vulnerabilidad simulada |
|----------|--------------------------|
| FTP      | Acceso anónimo, fuga de archivos |
| HTTP     | Fuzzing de directorios, metadata, subida de reverse shell |
| MySQL    | Inyección SQL para obtención de credenciales |
| SSH      | Claves simétricas expuestas para acceso sin contraseña |
| Sistema  | Usuarios con permisos sudo sin contraseña, archivos `shadow` accesibles |
| Archivos | Manipulación de extensiones y compresión para ocultar datos |

