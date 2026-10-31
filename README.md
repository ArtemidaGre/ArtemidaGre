```text
       /\         artemiy@arch  ·  artemiy@workstation
      /  \        ────────────────────────────────────────────
     /\   \       OS: Arch Linux x86_64 / Ubuntu 26.04 "Resolute Raccoon"
    /      \      Host: MSI Katana 17 · Arch workstation · 1 prod VPS
   /   ,,   \     Kernel: 7.0.0 PREEMPT_DYNAMIC (real-time patched mindset)
  /   |  |  -\    Shell: zsh + tmux · bash · pi (self-extended)
 /_-''    ''-_\   CPU: i5-12450H (12t) + RTX 4060 for local GGUF inference
                  Uptime: 24/7 — five domains behind one nginx-proxy
                  Packages: NestJS, Prisma, Telethon, Docker, Pascal, TypeScript
                  Bench: Arduino/MCU · PCB + enclosure sets · GGUF inference node
                  Memory: High cache hit ratio, 7 GiB in buff/cache
```

```yaml
# system_runtime.yml
identity:
  handle: "artemidagre"
  name: "Artemiy Korobov"
  role: "Backend Architect & Systems tinkerer"
  company: "RVTK"
  location: "RU / Global"

current_focus:
  - project: "Russia in Your Pocket"          # russia-in-your-pocket.ru
    desc: "Travel platform monorepo — NestJS 11 + Prisma 7 + PostGIS, check-in
           gamification, onboarding & route-recommender microservices"
  - project: "Autonomous Digital Twins"
    desc: "Persona-grade Telegram agent with layered memory + self-analysis;
           multi-agent clusters & MCP protocol orchestration"
  - research: "Local LLM edge-inference (Ollama + Q6_K GGUF quants, reasoning
               routing, streaming-first-token) & hardware telemetry"

stack_dump:
  core: [TypeScript, NestJS, Python, Free Pascal, C++, Rust, C]
  web: [React 19, Vite, EJS, SCSS, Kotlin/Android (MapKit)]
  infra: [Docker Compose, systemd, nginx-proxy, Hysteria2, WireGuard, ACME/TLS, GitLab CE, MinIO]
  storage: [PostgreSQL + PostGIS, SQLite/FTS5 + embeddings, Redis, pg/Prisma]
  agent: [MCP (FastMCP clients/servers), pi extensions, Telethon user-client]
  hardware: [Arduino & MCU platforms, PCB topology + enclosure drawings, BOM/costing,
             telemetry gateway (express + sqlite3, controllers(id,value) @ :8080)]
  bench: [RTX 4060 GGUF node, Hysteria2 VPN panel, self-hosted GitLab CE + MinIO,
          Ollama (Gemma Q6_K), Minecraft mega-server with 3.3 GB world]

principles:
  - "docs live next to the code, not in a graveyard"
  - "pytest + ruff as the gate; nothing merges red"
  - "the model should be able to break its own UI — so give it a pastel closet"

ping:
  telegram: "@artemidagre"
  codeforces: "artemidagre"
  web: "https://russia-in-your-pocket.ru"
```

<details open>
<summary><b>🩷 What I'm building right now</b></summary>

<br/>

