# Sednium Technologies

[![Website](https://img.shields.io/badge/website-sednium.com-111111?style=for-the-badge)](https://sednium.com)
[![Location](https://img.shields.io/badge/based%20in-West%20Bengal%2C%20India-111111?style=for-the-badge&labelColor=f4f4f4&logo=openstreetmap&logoColor=333333)](https://sednium.com)
[![Support](https://img.shields.io/badge/support-support%40sednium.com-EC5E27?style=for-the-badge&labelColor=111111)](mailto:support@sednium.com)
[![Bhoid](https://img.shields.io/badge/built%20by-bhoid-EC5E27?style=for-the-badge&labelColor=111111)](https://github.com/CoderBhoid)
[![Loid](https://img.shields.io/badge/built%20by-loid-06B6D4?style=for-the-badge&labelColor=111111)](https://github.com/AnkushDas4)

Sednium is a small software studio based in West Bengal, India. We build web applications, native Android
apps, design systems, and the infrastructure underneath them. Most of what we make is on-device software:
editors, launchers, chat clients, and AI tools that keep working without a network connection.

The people who write the code also run it in production and answer the bug reports, which keeps the feature
list honest.

Badge colours on this page say who built what. Orange is Bhoid ([@CoderBhoid](https://github.com/CoderBhoid))
and default Sednium work. Cyan is Loid ([@AnkushDas4](https://github.com/AnkushDas4), builds documented at
[loid.sednium.com](https://loid.sednium.com)). Black is neutral information: versions, licenses, status.

- Website: https://sednium.com
- Org repos: https://github.com/Sednium-Technologies
- Contact: support@sednium.com (support, bugs), bhoid@sednium.com (product, commissions), loid@sednium.com (engineering)

## Products

### Krypton IDE

[![Release v3.0](https://img.shields.io/badge/release-v3.0-111111?style=flat-square)](https://github.com/Sednium-Technologies/krypton-ide/releases/latest)
[![Built by Bhoid](https://img.shields.io/badge/built%20by-bhoid-EC5E27?style=flat-square&labelColor=111111)](https://github.com/CoderBhoid)
[![Built by Loid](https://img.shields.io/badge/built%20by-loid-06B6D4?style=flat-square&labelColor=111111)](https://github.com/AnkushDas4)
[![Website](https://img.shields.io/badge/website-kryptonide.sednium.com-EC5E27?style=flat-square&labelColor=111111)](https://kryptonide.sednium.com)
[![License MIT](https://img.shields.io/badge/license-MIT-111111?style=flat-square)](https://github.com/Sednium-Technologies/krypton-ide/blob/main/LICENSE)

A code editor and IDE for Android and the browser. The web stack runs locally through WebContainers, so
HTML, JavaScript, React and Python projects execute without a server. Kotlin and Java are supported
natively. The editor is Monaco, with a command palette, go-to-line, find and replace, and global search.

Projects sync two ways with Google Drive, and Git commit/push/pull runs on isomorphic-git so it works
offline. Larry AI is the bundled agent: bring your own API key, and it plans against the whole project tree
then applies small line-level edits instead of rewriting files.

- Website: https://kryptonide.sednium.com
- Source: [Sednium-Technologies/krypton-ide](https://github.com/Sednium-Technologies/krypton-ide) · MIT · [Releases](https://github.com/Sednium-Technologies/krypton-ide/releases/latest)
- Stack: TypeScript, Java, Vite, Capacitor, Monaco

### Blade Launcher

[![Release v2.4.7](https://img.shields.io/badge/release-v2.4.7-111111?style=flat-square)](https://github.com/Sednium-Technologies/Blade-Launcher/releases/tag/v2.4.7)
[![Built by Loid](https://img.shields.io/badge/built%20by-loid-06B6D4?style=flat-square&labelColor=111111)](https://github.com/AnkushDas4)
[![Android 8.0+](https://img.shields.io/badge/platform-android%208.0%2B-06B6D4?style=flat-square&labelColor=111111)](https://blade-launcher.sednium.com)
[![Website](https://img.shields.io/badge/website-blade--launcher.sednium.com-06B6D4?style=flat-square&labelColor=111111)](https://blade-launcher.sednium.com)
[![License GPL-3.0](https://img.shields.io/badge/license-GPL--3.0-111111?style=flat-square)](https://github.com/Sednium-Technologies/Blade-Launcher/blob/main/LICENSE)

Runs Minecraft: Java Edition on Android, from 1.7.2 through 1.21.4 and current snapshots. Mod loaders
supported are Fabric, Forge, NeoForge and Quilt, with modpack browsing for CurseForge and Modrinth inside
the app.

Different Minecraft versions need different Java versions, so OpenJDK 8, 11, 17, 21 and 26 are downloaded
on demand into a sandbox per version. That keeps the base APK small and avoids the "one runtime for every
version" problem. On startup the launcher reads the device's OpenGL ES and Vulkan capabilities and
recommends a renderer (GL4ES 1.1.6, Vulkan Zink, or VirGL) rather than forcing one. The game JVM runs in a
separate process from the UI, so a crash in the game does not take the launcher with it.

Microsoft accounts work for Realms and public servers. Offline profiles work for LAN and singleplayer. Skins
and capes are managed locally, including HD textures, with a 3D preview before applying.

- Website: https://blade-launcher.sednium.com · [Docs](https://blade-launcher.sednium.com/docs.html)
- Source: [Sednium-Technologies/Blade-Launcher](https://github.com/Sednium-Technologies/Blade-Launcher) · GPL-3.0 · APK is 292 MB for ARM64/ARMv7/x86/x86_64
- Stack: Kotlin, Jetpack Compose (M3), C/C++ graphics translation layers

### ONYXCHAT

[![Release Dec 2026](https://img.shields.io/badge/release-december%202026-111111?style=flat-square)](https://onyxchat.sednium.com)
[![Built by Loid](https://img.shields.io/badge/built%20by-loid-06B6D4?style=flat-square&labelColor=111111)](https://github.com/AnkushDas4)
[![Post-quantum](https://img.shields.io/badge/design-ML--KEM--768%20%2B%20Double%20Ratchet-06B6D4?style=flat-square&labelColor=111111)](https://sednium.com/onyxchat)
[![Website](https://img.shields.io/badge/website-onyxchat.sednium.com-06B6D4?style=flat-square&labelColor=111111)](https://onyxchat.sednium.com)

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

The client is closed source. The architecture, including the six-part S.H.I.E.L.D. design that Loid
specified, is written up in full at [sednium.com/onyxchat](https://sednium.com/onyxchat) and
[sednium.com/shield](https://sednium.com/shield) so it can be reviewed without the code.

- Website: https://onyxchat.sednium.com
- Status: releasing December 2026. Windows and Linux clients are in development. Architecture notes are public.

### Rosette

[![Status live](https://img.shields.io/badge/status-live-111111?style=flat-square)](https://rosette.sednium.com)
[![Built by Bhoid](https://img.shields.io/badge/built%20by-bhoid-EC5E27?style=flat-square&labelColor=111111)](https://github.com/CoderBhoid)
[![15 providers](https://img.shields.io/badge/providers-15%2C%20up%20to%205%20at%20once-EC5E27?style=flat-square&labelColor=111111)](https://rosette.sednium.com)
[![Website](https://img.shields.io/badge/website-rosette.sednium.com-EC5E27?style=flat-square&labelColor=111111)](https://rosette.sednium.com)

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

- Website: https://rosette.sednium.com

### Oorty

[![Status live](https://img.shields.io/badge/status-live%20on%20Android%20and%20web-111111?style=flat-square)](https://oorty.sednium.com)
[![Sednium default](https://img.shields.io/badge/built%20by-sednium-EC5E27?style=flat-square&labelColor=111111)](https://github.com/Sednium-Technologies/OORTY)
[![Website](https://img.shields.io/badge/website-oorty.sednium.com-EC5E27?style=flat-square&labelColor=111111)](https://oorty.sednium.com)
[![Source](https://img.shields.io/badge/source-Kotlin-111111?style=flat-square)](https://github.com/Sednium-Technologies/OORTY)

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

- Website: https://oorty.sednium.com
- Source: https://github.com/Sednium-Technologies/OORTY
- Stack: Kotlin, Jetpack Compose, llama.cpp, LiteRT, MCP

### Sednicon

[![Status operational](https://img.shields.io/badge/status-operational-111111?style=flat-square)](https://sednicon.sednium.com/status)
[![Built by Loid](https://img.shields.io/badge/built%20by-loid-06B6D4?style=flat-square&labelColor=111111)](https://github.com/AnkushDas4)
[![200k+ icons](https://img.shields.io/badge/icons-200%2C000%2B%20via%20URL-06B6D4?style=flat-square&labelColor=111111)](https://sednicon.sednium.com/library)
[![Website](https://img.shields.io/badge/website-sednicon.sednium.com-06B6D4?style=flat-square&labelColor=111111)](https://sednicon.sednium.com)
[![Source](https://img.shields.io/badge/source-AnkushDas4%2FSEDNICON-06B6D4?style=flat-square&labelColor=111111)](https://github.com/AnkushDas4/SEDNICON)

A headless icon API. Any icon from 200,000+ (Material Symbols, Material Design, Lucide, Simple Icons,
FontAwesome and thirteen other sets) comes back as SVG from a single URL:

```
https://sednicon.sednium.com/api/render?q=rocket&color=ff6600&size=32&anim=spin
```

There is no npm package, no build step and no bundler configuration. It is an `<img src>`. You can also
describe an icon in English and get a generated SVG back, using your own provider key, which is kept on your
device and never stored on a server. Runs on Vercel Edge Functions, under 50ms, free, no rate limits for
normal use.

- Website: https://sednicon.sednium.com · [Library](https://sednicon.sednium.com/library) · [Generate](https://sednicon.sednium.com/generate)
- Docs: https://sednicon.sednium.com/docs · [Status](https://sednicon.sednium.com/status)
- Source: [AnkushDas4/SEDNICON](https://github.com/AnkushDas4/SEDNICON) · MIT (declared in README)

### Sednium News

[![Status live](https://img.shields.io/badge/status-live-111111?style=flat-square)](https://news.sednium.com)
[![Built by Bhoid](https://img.shields.io/badge/built%20by-bhoid-EC5E27?style=flat-square&labelColor=111111)](https://github.com/CoderBhoid)
[![Website](https://img.shields.io/badge/website-news.sednium.com-EC5E27?style=flat-square&labelColor=111111)](https://news.sednium.com)

A reader for ten channels (Headlines, Technology, World, Business, Politics, Science, Health, Entertainment,
Sports, India) plus your own RSS feeds. Article HTML is fetched, passed through Mozilla Readability and
DOMPurify, and rendered with reading-time estimates and a progress bar. The audio reader uses the browser's
own speech engine, so nothing is recorded or uploaded. We also serve cached RSS 2.0 endpoints for feed
readers and launcher widgets.

No accounts, no analytics, no ad scripts. Theme, typography, bookmarks and custom feeds live in
localStorage. It is a PWA, so the shell and saved stories work offline.

- Website: https://news.sednium.com
- Source: https://github.com/CoderBhoid/Sednium-News
- Stack: TypeScript, Vite, Tailwind, Vercel serverless functions

### The `.ai` format

[![Spec v3](https://img.shields.io/badge/spec-v3-111111?style=flat-square)](https://ai.sednium.com)
[![Built by Bhoid](https://img.shields.io/badge/built%20by-bhoid-EC5E27?style=flat-square&labelColor=111111)](https://github.com/CoderBhoid)
[![Website](https://img.shields.io/badge/website-ai.sednium.com-EC5E27?style=flat-square&labelColor=111111)](https://ai.sednium.com)
[![License MIT](https://img.shields.io/badge/license-MIT-111111?style=flat-square)](https://github.com/CoderBhoid/ai-format/blob/main/LICENSE.md)

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
/ `llama_state_set_data()` in llama.cpp.

- Website: https://ai.sednium.com
- Source: [CoderBhoid/ai-format](https://github.com/CoderBhoid/ai-format) · MIT

## Distribution and privacy

Our Android apps ship as signed APKs through GitHub Releases with published SHA-256 checksums. Play Store
distribution is not an option for tools like Blade Launcher, which download and execute external JDK
binaries, because the dynamic code loading policy forbids it. Nothing we publish carries ads, tracking SDKs
or paid placements.

Closed-source products say so on their own page, and the security design gets documented publicly anyway.
Open repositories put the license at the root: MIT for tooling and formats, GPL-3.0 for derivative work that
should stay free, with upstream attribution kept intact.

## Open source

The org has two members: [@CoderBhoid](https://github.com/CoderBhoid) and
[@AnkushDas4](https://github.com/AnkushDas4). Product work lives in
[Sednium-Technologies](https://github.com/Sednium-Technologies); older and independent research sits under
their personal accounts.

| Repository | Built by | License | Site | Notes |
| :-- | :-- | :-- | :-- | :-- |
| [krypton-ide](https://github.com/Sednium-Technologies/krypton-ide) | Bhoid, Loid | MIT | [kryptonide.sednium.com](https://kryptonide.sednium.com) | IDE source, Android project and web runtime |
| [Blade-Launcher](https://github.com/Sednium-Technologies/Blade-Launcher) | Loid | GPL-3.0 | [blade-launcher.sednium.com](https://blade-launcher.sednium.com) | Launcher, runtime manager, renderer selection. READMEs in English, Simplified and Traditional Chinese |
| [OORTY](https://github.com/Sednium-Technologies/OORTY) | Sednium | MIT (declared in README) | [oorty.sednium.com](https://oorty.sednium.com) | On-device inference client |
| [SEDNICON](https://github.com/AnkushDas4/SEDNICON) | Loid | MIT (declared in README) | [sednicon.sednium.com](https://sednicon.sednium.com) | Headless icon and SVG generation API |
| [charon](https://github.com/Sednium-Technologies/charon) | Sednium | none yet | - | Internal video generation tool |
| [ai-format](https://github.com/CoderBhoid/ai-format) | Bhoid | MIT | [ai.sednium.com](https://ai.sednium.com) | `.ai` format spec, SDKs, optimizer |
| [Sednium-News](https://github.com/CoderBhoid/Sednium-News) | Bhoid | none yet | [news.sednium.com](https://news.sednium.com) | news.sednium.com |
| [Minecraft-Mods-Updater](https://github.com/CoderBhoid/Minecraft-Mods-Updater) | Bhoid | none yet | - | Mod update utility used by Blade Launcher |
| [PokeTools](https://github.com/CoderBhoid/PokeTools) | Bhoid | MIT | - | Offline Pokémon companion app, Vanilla JS and Capacitor |
| [Nothing-Calculator](https://github.com/AnkushDas4/Nothing-Calculator) | Loid | none yet | - | Calculator interface inspired by Nothing OS |

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
| Ayush Pal (Bhoid) | Founder. Product, full-stack, design systems, research. [github.com/CoderBhoid](https://github.com/CoderBhoid) · [bhoid.sednium.com](https://bhoid.sednium.com) |
| Ankush Das (Loid) | Co-founder and CTO since January 2024. Systems architecture, the S.H.I.E.L.D. protocol, Android and edge infrastructure in Go, Kotlin and TypeScript. [github.com/AnkushDas4](https://github.com/AnkushDas4) · [loid.sednium.com](https://loid.sednium.com) |
| Ayush Rudra | Creative direction, visual identity, motion |
| Debraj Chandra | Testing and bug hunting |

We also publish independent research outside the product line, including
[Dimensional Spark Theory](https://github.com/CoderBhoid/Dimensional-Sparks-Theory), a physics paper that
treats gravity, time and energy as properties of information.

## Contact

West Bengal, India, UTC+05:30. We answer within a day.

| | |
| :-- | :-- |
| Support, install problems, bug reports | [support@sednium.com](mailto:support@sednium.com) |
| Product, commissions, press | [bhoid@sednium.com](mailto:bhoid@sednium.com) |
| Engineering, protocol review, open source | [loid@sednium.com](mailto:loid@sednium.com) |
| Creative work | [revealyt@sednium.com](mailto:revealyt@sednium.com) |
| Security reports | [support@sednium.com](mailto:support@sednium.com), please email before opening a public issue |

Minecraft is a registered trademark of Mojang Synergies AB. Blade Launcher is not affiliated with Mojang or
Microsoft.
