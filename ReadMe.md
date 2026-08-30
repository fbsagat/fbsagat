# Hi 👋, I'm Fábio Augusto

🚀 Software, Web & Game Engineer | Python, JavaScript, TypeScript, GDScript, HTML/CSS
🇧🇷 Brazil

I design and build scalable software systems, production web platforms, backend services, multiplayer experiences, and independent software products.

My work focuses on architecture, performance, security, automation, infrastructure, distributed systems, and operational autonomy.

I work across the entire lifecycle of a product — from architecture and backend development to frontend applications, infrastructure, deployment, monitoring, payments, desktop/mobile clients, and production operations.

I also actively explore open-source AI and agentic software development, using AI coding agents as part of my engineering workflow.

---

## 🌐 Website & Profiles

<p align="left">
  <a href="http://memetrigger.com">
    <img src="https://img.shields.io/badge/MemeTrigger-Production-111111?style=for-the-badge&logo=googlechrome&logoColor=white" />
  </a>

  <a href="https://github.com/fbsagat">
    <img src="https://img.shields.io/badge/GitHub-fbsagat-181717?style=for-the-badge&logo=github" />
  </a>

  <a href="https://www.linkedin.com/in/fbaugustosantos">
    <img src="https://img.shields.io/badge/LinkedIn-Fábio%20Augusto%20Santos-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>

  <a href="https://www.facebook.com/fbaugusto">
    <img src="https://img.shields.io/badge/Facebook-fbaugusto-1877F2?style=for-the-badge&logo=facebook&logoColor=white" />
  </a>
</p>

---

# 🚀 MemeTrigger — Production Project

<a href="http://memetrigger.com">
  <img src="https://img.shields.io/badge/🌐%20memetrigger.com-Live%20in%20Production-111111?style=for-the-badge" />
</a>

**MemeTrigger** is a full-stack social soundboard and launchpad platform designed around short audio clips, community discovery, collections, real-time interaction, and companion applications.

Users can record or upload short sounds ("instants"), organize them into collections, share them publicly, privately, or through unlisted links, and discover content from their community.

The platform is currently **running in production**.

### What MemeTrigger includes

* 🎵 Personal soundboards with playable audio pads
* 🔊 Short-form audio clips
* 📚 User collections
* 🌎 Country-based community discovery
* 🔗 Public, private, and unlisted sharing
* ❤️ Favorites and liked collections
* 👍 Voting and play-count systems
* 🚨 Content reporting and moderation
* ⚡ Real-time moderation notifications
* 👤 Authentication and account management
* 🔐 JWT access authentication
* 🔄 Rotating refresh tokens
* 🌍 Internationalization across 14 languages
* 🕌 RTL support for Arabic
* 🎨 Customizable themes
* 💳 Free, Premium, and Premium Plus subscriptions
* 💰 Payment gateway integrations
* ₿ Self-custodial Bitcoin on-chain payments
* 🖥️ Windows desktop companion application
* 📱 Android companion application
* ⌨️ Global keyboard shortcuts
* 🎮 Game overlay
* 📡 Real-time mobile → desktop remote control
* ☁️ Cloud object storage and CDN
* 📊 Production monitoring and observability
* 🛡️ Multi-layer infrastructure security

### Production Architecture

MemeTrigger is not just a frontend application. It is a distributed production system composed of several independent layers.

```text
                         ┌─────────────────────┐
                         │      Users          │
                         └──────────┬──────────┘
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │     Cloudflare      │
                         │  Edge / WAF / TLS   │
                         └──────────┬──────────┘
                                    │
                   ┌────────────────┴────────────────┐
                   │                                 │
                   ▼                                 ▼
          ┌─────────────────┐              ┌─────────────────┐
          │     Vercel      │              │  Oracle Cloud   │
          │ React / Vite    │              │      VPS        │
          └─────────────────┘              └────────┬────────┘
                                                    │
                                           ┌────────▼────────┐
                                           │      Nginx      │
                                           │ Reverse Proxy   │
                                           └────────┬────────┘
                                                    │
                              ┌─────────────────────┼─────────────────────┐
                              │                     │                     │
                              ▼                     ▼                     ▼
                       ┌────────────┐       ┌────────────┐       ┌────────────┐
                       │   Flask    │       │   Celery   │       │     SSE    │
                       │    API     │       │   Workers  │       │   Server   │
                       └─────┬──────┘       └─────┬──────┘       └────────────┘
                             │                    │
                    ┌────────┴────────┐           │
                    │                 │           │
                    ▼                 ▼           ▼
              ┌───────────┐     ┌───────────┐ ┌───────────┐
              │PostgreSQL │     │   Redis   │ │   Tasks   │
              └───────────┘     └───────────┘ └───────────┘

                         ┌─────────────────────┐
                         │    Cloudflare R2    │
                         │     Media / CDN     │
                         └─────────────────────┘
```

