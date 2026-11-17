# PR-LAB-012 — Unidad 4 · Labs 6–8: simulador de filtrado, auditor de reglas e iptables

**Dominio:** D07 · **Enfoque:** Defensivo

| Campo | Descripción |
|---|---|
| Identificador | PR-LAB-012 |
| Nombre y versión | Unidad 4 · Labs 6–8 · v1.0 · nov-2026 · primera versión |
| Objetivo | Modelar, auditar y aplicar políticas de filtrado de tráfico. |
| Dominio y fase | D07 · Fase 05 Mitigación |
| Roles | Blue (ejecutor), docente (revisor). |
| Entorno y autorización | Kali Linux en VM propia (VirtualBox/VMware), red host-only aislada de Internet; autorización: actividad académica dirigida por el docente, objetivo propio. |
| Entradas | Scripts de simulación y auditoría de reglas; iptables en la VM Blue. |
| Procedimiento | Lab 6: simulador de política de filtrado. Lab 7: auditor de reglas de firewall. Lab 8: reglas reales con iptables (ejecutar desde la consola gráfica de la VM, no por SSH). |
| Evidencias | Listado de reglas (iptables -L -n) y salida de los scripts. |
| Criterio de aceptación | Las reglas aplicadas bloquean lo previsto sin cortar el acceso de administración. |
| Análisis defensivo | Riesgo de auto-bloqueo al aplicar DROP por SSH; probar desde consola local. |
| Resultado | Ejecutado; resultados registrados en la bitácora. |
