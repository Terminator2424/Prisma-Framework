# PR-LAB-007 — Burp Suite

**Dominio:** D03/D04 · **Enfoque:** Pruebas web

| Campo | Descripción |
|---|---|
| Identificador | PR-LAB-007 |
| Nombre y versión | Burp Suite · v1.0 · nov-2026 · primera versión |
| Objetivo | Interceptar y analizar solicitudes HTTP de una aplicación propia para evaluar autenticación, sesiones y validación. |
| Dominio y fase | D03/D04 · Fases 03 Identificación y 04 Análisis |
| Roles | Ejecutor: analista ofensivo. Revisor: analista defensivo. |
| Entorno y autorización | Kali Linux en VM propia (VirtualBox/VMware), red host-only aislada de Internet; autorización: actividad académica dirigida por el docente, objetivo propio. |
| Entradas | Burp Suite Community, navegador configurado con el proxy y aplicación de práctica local (por ejemplo la del PR-LAB-019). |
| Procedimiento | 1) Configurar el proxy de Burp y el certificado. 2) Navegar la aplicación y revisar el historial. 3) Interceptar y modificar una solicitud en Repeater. 4) Revisar cookies, cabeceras y tokens (CSRF). 5) Documentar hallazgos. |
| Evidencias | Historial de solicitudes, capturas de Repeater y cabeceras analizadas. |
| Criterio de aceptación | Se identifican parámetros, cookies y tokens y se explica la validación que hace el servidor. |
| Análisis defensivo | Control de acceso por recurso, tokens CSRF no reutilizables, cookies seguras y validación en el servidor. |
| Resultado | Protocolo definido; práctica complementaria al writeup de PR-LAB-019. |
