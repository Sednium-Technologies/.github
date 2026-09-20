<div align="center">

# SEDNIUM

**Architecting the silent backbone of the digital future.**

We strip away the noise to reveal the signal: robust, stark, high-impact software
that withstands the test of time.

[![Website](https://img.shields.io/badge/website-sednium.com-111111?style=for-the-badge)](https://sednium.com)
[![Studio](https://img.shields.io/badge/based%20in-West%20Bengal%2C%20India-111111?style=for-the-badge&labelColor=f4f4f4)](https://sednium.com)
[![R&D](https://img.shields.io/badge/focus-research%20%2F%20development-EC5E27?style=for-the-badge&labelColor=f4f4f4)](#002-index)
[![Contact](https://img.shields.io/badge/contact-bhoid%40sednium.com-111111?style=for-the-badge&labelColor=f4f4f4)](mailto:bhoid@sednium.com)

`// web applications // mobile applications // design systems // protocol research`

</div>

---

Sednium is an independent research and development group. We take the technologies
that already exist — WebContainers, llama.cpp, libsignal, Vulkan, ML-KEM, Jetpack
Compose — and push them as far as they can go, without wasting compute on abstractions
that do not earn their keep.

Everything we ship is deployed by the people who designed it. Our products run on
hardware our users already own: a phone, a tablet, a browser tab.

---

## (001) IDENTITY

### What we build

| Discipline | Scope |
| :--- | :--- |
| **Web Applications** | React, TypeScript, Vite and Tailwind frontends on Vercel serverless and edge runtimes — zero build bloat, no third-party trackers. |
| **Mobile Applications** | Native Android in Kotlin and Jetpack Compose, plus Capacitor/WebContainer hybrids, distributed as signed APKs with published checksums. |
| **Design Systems** | Shared component libraries, design tokens and monochrome interfaces tuned for accessibility, touch ergonomics and low-end hardware. |
| **Systems & Protocol Research** | Encrypted transport design, agent memory formats, runtime and renderer orchestration — documented publicly, independent of the client code. |

### How we work

- **Existing technology, fully exploited.** We prefer pressure-testing a mature primitive over adopting a new dependency.
- **Offline first.** Network access is an optimisation, never a prerequisite. If it dies on a train, it is not finished.
- **Privacy by architecture, not policy.** No message logs, no telemetry pixels, no phone numbers, no ad SDKs. Where we cannot see your data, we do not claim to protect it.
- **Ship it, then document it.** Public technical write-ups accompany our security-critical work so it can be reasoned about instead of taken on faith.
- **Open by default where it is honest.** Tooling, formats and infrastructure are published under MIT or GPL-3.0; closed products state that clearly and expose their architecture anyway.

---

## (002) INDEX

Everything Sednium currently ships, maintains or researches — in one index.

| # | Project | What it is | Status | Surfaces |
| :-- | :--- | :--- | :--- | :--- |
| 01 | **[Krypton IDE](https://kryptonide.sednium.com)** | Native mobile code editor and AI IDE — desktop-class editing, offline execution, agentic pairing | `PRODUCTION v3.0` | Android · Web |
| 02 | **[Blade Launcher](https://blade-launcher.sednium.com)** | Minecraft: Java Edition on Android with isolated JDK runtimes and selectable GPU backends | `PRODUCTION v2.4.7` | Android |
| 03 | **[ONYXCHAT](https://onyxchat.sednium.com)** | Blind-routed messenger. No phone number, hybrid post-quantum E2EE | `IN DEVELOPMENT` → Dec 2026 | Android · Desktop |
| 04 | **[Rosette](https://rosette.sednium.com)** | Multi-model orchestration and collaborative agent gateway with RBAC sandboxing | `PRODUCTION` | Web · API |
| 05 | **[Oorty](https://oorty.sednium.com)** | On-device AI client: local GGUF/LiteRT inference, MCP agent loops, Obsidian-native storage | `PRODUCTION` | Android · Web |
| 06 | **[Sednicon](https://sednicon.sednium.com)** | Headless icon API — 200,000+ icons and AI-generated SVG, served from a single URL | `PRODUCTION` | Edge API |
| 07 | **[Sednium News](https://news.sednium.com)** | Clutter-free reader with RSS ingestion, offline shell and an audio reader | `PRODUCTION` | Web · PWA |
| 08 | **[.ai format](https://ai.sednium.com)** | Open file format for durable, quantised memory in long-running AI agents | `OPEN SPEC v3` | Python · C++ |

---

## (003) PRODUCTS

### 01 · Krypton IDE — *desktop power, pocket sized*

A hyper-modern native development environment for phones, tablets and browsers, built
so that a mobile device stops being a preview window and becomes the machine you ship from.

- **Native execution** — HTML, JavaScript, React and Python run fully offline through WebContainers, with full Kotlin and Java support alongside.
- **Monaco-grade editor** — command palette, go-to-line, find and replace, and global search stay active on every screen.
- **Larry AI** — a model-agnostic agentic assistant with autonomous planning, global project-file awareness and token-efficient surgical `edit_lines` patches. Bring your own API key.
- **Continuous sync** — two-way Google Drive synchronisation plus Git integration (commit, pull, push) on `isomorphic-git`.
- **Tuned for hardware** — performance patches that eliminate out-of-memory freezes and sync storms, haptic undo/redo and a touch-first toolbar.

**Stack:** TypeScript · Java · Monaco Editor · WebContainers · Vite · Capacitor
**Source:** [Sednium-Technologies/krypton-ide](https://github.com/Sednium-Technologies/krypton-ide) · MIT
**Releases:** [latest APK](https://github.com/Sednium-Technologies/krypton-ide/releases/latest)

### 02 · Blade Launcher — *Java Edition, uncompromised, on Android*

Minecraft: Java Edition from 1.7.2 through 1.21.4 and modern snapshots, on phones and tablets,
with a portrait-first interface engineered around the thumb zone.

- **Isolated runtimes** — verified OpenJDK 8, 11, 17, 21 and 26 fetched on demand into per-version sandboxes, keeping the base APK compact.
- **Renderer intelligence** — GPU capability is inspected at startup and the most stable backend is recommended: GL4ES 1.1.6, Vulkan Zink or VirGL. No silent overrides.
- **Modding built in** — CurseForge and Modrinth browsing with automatic dependency resolution for Fabric, Forge, NeoForge and Quilt.
- **Real account support** — Microsoft OAuth2 for Realms and public servers, plus offline profiles for LAN and singleplayer.
- **Identity, local** — 3D skin and cape wardrobe with HD texture support and atomic cache persistence.
- **Engineered for stability** — a split-process architecture isolates the launcher UI from the game JVM for crash immunity; configurable touch controls, gyroscope aiming and Bluetooth gamepads are supported.

**Stack:** Kotlin · Jetpack Compose M3E · C/C++ graphics shims · OpenJDK
**Source:** [Sednium-Technologies/Blade-Launcher](https://github.com/Sednium-Technologies/Blade-Launcher) · GPL-3.0 with full upstream attribution
**Docs:** [blade-launcher.sednium.com/docs.html](https://blade-launcher.sednium.com/docs.html)

### 03 · ONYXCHAT — *no number, no footprint, just messaging*

An Android messenger whose backend cannot read what it routes. The relay moves an encrypted
payload over Firebase Cloud Messaging and forgets it existed — there is no message table to surrender.

- **Identity without a SIM** — an 8-character hex Routing ID replaces the phone number, removing SIM-swap risk and contact scraping from the threat model.
- **Hybrid, audited cryptography** — the stock `libsignal` Double Ratchet is wrapped in an outer envelope built from BouncyCastle's ML-KEM-768 and classic ECDH, combined through HKDF-SHA256 into AES-256-GCM. No custom ciphers.
- **Harvest-now-decrypt-later resistant** — post-quantum key encapsulation protects the handshake; a fresh 96-bit `SecureRandom` nonce per message removes reuse risk across devices and reinstalls.
- **Your Drive is the only server** — chat history is encrypted on-device with AES-256 and synced to the hidden `appDataFolder` of your own Google account, with the vault key wrapped behind device-held post-quantum material.
- **Metadata-blind by construction** — the S.H.I.E.L.D. protocol closes six specific attack surfaces, each documented in public.

**Architecture docs:** [sednium.com/onyxchat](https://sednium.com/onyxchat) · [sednium.com/shield](https://sednium.com/shield)
**Status:** closed-source client, open architecture. Desktop clients for Windows and Linux are in active development.

### 04 · Rosette — *multi-model orchestration and agent gateway*

A unified proxy gateway that replaces per-vendor API wrappers with a single, governed endpoint for
your whole agent stack.

- **Consensus pipeline** — query ingest, leader election, live web retrieval for package docs and CVEs, collaborator debate, then a resolved unified payload.
- **Dynamic leader election** — up to five models concurrently from fifteen providers, ranked against a live benchmark (60% reasoning, 40% coding capability).
- **Failover waterfalls** — requests cascade across providers on rate limits and server exceptions instead of failing the user.
- **RBAC command sandbox** — tool-call parameters are inspected before routing, so a rogue agent cannot execute arbitrary CLI commands or reach sensitive directory trees.
- **Semantic response cache and key-rotation pools** — repeated tool queries resolve locally; multiple credentials per provider rotate round-robin to dodge organisation-wide limits.
- **Loop breaker** — consecutive identical tool calls trip a circuit breaker that halts execution before a runaway agent drains your credits.

**Credential model:** decentralised and client-side. Keys live in an encrypted `rocky_vault.json` inside your own Google Drive AppData folder and are never stored in a Sednium backend.

### 05 · Oorty — *one interface, every model, zero lock-in*

A warm, editorial-styled AI client that runs real models on the device and treats your notes as the database.

- **Dual on-device inference** — a native `llama.cpp` JNI engine for GGUF weights plus Google LiteRT, executing ARM NEON and Vulkan paths directly. Zero Python, zero Node daemon, zero root.
- **Built-in Hugging Face GGUF hub** — search, inspect and stream quantised weights into `Documents/Oorty/models/` with live telemetry.
- **Hardware safety** — a dynamic RAM watchdog and fit matrix evaluate model footprint before load, so the app degrades instead of crashing.
- **Autonomous MCP loops** — multi-server tool calling with strict JSON schema validation, human approval prompts and local SQLite execution.
- **Your chats are plain text** — every turn is dual-written as Markdown with YAML frontmatter into your Obsidian, Logseq or Git-ready documents folder. No proprietary silo.
- **Bring your own keys** — Gemini, Claude, OpenAI, Groq, Mistral and NVIDIA NIM route through the same interface, alongside streaming reasoning and hands-free voice modes.

**Stack:** Kotlin · Jetpack Compose · llama.cpp · LiteRT · MCP
**Source:** [Sednium-Technologies/OORTY](https://github.com/Sednium-Technologies/OORTY)

### 06 · Sednicon — *one URL, every icon*

A headless icon service for teams that would rather not install anything.

- **200,000+ icons via URL** — Material Symbols, Lucide, Simple Icons and more, at any colour and size, encoded in the request path.
- **AI generation** — describe an icon in plain English and a clean SVG comes back through Gemini, GPT, Claude, Groq, Mistral or NVIDIA.
- **Edge-deployed** — Vercel Edge Functions with sub-50ms latency and no cold starts.
- **Zero setup, zero cost** — a plain `<img src>` in HTML, React, Vue or Webflow; no rate limits for normal use, and your provider key stays on your device.

**Docs:** [sednicon.sednium.com/docs](https://sednicon.sednium.com/docs) · **Status:** [sednicon.sednium.com/status](https://sednicon.sednium.com/status)

### 07 · Sednium News — *the signal, without the chrome*

A reader, not a feed platform: ten curated channels plus your own subscriptions, cleaned for typography.

- **Clean extraction** — source HTML parsed through Mozilla Readability and DOMPurify, with reading-time estimates and progress.
- **Audio reader** — client-side speech synthesis via the Web Speech API, on your device's engine.
- **Independent feeds** — self-hosted, cached RSS 2.0 endpoints that work in any feed reader or launcher widget.
- **Nothing collected** — no accounts, no analytics, no ad beacons; preferences live in your browser's `localStorage`.
- **Offline shell** — progressive-web-app caching with saved reading lists that survive a dead connection.

**Source:** [CoderBhoid/Sednium-News](https://github.com/CoderBhoid/Sednium-News) · TypeScript · Vite · Vercel serverless

### 08 · The `.ai` format — *context persistence for long-running agents*

An open, block-based, temporally-aware memory format so an agent can resume without re-reading its own history.

- **Quantisation tiers** — recent state is preserved lossless at `FP16_RAW`, ages to `INT8`, and collapses to `INT2` semantic summaries beyond a day, shrinking ancient payloads roughly sixteenfold.
- **Instant resumption** — a snapshot loads in one pass, skipping input-prefill computation entirely.
- **Partial envelope unpacking** — an HMAC-verified header index is read unencrypted, then only the requested blocks are decrypted.
- **Importance-weighted decay** — frequently referenced variables override temporal decay; dead context is compressed by a background optimiser.
- **Signed handoff** — authenticated encryption (encrypt-then-MAC, with a post-quantum layer) lets a checkpoint pass between agents verifiably, and pre-flight snapshots make destructive operations reversible.
- **First-class bindings** — Python 3.10+ and C++17 tooling, plus hooks into vLLM `PagedAttention` blocks and `llama_state_get_data()` / `llama_state_set_data()` for llama.cpp.

**Spec & guides:** [ai.sednium.com](https://ai.sednium.com) · **Source:** [CoderBhoid/ai-format](https://github.com/CoderBhoid/ai-format) · MIT

---

## (004) PRINCIPLES

```
01 / PUSH WHAT EXISTS      Mature primitives, taken further than they usually go.
02 / OFFLINE IS A FEATURE  If it needs the network to open a file, it is not finished.
03 / NO TELEMETRY PIXELS   We measure what we can fix, never what we can sell.
04 / DOCUMENT THE CRYPTO   Claims are cheap. Show the construction.
05 / RESPECT THE HARDWARE  RAM watchdogs, crash isolation, quantised memory.
06 / SHIP, THEN OPTIMISE   Public releases with checksums, not private demos.
```

**Distribution.** Our Android software ships as signed APKs through GitHub Releases with published
SHA-256 checksums, because dynamic runtime loading and mod-installation policies on commercial app
stores cannot accommodate what these tools legitimately do. No ads, no trackers, no paid placements.

**Licensing.** Every open repository states its terms up front — MIT for tooling and formats, GPL-3.0 for
derivative work that must stay free, with upstream attribution notices preserved.

---

## (005) OPEN SOURCE

Public work lives in [Sednium-Technologies](https://github.com/Sednium-Technologies) and, for
preceding and independent research, in [@CoderBhoid](https://github.com/CoderBhoid).

| Repository | Language | License | Purpose |
| :--- | :--- | :--- | :--- |
| [krypton-ide](https://github.com/Sednium-Technologies/krypton-ide) | TypeScript | MIT | Native Android IDE with Monaco and the Larry agent |
| [Blade-Launcher](https://github.com/Sednium-Technologies/Blade-Launcher) | Kotlin | GPL-3.0 | Minecraft: Java Edition launcher for Android |
| [OORTY](https://github.com/Sednium-Technologies/OORTY) | Kotlin | MIT (declared) | On-device AI client with GGUF, LiteRT and MCP |
| [charon](https://github.com/Sednium-Technologies/charon) | JavaScript | — | Internal video generation tooling |
| [ai-format](https://github.com/CoderBhoid/ai-format) | Python | MIT | `.ai` context format, SDKs and optimiser |
| [Sednium-News](https://github.com/CoderBhoid/Sednium-News) | TypeScript | — | News aggregator and reader powering news.sednium.com |
| [Minecraft-Mods-Updater](https://github.com/CoderBhoid/Minecraft-Mods-Updater) | TypeScript | — | Open-source mod update utility used by Blade Launcher |
| [PokeTools](https://github.com/CoderBhoid/PokeTools) | JavaScript | MIT | Offline-first companion app built with Vanilla JS and Capacitor |

Issues are open on every product repository. Contribution notes, code of conduct and terms are
maintained alongside the specifications they govern.

---

## (006) ROADMAP

| Horizon | Work in flight |
| :--- | :--- |
| **Now** | ONYXCHAT public release (targeted December 2026) and the blind-relay desktop client for Windows and Linux. |
| **Next** | Krypton IDE: expanded agentic editing, deeper Git workflows and additional offline language toolchains. |
| **Next** | Blade Launcher: broader snapshot and mod-loader compatibility, controller and peripheral improvements. |
| **Next** | Rosette: additional providers, richer RBAC policy controls and expanded benchmark-driven elections. |
| **Exploring** | Wider adoption of the `.ai` format as a shared memory layer between agents and editors. |

---

## (007) TEAM

Small by design. Everyone who builds a feature supports it.

| Person | Role | Channels |
| :--- | :--- | :--- |
| **Ayush Pal** · *Bhoid* | Founder — product, full-stack, design systems, research | [@CoderBhoid](https://github.com/CoderBhoid) · [bhoid.sednium.com](https://bhoid.sednium.com) · bhoid@sednium.com |
| **Ankush Das** · *Loid* | Co-Founder & CTO — systems architecture, protocols, distributed backends | [@AnkushDas4](https://github.com/AnkushDas4) · [loid.sednium.com](https://loid.sednium.com) · loid@sednium.com |
| **Ayush Rudra** | Creative Director — visual identity, motion, brand systems | revealyt@sednium.com |
| **Debraj Chandra** | Quality — beta testing and bug hunting | debu@sednium.com |

Beyond client and product work, the team publishes independent research — including the *Dimensional
Spark Theory*, which treats gravity, time and energy as properties of information rather than
fundamental forces ([repository](https://github.com/CoderBhoid/Dimensional-Sparks-Theory)).

---

## (008) CONTACT

**Initiate contact:** [bhoid@sednium.com](mailto:bhoid@sednium.com) — product, commissions and press.

| Need | Write to |
| :--- | :--- |
| Web apps, mobile apps or design systems for your business | [bhoid@sednium.com](mailto:bhoid@sednium.com) |
| Engineering, protocol review or open-source collaboration | [loid@sednium.com](mailto:loid@sednium.com) |
| Security disclosure | [bhoid@sednium.com](mailto:bhoid@sednium.com) — please do not open a public issue first |

Based in West Bengal, India (UTC+05:30). Response time: **under 24 hours**.
Portfolio sites and services: [sednium.com](https://sednium.com)

---

<div align="center">

**SEDNIUM** · *Monochromatic precision.*

[sednium.com](https://sednium.com) ·
[kryptonide](https://kryptonide.sednium.com) ·
[blade-launcher](https://blade-launcher.sednium.com) ·
[onyxchat](https://onyxchat.sednium.com) ·
[rosette](https://rosette.sednium.com) ·
[oorty](https://oorty.sednium.com) ·
[sednicon](https://sednicon.sednium.com) ·
[news](https://news.sednium.com) ·
[.ai format](https://ai.sednium.com)

© Sednium Technologies · Minecraft is a registered trademark of Mojang Synergies AB; Blade Launcher is not
affiliated with Mojang or Microsoft.

</div>
