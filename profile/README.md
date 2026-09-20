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
[![Next v4.0](https://img.shields.io/badge/next-v4.0%2C%2031%20oct%202026-111111?style=flat-square)](#roadmap)

A code editor and IDE for Android and the browser. The web stack runs locally through WebContainers, so
HTML, JavaScript, React and Python projects execute without a server. Kotlin and Java are supported
natively. The editor is Monaco, with a command palette, go-to-line, find and replace, and global search.

Projects sync two ways with Google Drive, and Git commit/push/pull runs on isomorphic-git so it works
offline. Larry AI is the bundled agent: bring your own API key, and it plans against the whole project tree
then applies small line-level edits instead of rewriting files.

v4.0 is scheduled for 31 October 2026 and ships on two channels: the native Kotlin and Jetpack Compose
client, and the legacy web-runtime build (Monaco with Capacitor and WebContainers) that current projects
are on. The legacy channel keeps receiving fixes after 4.0 so nobody has to rewrite a project to keep
working.

- Website: https://kryptonide.sednium.com
- Research: https://www.sednium.com/research/kryptonide
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
- Mod updates: [MC Mod Updater](https://mcmods.sednium.com) for batch checking and dependency resolution
- Stack: Kotlin, Jetpack Compose (M3), C/C++ graphics translation layers

Minecraft is a registered trademark of Mojang Synergies AB. Blade Launcher is not affiliated with Mojang or
Microsoft.

### MC Mod Updater

[![Status live](https://img.shields.io/badge/status-live%20on%20web-111111?style=flat-square)](https://mcmods.sednium.com)
[![Built by Bhoid](https://img.shields.io/badge/built%20by-bhoid-EC5E27?style=flat-square&labelColor=111111)](https://github.com/CoderBhoid)
[![Loaders](https://img.shields.io/badge/loaders-Fabric%20%C2%B7%20NeoForge%20%C2%B7%20Forge%20%C2%B7%20Quilt-EC5E27?style=flat-square&labelColor=111111)](https://mcmods.sednium.com)
[![Website](https://img.shields.io/badge/website-mcmods.sednium.com-EC5E27?style=flat-square&labelColor=111111)](https://mcmods.sednium.com)
[![Source](https://img.shields.io/badge/source-TypeScript-111111?style=flat-square)](https://github.com/CoderBhoid/Minecraft-Mods-Updater)

A browser tool for keeping a modpack current. You drop in your `mods` folder or a pile of `.jar` files and it
works out what is outdated across Modrinth and CurseForge, what companion libraries are missing, and hands
back one batch download. Nothing gets uploaded. Hashes are computed on your machine through the Web
Cryptography API in a worker, and folder sync uses the File System Access API, so in Chrome it writes results
straight back into `.minecraft/mods`.

Identification has two passes. A SHA-1 comparison against the Modrinth API and CurseForge is exact when the
JAR is a stock download. When a file was renamed or built by hand, a semantic pass cleans the name
(`fabric-sodium-mc1.20.1-0.5.8.jar` to `sodium`) and matches on project identity instead. Dependency checking
runs against the whole pack rather than mod by mod, so Fabric API or Cloth Config that is already present does
not show up as missing, and the one-click resolver only adds genuinely absent libraries to the queue. Alpha,
beta and release channels are picked per run.

Profiles make a pack reusable. Save, clone and switch between configurations, send a link like
`https://mcmods.sednium.com/?profile=...` that loads that exact setup in someone else's session, import
standard JSON manifests, or copy a formatted mod list for Discord, Markdown or plain text. An updated pack
exports as a single zip bundle.

It pairs with Blade Launcher, where the same loaders and version ranges matter, but it works standalone with
any desktop setup.

- Website: https://mcmods.sednium.com
- Source: [CoderBhoid/Minecraft-Mods-Updater](https://github.com/CoderBhoid/Minecraft-Mods-Updater) · MIT declared in the README, no LICENSE file in the repo yet
- Stack: TypeScript, React, Vite, Tailwind CSS, Vercel

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
specified, is written up in full at [sednium.com/research/onyxchat](https://www.sednium.com/research/onyxchat)
and [sednium.com/research/shield](https://www.sednium.com/research/shield) so it can be reviewed without the
code.

- Website: https://onyxchat.sednium.com
- Research: https://www.sednium.com/research/onyxchat
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
- Research: https://www.sednium.com/research/rosette

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
- Research: https://www.sednium.com/research/sedniumnews
- Source: [CoderBhoid/Sednium-News](https://github.com/CoderBhoid/Sednium-News)
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
- Research: https://www.sednium.com/research/aif
- Source: [CoderBhoid/ai-format](https://github.com/CoderBhoid/ai-format) · MIT

### Charon

[![Status internal](https://img.shields.io/badge/status-internal%20tooling-111111?style=flat-square)](https://github.com/Sednium-Technologies/charon)
[![Built by Sednium](https://img.shields.io/badge/built%20by-sednium-EC5E27?style=flat-square&labelColor=111111)](https://github.com/Sednium-Technologies)
[![Source](https://img.shields.io/badge/source-JavaScript-111111?style=flat-square)](https://github.com/Sednium-Technologies/charon)

The tool that makes our product videos. A Node and Express service drives Remotion: a prompt goes through
Gemini when a key is configured, and falls back to a local rules engine (`LocalAI.js`) that uses `compromise`
for semantic routing over named style templates. The chosen template renders through Remotion with a Three.js
scene to an MP4 in `out/`. Static files are served from `public/`, and background caching is there to stop
assets flickering mid render.

It is internal tooling and stays deliberately unpolished. The repo is public because the render setup is
fiddly and anyone wiring Remotion to a Node server will hit the same problems.

- Research: https://www.sednium.com/research/charon
- Source: [Sednium-Technologies/charon](https://github.com/Sednium-Technologies/charon) · ISC per `package.json`, no LICENSE file in the repo yet
- Stack: Node, Express, Remotion, Three.js, TypeScript, Google Generative AI SDK

### PokeTools

[![Release v1.0.0](https://img.shields.io/badge/release-v1.0.0-111111?style=flat-square)](https://github.com/CoderBhoid/PokeTools/releases)
[![Built by Bhoid](https://img.shields.io/badge/built%20by-bhoid-EC5E27?style=flat-square&labelColor=111111)](https://github.com/CoderBhoid)
[![Platforms](https://img.shields.io/badge/platform-Android%20%7C%20iOS%20%7C%20web-EC5E27?style=flat-square&labelColor=111111)](https://github.com/CoderBhoid/PokeTools)
[![License MIT](https://img.shields.io/badge/license-MIT-111111?style=flat-square)](https://github.com/CoderBhoid/PokeTools/blob/main/LICENSE)

A Pokémon companion app built with plain HTML, CSS and JavaScript, wrapped for mobile with Capacitor. No
framework, no bundler, and a 60fps target on the phone.

Data comes from PokéAPI and is cached into IndexedDB on first sync, so the full Pokédex, moves, abilities and
sprites stay available with no connection at all. The team builder works out shared weaknesses across your
six picks and suggests counter types while you edit. There is a move analyzer with filters, branching
evolution trees, an interactive type effectiveness matrix, and switchable sprite modes (official, pixel,
animated). Fifteen or more themes, including OLED Dark, Cyber Glass, Vaporwave and character-based palettes, with haptic feedback on
interactions.

- Source: [CoderBhoid/PokeTools](https://github.com/CoderBhoid/PokeTools) · MIT
- Run it: open `index.html` or serve the folder statically; `npx capacitor run android` or `run ios` for native builds
- Stack: Vanilla JS, Capacitor, IndexedDB, PokéAPI

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
| [Minecraft-Mods-Updater](https://github.com/CoderBhoid/Minecraft-Mods-Updater) | Bhoid | MIT (declared in README) | [mcmods.sednium.com](https://mcmods.sednium.com) | Browser mod updater and dependency resolver, pairs with Blade Launcher |
| [PokeTools](https://github.com/CoderBhoid/PokeTools) | Bhoid | MIT | - | Offline Pokémon companion app, Vanilla JS and Capacitor |

Issues are open on all of them. If you want to contribute to something non-trivial, open an issue first so
we can agree on scope before you spend time on it.

## Research

The eight studies we keep current at [sednium.com/research](https://www.sednium.com/research). Product
sections above describe shipped behaviour; these describe the design work underneath, and every one of them
has its own page at `sednium.com/research/<name>`.

### AIF Context Engine

[![Spec v3](https://img.shields.io/badge/spec-v3-111111?style=flat-square)](https://www.sednium.com/research/aif)
[![Built by Bhoid](https://img.shields.io/badge/built%20by-bhoid-EC5E27?style=flat-square&labelColor=111111)](https://github.com/CoderBhoid)
[![Research](https://img.shields.io/badge/research-sednium.com%2Fresearch%2Faif-EC5E27?style=flat-square&labelColor=111111)](https://www.sednium.com/research/aif)
[![Source MIT](https://img.shields.io/badge/source-MIT-111111?style=flat-square)](https://github.com/CoderBhoid/ai-format)

A compressed, non-human-readable neural context format with post-quantum cryptography and temporal memory
decay. `research.md` in the repo is the reasoning behind it: text context files force a full forward pass
before a model can use them, so the format stores pre-computed state instead, serialising activations and KV
cache and quantising them hard, with gist tokens collapsing long instruction templates into a handful of
vectors. General format versus post-quantum keyed format is measured there too, and the decryption overhead
comes out marginal next to ingestion latency, which is why encryption is mandatory in the spec rather than a
flag someone has to remember to turn on.

- Research: https://www.sednium.com/research/aif · [Spec site](https://ai.sednium.com)
- Source: [CoderBhoid/ai-format](https://github.com/CoderBhoid/ai-format) · MIT · includes `brute_force_audit.py` and an `agentic-skill/` package
- Stack: Python, C++, WebAssembly, ML-KEM/Kyber

### Rosette Gateway

[![Status live](https://img.shields.io/badge/status-live-111111?style=flat-square)](https://www.sednium.com/research/rosette)
[![Built by Bhoid](https://img.shields.io/badge/built%20by-bhoid-EC5E27?style=flat-square&labelColor=111111)](https://github.com/CoderBhoid)
[![Research](https://img.shields.io/badge/research-sednium.com%2Fresearch%2Frosette-EC5E27?style=flat-square&labelColor=111111)](https://www.sednium.com/research/rosette)

A decentralised, zero-server multi-model API gateway. The research is in how the routing decisions get made:
consensus leader election ranks models on live benchmark data (60% reasoning, 40% coding) instead of a static
priority list, failover waterfalls handle provider limits and outages, and an RBAC sandbox inspects tool-call
arguments before they reach a machine. Credential storage is part of the same study, since a gateway holding
everyone's keys would be the best target in the system, so keys stay encrypted in your own Drive appData
folder.

- Research: https://www.sednium.com/research/rosette · [Gateway](https://rosette.sednium.com)
- Stack: React, TypeScript, Tailwind CSS, OpenAI-compatible API, WebSockets

### Krypton IDE

[![Release v3.0](https://img.shields.io/badge/release-v3.0-111111?style=flat-square)](https://www.sednium.com/research/kryptonide)
[![Built by Bhoid and Loid](https://img.shields.io/badge/built%20by-bhoid%20%2B%20loid-06B6D4?style=flat-square&labelColor=111111)](https://github.com/AnkushDas4)
[![Research](https://img.shields.io/badge/research-sednium.com%2Fresearch%2Fkryptonide-06B6D4?style=flat-square&labelColor=111111)](https://www.sednium.com/research/kryptonide)
[![Source MIT](https://img.shields.io/badge/source-MIT-111111?style=flat-square)](https://github.com/Sednium-Technologies/krypton-ide)

A native mobile and web development environment with offline WebContainer execution and AI coding
integration. The research question was whether a phone can hold a real toolchain: a browser-based container
runtime for Node-family projects, Kotlin and Java compiling on device, an incremental parser cheap enough to
re-highlight on every keystroke, and a PTY bridge so a terminal is a real terminal. The agent side is the
other half of the study, since an autonomous loop on mobile hardware has to edit line ranges instead of
rewriting files or it spends its whole budget on tokens.

- Research: https://www.sednium.com/research/kryptonide · [Website](https://kryptonide.sednium.com)
- Source: [Sednium-Technologies/krypton-ide](https://github.com/Sednium-Technologies/krypton-ide) · MIT
- Stack: React, Vite, WebContainers, TypeScript, Kotlin

### ONYX Chat

[![Release Dec 2026](https://img.shields.io/badge/release-december%202026-111111?style=flat-square)](https://www.sednium.com/research/onyxchat)
[![Built by Loid](https://img.shields.io/badge/built%20by-loid-06B6D4?style=flat-square&labelColor=111111)](https://github.com/AnkushDas4)
[![Research](https://img.shields.io/badge/research-sednium.com%2Fresearch%2Fonyxchat-06B6D4?style=flat-square&labelColor=111111)](https://www.sednium.com/research/onyxchat)

A minimal encrypted messaging client built for absolute privacy and real-time sync. The design work sits in
three decisions. Identity is a non-deterministic 8-character hex Routing ID rather than a phone number, which
removes contact scraping and gives nothing stable to correlate. The relay only moves ciphertext and persists
nothing, with push transport treated as untrusted. Key agreement pairs X25519 with ML-KEM-768 through
HKDF-SHA256 while the Double Ratchet underneath keeps per-message forward secrecy and post-compromise
recovery.

Backups got their own revision: the vault key used to be derived from the Google account ID, which meant an
identifier alone was in the trust path. It is now wrapped behind device-held post-quantum key material and the
encrypted archive sits in the appData folder of your own Drive.

- Research: https://www.sednium.com/research/onyxchat · [Website](https://onyxchat.sednium.com)
- Status: closed-source client, published architecture. Stack: TypeScript, Vite, CSS, WebSockets

### Charon

[![Status internal](https://img.shields.io/badge/status-internal%20tooling-111111?style=flat-square)](https://www.sednium.com/research/charon)
[![Built by Sednium](https://img.shields.io/badge/built%20by-sednium-EC5E27?style=flat-square&labelColor=111111)](https://github.com/Sednium-Technologies)
[![Research](https://img.shields.io/badge/research-sednium.com%2Fresearch%2Fcharon-EC5E27?style=flat-square&labelColor=111111)](https://www.sednium.com/research/charon)
[![Source](https://img.shields.io/badge/source-JavaScript-111111?style=flat-square)](https://github.com/Sednium-Technologies/charon)

A programmatic video rendering engine: React components composed with Remotion, driven by code scripts
instead of a timeline editor, with WebAssembly stacks in the pipeline for dynamic frame generation. The
working version runs as a Node and Express service. A prompt either goes through Gemini when a key is set or
falls back to `LocalAI.js`, a rules engine that uses `compromise` to route the text across ten named style
templates, and the selected template renders through a Three.js scene to an MP4 in `out/`. Assets are cached
under `public/` so backgrounds do not flicker mid render.

- Research: https://www.sednium.com/research/charon
- Source: [Sednium-Technologies/charon](https://github.com/Sednium-Technologies/charon) · ISC per `package.json`, no LICENSE file in the repo yet
- Stack: React, Remotion, Three.js, WebAssembly, TypeScript

### Dimensional Spark Theory

[![Status active](https://img.shields.io/badge/status-research%20active-111111?style=flat-square)](https://www.sednium.com/research/dst)
[![Built by Bhoid](https://img.shields.io/badge/built%20by-bhoid-EC5E27?style=flat-square&labelColor=111111)](https://github.com/CoderBhoid)
[![Research](https://img.shields.io/badge/research-sednium.com%2Fresearch%2Fdst-EC5E27?style=flat-square&labelColor=111111)](https://www.sednium.com/research/dst)
[![Source MIT](https://img.shields.io/badge/source-MIT-111111?style=flat-square)](https://github.com/CoderBhoid/Dimensional-Sparks-Theory)

A theoretical physics and cosmological model, three revisions deep, that redefines gravity, spacetime and
quantum behaviour in terms of digital information processing. Under it, gravity is the tension produced by
compressed information, dark energy is the repulsive pressure of information density, time is the local
processing rate that slows under load, and `c` is the bandwidth ceiling of the system. It is written to
remove the singularities that break standard models rather than to patch them.

The repository ships the theory as a working calculator: mass is converted to bits with the Landauer
equivalence (about 3.0e-38 kg per bit), a Spark gravitational constant near 2.0e-48 is applied, and pull is
balanced against quantum repulsion. The Earth preset returns 9.81 m/s². This is independent research and not
an accepted result; it is public so the arithmetic can be checked.

- Research: https://www.sednium.com/research/dst · [Papers and engine](https://github.com/CoderBhoid/Dimensional-Sparks-Theory)
- Stack: cosmology, information theory, physics. `DST.pdf`, `DSTv2.pdf`, `Dst_3.pdf`

### Sednium News

[![Status live](https://img.shields.io/badge/status-live-111111?style=flat-square)](https://www.sednium.com/research/sedniumnews)
[![Built by Bhoid](https://img.shields.io/badge/built%20by-bhoid-EC5E27?style=flat-square&labelColor=111111)](https://github.com/CoderBhoid)
[![Research](https://img.shields.io/badge/research-sednium.com%2Fresearch%2Fsedniumnews-EC5E27?style=flat-square&labelColor=111111)](https://www.sednium.com/research/sedniumnews)
[![Source](https://img.shields.io/badge/source-TypeScript-111111?style=flat-square)](https://github.com/CoderBhoid/Sednium-News)

A distraction-free news reader and PWA built on local readability parsers, with clean typography and the
reader in control of their own information diet. The research here is mostly subtraction: what a reader
needs before it becomes a feed platform. Ten channels plus your own RSS feeds, article bodies extracted
through Readability and sanitised with DOMPurify, an audio path that runs entirely on the browser's speech
engine, and outbound RSS 2.0 endpoints so the thing works with real feed readers instead of only with itself.

State lives in localStorage, so there is no user database to secure and no account to leak. Nothing is
instrumented.

- Research: https://www.sednium.com/research/sedniumnews · [Website](https://news.sednium.com)
- Source: [CoderBhoid/Sednium-News](https://github.com/CoderBhoid/Sednium-News)
- Stack: PWA, RSS, TypeScript, Tailwind CSS, Vercel serverless

### Shield Gateway

[![Status internal](https://img.shields.io/badge/status-security%20perimeter-111111?style=flat-square)](https://www.sednium.com/research/shield)
[![Built by Loid](https://img.shields.io/badge/built%20by-loid-06B6D4?style=flat-square&labelColor=111111)](https://github.com/AnkushDas4)
[![Research](https://img.shields.io/badge/research-sednium.com%2Fresearch%2Fshield-06B6D4?style=flat-square&labelColor=111111)](https://www.sednium.com/research/shield)

Zero-trust identity verification, an OAuth security boundary and a rate-limiting perimeter, written for the
kind of infrastructure where the services behind it should not have to make authorisation decisions at all.
Go, OAuth2 and Docker. It is the same threat model as the ONYXCHAT work at a different layer: trust nothing
that arrives, verify at the edge, and keep no record that would be worth subpoenaing.

This page also carries the S.H.I.E.L.D. protocol layers referenced by ONYXCHAT, so the messaging crypto and
the gateway perimeter are documented together.

- Research: https://www.sednium.com/research/shield
- Stack: Go, OAuth2, Docker, security middleware

## Roadmap

- ONYXCHAT public release, targeted December 2026, plus the Windows and Linux desktop clients.
- Krypton IDE 4.0, launching 31 October 2026: the native client and the legacy web-runtime build, plus more agentic editing and deeper Git workflows.
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

Independent research is listed under Research above.

## Contact

West Bengal, India, UTC+05:30. We answer within a day.

| | |
| :-- | :-- |
| Support, install problems, bug reports | [support@sednium.com](mailto:support@sednium.com) |
| Product, commissions, press | [bhoid@sednium.com](mailto:bhoid@sednium.com) |
| Engineering, protocol review, open source | [loid@sednium.com](mailto:loid@sednium.com) |
| Creative work | [revealyt@sednium.com](mailto:revealyt@sednium.com) |
| Security reports | [support@sednium.com](mailto:support@sednium.com), please email before opening a public issue |
