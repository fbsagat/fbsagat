# Hi 👋, I'm Fábio Augusto

🚀 **Software, Web & Game Engineer** | Python · JavaScript · TypeScript · GDScript · HTML/CSS
🇧🇷 Brazil

I design and build scalable software systems, production web platforms, backend services, multiplayer experiences, and independent software products focused on **architecture, performance, security, automation, infrastructure, and operational autonomy**.

I work across the complete product lifecycle — from architecture and implementation to infrastructure, deployment, monitoring, payments, desktop/mobile clients, and production operations.

I also actively explore **open-source AI and agentic software development**, using AI coding agents as part of my engineering workflow.

---

## 🌐 Website & Profiles

<p align="left">
  <a href="http://memetrigger.com"><img src="https://img.shields.io/badge/MemeTrigger-LIVE%20IN%20PRODUCTION-111111?style=for-the-badge&logo=googlechrome&logoColor=white" /></a>
  <a href="https://github.com/fbsagat"><img src="https://img.shields.io/badge/GitHub-fbsagat-181717?style=for-the-badge&logo=github" /></a>
  <a href="https://www.linkedin.com/in/fbaugustosantos"><img src="https://img.shields.io/badge/LinkedIn-Fábio%20Augusto%20Santos-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://www.facebook.com/fbaugusto"><img src="https://img.shields.io/badge/Facebook-fbaugusto-1877F2?style=for-the-badge&logo=facebook&logoColor=white" /></a>
</p>

---

# 🚀 MemeTrigger

<a href="http://memetrigger.com"><img src="https://img.shields.io/badge/🌐%20memetrigger.com-PRODUCTION-111111?style=for-the-badge" /></a>

**MemeTrigger** is a full-stack social soundboard and launchpad platform where users record or upload short audio clips ("instants"), organize them into collections, share them publicly, privately, or through unlisted links, and discover community content.

**The platform is live in production.**

### Product

<p align="left">
<img src="https://img.shields.io/badge/Soundboards-Short%20Audio-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Collections-Organization-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Community-Country%20Discovery-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Sharing-Public%20%7C%20Private%20%7C%20Unlisted-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Voting-Social%20Features-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Moderation-Realtime-181717?style=flat-square" />
<img src="https://img.shields.io/badge/i18n-14%20Languages-181717?style=flat-square" />
<img src="https://img.shields.io/badge/RTL-Arabic-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Themes-Customizable-181717?style=flat-square" />
</p>

### Companion Apps

<p align="left">
<img src="https://img.shields.io/badge/Windows-Tauri%202-24C8DB?style=flat-square&logo=tauri&logoColor=white" />
<img src="https://img.shields.io/badge/Rust-Desktop-000000?style=flat-square&logo=rust&logoColor=white" />
<img src="https://img.shields.io/badge/WebView2-Microsoft-0078D4?style=flat-square" />
<img src="https://img.shields.io/badge/Global%20Hotkeys-Supported-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Game%20Overlay-Supported-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Android-TWA-3DDC84?style=flat-square&logo=android&logoColor=white" />
<img src="https://img.shields.io/badge/Mobile%E2%86%92Desktop-Realtime%20Control-181717?style=flat-square" />
</p>

### Platform Capabilities

<p align="left">
<img src="https://img.shields.io/badge/Auth-JWT%20%2B%20Refresh%20Rotation-181717?style=flat-square" />
<img src="https://img.shields.io/badge/RBAC-Granular%20Permissions-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Payments-Subscriptions-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Bitcoin-Self--Custodial-F7931A?style=flat-square&logo=bitcoin&logoColor=white" />
<img src="https://img.shields.io/badge/Webhooks-Payment%20Confirmation-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Storage-S3%20Compatible-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Presigned%20URLs-Supported-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Soft%20Delete-Implemented-181717?style=flat-square" />
</p>

---

# 🏗️ Production Architecture

