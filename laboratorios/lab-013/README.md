# PR-LAB-013 — Unidad 4 · Labs 9–12: fuerza bruta SSH, detección de escaneo, mini-SIEM y análisis de incidentes

**Dominio:** D07 · **Enfoque:** Defensivo

| Campo | Descripción |
|---|---|
| Identificador | PR-LAB-013 |
| Nombre y versión | Unidad 4 · Labs 9–12 · v1.0 · nov-2026 · primera versión |
| Objetivo | Pasar del registro a la alerta: detectar fuerza bruta y escaneos, correlacionar eventos y analizar incidentes reales. |
| Dominio y fase | D07 · Fases 03 Identificación y 04 Análisis |
| Roles | Blue (ejecutor), Red (genera la actividad), docente (revisor). |
| Entorno y autorización | Kali Linux en VM propia (VirtualBox/VMware), red host-only aislada de Internet; autorización: actividad académica dirigida por el docente, objetivo propio. |
| Entradas | lab9_generar_log.py, lab11_generar_eventos.py y registros simulados de SSH. |
| Procedimiento | Lab 9: log simulado y alerta por fuerza bruta en SSH. Lab 10: detectar un escaneo de puertos. Lab 11: mini-SIEM con correlación. Lab 12: análisis de incidentes reales y exposición de 3 minutos. |
| Evidencias | Logs, alertas generadas y bitácora. |
| Criterio de aceptación | Cada actividad adversaria de prueba produce una alerta o queda registrada como brecha de detección. |
| Análisis defensivo | Documentar umbrales de detección y retroalimentar reglas con la actividad Red. |
| Resultado | Ejecutado; la tasa de detección se calcula con la métrica del capítulo 13. |
