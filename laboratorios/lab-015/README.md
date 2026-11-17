# PR-LAB-015 — Laboratorio 2: hash, reinicio auditable, phishing, multibanner, riesgos, NVD e indicador

**Dominio:** D04/D05/D06/D07 · **Enfoque:** Purple

| Campo | Descripción |
|---|---|
| Identificador | PR-LAB-015 |
| Nombre y versión | Laboratorio 2 (Python) · v1.0 · nov-2026 · primera versión |
| Objetivo | Automatizar controles básicos de integridad, phishing, banners y priorización de riesgos. |
| Dominio y fase | D04/D05/D06/D07 · Fases 03, 04 y 06 |
| Roles | Estudiante (Red/Blue), docente (revisor). |
| Entorno y autorización | Kali Linux en VM propia (VirtualBox/VMware), red host-only aislada de Internet; autorización: actividad académica dirigida por el docente, objetivo propio. |
| Entradas | Scripts Lab2_hash, Lab2_reinicio, Lab2_phishing, Lab2_multibanner, Lab2_riesgos, Lab2_nvd y Lab2_indicador. |
| Procedimiento | Hash SHA-256 de mensaje.txt; reinicio con confirmación y registro; heurística de phishing; banners en varios puertos; matriz de riesgos; consulta de CVE a NVD; cálculo de indicador. |
| Evidencias | Capturas de terminal en Laboratorio_2.docx. |
| Criterio de aceptación | Cada script produce una salida verificable (hash, log, veredicto, banner, tabla de riesgo, CVE). |
| Análisis defensivo | El hash detecta alteraciones; el registro propio debe contrastarse con el del sistema (journalctl). |
| Resultado | Ejecutado; ver pruebas P02–P08 del capítulo 12. |
