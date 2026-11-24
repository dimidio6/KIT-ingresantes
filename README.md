# KIT de herramientas esenciales

Herramientas de utilidad para estudiantes de Informática.

Este repositorio acompaña la charla para ingresantes de las **Jornadas de Informática 2026** (Universidad Nacional de la Patagonia San Juan Bosco). Acá está todo lo que mostramos, con el primer paso para arrancar con cada herramienta y algunos recursos para seguir aprendiendo por tu cuenta.

> Estás viendo un repositorio de GitHub, y este texto es un archivo en Markdown (`README.md`). Las dos cosas son parte de lo que vimos en la charla.

## Contenido

- [Git: guardar versiones de tu código](#git-guardar-versiones-de-tu-código)
- [GitHub: compartir con tu grupo](#github-compartir-con-tu-grupo)
- [Docker: que corra en cualquier compu](#docker-que-corra-en-cualquier-compu)
- [IA: aprender mejor](#ia-aprender-mejor)
- [Extras: terminal, IDE y Markdown](#extras-terminal-ide-y-markdown)
- [Un caso real: Charmy](#un-caso-real-charmy)
- [¿Dudas?](#dudas)

---

## Git: guardar versiones de tu código

**Qué es.** Un sistema de control de versiones: cada *commit* es una versión guardada de tu proyecto, con un mensaje que dice qué cambiaste. Si algo se rompe, volvés a la anterior.

**Primer paso.** Instalá Git desde [git-scm.com/downloads](https://git-scm.com/downloads) (en Windows, con las opciones por defecto). Después, en una terminal:

```powershell
git config --global user.name "Tu Nombre"
git config --global user.email "tu-mail@ejemplo.com"

mkdir mi-primer-repo
cd mi-primer-repo
git init
# creá un archivo cualquiera y guardalo, después:
git add .
git commit -m "Primera versión"
git log --oneline
```

**Para seguir aprendiendo**

- [Learn Git Branching](https://learngitbranching.js.org/?locale=es_AR): un juego para entender commits y ramas viéndolos dibujados.
- [Pro Git, en español](https://git-scm.com/book/es/v2): el libro gratuito de Git. Con los capítulos 1 (*Inicio: Sobre el Control de Versiones*) y 2 (*Fundamentos de Git*) alcanza para empezar.

## GitHub: compartir con tu grupo

**Qué es.** Un sitio donde subís el historial de Git para compartirlo, trabajar en grupo y mostrar lo que hacés. Git vive en tu compu; GitHub, en internet. Con `git push` subís tus commits y con `git pull` traés los de tus compañeros.

**Primer paso.** Creá tu cuenta en [github.com](https://github.com) con el mail de la facultad (te sirve para el paquete de estudiante) y seguí el tutorial oficial [Hola mundo](https://docs.github.com/es/get-started/start-your-journey/hello-world), en español.

**Para seguir aprendiendo**

- [GitHub Skills](https://skills.github.com/): cursos cortos y prácticos que se hacen dentro del propio GitHub.
- [GitHub Student Developer Pack](https://education.github.com/pack): herramientas gratis para estudiantes verificados.
- [GitHub Copilot gratis para estudiantes](https://docs.github.com/en/copilot/how-tos/copilot-on-github/set-up-copilot/enable-copilot/set-up-for-students): cómo activarlo con tu cuenta de estudiante.

> Tu perfil de GitHub funciona como portfolio: lo que subas ahí lo puede ver cualquiera, incluidas las empresas que buscan pasantes.

## Docker: que corra en cualquier compu

**Qué es.** Una herramienta que empaqueta tu programa con todo lo que necesita (lenguaje, librerías, configuración) en un *contenedor*, para que corra igual en tu compu, en la del profe o en un servidor. Se acabó el "en mi compu anda".

**Primer paso.** Dos opciones:

- **Sin instalar nada:** [Play with Docker](https://labs.play-with-docker.com/), un entorno de Docker en el navegador (necesitás una cuenta gratuita de Docker Hub).
- **En tu compu:** instalá Docker Desktop siguiendo la [guía oficial](https://docs.docker.com/get-started/) y probá:

```powershell
docker run hello-world
```

**Para seguir aprendiendo**

- [DOCKER De NOVATO a PRO! (curso completo en español)](https://www.youtube.com/watch?v=CV_Uf3Dq-EU), del canal Pelado Nerd: alrededor de una hora, desde cero.
- [¿Qué es un contenedor?](https://docs.docker.com/get-started/docker-concepts/the-basics/what-is-a-container/), en la documentación oficial (en inglés).

## IA: aprender mejor

**La idea.** La IA es tu copiloto, no el piloto. Bien usada, te ayuda a entender más rápido; si la usás para que te haga el TP, el día del parcial (sin IA) no vas a saber nada.

**Cómo usarla para aprender**

1. **Pedile que explique, no que resuelva.** Pegá el error y preguntá por qué pasa.
2. **Dale contexto.** Contale quién sos y qué necesitás.
3. **Verificá siempre.** Se equivoca con total seguridad: probá el código.
4. **Respetá las reglas de cada cátedra.** Antes de usarla en un TP, preguntá. Y nunca pegues contraseñas ni datos personales.

**Probalo así** (copiá este prompt en [Gemini](https://gemini.google.com) o [Claude](https://claude.ai)):

```text
Soy estudiante de primer año de Informática. Este código me da este error: [pegá el error y el código]. Explicame por qué pasa y dame una pista para arreglarlo, pero no me des la solución completa.
```

**Qué tipos de herramientas hay**

| Tipo | Ejemplos | Para qué te sirve |
| --- | --- | --- |
| Chat | Gemini, Claude, ChatGPT | Entender conceptos, errores y enunciados |
| En el editor | GitHub Copilot | Sugerencias y chat dentro de VS Code |
| Agentes de código | Claude Code, Codex CLI, Gemini CLI | Trabajan sobre un proyecto entero. Para más adelante, cuando domines lo básico |

**Podés adaptarla a vos**

- **Instrucciones:** le decís una vez cómo responder ("soy estudiante, explicame paso a paso") y lo aplica siempre.
- **Skills:** una carpeta con un archivo `SKILL.md` que le enseña una tarea concreta. Es un estándar abierto que usan varias herramientas: [agentskills.io](https://agentskills.io).
- **Plugins y MCP:** conectan la IA con otras apps, como GitHub o Google Drive, para que pueda leer o hacer cosas ahí.

## Extras: terminal, IDE y Markdown

- **La terminal.** Muchas herramientas se usan escribiendo comandos. En Windows es PowerShell: [Introducción a PowerShell](https://learn.microsoft.com/es-es/powershell/scripting/learn/ps101/01-getting-started) (Microsoft Learn, en español).
- **Un entorno de desarrollo (IDE).** Editor, terminal, Git y asistentes de IA en un solo lugar. El más usado hoy es [VS Code](https://code.visualstudio.com/), pero hay muchos más (IntelliJ, PyCharm, Eclipse…).
- **Markdown.** El formato de los README y de la documentación de tus TP: [Sintaxis básica de redacción y formato](https://docs.github.com/es/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) (GitHub Docs, en español).

## Un caso real: Charmy

[**Charmy**](https://github.com/cosmosnehu77/Charmy) es un proyecto que hicimos en la NASA Space Apps Challenge 2026: un mapa de más de veinte años de focos de calor de Argentina y Chile vistos desde satélites.

Lo armamos cinco personas, cada una con su propio agente de IA. Los agentes se coordinaban en un *issue* fijado de GitHub que funcionaba como tablero de mensajes: se avisaban qué cambiaban, pedían permiso antes de tocar carpetas ajenas y cada cambio entraba por un *pull request* revisado por las personas del equipo. En 36 horas: **598 commits y 221 pull requests fusionados**.

Todo lo que viste en la charla (Git, GitHub, Docker e IA) está ahí funcionando en un proyecto real. Entrá al repositorio, mirá el historial de commits y los pull requests.

## ¿Dudas?

Abrí un [issue en este repositorio](https://github.com/dimidio6/KIT-ingresantes/issues) con tu pregunta: te respondemos ahí, y de paso practicás GitHub.

---

Hecho por Bruno Aguinaga, Angelo Duarte y Samuel Valenciano para las Jornadas de Informática 2026.
