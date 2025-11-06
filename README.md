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
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:dennis@dyallo.se)

📍 Stockholm, Sweden | 🗣️ English, Swedish (native) | Spanish, Portuguese (elementary)
📱 +46737124377 | 🔗 [dennisdyallo.github.io](https://github.com/DennisDyallo/dennisdyallo.github.io)

---

## 👨‍💻 Who Am I?

A battle-tested full-stack developer (backend focus) with **11+ years** wrangling microservices, APIs, and the occasional thread safety nightmare. BSc in Computer Science from Stockholm University. People describe me as a "stand-up guy"—nerdy, bold, communicative, and supportive (their words, but I'll take it).

I write clean C# like it's poetry, champion test-driven development, and get unreasonably excited about reducing technical debt. Currently living at the intersection of **security, AI, and blockchain**—because apparently one rabbit hole wasn't enough.

**Ikigai check:** Mission-driven projects that improve society + code that doesn't crash in production + learning cutting-edge tech = 🎯

---

## 🔐 What I'm Building Now

### Yubico — Senior Software Engineer *(Feb 2024 - Present)*

Working on the [Yubico.NET.SDK](https://github.com/Yubico/Yubico.NET.SDK)—a cross-platform SDK for YubiKey authentication targeting enterprise customers. Think cryptographic signing, public key infrastructure, and making hardware security accessible to .NET developers.

**Day-to-day:**
- Managing open source repository (reviewing/merging 120+ PRs and counting)
- Publishing cryptographically signed multi-platform libraries (Windows, macOS, Linux, Android)
- Implementing FIDO2/CTAP protocols in C# and C
- Improving performance, logging, and developer experience
- Reducing technical debt (my favorite hobby)

**Notable work that keeps production running:**

#### 🛡️ [PR #325](https://github.com/Yubico/Yubico.NET.SDK/pull/325) — Background Thread Crash Safety (Oct 2024)
*When your callbacks get garbage-collected mid-flight*

Fixed production crashes on macOS when users inserted/removed YubiKeys. The culprit? Background threads invoking callbacks on garbage-collected delegates. The solution? Comprehensive thread-safe disposal patterns across all platforms.

- **Impact:** Eliminated production crashes in long-running services
- **Scale:** 31 commits, 4,000+ tests passing, 50% code coverage maintained
- **Technical depth:** Implemented poll-based event detection on Linux, CFRunLoop timeouts on macOS, deterministic finalizer testing, resource leak detection via file descriptor monitoring
- **Skills:** Concurrency patterns, platform-specific APIs, defensive programming, stress testing

#### 🚀 [PR #299](https://github.com/Yubico/Yubico.NET.SDK/pull/299) — CTAP 2.2 Protocol Support (Sep 2024)
*Upgrading authentication protocols without breaking the internet*

Implemented Client to Authenticator Protocol 2.2 with extension support, encrypted identifiers, and FIDO2 capabilities for YubiKey firmware 5.4.3-5.8.3.

- **Impact:** Enabled modern FIDO2 features while maintaining backward compatibility
- **Scale:** 67 files modified, 40 commits, 3,964+ tests across Windows/Ubuntu/macOS
- **Technical depth:** HKDF key derivation (RFC 5869), CBOR encoding standardization, PIN/UV authentication protocols, hmac-secret-mc extension support
- **Skills:** Security protocols, cryptography, protocol design, multi-platform development

---

## 💼 Experience Highlights

### Sveriges Radio — Full-Stack Developer *(2014 - 2024, 9y 11m)*

Sweden's public radio (think NPR meets Spotify's engineering culture). Progressed from developer → team lead/scrum master → senior developer across three phases managing editorial tools and infrastructure.

**Senior Developer (2022-2024):**
- Built microservices pipeline from .NET 5 → .NET 8
- Deployed to Kubernetes (Rancher) via ArgoCD + Harbor private registry
- Created health monitoring dashboard (Vue 3 + .NET)
- Modularized GitHub Actions for build processes
- **Stack:** Aurelia, TypeScript, Vue 3, .NET 8, Azure Service Bus, RabbitMQ, SQL Server, Elasticsearch, Kubernetes, ArgoCD

**Scrum Master/Team Lead (2017-2022):**
- Led team managing **30 legacy applications** with diverse tech stacks
- Implemented CI/CD for all systems (TeamCity → Octopus Deploy → GitHub Actions)
- Established monitoring, logging, health checks across the application portfolio
- Ran agile ceremonies while shipping code (multitasking level: expert)
- **Achievement:** Transformed legacy chaos into manageable, documented systems

**Full-Stack Developer (2014-2017):**
- Built CMS from scratch (.NET Core, Knockout.js, Entity Framework, Elasticsearch)
- Architected logging solution (shared library + cluster provisioning)
- Migrated entire user base from legacy system to new platform
- Served as interim Tech Lead for 5 months
- **Achievement:** Zero-downtime migration for public-facing radio infrastructure

---

## 🧰 Technical Arsenal

### Languages & Frameworks
![C#](https://img.shields.io/badge/C%23-239120?style=flat&logo=c-sharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat&logo=dotnet&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat&logo=typescript&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat&logo=rust&logoColor=white)

**Primary:** C# (10+ years), .NET Core/.NET 5-8, Entity Framework
**Secondary:** Python, TypeScript, JavaScript, Rust (learning), C (when necessary)
**Protocols:** FIDO2/CTAP, OAuth, OIDC, REST, gRPC

### Infrastructure & DevOps
**Containers:** Docker, Kubernetes, Rancher, ArgoCD, Harbor
**CI/CD:** GitHub Actions, TeamCity, Octopus Deploy
**Cloud:** Azure (Service Bus, EntraID, S3)
**Databases:** SQL Server, Elasticsearch, PostgreSQL
**Monitoring:** Kibana, Logstash, custom health dashboards

### Emerging Tech (Where My Curiosity Lives)
**AI & Agents:** MCP (Model Context Protocol), AI agent workflows, prompt engineering
**Blockchain:** Bitcoin, decentralized exchanges, distributed systems
**WebAssembly:** Rust → WASM experiments
**Security:** Public key cryptography, hardware authentication, secure enclaves

---

## 🚀 Featured Projects

### [yubikit-mcp](https://github.com/DennisDyallo/yubikit-mcp) (Python)
MCP server for YubiKey integration. Bridging hardware security tokens with AI agent workflows—because your LLM should probably authenticate users.

### [fast-agent](https://github.com/DennisDyallo/fast-agent) (Python)
*"Define, Prompt and Test MCP enabled Agents and Workflows"*

Framework for building and testing AI agents using Model Context Protocol. Accelerating the feedback loop between prompt engineering and production deployment.

### [Yubico.NET.SDK](https://github.com/Yubico/Yubico.NET.SDK) (C#)
Open source SDK with **117 stars**, **59 forks**, and **120+ merged PRs** from yours truly. Making enterprise authentication accessible to .NET developers worldwide.

### [wasm-game-of-life](https://github.com/DennisDyallo/wasm-game-of-life) (Rust)
Conway's Game of Life in Rust compiled to WebAssembly. Because sometimes you just need to watch patterns emerge at 60fps.

### [bisq](https://github.com/DennisDyallo/bisq) (Java fork)
Decentralized Bitcoin exchange network. Exploring peer-to-peer trading infrastructure and distributed consensus.

### [dennisdyallo.github.io](https://github.com/DennisDyallo/dennisdyallo.github.io)
Personal blog and demo apps (Jekyll/HTML). Where I write about tech, experiments, and occasionally make things work in the browser.

---

## 🏆 GitHub Achievements

![Pull Shark x3](https://img.shields.io/badge/Pull%20Shark-x3-blue?style=flat)
![Pair Extraordinaire x2](https://img.shields.io/badge/Pair%20Extraordinaire-x2-green?style=flat)
![Quickdraw](https://img.shields.io/badge/Quickdraw-orange?style=flat)
![YOLO](https://img.shields.io/badge/YOLO-red?style=flat)

**28 repositories** | **52 starred repos** | **120+ PRs merged** in Yubico.NET.SDK alone

---

## 🎭 Beyond Code

### Stockholm Flow — Chair of the Board *(2016 - Present)*
Founded and chair Sweden's largest flow arts community—a non-profit spreading poi, staff, and fire spinning across the nation. Turns out coordinating flaming objects and coordinating developers require similar risk management skills.

### Education
**BSc Computer Science & Software Engineering**
Stockholm University (2011-2014)

### Certifications & Training
- Certified Scrum Master (2016)
- Kubernetes App Developer (2023)
- Elasticsearch Core Developer & Operations (2017)

---

## 💬 Let's Talk

I'm particularly interested in roles at companies pushing the boundaries of AI integration, blockchain infrastructure, and developer tooling. If you're at **Anthropic** (MCP evangelist here), **Block** (decentralized systems enthusiast), **Windsurf** (AI-enhanced IDEs are the future), or anywhere experimenting with AI in production—I want to hear from you.

**What gets me out of bed:**
- Building developer tools that don't suck
- Making security accessible (hardware tokens + AI agents = 🤯)
- Open source communities solving real problems
- Mission-driven work with societal impact
- Remote-friendly cultures (occasional work-from-abroad? Yes please)

**What I bring:**
- Production-hardened code that scales
- Open source maintenance experience (PR reviews, community management)
- Cross-platform development chops (Windows/macOS/Linux/Android)
- Agile delivery methods and stakeholder management
- Strong communication skills (presentations, documentation, teaching)
- Passion for learning and adapting (see: current tech stack evolution)

---

**📫 Reach out:**
- Email: [dennis@dyallo.se](mailto:dennis@dyallo.se)
- Signal: [@moonkin88.88](https://signal.me/#eu/fPYYsOYSCRmShf67DQB1UwR0c7D94fsmTgLuuBAzaAM-8PsXA2MNiJOz30FTUYrk)
- LinkedIn: [in/dennis-dyallo](https://www.linkedin.com/in/dennis-dyallo)
- GitHub: You're already here 😎

---

*"Debugging is like being a detective in a crime movie where you're also the murderer."* — Filipe Fortes
*I write tests so my future self doesn't hunt down my past self.*
