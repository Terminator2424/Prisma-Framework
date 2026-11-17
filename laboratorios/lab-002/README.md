# PR-LAB-002 — DNS Footprinting con nslookup y dig

**Dominio:** D02 · **Enfoque:** Ofensivo controlado

| Campo | Descripción |
|---|---|
| Identificador | PR-LAB-002 |
| Nombre y versión | DNS Footprinting con nslookup y dig · v1.0 · nov-2026 · primera versión |
| Objetivo | Obtener información pública de un dominio autorizado sin atacarlo (registros, servidores de nombres y correo). |
| Dominio y fase | D02 · Fase 03 Identificación |
| Roles | Ejecutor: analista ofensivo. Revisor: analista defensivo. |
| Entorno y autorización | Kali Linux en VM propia (VirtualBox/VMware), red host-only aislada de Internet; autorización: actividad académica dirigida por el docente, objetivo propio. |
| Entradas | Dominio de práctica autorizado (por ejemplo ejemplo.com o un dominio propio); nslookup, dig y whois. |
| Procedimiento | 1) whois del dominio. 2) nslookup y dig para registros A, MX, NS y TXT. 3) Consulta de servidores de nombres con dig @servidor. 4) Documentar lo observado y clasificarlo como pasivo o activo. |
| Evidencias | Salidas de consola con fecha y hora; tabla de registros obtenidos. |
| Criterio de aceptación | Se documentan al menos los registros A, MX, NS y TXT y su significado. |
| Análisis defensivo | Minimizar información publicada en DNS, retirar subdominios olvidados y revisar registros TXT. Marco teórico en PR-LAB-017. |
| Resultado | Protocolo definido; la evidencia se registra al ejecutarlo en el dominio autorizado. |