| Project | What it actually is |
|---|---|
| [`pi-femboy-tui`](https://github.com/ArtemidaGre/pi-femboy-tui) | Pastel TUI chrome takeover for the **pi** coding agent — every visual slot wired: welcome panel, status bar, chibi companion dock, `/femboy` overlay closet, custom tool-row renderers, display-only `uwu` markdown transform, and a headpat economy. TypeScript, zero runtime deps. |
| **Russia in Your Pocket** | Monorepo: `back/` (NestJS 11 + Prisma 7 + PostGIS, REST `/v1`), `onboard/` + `recommender/` (NestJS microservices), `admin/` + `front/` (React/Vite), `app/` (Kotlin + MapKit, AR pose configs), `hardware/` (telemetry gateway). Docker Compose behind a single nginx-proxy. |
| **helper** | A Telegram *persona* (not an assistant) on Telethon: router gate that skips the LLM for short replies, presence layer with typing delays and moods, decaying memory (FTS5 + semantic top-k), nightly curator consolidation, proactive reach-out, group batch decisions, and an embedded FastAPI kanban spoken to over **MCP**. |

<sub>Most of my day lives on a self-hosted GitLab and a private git service — this profile is the pastel-colored reception area.</sub>

</details>

<details>
<summary><b>🔧 Hardware & the bench</b></summary>

<br/>

Code that touches the physical world, and the machines it runs on:

```text
rvtk/hardware/server.js        Node.js · express + sqlite3 · :8080
  POST /update { id, value }   → upsert into controllers(id, value)
  a single-table command/telemetry register — the thin edge a microcontroller
  node talks to before anything in the platform knows a check-in happened.
```

| | |
|---|---|
| **Microcontrollers** | Arduino and friends — the interest that predates the backend job and never left |
| **PCB & mechanical** | RSATU coursework: passive buzzer build — board topology (3D render), enclosure + lid + assembly drawings, cost calculation/BOM |
| **Inference node** | i5-12450H + **RTX 4060** running quantized GGUF locally (Ollama, Gemma Q6_K) — reasoning routing and first-token latency over anything a cloud API would give |
| **Network** | A **Hysteria2** control panel — FastAPI + React + SQLite on one Docker Compose stack: the panel is the auth webhook, Compose's Traffic Stats API drives online/traffic/kick, TLS via ACME HTTP challenge, and the UI is reachable only from a pinned client CIDR through nginx. Plus WireGuard between hosts. |
| **Self-hosted** | GitLab CE + MinIO + mail on the prod box, a decommissioned second host kept as cold backup, and a Minecraft server with a 3.3 GB world that refused to fit on the new box |

</details>

<details>
<summary><b>🧬 Archaeology (how I got here)</b></summary>

<br/>

```text
2022  My-first-py-game- ★2 · box-engine · Simulator-Of-Console-Quest-2 (C#)
2022  BoxOS_V3 (C#)              ← I wanted to write an operating system
2023  BoxEngineM2 / BoxBuilder (C++) ← …and my own game engine
2023  git-node · my-site · site-1    ← then I discovered the web
2025  boxTests · riyp-backend        ← then I discovered production
2026  pi-femboy-tui                  ← then I discovered agent harnesses
```

</details>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=ArtemidaGre&show_icons=true&count_private=true&theme=dark&hide_border=true&bg_color=0d1117" alt="github stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=ArtemidaGre&layout=compact&theme=dark&hide_border=true&bg_color=0d1117&card_width=320" alt="top langs" />
</p>

<p align="center">
  <a href="https://github.com/ArtemidaGre/pi-femboy-tui"><img alt="pi-femboy-tui" src="https://img.shields.io/badge/pastel%20chrome-femboy%20extension-ff9ecd?style=flat-square&labelColor=1a1d23"/></a>
  <a href="https://russia-in-your-pocket.ru"><img alt="riyp" src="https://img.shields.io/badge/Россия%20в%20твоём%20кармане-live-7aa2f7?style=flat-square&labelColor=1a1d23"/></a>
  <a href="https://github.com/QwenLM/qwen-code"><img alt="qwen" src="https://img.shields.io/badge/running-Qwen3--flash-cdA8ff?style=flat-square&labelColor=1a1d23"/></a>
  <img alt="arch" src="https://img.shields.io/badge/Arch%20Linux-rolling-00d5ff?style=flat-square&labelColor=1a1d23"/>
  <img alt="mcu" src="https://img.shields.io/badge/Arduino%20%2F%20MCU-bench-9ece6a?style=flat-square&labelColor=1a1d23"/>
  <img alt="wg" src="https://img.shields.io/badge/Hysteria2%20%2F%20WireGuard-ops-e0af70?style=flat-square&labelColor=1a1d23"/>
  <img alt="gpu" src="https://img.shields.io/badge/RTX%204060-local%20GGUF-f7768e?style=flat-square&labelColor=1a1d23"/>
</p>

<p align="center">
  <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=dark" alt="Dev Quote" />
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=ArtemidaGre&style=flat-square&color=ff9ecd&label=visits" alt="profile views" />
  <sub>・˚ ✧ ˚・ &nbsp; <code>theme: femboy · outfit: Pastel Sailor · mood: fluffy</code> &nbsp; ・˚ ✧ ˚・</sub>
</p>