```text
Users
  │
  ▼
Cloudflare
  │
  ├──────────────► Vercel
  │                 React / TypeScript / Vite
  │
  └──────────────► Oracle Cloud VPS
                    │
                    ▼
                  Nginx
                    │
        ┌───────────┼────────────┐
        ▼           ▼            ▼
      Flask      Celery         SSE
       API       Workers       Realtime
        │           │
        ├───────────┼───────────┐
        ▼           ▼           ▼
   PostgreSQL     Redis       Tasks
        │
        ▼
 Cloudflare R2
  Media / CDN
```

### Production Infrastructure

<p align="left">
<img src="https://img.shields.io/badge/Oracle%20Cloud-VPS-F80000?style=flat-square&logo=oracle&logoColor=white" />
<img src="https://img.shields.io/badge/Ubuntu-24.04-E95420?style=flat-square&logo=ubuntu&logoColor=white" />
<img src="https://img.shields.io/badge/Docker-Compose-2496ED?style=flat-square&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/Nginx-Reverse%20Proxy-009639?style=flat-square&logo=nginx&logoColor=white" />
<img src="https://img.shields.io/badge/Cloudflare-Edge%20%2F%20WAF%20%2F%20TLS-F38020?style=flat-square&logo=cloudflare&logoColor=white" />
<img src="https://img.shields.io/badge/Cloudflare%20R2-Media%20%2F%20CDN-F38020?style=flat-square" />
<img src="https://img.shields.io/badge/Vercel-Frontend-000000?style=flat-square&logo=vercel&logoColor=white" />
<img src="https://img.shields.io/badge/Tailscale-Private%20Access-4C75F2?style=flat-square&logo=tailscale&logoColor=white" />
</p>

### Security

<p align="left">
<img src="https://img.shields.io/badge/TLS-Full%20Strict-181717?style=flat-square" />
<img src="https://img.shields.io/badge/mTLS-Origin%20Protection-181717?style=flat-square" />
<img src="https://img.shields.io/badge/WAF-Cloudflare-F38020?style=flat-square" />
<img src="https://img.shields.io/badge/Rate%20Limiting-Nginx-009639?style=flat-square" />
<img src="https://img.shields.io/badge/CrowdSec-Security-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Fail2Ban-Security-181717?style=flat-square" />
<img src="https://img.shields.io/badge/UFW-Firewall-181717?style=flat-square" />
</p>

### Observability

<p align="left">
<img src="https://img.shields.io/badge/Prometheus-Metrics-E6522C?style=flat-square&logo=prometheus&logoColor=white" />
<img src="https://img.shields.io/badge/Grafana-Dashboards-F46800?style=flat-square&logo=grafana&logoColor=white" />
<img src="https://img.shields.io/badge/Loki-Logs-F46800?style=flat-square&logo=grafana&logoColor=white" />
<img src="https://img.shields.io/badge/Alloy-Log%20Collection-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Netdata-Monitoring-00AB44?style=flat-square&logo=netdata&logoColor=white" />
<img src="https://img.shields.io/badge/Flower-Celery-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Uptime%20Kuma-Uptime-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Sentry-Errors-362D59?style=flat-square&logo=sentry&logoColor=white" />
</p>

---

# 🧠 What I Do

<p align="left">
<img src="https://img.shields.io/badge/Backend-Python%20%2F%20Flask%20%2F%20Django-3776AB?style=flat-square&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Architecture-Scalable%20Systems-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Realtime-Event--Driven-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Async-Celery%20%2F%20Redis-37814A?style=flat-square" />
<img src="https://img.shields.io/badge/APIs-REST%20%2F%20Secure-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Auth-JWT%20%2F%20RBAC-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Payments-Subscriptions-635BFF?style=flat-square" />
<img src="https://img.shields.io/badge/Bitcoin-Self--Custodial-F7931A?style=flat-square&logo=bitcoin&logoColor=white" />
<img src="https://img.shields.io/badge/DevOps-Docker%20%2F%20Linux-2496ED?style=flat-square" />
<img src="https://img.shields.io/badge/Security-Defense%20in%20Depth-181717?style=flat-square" />
<img src="https://img.shields.io/badge/AI-Agentic%20Development-blueviolet?style=flat-square" />
<img src="https://img.shields.io/badge/Automation-Systems-orange?style=flat-square" />
<img src="https://img.shields.io/badge/PDF-Reports%20%2F%20Documents-red?style=flat-square" />
<img src="https://img.shields.io/badge/Game%20Development-Godot%20%2F%20GDScript-478CBF?style=flat-square&logo=godot-engine&logoColor=white" />
</p>

