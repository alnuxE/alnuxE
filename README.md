<!-- ░░ Encabezado ░░ -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=200&color=0:1a1b27,50:3d59a1,100:7aa2f7&text=Alejandro%20Estrada&fontColor=c0caf5&fontSize=56&fontAlignY=36&desc=Software%20Engineer%20%C2%B7%20Backend&descSize=20&descAlignY=58&animation=fadeIn" width="100%" alt="Alejandro Estrada — Software Engineer · Backend">
</p>

<p align="center">
  <a href="https://alnuxe.github.io/Portafolio/">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3200&pause=900&color=7AA2F7&center=true&vCenter=true&width=620&lines=Backend%20en%20producci%C3%B3n%20desde%20abril%20de%202024;Laravel%20%C2%B7%20Node.js%20%C2%B7%20MySQL%20%C2%B7%20MongoDB%20%C2%B7%20Redis;808%20pruebas%20automatizadas%20en%20verde;Arquitectura%20por%20capas%20%C2%B7%20CI/CD%20%C2%B7%20Kubernetes;Ingenier%C3%ADa%20en%20Inform%C3%A1tica%20%C2%B7%20UPIICSA-IPN" alt="Backend en producción · Laravel · Node.js · 808 pruebas · Arquitectura por capas">
  </a>
</p>

<p align="center">
  <a href="https://alnuxe.github.io/Portafolio/"><img src="https://img.shields.io/badge/Portafolio-alnuxe.github.io-7aa2f7?style=for-the-badge&logo=githubpages&logoColor=white&labelColor=1a1b27" alt="Portafolio"></a>
  <a href="https://www.linkedin.com/in/daniel-alejandro-estrada-olalde-532a16233/"><img src="https://img.shields.io/badge/LinkedIn-Conectemos-0a66c2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=1a1b27" alt="LinkedIn"></a>
  <a href="mailto:ingeniero.alejandro.estrada@gmail.com"><img src="https://img.shields.io/badge/Email-Escr%C3%ADbeme-bb9af7?style=for-the-badge&logo=gmail&logoColor=white&labelColor=1a1b27" alt="Email"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/📍_CDMX-1a1b27?style=flat-square" alt="Ciudad de México">
  <img src="https://img.shields.io/badge/En_producción-desde_abr_2024-9ece6a?style=flat-square&labelColor=1a1b27" alt="En producción desde abril de 2024">
  <img src="https://img.shields.io/badge/Tests-808_passing-9ece6a?style=flat-square&logo=checkmarx&logoColor=white&labelColor=1a1b27" alt="808 pruebas pasando">
  <img src="https://komarev.com/ghpvc/?username=alnuxE&style=flat-square&color=7aa2f7&label=Visitas" alt="Visitas al perfil">
</p>

---

### `$ whoami`

```ts
const alnuxE: SoftwareEngineer = {
  nombre:      "Daniel Alejandro Estrada Olalde",
  rol:         "Backend Developer @ Fay Publicidad · Metrix",
  produccion:  { desde: "2024-04", clientes: ["Walmart", "Waldos", "P&G"] },
  formacion:   "Ingeniería en Informática · UPIICSA-IPN (9.º semestre)",
  enfoque:     ["arquitectura por capas", "pruebas automatizadas", "datos a gran volumen"],
  despliegue:  ["Docker", "Kubernetes (GKE Autopilot)", "CI/CD", "Nginx"],
  idiomas:     { es: "nativo", en: "B1/B2 · documentación técnica" },
};
```

Escribo backend para sistemas en producción con volúmenes de datos altos, consultas que tienen que responder rápido y despliegues con gente esperando al otro lado. Fuera del trabajo diseño y publico mis propias aplicaciones de principio a fin —arquitectura, pruebas y publicación—, que es donde se aprende lo que un tutorial no enseña: qué hacer cuando la red se cae a mitad de una operación o por qué una decisión cómoda hoy se paga en tres meses.

---

### 📐 Ingeniería en números

<div align="center">

| Pruebas automatizadas | Apps publicadas | Ficheros bajo prueba | Plataformas | En producción desde |
|:---:|:---:|:---:|:---:|:---:|
| **808** ✅ | **3** | **218** | **4** | **2024** |

</div>

> Mis apps son privadas: lo que se puede auditar son las cifras y las decisiones de ingeniería. Las detallo abajo.

---

### 🏗️ Cómo construyo software

Separo cada sistema en capas con dependencias en un solo sentido. En SwitchIot **una prueba falla si alguna capa importa hacia arriba**, así la arquitectura no se erosiona con el tiempo.

```mermaid
flowchart LR
    UI["🖥️ Presentación<br/><sub>UI · controladores</sub>"] --> APP["⚙️ Aplicación<br/><sub>casos de uso</sub>"]
    APP --> DOM["🧩 Dominio<br/><sub>tipos inmutables · reglas</sub>"]
    INF["🔌 Infraestructura<br/><sub>BD · red · almacén seguro</sub>"] -. implementa contratos .-> DOM
    TEST["🧪 Pruebas por capa"] -. verifican .-> APP
    TEST -. verifican .-> DOM
```

