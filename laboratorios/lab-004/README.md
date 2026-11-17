# PR-LAB-004 — Esteganografía con Steghide: partes 1–3

**Dominio:** D06 · **Enfoque:** Forense y colaborativo

| Campo | Descripción |
|---|---|
| Identificador | PR-LAB-004 |
| Nombre y versión | Esteganografía con Steghide (partes 1–3) · v1.0 · nov-2026 · primera versión |
| Objetivo | Ocultar y extraer información en archivos y verificar su integridad como práctica forense colaborativa. |
| Dominio y fase | D06 · Fases 03 Identificación y 04 Análisis |
| Roles | Parte 1: emisor (oculta). Parte 2: receptor (extrae). Parte 3: analista (verifica integridad). Revisor: docente. |
| Entorno y autorización | Kali Linux en VM propia (VirtualBox/VMware), red host-only aislada de Internet; autorización: actividad académica dirigida por el docente, objetivo propio. |
| Entradas | Imagen portadora y archivo secreto sintéticos; Steghide; sha256sum. |
| Procedimiento | Parte 1: steghide embed con contraseña. Parte 2: steghide extract y comparación del contenido. Parte 3: hash del archivo antes y después, steghide info y análisis de diferencias. |
| Evidencias | Archivos portador y estego, hashes SHA-256 y salidas de steghide. |
| Criterio de aceptación | El contenido extraído coincide con el original y la diferencia entre hashes queda documentada. |
| Análisis defensivo | Detectar esteganografía revisando hashes, tamaños y metadatos; preservar los originales con cadena de custodia. |
| Resultado | Protocolo definido con archivos sintéticos (sin datos reales). |