### Production Infrastructure

The production environment uses:

* **Oracle Cloud VPS**
* **Ubuntu 24.04**
* **Docker & Docker Compose**
* **Flask**
* **Gunicorn**
* **PostgreSQL**
* **Redis**
* **Celery**
* **Nginx**
* **Cloudflare**
* **Cloudflare R2**
* **Vercel**
* **Prometheus**
* **Grafana**
* **Loki**
* **Alloy**
* **Netdata**
* **Flower**
* **Uptime Kuma**
* **Sentry**
* **CrowdSec**
* **Fail2Ban**
* **UFW**
* **Tailscale**

The infrastructure is designed with security boundaries, observability, backups, origin protection, rate limiting, and operational recovery in mind.

---

# 🏗️ Engineering

I work primarily with systems where the software architecture matters as much as the individual feature.

### Backend Engineering

* REST APIs
* Flask and Django
* SQLAlchemy
* PostgreSQL
* Authentication systems
* JWT
* Refresh-token rotation
* RBAC
* Authorization
* API validation
* Background processing
* Async task queues
* Webhooks
* Payment processing
* File storage
* Presigned URLs
* Soft deletion
* Domain-driven service layers

### Distributed & Realtime Systems

* Celery
* Redis
* RabbitMQ
* WebSocket
* Server-Sent Events
* Pub/Sub
* Remote-control systems
* Event-driven workflows
* Background workers
* Scheduled jobs

### Infrastructure

* Linux
* Docker
* Docker Compose
* Nginx
* Cloudflare
* Oracle Cloud
* Vercel
* Cloudflare R2
* S3-compatible storage
* TLS
* mTLS
* Origin protection
* WAF
* DDoS protection
* Rate limiting
* Monitoring
* Logging
* Alerting
* Backup and recovery

### Security

I treat security as part of system architecture rather than a final step.

Areas I work with include:

* Authentication
* Authorization
* RBAC
* JWT security
* Refresh-token rotation
* HTTP security
* TLS
* mTLS
* Origin locking
* Rate limiting
* Firewall configuration
* Cloud security
* Secret management
* Backup security
* Infrastructure isolation
* Server validation
* Webhook verification

---

# 🎮 Game Development

I also develop multiplayer systems and games using **Godot and GDScript**, with particular interest in networking architecture and authoritative server design.

### Areas of interest

* Multiplayer networking
* Authoritative servers
* Client/server architecture
* Server-side validation
* Synchronization
* Game state management
* Networked gameplay
* Dedicated servers
* Real-time systems
* Performance optimization
* Godot
* GDScript

I am particularly interested in systems where the server is the source of truth and clients are treated as untrusted participants.

---

# 💻 Desktop & Mobile

MemeTrigger extends beyond the browser into companion applications.

### Windows

The desktop application is built using:

* Tauri 2
* Rust
* WebView2
* Global keyboard shortcuts
* System tray
* Game overlay
* Automatic updates
* Remote control

The desktop application reuses the same accounts and backend infrastructure as the web platform.

### Android

The Android application uses:

* Trusted Web Activity
* Bubblewrap
* The existing MemeTrigger web application
* The same backend
* The same user accounts

The goal is to maintain a unified product rather than create completely independent platforms.

---

# 🧠 AI-Assisted Software Engineering

AI is an active part of my development workflow.

I use AI not only to generate code, but as an engineering tool for:

* Codebase exploration
* Architecture analysis
* Debugging
* Refactoring
* Feature implementation
* Documentation
* Testing
* Security analysis
* Dependency research
* Repository maintenance
* Development planning
* Repetitive engineering tasks

My approach is **agentic software development**: the AI operates inside a structured repository with explicit project rules, documentation, specialized agents, skills, and development conventions.

---

# 🤖 OpenCode

I use **OpenCode** as an open-source AI coding agent as part of my development workflow.

OpenCode provides an agentic development environment that can operate from the terminal, desktop, or IDE, and supports different LLM providers and models.

<a href="https://opencode.ai">
  <img src="https://img.shields.io/badge/OpenCode-Open--Source%20AI%20Coding%20Agent-000000?style=for-the-badge" />
</a>

### How I use OpenCode

I use OpenCode for substantially more than autocomplete or isolated code generation.

My workflow can involve:

