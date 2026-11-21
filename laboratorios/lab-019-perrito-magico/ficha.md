# PR-LAB-019 — DockerLabs · Perrito Mágico: writeup de API y CSRF

| Campo | Descripción / dato |
|---|---|
| Identificador | PR-LAB-019 |
| Nombre y versión | DockerLabs · Perrito Mágico (writeup) · v1.0 · nov-2026 · primera versión |
| Objetivo | Documentar reconocimiento y explotación de una API web vulnerable en un contenedor de práctica. |
| Dominio y fase | D03/D04 · Fases 03 Identificación y 04 Análisis |
| Roles | Equipo de tres estudiantes (Red): Cristian Chaves, Matheo Puentes y Edison Gonzales. Docente (revisor). |
| Entorno y autorización | Contenedor de práctica DockerLabs (entorno tipo CTF) en VM propia. |
| Entradas | Contenedor DockerLabs en 172.17.0.2 (puertos 22 SSH y 5000 HTTP/Werkzeug, Ubuntu). |
| Procedimiento | `ping` y análisis de TTL=64 (Linux); `nmap -sS -p- --min-rate 1000` y `nmap -sCV -p 22,5000`; revisión del sitio clon de BunkerLabs y de la cookie de sesión; documentación Swagger en `/api` (`/api/summary` y `/gestion-maquinas/upload-logo`); cURL a `/api/summary`; descubrimiento del parámetro `origen` en el repo público de DockerLabs; petición a `upload-logo` con `machine_id=1`, `origen=bunker`, `logo` y el token CSRF tomado del código fuente (`view-source`); acceso SSH con las credenciales obtenidas; escalada de privilegios vía `sudo -l` → `/usr/bin/nano` (NOPASSWD) explotado con GTFOBins hasta shell de root. |
| Evidencias | Writeup `Lab_Perrito_Magico.pdf` con capturas (este mismo directorio). |
| Criterio de aceptación | Se reproduce la petición y el servidor confirma la modificación del logo; se valida acceso SSH y escalada a root. |
| Análisis defensivo | Autenticación y control de acceso en cada recurso de la API; validar el token CSRF en el servidor (no solo exigirlo); no exponer credenciales en las respuestas de éxito; restringir binarios con `sudo NOPASSWD` (ver GTFOBins) en `sudoers`. |
| Resultado | Ejecutado; la explotación de CSRF/control de acceso en `upload-logo` entregó credenciales SSH del usuario `renec`, y el binario `nano` con NOPASSWD permitió escalar a root. |

Referencia externa: [GTFOBins — nano](https://gtfobins.org/gtfobins/nano/#shell)
