# Proyecto 1: Captura y Análisis de Tráfico de Red con Wireshark

## Registro Diario de Progreso
- Día 1 (21/09/2026 - 6%):** Instalación de Wireshark y Npcap, identificación de la interfaz Wi-Fi activa, captura de paquetes ICMP y documentación inicial del laboratorio.

![Evidencia Día 1](Captura%20de%20pantalla%202026-09-21%20150932.png)

- Día 2 (22/09/2026 - 12%):** Captura de tráfico web y práctica de filtrado entre protocolos HTTP (texto plano) y TLS/HTTPS (cifrado).

**Tráfico HTTP (Texto plano):**
![Evidencia Día 2 HTTP](Captura%20de%20pantalla%202026-09-22%20152030.png)

**Tráfico TLS/HTTPS (Cifrado):**
![Evidencia Día 2 TLS](Captura%20de%20pantalla%202026-09-22%20152101.png)

- **Día 3 (23/09/2026 - 18%):** Aislamiento de tráfico de red mediante filtros por dirección IP de origen (`ip.src`), analizando las conexiones salientes desde el equipo.

![Evidencia Día 3](Captura%20de%20pantalla%202026-09-23%20203018.png)

- **Día 4 (24/09/2026 - 24%):** Filtrado avanzado de tráfico de red por número de puerto (`tcp.port == 443`) para aislar servicios y conexiones seguras.

![Evidencia Día 4](Captura%20de%20pantalla%202026-09-24%20164319.png)

- **Día 5 (25/09/2026 - 30%):** Aplicación de operadores lógicos (`and`) para combinar filtros de dirección IP y puertos, optimizando el análisis detallado de tráfico.

![Evidencia Día 5](Captura%20de%20pantalla%202026-09-29%20131535.png)

- **Día 6 (29/09/2026 - 36%):** Uso de operadores de exclusión (`!=`) en Wireshark para descartar tráfico irrelevante (como el del router) y enfocar la investigación.

![Evidencia Día 6](Captura%20de%20pantalla%202026-09-29%20132236.png)

- **Día 7 (29/09/2026 - 42%):** Inspección profunda de las capas de red (Ethernet, IPv4 y TCP) utilizando el panel de detalles de paquetes en Wireshark.

![Evidencia Día 7](Captura%20de%20pantalla%202026-09-29%20132648.png)

- **Día 8 (30/09/2026 - 48%):** Seguimiento de flujos de red completos (`TCP Stream`) para reconstruir e inspeccionar conversaciones de datos entre el host y los servidores.

![Evidencia Día 8](Captura%20de%20pantalla%202026-09-29%20133130.png)

- **Día 9 (29/09/2026 - 54%):** Análisis de estadísticas globales de red mediante el panel de conversaciones (`Conversations > IPv4`) para identificar volúmenes de tráfico y endpoints principales.

![Evidencia Día 9](Captura%20de%20pantalla%202026-09-29%20133509.png)

- **Día 10 (29/09/2026 - 60%):** Identificación de hosts únicos mediante el panel de puntos finales (`Endpoints > IPv4`) para mapear dispositivos activos en la captura de tráfico.

![Evidencia Día 10](Captura%20de%20pantalla%202026-09-29%20134051.png)

- **Día 11 (11/10/2026 - 66%):** Extracción y exportación de archivos u objetos multimedia directamente desde el tráfico de red (`Export Objects > HTTP`) usando Wireshark.

![Evidencia Día 11](Captura%20de%20pantalla%202026-10-11%20054509.png)

- **Día 12 (11/10/2026 - 72%):** Inspección y diagnóstico de consultas y respuestas del protocolo DNS (`dns`) para analizar la resolución de nombres de dominio.

![Evidencia Día 12](Captura%20de%20pantalla%202026-10-11%20054856.png)

- **Día 13 (11/10/2026 - 78%):** Diagnóstico de rendimiento y pérdida de paquetes mediante el análisis de banderas TCP (`tcp.analysis.flags`) para identificar retransmisiones y congestión en la red.

![Evidencia Día 13](Captura%20de%20pantalla%202026-10-11%20055155.png)

- **Día 14 (11/10/2026 - 84%):** Análisis de tráfico de control y pruebas de diagnóstico de red mediante la inspección del protocolo ICMP (`icmp`).

![Evidencia Día 14](Captura%20de%20pantalla%202026-10-11%20055655.png)

- **Día 15 (11/10/2026 - 90%):** Creación y aplicación de filtros lógicos combinados (`and` / `or` / `not`) en Wireshark para el aislamiento preciso de tráfico multiprotocolo.

![Evidencia Día 15](Captura%20de%20pantalla%202026-10-11%20060028.png)

- **Día 16 (11/10/2026 - 96%):** Generación de reportes estadísticos globales de conversaciones y endpoints (`Statistics > Conversations`) para auditar el volumen total de paquetes y consumo de ancho de banda.

![Evidencia Día 16](Captura%20de%20pantalla%202026-10-11%20060302.png)

- **Día 17 (11/10/2026 - 100%):** Consolidación y cierre del proyecto de análisis de tráfico con Wireshark, documentando hallazgos clave de red (análisis de protocolos, diagnóstico TCP, aislamiento ICMP y auditoría de tráfico IPv4). ¡Proyecto Finalizado! 🎉

## 🏁 Resumen General y Cierre del Proyecto (100%)

Este proyecto documenta el análisis práctico de tráfico de red a través de capturas de paquetes con **Wireshark**, abarcando desde la inspección básica hasta el diagnóstico avanzado de rendimiento y análisis estadístico.

### 📌 Hitos y Aprendizajes Clave:

1. **Inspección de Protocolos y Aplicación (Días 1–12):**
   * Extracción de objetos y análisis de peticiones HTTP.
   * Diagnóstico de resolución de nombres mediante consultas y respuestas DNS.
   * Identificación de la arquitectura de la red local y asignación de direcciones.

2. **Diagnóstico de Rendimiento y Capa de Transporte (Días 13–15):**
   * Identificación de retransmisiones, ACKs duplicados e inestabilidad temporal en conexiones TCP mediante el filtro `tcp.analysis.flags`.
   * Pruebas de conectividad y control de red inspeccionando tráfico ICMP (`Echo Request/Reply`).
   * Creación de filtros de visualización avanzados utilizando operadores lógicos combinados (`and`, `or`, `not`).

3. **Auditoría Estadística y Hallazgos Globales (Días 16–17):**
   * Análisis de conversaciones globales (`Statistics > Conversations`) para evaluar el consumo de ancho de banda y flujo de paquetes.
   * **Hallazgo relevante:** Se identificó una dependencia total del direccionamiento **IPv4** en el entorno analizado, con ausencia completa de tráfico registrado bajo IPv6.
   