```text
Project
   │
   ├── AGENTS.md
   │
   ├── .opencode/
   │   └── skills/
   │
   ├── agents/
   │   ├── backend
   │   ├── frontend
   │   ├── desktop
   │   ├── security
   │   ├── i18n
   │   └── infrastructure
   │
   ├── Documentation
   │
   └── TODO / Development Plans
           │
           ▼
      OpenCode Agents
           │
     ┌─────┼─────┐
     ▼     ▼     ▼
   Plan  Explore  Build
     │     │       │
     └─────┴───────┘
             │
             ▼
       Implementation
             │
             ▼
       Tests / Review
             │
             ▼
        Git / Deploy
```

The MemeTrigger repository contains project-level instructions, specialized AI agents, skills, technical documentation, and an explicit development workflow.

OpenCode itself supports primary agents such as **Build** and **Plan**, as well as specialized subagents for tasks such as exploration and multi-step work. Custom agents can also be defined for project-specific workflows.

### AI does not replace engineering judgment

My approach is to use AI as an engineering multiplier.

The developer remains responsible for:

* Architecture
* Requirements
* Security decisions
* Infrastructure decisions
* Product decisions
* Code review
* Validation
* Production deployment
* Operational responsibility

AI accelerates implementation and exploration, but the system still needs engineering discipline.

---

# 🛠️ Tech Stack