---

# 🛠️ Technology Stack

### Backend & Web

<p align="left">
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white" />
<img src="https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white" />
<img src="https://img.shields.io/badge/JavaScript-323330?style=flat-square&logo=javascript&logoColor=F7DF1E" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
<img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" />
<img src="https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white" />
<img src="https://img.shields.io/badge/Gunicorn-499848?style=flat-square&logo=gunicorn&logoColor=white" />
<img src="https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white" />
</p>

### Async, Queues & Realtime

<p align="left">
<img src="https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white" />
<img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white" />
<img src="https://img.shields.io/badge/Redis-D92C20?style=flat-square&logo=redis&logoColor=white" />
<img src="https://img.shields.io/badge/WebSocket-010101?style=flat-square" />
<img src="https://img.shields.io/badge/SSE-Realtime-181717?style=flat-square" />
<img src="https://img.shields.io/badge/AMQP-FC4C02?style=flat-square&logo=rabbitmq&logoColor=white" />
</p>

### Database, Storage & Cloud

<p align="left">
<img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/MinIO-C72E49?style=flat-square&logo=minio&logoColor=white" />
<img src="https://img.shields.io/badge/Cloudflare%20R2-F38020?style=flat-square&logo=cloudflare&logoColor=white" />
<img src="https://img.shields.io/badge/S3-Compatible-569A31?style=flat-square&logo=amazons3&logoColor=white" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
<img src="https://img.shields.io/badge/Oracle%20Cloud-F80000?style=flat-square&logo=oracle&logoColor=white" />
<img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white" />
<img src="https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white" />
</p>

### Monitoring & Operations

<p align="left">
<img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white" />
<img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white" />
<img src="https://img.shields.io/badge/Loki-F46800?style=flat-square&logo=grafana&logoColor=white" />
<img src="https://img.shields.io/badge/Alloy-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Netdata-00AB44?style=flat-square&logo=netdata&logoColor=white" />
<img src="https://img.shields.io/badge/Uptime%20Kuma-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white" />
<img src="https://img.shields.io/badge/Tailscale-4C75F2?style=flat-square&logo=tailscale&logoColor=white" />
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
</p>

### Game Development

<p align="left">
<img src="https://img.shields.io/badge/Godot-478CBF?style=flat-square&logo=godot-engine&logoColor=white" />
<img src="https://img.shields.io/badge/GDScript-355570?style=flat-square&logo=godot-engine&logoColor=white" />
<img src="https://img.shields.io/badge/Multiplayer-Networking-blue?style=flat-square" />
<img src="https://img.shields.io/badge/Authoritative%20Server-darkgreen?style=flat-square" />
</p>

### Desktop, Mobile & Tools

<p align="left">
<img src="https://img.shields.io/badge/Tauri-24C8DB?style=flat-square&logo=tauri&logoColor=white" />
<img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" />
<img src="https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white" />
<img src="https://img.shields.io/badge/WebView2-0078D4?style=flat-square&logo=microsoft&logoColor=white" />
<img src="https://img.shields.io/badge/PyQt6-41CD52?style=flat-square&logo=qt&logoColor=white" />
</p>

### Payments

<p align="left">
<img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white" />
<img src="https://img.shields.io/badge/Bitcoin-F7931A?style=flat-square&logo=bitcoin&logoColor=white" />
<img src="https://img.shields.io/badge/Payment%20Systems-Automation-181717?style=flat-square" />
</p>

---

# 🤖 AI-Assisted Engineering

I use AI as an **engineering multiplier**, not simply as a code autocomplete tool.

My workflow includes:

