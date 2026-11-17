# PR-LAB-016 — Laboratorio 3: permisos, política de contraseñas, bcrypt, cifrado Fernet, hardening SSH, usuarios y exposición

**Dominio:** D01/D07 · **Enfoque:** Defensivo

| Campo | Descripción |
|---|---|
| Identificador | PR-LAB-016 |
| Nombre y versión | Laboratorio 3 (hardening) · v1.0 · nov-2026 · primera versión |
| Objetivo | Aplicar y justificar controles de endurecimiento sobre permisos, credenciales, cifrado y exposición. |
| Dominio y fase | D01/D07 · Fase 05 Mitigación |
| Roles | Estudiante (Blue), docente (revisor). |
| Entorno y autorización | Kali Linux en VM propia (VirtualBox/VMware), red host-only aislada de Internet; autorización: actividad académica dirigida por el docente, objetivo propio. |
| Entradas | Archivo con permisos 777, política de contraseñas, comparación MD5/bcrypt, informe.txt, sshd_config y /etc/passwd. |
| Procedimiento | Permisos 777→600; política de complejidad; MD5 vs. bcrypt; cifrado simétrico Fernet y prueba con clave incorrecta; hardening de SSH (PermitRootLogin no, PasswordAuthentication no, PermitEmptyPasswords no, X11Forwarding no) validando con sshd -t; auditoría de usuarios (UID 0, shells); tabla de mitigación por puerto. |
| Evidencias | Respuestas y salidas en Laboratorio_3.docx. |
| Criterio de aceptación | Cada control se aplica y se explica el riesgo que reduce; el descifrado con clave errónea falla (InvalidToken). |
| Análisis defensivo | bcrypt usa salt aleatorio; solo cuentas humanas con shell interactiva; FTP/Telnet sustituidos por SFTP/SSH; RDP tras VPN; MySQL en 127.0.0.1. |
| Resultado | Ejecutado y documentado; tabla de mitigación por puerto en el Anexo D. |
