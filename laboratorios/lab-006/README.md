# PR-LAB-006 — Maltego: instalación y aplicación

**Dominio:** D02 · **Enfoque:** OSINT

| Campo | Descripción |
|---|---|
| Identificador | PR-LAB-006 |
| Nombre y versión | Maltego: instalación y aplicación · v1.0 · nov-2026 · primera versión |
| Objetivo | Mapear relaciones de infraestructura y personas a partir de fuentes abiertas sobre un objetivo autorizado. |
| Dominio y fase | D02 · Fase 03 Identificación |
| Roles | Ejecutor: analista ofensivo. Revisor: analista defensivo. |
| Entorno y autorización | Kali Linux en VM propia (VirtualBox/VMware), red host-only aislada de Internet; autorización: actividad académica dirigida por el docente, objetivo propio. |
| Entradas | Maltego Community Edition en Kali; dominio de práctica autorizado. |
| Procedimiento | 1) Instalar y registrar Maltego CE. 2) Crear un grafo a partir del dominio. 3) Ejecutar transformaciones sobre DNS, correos y subdominios. 4) Exportar el grafo y documentar relaciones. 5) Clasificar los datos obtenidos según sensibilidad. |
| Evidencias | Archivo de grafo exportado y capturas. |
| Criterio de aceptación | El grafo muestra relaciones del dominio y se documentan las fuentes de cada dato. |
| Análisis defensivo | Reducir la información corporativa visible, dar de baja subdominios olvidados y vigilar la exposición de correos. |
| Resultado | Protocolo definido; no se consultan datos personales de terceros. |