<p align="left">
<img src="https://img.shields.io/badge/Code%20Exploration-AI-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Architecture%20Analysis-AI-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Implementation-AI-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Refactoring-AI-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Debugging-AI-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Testing-AI-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Security%20Review-AI-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Documentation-AI-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Repository%20Maintenance-AI-181717?style=flat-square" />
</p>

The development process is structured around explicit project instructions, specialized agents, reusable skills, documentation, development plans, and validation.

---

# ⚡ OpenCode

<a href="https://opencode.ai"><img src="https://img.shields.io/badge/OpenCode-Open--Source%20AI%20Coding%20Agent-000000?style=for-the-badge" /></a>

I use **OpenCode** as an open-source AI coding agent for repository exploration, architecture, implementation, debugging, refactoring, testing, documentation, and maintenance.

OpenCode supports multiple LLM providers and models and can be used through terminal, desktop, or IDE environments.

### Agentic Workflow

```text
AGENTS.md
   +
.opencode/skills/
   +
agents/
   +
Project Documentation
   +
TODO / Development Plans
        │
        ▼
     OpenCode
        │
   ┌────┼─────┐
   ▼    ▼     ▼
 Plan Explore Build
   │    │     │
   └────┴─────┘
         │
         ▼
   Implementation
         │
         ▼
   Testing / Review
         │
         ▼
      Git / Deploy
```

### Specialized Agents

<p align="left">
<img src="https://img.shields.io/badge/Backend-Agent-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Frontend-Agent-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Desktop-Agent-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Security-Agent-181717?style=flat-square" />
<img src="https://img.shields.io/badge/i18n-Agent-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Infrastructure-Agent-181717?style=flat-square" />
</p>

MemeTrigger uses project-level AI development conventions including `AGENTS.md`, specialized agents under `agents/`, and reusable procedures under `.opencode/skills/`.

AI accelerates exploration and implementation, but architectural, security, product, infrastructure, validation, and production decisions remain engineering responsibilities.

---

# 🌍 Internationalization

<p align="left">
<img src="https://img.shields.io/badge/14%20Languages-Supported-181717?style=flat-square" />
<img src="https://img.shields.io/badge/i18next-Localization-26A69A?style=flat-square" />
<img src="https://img.shields.io/badge/RTL-Arabic-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Country--Aware%20Discovery-Supported-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Country%20Pricing-Supported-181717?style=flat-square" />
</p>

Localization is treated as part of the application architecture rather than as a final-stage feature.

---

# 📚 Documentation & System Design

Technical documentation is treated as part of the software.

MemeTrigger maintains documentation covering:

<p align="left">
<img src="https://img.shields.io/badge/Architecture-Documented-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Backend-Documented-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Frontend-Documented-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Infrastructure-Documented-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Deployment-Documented-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Auth%20%2F%20Security-Documented-181717?style=flat-square" />
<img src="https://img.shields.io/badge/i18n-Documented-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Payments-Documented-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Subscriptions-Documented-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Backup%20%2F%20Recovery-Documented-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Secrets-Documented-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Scalability-Documented-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Runbooks-Documented-181717?style=flat-square" />
</p>

---

# 🔐 Security & Operational Autonomy

I prefer architectures that provide clear system boundaries, server-side validation, observability, backup and recovery, secret rotation, infrastructure visibility, and reduced dependence on unnecessary external services.

Core principles:

<p align="left">
<img src="https://img.shields.io/badge/Security%20by%20Design-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Server--Side%20Validation-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Explicit%20Boundaries-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Observable%20Systems-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Reproducible%20Deployments-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Backup%20%26%20Recovery-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Secret%20Rotation-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Provider%20Independence-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Infrastructure%20Autonomy-181717?style=flat-square" />
</p>

---

# 💻 Development Environment

<p align="left">
<img src="https://img.shields.io/badge/Windows%2011-0078D4?style=flat-square&logo=windows&logoColor=white" />
<img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
<img src="https://img.shields.io/badge/PyCharm-000000?style=flat-square&logo=pycharm&logoColor=white" />
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/Docker%20Compose-2496ED?style=flat-square&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/OpenCode-000000?style=flat-square" />
<img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" />
</p>

