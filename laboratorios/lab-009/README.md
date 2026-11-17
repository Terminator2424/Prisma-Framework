# PR-LAB-009 — Unidad 4 · Labs 1–2: superficie de exposición y estados de puerto (Red/Blue)

**Dominio:** D02/D07 · **Enfoque:** Purple

| Campo | Descripción |
|---|---|
| Identificador | PR-LAB-009 |
| Nombre y versión | Unidad 4 · Labs 1–2 (Red/Blue) · v1.0 · nov-2026 · primera versión |
| Objetivo | Mapear la superficie de exposición y distinguir puertos abiertos, cerrados y filtrados desde ambos equipos. |
| Dominio y fase | D02/D07 · Fases 02 Prevención y 03 Identificación |
| Roles | Red: escanea con nmap. Blue: inspecciona con ss y prepara los estados. Revisor: docente (Purple). |
| Entorno y autorización | Dos VMs Kali en red host-only compartida, sin salida a otras redes (NAT solo para instalar paquetes); autorización académica. |
| Entradas | Dos VMs Kali en red host-only; en Blue: SSH (22), Apache (80) y vsftpd (21). Scripts lab1_superficie.py y lab2_estados.py. |
| Procedimiento | Blue: sudo ss -tulpn (0.0.0.0 vs 127.0.0.1); python3 -m http.server 8000 --bind 127.0.0.1 (abierto); iptables DROP al 8002 (filtrado); 8001 sin servicio (cerrado). Red: nmap -sV hacia Blue y exportación -oG. Ejecución de lab1_superficie.py sobre el .gnmap. |
| Evidencias | Archivo lab1_escaneo.gnmap, inventario con criticidad por puerto, bitácora (una entrada por máquina). |
| Criterio de aceptación | Inventario con criticidad por servicio y clasificación correcta de los tres estados de puerto. |
| Análisis defensivo | Reducir servicios que escuchan en 0.0.0.0; justificar cada puerto abierto; documentar el filtrado intencional. |
| Resultado | Ejecutado; resultados registrados en la bitácora de cada estudiante. |
