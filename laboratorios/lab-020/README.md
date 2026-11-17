# PR-LAB-020 — Caso de estudio: auditoría interna de NubeSegura S.A.

**Dominio:** D02/D04/D05/D06/D07 · **Enfoque:** Purple (integrador)

| Campo | Descripción |
|---|---|
| Identificador | PR-LAB-020 |
| Nombre y versión | Caso de estudio: auditoría NubeSegura S.A. · v1.0 · nov-2026 · primera versión |
| Objetivo | Integrar todas las fases en una auditoría interna sobre la propia VM usada como servidor de pruebas. |
| Dominio y fase | D02/D04/D05/D06/D07 · Fases 01 a 06 |
| Roles | Analista junior (Red y Blue), jefa de equipo/docente (coordinador y evaluador). |
| Entorno y autorización | Kali Linux en VM propia (VirtualBox/VMware), red host-only aislada de Internet; autorización: actividad académica dirigida por el docente, objetivo propio. |
| Entradas | VM Kali con SSH y Apache; scripts de Labs 1 y 2; nmap, Scapy, journalctl. |
| Procedimiento | Nueve puntos: inventario, banner grabbing, tráfico real, veredicto de phishing, integridad y diccionario, CVE y reputación de IP por API, matriz de riesgo y BIA, registro auditable, tres recomendaciones. |
| Evidencias | Informe TALLER_CASO_DE_ESTUDIO con capturas (Anexo C). |
| Criterio de aceptación | Cada hallazgo respaldado por dos fuentes independientes (script y herramienta estándar). |
| Análisis defensivo | Ver recomendaciones priorizadas en el Anexo D. |
| Resultado | Ejecutado; resultados en el capítulo 12. |