---

# 📊 GitHub Stats

<p align="center">
  <img width="48%" src="https://ghstats.dev/api/card?username=fbsagat&theme=tokyonight" />
  <img width="44%" src="https://github-readme-streak-stats.herokuapp.com/?user=fbsagat&theme=tokyonight&hide_border=true" />
</p>

---

# 🚀 Currently Building

### MemeTrigger

**A production-grade social soundboard platform combining:**

<p align="center">
<img src="https://img.shields.io/badge/Web-React%20%2B%20TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/Backend-Flask-000000?style=for-the-badge&logo=flask&logoColor=white" />
<img src="https://img.shields.io/badge/Realtime-SSE%20%2B%20Redis-D92C20?style=for-the-badge&logo=redis&logoColor=white" />
<img src="https://img.shields.io/badge/Desktop-Tauri%202-24C8DB?style=for-the-badge&logo=tauri&logoColor=white" />
<img src="https://img.shields.io/badge/Android-TWA-3DDC84?style=for-the-badge&logo=android&logoColor=white" />
<img src="https://img.shields.io/badge/Payments-Multi--Provider-635BFF?style=for-the-badge" />
<img src="https://img.shields.io/badge/Bitcoin-Self--Custodial-F7931A?style=for-the-badge&logo=bitcoin&logoColor=white" />
<img src="https://img.shields.io/badge/Cloud-Cloudflare%20%2B%20Oracle-F38020?style=for-the-badge&logo=cloudflare&logoColor=white" />
<img src="https://img.shields.io/badge/AI-OpenCode-000000?style=for-the-badge" />
</p>

🌐 **http://memetrigger.com**

The platform is actively evolving across web, desktop, mobile, realtime communication, payments, infrastructure, community features, and AI-assisted development.

---

# 🧭 Engineering Philosophy

> *"I don't just build software.*
>
> *I build systems designed to be scalable, authoritative, efficient, secure, and independent."*

```text
Requirements
      ↓
Architecture
      ↓
Implementation
      ↓
Security
      ↓
Testing
      ↓
Deployment
      ↓
Observability
      ↓
Maintenance
      ↓
Evolution
```

<p align="left">
<img src="https://img.shields.io/badge/Architecture%20First-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Automation%20First-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Security%20by%20Design-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Observable%20Production-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Infrastructure%20Autonomy-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Provider%20Independence-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Reproducible%20Deployments-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Documentation%20as%20Engineering-181717?style=flat-square" />
<img src="https://img.shields.io/badge/AI%20as%20Multiplier-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Human%20Judgment-181717?style=flat-square" />
</p>

---

# 🤝 Collaboration

<p align="left">
<img src="https://img.shields.io/badge/Software%20Architecture-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Backend%20Engineering-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Distributed%20Systems-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Multiplayer-478CBF?style=flat-square" />
<img src="https://img.shields.io/badge/Game%20Development-478CBF?style=flat-square" />
<img src="https://img.shields.io/badge/AI%20Engineering-blueviolet?style=flat-square" />
<img src="https://img.shields.io/badge/Automation-orange?style=flat-square" />
<img src="https://img.shields.io/badge/Infrastructure-F38020?style=flat-square" />
<img src="https://img.shields.io/badge/Developer%20Tools-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Independent%20Products-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Payments-635BFF?style=flat-square" />
<img src="https://img.shields.io/badge/Bitcoin-F7931A?style=flat-square&logo=bitcoin&logoColor=white" />
<img src="https://img.shields.io/badge/Realtime%20Systems-181717?style=flat-square" />
<img src="https://img.shields.io/badge/Scalable%20Platforms-181717?style=flat-square" />
</p>

⭐ If you like my work, consider starring a repository.

🤝 Open to collaborations, partnerships, interesting technical challenges, and independent software projects.

---

<p align="center">

### Building software. Designing systems. Automating the work.

</p>
