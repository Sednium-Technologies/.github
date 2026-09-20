# Sednium Technologies

[![Website](https://img.shields.io/badge/website-sednium.com-111111?style=for-the-badge&labelColor=f4f4f4)](https://sednium.com)
[![Location](https://img.shields.io/badge/based_in-West_Bengal,_India-111111?style=for-the-badge&labelColor=f4f4f4)](https://sednium.com)
[![Repositories](https://img.shields.io/badge/repos-Sednium--Technologies-111111?style=for-the-badge&labelColor=f4f4f4)](https://github.com/Sednium-Technologies)
[![Contact](https://img.shields.io/badge/contact-bhoid%40sednium.com-111111?style=for-the-badge&labelColor=f4f4f4)](mailto:bhoid@sednium.com)

Sednium is a small software studio based in West Bengal, India. We build web applications, native Android
apps, design systems, and the infrastructure underneath them. Most of what we make is on-device software:
editors, launchers, chat clients, and AI tools that keep working without a network connection.

The people who write the code also run it in production and answer the bug reports, which keeps the feature
list honest.

## Products

### Krypton IDE

[![v3.0](https://img.shields.io/badge/production-v3.0-EC5E27?style=flat)](https://github.com/Sednium-Technologies/krypton-ide/releases/latest)
[![Platform](https://img.shields.io/badge/platform-Android_%2F_Web-555555?style=flat)](https://kryptonide.sednium.com)
[![License](https://img.shields.io/badge/license-MIT-555555?style=flat)](https://github.com/Sednium-Technologies/krypton-ide/blob/main/LICENSE)
[![Source](https://img.shields.io/badge/source-TypeScript_%2F_Java-555555?style=flat)](https://github.com/Sednium-Technologies/krypton-ide)
[![Site](https://img.shields.io/badge/site-kryptonide.sednium.com-555555?style=flat)](https://kryptonide.sednium.com)

A code editor and IDE for Android and the browser. The web stack runs locally through WebContainers, so
HTML, JavaScript, React and Python projects execute without a server. Kotlin and Java are supported
natively. The editor is Monaco, with a command palette, go-to-line, find and replace, and global search.

Projects sync two ways with Google Drive, and Git commit/push/pull runs on isomorphic-git so it works
offline. Larry AI is the bundled agent: bring your own API key, and it plans against the whole project tree
then applies small line-level edits instead of rewriting files.

### Blade Launcher

[![v2.4.7](https://img.shields.io/badge/production-v2.4.7-EC5E27?style=flat)](https://github.com/Sednium-Technologies/Blade-Launcher/releases/latest)
[![Android](https://img.shields.io/badge/Android-8.0%2B_API_26-555555?style=flat)](https://github.com/Sednium-Technologies/Blade-Launcher)
[![Java](https://img.shields.io/badge/OpenJDK-8_to_26-555555?style=flat)](https://blade-launcher.sednium.com/docs.html)
[![License](https://img.shields.io/badge/license-GPL--3.0-555555?style=flat)](https://github.com/Sednium-Technologies/Blade-Launcher/blob/main/LICENSE)
[![Source](https://img.shields.io/badge/source-Kotlin_%2F_Compose_M3-555555?style=flat)](https://github.com/Sednium-Technologies/Blade-Launcher)
[![Site](https://img.shields.io/badge/site-blade--launcher.sednium.com-555555?style=flat)](https://blade-launcher.sednium.com)

Runs Minecraft: Java Edition on Android, from 1.7.2 through 1.21.4 and current snapshots. Mod loaders
supported are Fabric, Forge, NeoForge and Quilt, with modpack browsing for CurseForge and Modrinth inside
the app.

Different Minecraft versions need different Java versions, so OpenJDK 8, 11, 17, 21 and 26 are downloaded
on demand into a sandbox per version. That keeps the base APK small and avoids the "one runtime for every
version" problem. On startup the launcher reads the device's OpenGL ES and Vulkan capabilities and
recommends a renderer (GL4ES 1.1.6, Vulkan Zink, or VirGL) rather than forcing one. The game JVM runs in a
separate process from the UI, so a crash in the game does not take the launcher with it.

Microsoft accounts work for Realms and public servers. Offline profiles work for LAN and singleplayer. Skins
and capes are managed locally, including HD textures, with a 3D preview before applying. The APK is 292 MB
and covers ARM64, ARMv7, x86 and x86_64.

### ONYXCHAT

[![December 2026](https://img.shields.io/badge/in_development-December_2026-EC5E27?style=flat)](https://onyxchat.sednium.com)
[![Platform](https://img.shields.io/badge/platform-Android%2C_desktop_in_progress-555555?style=flat)](https://onyxchat.sednium.com)
[![Cipher](https://img.shields.io/badge/E2EE-libsignal_%2B_ML--KEM--768-555555?style=flat)](https://sednium.com/onyxchat)
[![Source](https://img.shields.io/badge/client-closed,_docs_public-555555?style=flat)](https://sednium.com/shield)

An Android messenger with no phone number and no server-side message history. The relay forwards an
encrypted payload over Firebase Cloud Messaging and stores nothing, so there is no message table to hand
over under compulsion.

Identity is an 8-character hex Routing ID derived from a Google account. Adding someone means scanning a QR
code or pasting their ID, which removes contact syncing and SIM-swap attacks from the model.

Encryption is layered rather than invented. The inner layer is the standard libsignal Double Ratchet for
forward secrecy and post-compromise security. The outer layer wraps the handshake with an AES-256-GCM key
derived by HKDF-SHA256 from the classic ECDH secret concatenated with an ML-KEM-768 shared secret
(BouncyCastle), which is what makes recorded traffic useless later. Each message gets a fresh 96-bit nonce
from SecureRandom. Chat history is encrypted with AES-256 on device and synced to the hidden appData folder
of your own Google Drive.

The client is closed source. The architecture, including the six-part S.H.I.E.L.D. design, is written up in
full at [sednium.com/onyxchat](https://sednium.com/onyxchat) and
[sednium.com/shield](https://sednium.com/shield) so it can be reviewed without the code.

### Rosette

[![Live](https://img.shields.io/badge/production-live-EC5E27?style=flat)](https://rosette.sednium.com)
[![Models](https://img.shields.io/badge/models_up_to_5-from_15_providers-555555?style=flat)](https://rosette.sednium.com)
[![Keys](https://img.shields.io/badge/keys_client_side-Google_Drive_appData-555555?style=flat)](https://rosette.sednium.com)
[![Site](https://img.shields.io/badge/site-rosette.sednium.com-555555?style=flat)](https://rosette.sednium.com)

An OpenAI-compatible gateway for running several models at once. Up to five models from fifteen providers
share one endpoint, and a request starts a cycle: a leader model is elected from live benchmark scores
(60% reasoning, 40% coding), it pulls current package documentation and CVE data, the other models review
and argue about the result, and one merged answer comes back.

The operational parts are the reason people keep it around. Requests cascade to the next provider on a 429
or a 500. Multiple keys per provider rotate round-robin. Tool calls are checked against an RBAC policy
before routing, so an agent cannot run arbitrary CLI commands or read outside allowed directories. Repeated
identical tool calls trip a circuit breaker (default 3) to stop an agent burning credits in a loop.
Frequently repeated queries are answered from a local semantic cache.

Provider keys never touch a Sednium server. They are encrypted into a `rocky_vault.json` file in your Google
Drive appData folder and decrypted client-side. From the vault you can mint scoped keys for your own apps
that talk to the gateway.

### Oorty

[![Live](https://img.shields.io/badge/production-Android_%2F_Web-EC5E27?style=flat)](https://oorty.sednium.com)
[![Engines](https://img.shields.io/badge/on_device-llama.cpp_%2B_LiteRT-555555?style=flat)](https://github.com/Sednium-Technologies/OORTY)
[![License](https://img.shields.io/badge/license-MIT_per_README-555555?style=flat)](https://github.com/Sednium-Technologies/OORTY/blob/main/README.md)
[![Source](https://img.shields.io/badge/source-Kotlin-555555?style=flat)](https://github.com/Sednium-Technologies/OORTY)
[![Site](https://img.shields.io/badge/site-oorty.sednium.com-555555?style=flat)](https://oorty.sednium.com)

An AI client that runs models on the phone. Inference goes through a native llama.cpp JNI binding for GGUF
weights, with Google LiteRT as a second engine, so there is no Python runtime or Node daemon in the app and
no root needed. A RAM watchdog reads ActivityManager.MemoryInfo before loading a model and tells you when a
quantisation is too large for the device instead of letting Android kill it.

Quantised weights can be searched and streamed from a built-in Hugging Face browser into
`Documents/Oorty/models/`. Conversations are dual-written as plain Markdown with YAML frontmatter into
`Documents/Oorty/chats/`, which you can open in Obsidian, Logseq, VS Code or commit to Git. Nothing is
locked in a private database.

It also speaks MCP, so multi-server tool loops run with JSON schema validation, approval prompts before
side effects, and local SQLite queries. Cloud models (Gemini, Claude, OpenAI, Groq, Mistral, NVIDIA NIM)
route through the same UI with your own keys. No telemetry, and airplane mode changes nothing except cloud
availability.

### Sednicon

[![Live](https://img.shields.io/badge/production-live-EC5E27?style=flat)](https://sednicon.sednium.com)
[![Icons](https://img.shields.io/badge/icons-200%2C000%2B-555555?style=flat)](https://sednicon.sednium.com/library)
[![Latency](https://img.shields.io/badge/latency-under_50ms-555555?style=flat)](https://sednicon.sednium.com/status)
[![Cost](https://img.shields.io/badge/cost-free-555555?style=flat)](https://sednicon.sednium.com)
[![Docs](https://img.shields.io/badge/docs-sednicon.sednium.com%2Fdocs-555555?style=flat)](https://sednicon.sednium.com/docs)

A headless icon API. Any icon from 200,000+ (Material Symbols, Lucide, Simple Icons and thirteen other
sets) comes back as SVG from a single URL: `https://sednicon.sednium.com/api/render?q=rocket&color=000000&size=64`.
There is no npm package and no build step; it is an `<img src>`. You can also describe an icon in English
and get a generated SVG back, using your own provider key, which is kept on your device.

Runs on Vercel Edge Functions, under 50ms, free, no rate limits for normal use.
[Docs](https://sednicon.sednium.com/docs) · [Status](https://sednicon.sednium.com/status)

### Sednium News

[![Live](https://img.shields.io/badge/production-live-EC5E27?style=flat)](https://news.sednium.com)
[![Channels](https://img.shields.io/badge/channels-10_+_yours-555555?style=flat)](https://news.sednium.com)
[![Trackers](https://img.shields.io/badge/trackers-0-555555?style=flat)](https://news.sednium.com)
[![Source](https://img.shields.io/badge/source-TypeScript_%2F_Vite-555555?style=flat)](https://github.com/CoderBhoid/Sednium-News)

A reader for ten channels (Headlines, Technology, World, Business, Politics, Science, Health, Entertainment,
Sports, India) plus your own RSS feeds. Article HTML is fetched, passed through Mozilla Readability and
DOMPurify, and rendered with reading-time estimates and a progress bar. The audio reader uses the browser's
own speech engine, so nothing is recorded or uploaded. We also serve cached RSS 2.0 endpoints for feed
readers and launcher widgets.

No accounts, no analytics, no ad scripts. Theme, typography, bookmarks and custom feeds live in
localStorage. It is a PWA, so the shell and saved stories work offline.

### The `.ai` format

[![Spec v3](https://img.shields.io/badge/open_spec-v3-EC5E27?style=flat)](https://ai.sednium.com)
[![Runtimes](https://img.shields.io/badge/runtimes-Python_3.10%2B_%2F_C%2B%2B17-555555?style=flat)](https://github.com/CoderBhoid/ai-format)
[![License](https://img.shields.io/badge/license-MIT-555555?style=flat)](https://github.com/CoderBhoid/ai-format/blob/main/LICENSE.md)
[![Source](https://img.shields.io/badge/source-CoderBhoid%2Fai--format-555555?style=flat)](https://github.com/CoderBhoid/ai-format)

An open file format for agent memory, which solves the practical problem of an agent that has to restart
without re-reading forty thousand tokens of history.

State is saved as signed, block-partitioned snapshots. Retrieval is lazy: an unencrypted but HMAC-verified
header index is read first, and only the blocks you ask for are decrypted. Old context degrades on a
schedule (under an hour stays `FP16_RAW` and lossless, an hour to a day goes to `INT8`, anything older
collapses to `INT2` semantic summaries), which makes ancient sessions roughly sixteen times cheaper to
store and load. Reference counts can override decay, so a variable that is still in use keeps full
precision. A background optimizer decays inactive blocks and migrates older files. Encryption is AEAD,
encrypt-then-MAC, with a post-quantum layer on the key wrapping.

Bindings exist for Python 3.10+ and C++17, including `save_active_context.py`, `recall_context.py` and
`autonomous_optimizer.py`, plus direct hooks into vLLM `PagedAttention` blocks and `llama_state_get_data()`
/ `llama_state_set_data()` in llama.cpp. The spec and integration guides are at
[ai.sednium.com](https://ai.sednium.com).

## Distribution and privacy

Our Android apps ship as signed APKs through GitHub Releases with published SHA-256 checksums. Play Store
distribution is not an option for tools like Blade Launcher, which download and execute external JDK
binaries, because the dynamic code loading policy forbids it. Nothing we publish carries ads, tracking SDKs
or paid placements.

Closed-source products say so on their own page, and the security design gets documented publicly anyway.
Open repositories put the license at the root: MIT for tooling and formats, GPL-3.0 for derivative work that
should stay free, with upstream attribution kept intact.

## Open source

Public work lives in [Sednium-Technologies](https://github.com/Sednium-Technologies). Older and independent
research lives under [@CoderBhoid](https://github.com/CoderBhoid).

| Repository | License | Notes |
| :-- | :-- | :-- |
| [krypton-ide](https://github.com/Sednium-Technologies/krypton-ide) | MIT | IDE source, Android project and web runtime |
| [Blade-Launcher](https://github.com/Sednium-Technologies/Blade-Launcher) | GPL-3.0 | Launcher, runtime manager, renderer selection. READMEs in English, Simplified and Traditional Chinese |
| [OORTY](https://github.com/Sednium-Technologies/OORTY) | MIT (declared in README) | On-device inference client |
| [charon](https://github.com/Sednium-Technologies/charon) | none yet | Internal video generation tool |
| [ai-format](https://github.com/CoderBhoid/ai-format) | MIT | `.ai` format spec, SDKs, optimizer |
| [Sednium-News](https://github.com/CoderBhoid/Sednium-News) | none yet | news.sednium.com |
| [Minecraft-Mods-Updater](https://github.com/CoderBhoid/Minecraft-Mods-Updater) | none yet | Mod update utility used by Blade Launcher |
| [PokeTools](https://github.com/CoderBhoid/PokeTools) | MIT | Offline Pokémon companion app, Vanilla JS and Capacitor |

Issues are open on all of them. If you want to contribute to something non-trivial, open an issue first so
we can agree on scope before you spend time on it.

## Roadmap

- ONYXCHAT public release, targeted December 2026, plus the Windows and Linux desktop clients.
- Krypton IDE: more agentic editing, deeper Git workflows, more offline language toolchains.
- Blade Launcher: newer snapshots and mod loader compatibility, controller and input improvements.
- Rosette: more providers, finer RBAC policy controls, better benchmark data for elections.
- Oorty: the v2.0 branch in the repository, covering voice mode and the current MCP framework.

## Team

| | |
| :-- | :-- |
| Ayush Pal (Bhoid) | Founder. Product, full-stack, design systems, research. [@CoderBhoid](https://github.com/CoderBhoid), [bhoid.sednium.com](https://bhoid.sednium.com) |
| Ankush Das (Loid) | Co-founder and CTO since January 2024. Architecture, protocols, backends. [@AnkushDas4](https://github.com/AnkushDas4), [loid.sednium.com](https://loid.sednium.com) |
| Ayush Rudra | Creative direction, visual identity, motion |
| Debraj Chandra | Testing and bug hunting |

We also publish independent research outside the product line, including
[Dimensional Spark Theory](https://github.com/CoderBhoid/Dimensional-Sparks-Theory), a physics paper that
treats gravity, time and energy as properties of information.

## Contact

West Bengal, India, UTC+05:30. We answer within a day.

[![Product](https://img.shields.io/badge/product_%2F_press-bhoid%40sednium.com-111111?style=flat&labelColor=f4f4f4)](mailto:bhoid@sednium.com)
[![Engineering](https://img.shields.io/badge/engineering-loid%40sednium.com-111111?style=flat&labelColor=f4f4f4)](mailto:loid@sednium.com)
[![Creative](https://img.shields.io/badge/creative-revealyt%40sednium.com-111111?style=flat&labelColor=f4f4f4)](mailto:revealyt@sednium.com)

| | |
| :-- | :-- |
| Product, commissions, press | bhoid@sednium.com |
| Engineering, protocol review, open source | loid@sednium.com |
| Creative work | revealyt@sednium.com |
| Security reports | bhoid@sednium.com, please email before opening a public issue |

Minecraft is a registered trademark of Mojang Synergies AB. Blade Launcher is not affiliated with Mojang or
Microsoft.
