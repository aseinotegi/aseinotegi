<h1 align="center">Hola, soy Ander Sein 👋</h1>

<p align="center">
  <b>Ingeniero de Automatización · IIoT · Visión Artificial</b><br>
  Conecto la planta (PLCs, sensores, robots) con el software que la explota: datos, IA y plataformas en producción.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/ander-sein-a24097195/"><img src="https://img.shields.io/badge/LinkedIn-Ander%20Sein-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:aseinotegi@gmail.com"><img src="https://img.shields.io/badge/Email-aseinotegi%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://img.shields.io/badge/📍-Donostia%20·%20País%20Vasco-555?style=flat" alt="Donostia">
</p>

---

## 🧭 Quién soy

Más de **9 años** entre el cuadro eléctrico y el servidor. Empecé programando y poniendo en marcha PLCs en líneas de producción por medio mundo, seguí como especialista en automatización, y hoy diseño de extremo a extremo plataformas que **operan flotas de robots de inspección autónoma** en refinerías.

Ese recorrido me da algo poco común: entiendo el proceso, el PLC y la red OT **y** también el backend, el contenedor y el modelo de visión que los explotan. Hablo el idioma del jefe de mantenimiento y el del equipo de software.

**Qué me puedes pedir:**

- 🏭 **Automatización industrial** — programación de PLC (Siemens, Rockwell, Omron, Schneider), puesta en marcha, retrofit y conectividad de parques de PLC heterogéneos y legacy.
- 📡 **IIoT / Edge** — captura de datos de planta (S7, EtherNet/IP, OPC UA, Modbus), pasarelas y brokers (MQTT, RabbitMQ), pipelines a base de datos y dashboards, todo dockerizado.
- 🐍 **Python a medida** — librerías propias de adquisición, procesamiento y automatización; servicios FastAPI; integración con sistemas existentes.
- 👁️ **Visión artificial aplicada** — detección de objetos (YOLO / OpenCV), lectura de instrumentos, clasificación de obstáculos, modelos multimodales en producción.
- 🔗 **Integración low-code** — Node-RED y n8n para orquestar flujos entre planta, IT y servicios cloud cuando no hace falta reinventar la rueda.
- 🤖 **Robótica móvil autónoma** — plataformas de scheduling, monitorización, KPIs/OEE e informes con IA para flotas en entornos oil & gas.

---

## 🛠️ Stack

| Capa | Tecnologías |
|---|---|
| **OT / Control** | Siemens (TIA Portal, S7-300/1200/1500) · Rockwell (Studio 5000, CompactLogix) · Omron · Schneider · Profinet / Profibus / EtherNet/IP · OPC UA · Modbus |
| **IIoT / Mensajería** | MQTT (Mosquitto) · RabbitMQ · Node-RED · n8n · Kepware · ThingWorx |
| **Lenguajes** | Python (principal) · TypeScript / JavaScript · SQL · Structured Text / Ladder |
| **Backend & Datos** | FastAPI · SQLAlchemy · PostgreSQL (+ PostGIS) · Redis · GraphQL · MySQL |
| **Visión / IA** | YOLO · OpenCV · dlib · modelos multimodales (Gemini) · pipelines de inferencia en edge |
| **Frontend** | React 18 · TypeScript · Vite · TailwindCSS · Leaflet · Recharts |
| **Infra / DevOps** | Docker & Docker Compose · Caddy / Nginx · GitHub Actions (CI/CD) · AWS S3 · Sentry · Linux |

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,ts,react,fastapi,postgres,redis,docker,nodejs,linux,aws,githubactions,opencv&perline=12" alt="stack icons">
</p>

---

## 🚀 Proyectos destacados

