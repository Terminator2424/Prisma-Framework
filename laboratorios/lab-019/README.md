# PR-LAB-019 — DockerLabs · Perrito Mágico: writeup de API y CSRF

**Dominio:** D03/D04 · **Enfoque:** Ofensivo controlado

| Campo | Descripción |
|---|---|
| Identificador | PR-LAB-019 |
| Nombre y versión | DockerLabs · Perrito Mágico (writeup) · v1.0 · nov-2026 · primera versión |
| Objetivo | Documentar reconocimiento y explotación de una API web vulnerable en un contenedor de práctica. |
| Dominio y fase | D03/D04 · Fases 03 Identificación y 04 Análisis |
| Roles | Equipo de tres estudiantes (Red), docente (revisor). |
| Entorno y autorización | Contenedor de práctica DockerLabs (entorno tipo CTF) en VM propia. |
| Entradas | Contenedor DockerLabs en 172.17.0.2 (22 SSH y 5000 HTTP/Werkzeug, Ubuntu). |
| Procedimiento | ping y TTL=64 (Linux); nmap -sS -p- y nmap -sCV; revisión del sitio y la cookie de sesión; documentación de /api; cURL a /api/summary; petición a upload-logo con machine_id, origen=bunker y token CSRF tomado del código fuente. |
| Evidencias | Writeup Lab_Perrito_Magico.pdf con capturas. |
| Criterio de aceptación | Se reproduce la petición y el servidor confirma la modificación del logo. |
| Análisis defensivo | Autenticación y control de acceso en cada recurso; no exponer token CSRF ni credenciales en respuestas. |
| Resultado | Ejecutado; la explotación entregó credenciales SSH del objetivo. |