| Principio | Cómo se ve en el código |
|---|---|
| **Probar, no afirmar** | Cada capa se prueba sin arrastrar a las demás; 808 pruebas entre tres apps. |
| **Una sola fuente de verdad** | Los totales se calculan, nunca se escriben a mano. |
| **Fallar de forma segura** | Apps que funcionan sin conexión; la red es una mejora, no un requisito. |
| **Seguridad desde el diseño** | Una credencial por dispositivo, guardada en el almacén seguro del sistema. |

---

### 🚀 Proyectos destacados

| App | Qué resuelve | Pruebas | Ficheros | Plataformas |
|---|---|:---:|:---:|---|
| 🔌 **SwitchIot** `v1.1.0` | Control de una bomba de agua sobre **ESP32** por red local, sin nube y sin cuenta. | **338** | 85 | Android · Linux · Windows |
| ✍️ **PromptEngine** `v1.4.0` | Compositor de prompts por secciones con vista previa en vivo y salida en Markdown. | **320** | 54 | Android · Web · Linux |
| 📚 **Classly** `v1.0.0` | Horario académico y tareas con el dominio en tipos inmutables. Funciona sin conexión. | **150** | 79 | Android |

<details>
<summary><b>🔍 Decisiones de ingeniería por proyecto</b> (clic para expandir)</summary>
<br>

**SwitchIot**
- Descubre los equipos por **difusión UDP** y, si la red la bloquea, **barre la subred** como respaldo.
- Aprovisiona el ESP32 desde su propio punto de acceso, sin servidor de por medio.
- Una credencial por dispositivo, guardada en el almacén seguro del sistema.
- Registra tiempos de extremo a extremo y el registro sobrevive al cierre de la app.

**PromptEngine**
- Cada sección del prompt es una pieza independiente que se reordena sin romper las demás.
- La vista previa se recalcula en vivo y exporta Markdown limpio.
- Su sitio corre en un servidor propio, en contenedores, detrás de **Nginx** como proxy inverso.

**Classly**
- Dominio modelado en tipos inmutables: un horario no se corrompe a medias.
- *Offline-first*: la red es una mejora, no un requisito.

</details>

---

### 💼 Experiencia

**Desarrollador Backend · Fay Publicidad · Metrix** — *abril 2024 → hoy*
<sub>Sistemas en producción usados por **Walmart**, **Waldos** y **P&G**</sub>

- Aplicaciones **Laravel** dentro de un monorepo desplegado sobre **Kubernetes (GKE Autopilot)** con integración y despliegue continuos.
- Consultas complejas sobre grandes volúmenes en **MySQL** y **MongoDB**, con foco en el tiempo de respuesta de los reportes de negocio.
- Funcionalidades de extremo a extremo, desde el modelo de datos hasta la interfaz.
- Diagnóstico de incidencias en producción: reproducir, acotar la causa con el equipo y después tocar código.

---

### 🧰 Stack por capas

| Capa | Tecnologías |
|---|---|
| **Backend** | <img src="https://skillicons.dev/icons?i=php,laravel,nodejs,express,ts,js,java" height="40" alt="PHP, Laravel, Node.js, Express, TypeScript, JavaScript, Java"> |
| **Datos** | <img src="https://skillicons.dev/icons?i=mysql,mongodb,redis" height="40" alt="MySQL, MongoDB, Redis"> |
| **Plataforma** | <img src="https://skillicons.dev/icons?i=docker,kubernetes,gcp,nginx,linux,bash,githubactions,git" height="40" alt="Docker, Kubernetes, Google Cloud, Nginx, Linux, Bash, GitHub Actions, Git"> |
| **Móvil** | <img src="https://skillicons.dev/icons?i=flutter,dart" height="40" alt="Flutter, Dart"> |
| **Web** | <img src="https://skillicons.dev/icons?i=react,nextjs,vite,tailwind" height="40" alt="React, Next.js, Vite, Tailwind CSS"> |

**Práctica:** arquitectura limpia · arquitectura por capas · microservicios · pruebas automatizadas · revisión de código · documentación de API · POO y programación funcional

---

### 📈 Actividad

<p align="center">
  <img width="100%" src="https://streak-stats.demolab.com?user=alnuxE&theme=tokyonight&hide_border=true&background=1a1b27" alt="Racha de contribuciones">
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/alnuxE/alnuxE/output/github-snake-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/alnuxE/alnuxE/output/github-snake.svg">
    <img alt="Serpiente comiéndose mi gráfica de contribuciones" src="https://raw.githubusercontent.com/alnuxE/alnuxE/output/github-snake-dark.svg">
  </picture>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=110&color=0:7aa2f7,50:3d59a1,100:1a1b27&section=footer&text=%C2%BFTu%20equipo%20necesita%20llevar%20software%20a%20producci%C3%B3n%3F&fontSize=18&fontColor=c0caf5&fontAlignY=68" width="100%" alt="¿Tu equipo necesita llevar software a producción?">
</p>
