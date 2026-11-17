# PR-LAB-003 — Clonación controlada HTTrack

**Dominio:** D03 · **Enfoque:** Ofensivo/defensivo

| Campo | Descripción |
|---|---|
| Identificador | PR-LAB-003 |
| Nombre y versión | Clonación controlada con HTTrack · v1.0 · nov-2026 · primera versión |
| Objetivo | Replicar un sitio propio o autorizado para analizar recursos expuestos y evaluar su superficie web. |
| Dominio y fase | D03 · Fases 03 Identificación y 04 Análisis |
| Roles | Ejecutor: analista ofensivo. Revisor: analista defensivo. |
| Entorno y autorización | Kali Linux en VM propia (VirtualBox/VMware), red host-only aislada de Internet; autorización: actividad académica dirigida por el docente, objetivo propio. |
| Entradas | Sitio web propio o servidor de prueba local (por ejemplo Apache en la VM Blue); HTTrack. |
| Procedimiento | 1) Confirmar autorización y alcance. 2) Clonar el sitio con HTTrack en un directorio aislado. 3) Inventariar archivos, formularios y enlaces. 4) Revisar comentarios, rutas y datos sensibles. 5) Calcular hash de los archivos clonados. |
| Evidencias | Árbol de archivos clonado, inventario y hashes. |
| Criterio de aceptación | El clon permite identificar recursos expuestos y se documentan hallazgos con su impacto. |
| Análisis defensivo | Eliminar información sensible del contenido público; limitar el rastreo automatizado; la clonación de sitios de terceros sin permiso está prohibida. |
| Resultado | Protocolo definido; la clonación se realiza únicamente sobre el servidor propio de laboratorio. |