### 🤖 [Robot Mission Scheduler & Monitoring Platform](https://github.com/aseinotegi/robot-mission-scheduler-showcase)
Plataforma **en producción** para planificar y monitorizar misiones de robots de inspección autónoma en instalaciones oil & gas. Multi-planta, multi-robot, tiempo real, KPIs/OEE, informes PDF con lectura de manómetros por IA de visión, clasificación de obstáculos con fallback automático, scheduler con leader election, backups a S3, CI/CD y observabilidad end-to-end.
`Python` `FastAPI` `React` `PostgreSQL` `Redis` `Docker` `Gemini Vision`

### 📡 Adquisición de datos de PLC Siemens → broker
Dos implementaciones del mismo patrón IIoT — leer un DB del PLC, detectar cambios y publicar solo lo que cambia — en los dos lenguajes que uso en el edge:
- [**snap7_PLC_adquisition**](https://github.com/aseinotegi/snap7_PLC_adquisition) — Python + Snap7 + asyncio → **RabbitMQ**. Lectura tipada de bools, bytes, int16, int32 y float sobre offsets del DB.
- [**nodes7_js**](https://github.com/aseinotegi/nodes7_js) — Node.js + nodes7 → **MQTT**, con web service Express para configurar el PLC (IP, rack/slot, DB, variables) desde el navegador. Ciclo de lectura de 30 ms.

### 🗺️ [Mapa de Balizas V16 — España](https://github.com/aseinotegi/DGT) · [mapabalizasv16.info](https://mapabalizasv16.info)
Servicio público en vivo que integra tres fuentes oficiales de la DGT, persiste incidencias con geodatos en PostgreSQL y calcula un **índice de vulnerabilidad** (aislamiento, exposición temporal, horario, tipo de vía) para detectar conductores en riesgo. Backend + frontend + Nginx en Docker Compose.
`TypeScript` `PostgreSQL/PostGIS` `Docker` `Leaflet`

### 👁️ [Detector de somnolencia](https://github.com/aseinotegi/DetectorSomnolencia)
Visión artificial en tiempo real sobre cámara: landmarks faciales, detección de parpadeo, bostezo y ojos cerrados con alerta. Base del mismo tipo de pipeline que aplico a detección de objetos con YOLO en entornos industriales.
`Python` `OpenCV` `dlib`

### 🧰 [MyTools](https://github.com/aseinotegi/MyTools)
Caja de herramientas Python que uso en proyectos reales: cliente **OPC UA**, servidor **Snap7** simulado, consumidores RabbitMQ → CSV, escáneres ARP/ICMP de red OT, generación automática de informes, dashboards, transcripción y traducción de audio…

---

## 🧩 Cómo trabajo

- **Primero el proceso, luego el código.** Antes de conectar nada, entiendo qué hace la máquina y qué NO se puede tocar. Regla de oro en planta: no penalizar la producción.
- **Patrón DB única.** En proyectos nuevos, todo lo que el PLC debe comunicar se copia a un único DB; el mundo exterior solo toca ese DB. Menos riesgo, más mantenible.
- **Publicar por cambio, no por ciclo.** Los sistemas IIoT que diseño detectan cambios en origen y publican solo lo que varía: menos tráfico, menos carga en el broker, histórico limpio.
- **Producción de verdad.** Seguridad (RBAC, secretos, cabeceras), observabilidad (Sentry end-to-end), CI/CD y backups no son extras: van en la primera entrega.

---

## 📊 GitHub

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=aseinotegi&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true" alt="stats" height="165">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=aseinotegi&layout=compact&theme=tokyonight&hide_border=true" alt="langs" height="165">
</p>

---

## 📬 ¿Hablamos?

¿Tienes un parque de PLCs que quieres conectar, una planta que necesita datos en tiempo real, un caso de visión artificial en línea de producción o una flota de robots que operar? Escríbeme.

<p align="center">
  <a href="https://www.linkedin.com/in/ander-sein-a24097195/">LinkedIn</a> · <a href="mailto:aseinotegi@gmail.com">aseinotegi@gmail.com</a>
</p>