## 🚀 Backend & Web

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge\&logo=python\&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge\&logo=flask\&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge\&logo=django\&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge\&logo=javascript\&logoColor=F7DF1E)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge\&logo=typescript\&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge\&logo=react\&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge\&logo=vite\&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge\&logo=sqlalchemy\&logoColor=white)
![Gunicorn](https://img.shields.io/badge/Gunicorn-499848?style=for-the-badge\&logo=gunicorn\&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge\&logo=nginx\&logoColor=white)

---

## ⚡ Async, Queue & Realtime

![Celery](https://img.shields.io/badge/Celery-37814A?style=for-the-badge\&logo=celery\&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge\&logo=rabbitmq\&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-D92C20?style=for-the-badge\&logo=redis\&logoColor=white)
![WebSocket](https://img.shields.io/badge/WebSocket-010101?style=for-the-badge)
![SSE](https://img.shields.io/badge/Server--Sent%20Events-Realtime-111111?style=for-the-badge)
![AMQP](https://img.shields.io/badge/AMQP-FC4C02?style=for-the-badge\&logo=rabbitmq\&logoColor=white)

---

## 🗄️ Database & Storage

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge\&logo=postgresql\&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-D92C20?style=for-the-badge\&logo=redis\&logoColor=white)
![MinIO](https://img.shields.io/badge/MinIO-C72E49?style=for-the-badge\&logo=minio\&logoColor=white)
![Cloudflare R2](https://img.shields.io/badge/Cloudflare%20R2-F38020?style=for-the-badge\&logo=cloudflare\&logoColor=white)
![S3](https://img.shields.io/badge/S3-Compatible-569A31?style=for-the-badge\&logo=amazons3\&logoColor=white)

---

## ☁️ Infrastructure & DevOps

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge\&logo=docker\&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge\&logo=linux\&logoColor=black)
![Oracle Cloud](https://img.shields.io/badge/Oracle%20Cloud-F80000?style=for-the-badge\&logo=oracle\&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge\&logo=cloudflare\&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge\&logo=vercel\&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge\&logo=nginx\&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge\&logo=git\&logoColor=white)
![Tailscale](https://img.shields.io/badge/Tailscale-4C75F2?style=for-the-badge\&logo=tailscale\&logoColor=white)

---

## 📊 Observability

![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge\&logo=prometheus\&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge\&logo=grafana\&logoColor=white)
![Loki](https://img.shields.io/badge/Loki-F46800?style=for-the-badge\&logo=grafana\&logoColor=white)
![Sentry](https://img.shields.io/badge/Sentry-362D59?style=for-the-badge\&logo=sentry\&logoColor=white)
![Netdata](https://img.shields.io/badge/Netdata-00AB44?style=for-the-badge\&logo=netdata\&logoColor=white)

---

## 🎮 Game Development

![Godot](https://img.shields.io/badge/Godot-478CBF?style=for-the-badge\&logo=godot-engine\&logoColor=white)
![GDScript](https://img.shields.io/badge/GDScript-355570?style=for-the-badge\&logo=godot-engine\&logoColor=white)
![Multiplayer](https://img.shields.io/badge/Multiplayer-Networking-blue?style=for-the-badge)
![Authoritative Server](https://img.shields.io/badge/Authoritative-Server-darkgreen?style=for-the-badge)

---

## 🖥️ Desktop & Mobile

![Tauri](https://img.shields.io/badge/Tauri-24C8DB?style=for-the-badge\&logo=tauri\&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge\&logo=rust\&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge\&logo=android\&logoColor=white)
![WebView2](https://img.shields.io/badge/WebView2-0078D4?style=for-the-badge\&logo=microsoft\&logoColor=white)

---

## 💳 Payments & Bitcoin

![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=for-the-badge\&logo=stripe\&logoColor=white)
![Bitcoin](https://img.shields.io/badge/Bitcoin-F7931A?style=for-the-badge\&logo=bitcoin\&logoColor=white)

I am particularly interested in payment systems that provide automation, reliability, and control over the infrastructure.

MemeTrigger includes multiple payment paths, including traditional payment processing, cryptocurrency payments, and a self-custodial Bitcoin on-chain architecture.

---

## 🌍 Internationalization

I build software intended to operate across different markets and languages.

MemeTrigger currently supports:

* 14 languages
* RTL interfaces
* Country-aware discovery
* Country-based pricing
* International payment considerations
* Localized frontend interfaces

The architecture is designed so that localization is part of the application rather than an afterthought.

---

# 📚 Documentation & System Design

I consider technical documentation part of the software itself.

MemeTrigger maintains documentation covering:

* System architecture
* Backend architecture
* Frontend architecture
* Infrastructure
* Deployment
* Authentication
* Security
* Internationalization
* Payments
* Subscriptions
* Themes
* Remote control
* Backup and recovery
* Secret rotation
* Operational runbooks
* Scalability
* Desktop architecture
* Android deployment

The repository also maintains explicit development plans and operational documentation.

---

# 🔐 Security & Operational Autonomy

One of my main engineering goals is to reduce unnecessary dependency on external infrastructure while still taking advantage of managed services where they provide meaningful value.

I prefer architectures where:

* Services have clear boundaries
* Sensitive operations are validated server-side
* Infrastructure can be inspected and operated independently
* Backups exist outside the primary environment
* Production systems are observable
* Secrets can be rotated
* Failure scenarios are considered before deployment
* External services can be replaced when practical

This philosophy influences both software architecture and infrastructure design.

---

# ⚙️ Development Environment

My development environment is primarily based around:

* Windows 11
* Linux
* PyCharm
* Git
* Docker
* Docker Compose
* OpenCode
* GitHub
* Cloud infrastructure
* Local and remote development environments

I also use specialized tooling depending on the project, including AI/ML frameworks, audio processing tools, automation systems, and game-development tooling.

---

# 📈 GitHub Stats

<p align="center">
  <img width="52%" src="https://ghstats.dev/api/card?username=fbsagat&theme=tokyonight" />
  <img width="40%" src="https://github-readme-streak-stats.herokuapp.com/?user=fbsagat&theme=tokyonight&hide_border=true" />
</p>

---

# 🚀 Currently Building

## MemeTrigger

A production-grade social soundboard platform combining:

```text
Web
+
Backend
+
Realtime
+
Desktop
+
Android
+
Payments
+
Bitcoin
+
Cloud Infrastructure
+
Observability
+
AI-Assisted Development
```

🌐 **http://memetrigger.com**

The project is continuously evolving from a soundboard application into a broader software platform with web, desktop, mobile, realtime, payment, and community capabilities.

---

# 🧭 Engineering Philosophy

> *"I don't just build software.*
>
> *I build systems designed to be scalable, authoritative, efficient, secure, and independent."*

I believe good software engineering is not only about writing code.

It is about understanding the complete system:

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

I value:

* Architecture over accidental complexity
* Automation over repetitive manual work
* Security by design
* Explicit system boundaries
* Observable production systems
* Infrastructure autonomy
* Provider independence where practical
* Reproducible deployments
* Documentation as part of engineering
* AI as an engineering multiplier
* Human judgment over blind automation

---

# 🤝 Collaboration

I'm interested in:

* Software architecture
* Backend engineering
* Distributed systems
* Multiplayer networking
* Game development
* AI-assisted development
* Open-source AI
* Automation
* Infrastructure
* Developer tools
* Independent software products
* Payments
* Bitcoin
* Real-time systems
* Scalable web platforms

⭐ If you like my work, consider starring a repository.

🤝 Open to collaborations, partnerships, interesting technical challenges, and independent software projects.

---

<p align="center">

### Building software. Designing systems. Automating the work.

</p>
