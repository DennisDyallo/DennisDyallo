```
                 /\_/\
                ( o.o )
                 > ^ <    "In code we trust, in bugs we debug."
              /|      |\
             (_|      |_)
```

# Dennis Dyallo

**Senior Software Engineer @ Yubico** | Open Source Maintainer | Certified Scrum Master
*Building secure systems, AI workflows, and the occasional decentralized dream*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dennis-dyallo)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=flat&logo=github&logoColor=white)](https://github.com/DennisDyallo)
[![Linktree](https://img.shields.io/badge/Linktree-43E55E?style=flat&logo=linktree&logoColor=white)](https://linktr.ee/dyallo)

📍 Stockholm, Sweden | 🗣️ English, Swedish (native) | Spanish, Portuguese (elementary)

---

## Who am I?

Full-stack dev (mostly backend) with 11 years building microservices, APIs, and fixing thread safety bugs. BSc in Computer Science from Stockholm University.

I like writing clean C#, test-driven development, and reducing technical debt. Currently working at the intersection of security, AI, and blockchain—turns out one rabbit hole wasn't enough.

Mission-driven projects that improve society + code that doesn't crash in production + learning new tech = what gets me up in the morning.

---

## What I'm building now

### Yubico — Senior Software Engineer *(Feb 2024 - Present)*

Working on the [Yubico.NET.SDK](https://github.com/Yubico/Yubico.NET.SDK), a cross-platform SDK for YubiKey authentication targeting enterprise customers. Cryptographic signing, PKI, hardware security for .NET devs.

Day-to-day work:
- Authored 120+ PRs, reviewed 75+ PRs from contributors
- Mentoring on crypto correctness, backward compatibility, test quality
- Publishing signed libraries for Windows, macOS, Linux, Android
- Implementing FIDO2/CTAP protocols in C# and C
- Filed and resolved 25+ issues (bug fixes, features, build stuff)
- Performance improvements, logging, reducing tech debt

Some notable work:

#### [PR #325](https://github.com/Yubico/Yubico.NET.SDK/pull/325) — Background thread crash safety (Oct 2024)

Fixed production crashes on macOS when people plugged in/removed YubiKeys. Turns out callbacks were firing on garbage-collected delegates. Implemented thread-safe disposal patterns across all platforms.

31 commits, 4,000+ tests, kept code coverage at 50%. Poll-based event detection on Linux, CFRunLoop timeouts on macOS, deterministic finalizer testing, resource leak detection via file descriptor monitoring.

#### [PR #299](https://github.com/Yubico/Yubico.NET.SDK/pull/299) — CTAP 2.2 protocol support (Sep 2024)

Implemented Client to Authenticator Protocol 2.2 with extension support, encrypted identifiers, FIDO2 capabilities for YubiKey firmware 5.4.3-5.8.3. Kept backward compatibility.

67 files modified, 40 commits, 3,964+ tests across Windows/Ubuntu/macOS. HKDF key derivation (RFC 5869), CBOR encoding, PIN/UV auth protocols, hmac-secret-mc extension.

---

## Experience

### Sveriges Radio — Full-stack developer *(2014 - 2024, 9y 11m)*

Sweden's public radio (think NPR meets Spotify's engineering culture). Started as a dev, became team lead/scrum master for a while, then senior dev. Managed editorial tools and infrastructure.

**Senior developer (2022-2024):**
- Built microservices pipeline from .NET 5 → .NET 8
- Deployed to Kubernetes (Rancher) via ArgoCD + Harbor
- Created health monitoring dashboard (Vue 3 + .NET)
- Modularized GitHub Actions for build processes
- Stack: Aurelia, TypeScript, Vue 3, .NET 8, Azure Service Bus, RabbitMQ, SQL Server, Elasticsearch, Kubernetes

**Scrum master/team lead (2017-2022):**
- Led team managing 30 legacy applications with different tech stacks
- Implemented CI/CD for all systems (TeamCity → Octopus Deploy → GitHub Actions)
- Set up monitoring, logging, health checks everywhere
- Ran agile ceremonies while shipping code
- Transformed legacy chaos into manageable systems

**Full-stack developer (2014-2017):**
- Built CMS from scratch (.NET Core, Knockout.js, Entity Framework, Elasticsearch)
- Architected logging solution (shared library + cluster provisioning)
- Migrated entire user base from legacy to new platform
- Interim Tech Lead for 5 months
- Zero-downtime migration for public-facing infrastructure

---

## Tech stack

### Languages & frameworks
![C#](https://img.shields.io/badge/C%23-239120?style=flat&logo=c-sharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat&logo=dotnet&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat&logo=typescript&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat&logo=rust&logoColor=white)

**Expert (daily use, 5+ years):** C#, .NET Core/.NET 5-8, Entity Framework
**Proficient:** Python, TypeScript, JavaScript, SQL, REST APIs, gRPC
**Familiar:** Rust, C, OAuth, OIDC, FIDO2/CTAP
**Learning:** WebAssembly, blockchain protocols

### Infrastructure
**Expert:** Docker, Git, GitHub Actions
**Proficient:** Kubernetes, Rancher, ArgoCD, Harbor, TeamCity, Octopus Deploy
**Familiar:** Azure (Service Bus, EntraID, S3)

### Databases & monitoring
**Expert:** SQL Server, Elasticsearch
**Proficient:** PostgreSQL, Kibana, Logstash
**Familiar:** Redis

### Currently exploring
- MCP (Model Context Protocol) and AI agent workflows
- Bitcoin and decentralized exchanges
- Rust → WebAssembly compilation
- Hardware authentication and secure enclaves

---

## My projects

### [yubikit-mcp](https://github.com/DennisDyallo/yubikit-mcp) (Python)

MCP server that lets AI assistants manage YubiKey operations. Instead of manual CLI commands, AI agents can discover devices, generate RSA keys on-hardware, configure touch policies, manage OATH/PIV/FIDO2 apps.

Built with FastMCP framework, translates JSON-RPC 2.0 MCP requests into `ykman` CLI operations. Supports Claude Code, VS Code, JetBrains IDEs.

### [fast-agent](https://github.com/DennisDyallo/fast-agent) (Python)

Framework for building AI agent workflows with full MCP support. Makes it easy to iterate on agent architectures without tons of boilerplate.

Features:
- 5 workflow patterns (Chain, Parallel, Evaluator-Optimizer, Router, Orchestrator)
- Interactive debugging
- Swap between Anthropic (Claude) and OpenAI (GPT-4o, o1/o3) via flags
- Config-driven MCP servers
- Multi-modal (images/PDFs)

### [wasm-game-of-life](https://github.com/DennisDyallo/wasm-game-of-life) (Rust)

Conway's Game of Life in Rust compiled to WebAssembly. Sometimes you just need to watch patterns emerge at 60fps.

### [dennisdyallo.github.io](https://github.com/DennisDyallo/dennisdyallo.github.io)

Personal blog and demo apps (Jekyll/HTML). Where I write about tech experiments and occasionally make things work in the browser.

---

## Open source contributions

### [Yubico.NET.SDK](https://github.com/Yubico/Yubico.NET.SDK) (C#)

Open source SDK with 117 stars, 59 forks. My day job, but also where I've contributed 120+ merged PRs. Enterprise authentication for .NET developers.

### Other stuff I'm interested in

**Forked/tracking:**
- [bisq](https://github.com/DennisDyallo/bisq) (Java) - Decentralized Bitcoin exchange, exploring P2P trading infrastructure
- Bitcoin Core - Following development
- Hyperliquid DEX SDK - Current DeFi stuff

**MCP ecosystem:**
- Filed issues in Anthropic's claude-code and MCP python-sdk repos (protocol limitations, feature gaps)
- Active in discussions on MCP development
- Early adopter of Claude Code, Continue, and other agentic coding tools

**Other interests:**
- Bevy (Rust game engine)
- Anki (spaced repetition learning—yes I optimize how I learn)
- Open-WebUI, ChatterUI (LLM interfaces)

---

## GitHub stats

![Pull Shark x3](https://img.shields.io/badge/Pull%20Shark-x3-blue?style=flat)
![Pair Extraordinaire x2](https://img.shields.io/badge/Pair%20Extraordinaire-x2-green?style=flat)
![Quickdraw](https://img.shields.io/badge/Quickdraw-orange?style=flat)
![YOLO](https://img.shields.io/badge/YOLO-red?style=flat)

28 repositories | 52 starred repos | 120+ PRs merged in Yubico.NET.SDK | 75+ PR reviews | 25+ issues filed

---

## Beyond code

### Stockholm Flow — Chair of the board *(2016 - Present)*

Founded and chair Sweden's largest flow arts community, a non-profit spreading poi, staff, and fire spinning. Turns out coordinating flaming objects and developers need similar risk management skills.

### Education

**BSc Computer Science & Software Engineering**
Stockholm University (2011-2014)

### Certifications

- Certified Scrum Master (2016)
- Kubernetes App Developer (2023)
- Elasticsearch Core Developer & Operations (2017)

---

## Looking for

Interested in companies pushing AI integration, blockchain infrastructure, and developer tooling.

**Anthropic:** Already engaged—filed issues in your repos, built two MCP servers, using Claude Code daily. I get MCP architecture (sampling, tools, resources) and bring security consciousness from hardware auth work.

**Block:** Blockchain isn't just buzzwords for me. Forked Bisq, track Bitcoin Core, follow DEX infrastructure. Your mission around economic empowerment and open financial systems aligns with what I care about.

**Similar companies:** Already using AI agents for code reviews, docs, workflow automation. I understand what developers need because I am one.

What I'm looking for:
- Building dev tools that don't suck
- Making security accessible
- Open source communities solving real problems
- Mission-driven work
- Remote-friendly (occasional work from abroad would be nice)

What I bring:
- 11 years shipping systems that work
- Open source experience (120+ PRs authored, 75+ reviewed)
- Mentorship (code reviews on security, architecture, knowledge sharing)
- Cross-platform dev (Windows/macOS/Linux/Android)
- MCP understanding (two production servers built)
- Security background (FIDO2/CTAP, crypto signing, hardware tokens)
- Agile delivery (Scrum Master, led teams through migrations)
- Communication (technical writing, stakeholder management)

---

**Reach out:**
- **Signal:** [@moonkin88.88](https://signal.me/#eu/fPYYsOYSCRmShf67DQB1UwR0c7D94fsmTgLuuBAzaAM-8PsXA2MNiJOz30FTUYrk)
- **LinkedIn:** [in/dennis-dyallo](https://www.linkedin.com/in/dennis-dyallo)
- **Linktree:** [linktr.ee/dyallo](https://linktr.ee/dyallo) (all my links)
- **Portfolio:** [dennisdyallo.github.io](https://dennisdyallo.github.io)
- **GitHub:** You're already here

---

*"Debugging is like being a detective in a crime movie where you're also the murderer."* — Filipe Fortes
*I write tests so my future self doesn't hunt down my past self.*
