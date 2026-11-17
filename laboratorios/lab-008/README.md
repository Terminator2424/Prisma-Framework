# PR-LAB-008 — Laboratorio 1 de Ciberseguridad: escáner de puertos, psutil y cabeceras HTTP (Python)

**Dominio:** D02/D03 · **Enfoque:** Ofensivo controlado

| Campo | Descripción |
|---|---|
| Identificador | PR-LAB-008 |
| Nombre y versión | Laboratorio 1 de Ciberseguridad (Python) · v1.0 · nov-2026 · primera versión |
| Objetivo | Construir herramientas mínimas de reconocimiento local y comprender sus límites. |
| Dominio y fase | D02/D03 · Fase 03 Identificación |
| Roles | Ejecutor: estudiante (Red). Revisor: docente. |
| Entorno y autorización | Kali Linux en VM propia (VirtualBox/VMware), red host-only aislada de Internet; autorización: actividad académica dirigida por el docente, objetivo propio. |
| Entradas | Entorno virtual de Python; librerías socket, psutil y requests; objetivo 127.0.0.1. |
| Procedimiento | 1) Configurar Python y crear el entorno virtual. 2) Instalar librerías. 3) Mini escáner de puertos con socket. 4) Inspección de conexiones activas con psutil. 5) Consulta de cabeceras HTTP con requests. |
| Evidencias | Scripts y salidas de consola incluidos en el informe Laboratorio_1_de_Ciberseguridad.pdf. |
| Criterio de aceptación | El escáner lista puertos abiertos/cerrados y se responde la pregunta guía sobre puertos cerrados vs. filtrados. |
| Análisis defensivo | Un escáner que solo detecta respuestas no distingue con seguridad un puerto cerrado de uno filtrado por firewall; la ausencia de servicio debe confirmarse con otra herramienta. |
| Resultado | Ejecutado; pregunta guía respondida y documentada en el informe. |
