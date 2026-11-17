# PR-LAB-010 — Unidad 4 · Labs 3–4: inventario autorizado vs. servicios observados y configuraciones débiles

**Dominio:** D01/D07 · **Enfoque:** Defensivo

| Campo | Descripción |
|---|---|
| Identificador | PR-LAB-010 |
| Nombre y versión | Unidad 4 · Labs 3–4 · v1.0 · nov-2026 · primera versión |
| Objetivo | Contrastar el inventario autorizado con los servicios realmente observados y auditar configuraciones débiles. |
| Dominio y fase | D01/D07 · Fase 02 Prevención |
| Roles | Blue (ejecutor), Red (aporta observaciones), docente (revisor). |
| Entorno y autorización | Kali Linux en VM propia (VirtualBox/VMware), red host-only aislada de Internet; autorización: actividad académica dirigida por el docente, objetivo propio. |
| Entradas | Inventario autorizado de servicios y resultado de escaneo de la VM Blue. |
| Procedimiento | Comparar lista autorizada vs. observada; revisar configuraciones débiles de los servicios activos; registrar en bitácora. |
| Evidencias | Tabla de diferencias y bitácora. |
| Criterio de aceptación | Toda diferencia entre inventario y observación queda clasificada (autorizada, no autorizada, a corregir). |
| Análisis defensivo | Retirar o justificar servicios no autorizados; endurecer configuraciones débiles. |
| Resultado | Ejecutado; resultados registrados en la bitácora. |
