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

Minecraft is a registered trademark of Mojang Synergies AB. Blade Launcher is not affiliated with Mojang or
Microsoft.

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
| [Minecraft-Mods-Updater](https://github.com/CoderBhoid/Minecraft-Mods-Updater) | Bhoid | none yet | - | Mod update utility used by Blade Launcher |
| [PokeTools](https://github.com/CoderBhoid/PokeTools) | Bhoid | MIT | - | Offline Pokémon companion app, Vanilla JS and Capacitor |

Issues are open on all of them. If you want to contribute to something non-trivial, open an issue first so
we can agree on scope before you spend time on it.

## Research

Work that is not a product: papers, protocol designs and measurements. Some of it ends up inside the apps
above, some of it stays a document.

### Dimensional Spark Theory

[![Status active](https://img.shields.io/badge/status-research%20active-111111?style=flat-square)](https://github.com/CoderBhoid/Dimensional-Sparks-Theory)
[![Built by Bhoid](https://img.shields.io/badge/built%20by-bhoid-EC5E27?style=flat-square&labelColor=111111)](https://github.com/CoderBhoid)
[![Papers](https://img.shields.io/badge/papers-v1%20%C2%B7%20v2%20%C2%B7%20v3-EC5E27?style=flat-square&labelColor=111111)](https://github.com/CoderBhoid/Dimensional-Sparks-Theory)
[![License MIT](https://img.shields.io/badge/license-MIT-111111?style=flat-square)](https://github.com/CoderBhoid/Dimensional-Sparks-Theory/blob/main/LICENSE)

A theoretical physics framework proposed by Ayush Pal, three revisions deep and public. It treats the universe
as a recursive information processing system instead of a machine, and derives mass-side effects from
information rather than taking them as fundamental: gravity as tension from compressed data, dark energy as
repulsive pressure from information density, time as the local processing rate that slows under load, and
`c` as the bandwidth ceiling of that processing.

The repo carries a calculator that runs the theory instead of describing it. Mass is converted to bits with
the Landauer equivalence (about 3.0e-38 kg per bit), a Spark gravitational constant of roughly 2.0e-48 is
applied, and gravitational pull is balanced against quantum repulsion. On the Earth preset it returns
9.81 m/s², which is the point the papers make: Newtonian gravity recoverable from information terms alone.
This is independent research, not an accepted result, and it is published so the arithmetic can be checked.

- Papers and engine: https://github.com/CoderBhoid/Dimensional-Sparks-Theory

### S.H.I.E.L.D. and blind-relay messaging

[![Status shipped in ONYXCHAT](https://img.shields.io/badge/status-designed%20%2B%20implementing-06B6D4?style=flat-square&labelColor=111111)](https://sednium.com/shield)
[![Built by Loid](https://img.shields.io/badge/built%20by-loid-06B6D4?style=flat-square&labelColor=111111)](https://github.com/AnkushDas4)
[![Docs](https://img.shields.io/badge/docs-sednium.com%2Fshield-06B6D4?style=flat-square&labelColor=111111)](https://sednium.com/shield)
[![Docs](https://img.shields.io/badge/docs-sednium.com%2Fonyxchat-06B6D4?style=flat-square&labelColor=111111)](https://sednium.com/onyxchat)

The messaging work by Ankush Das, written up in full outside the app. S.H.I.E.L.D. is a six-layer
zero-knowledge architecture aimed at three specific failures of normal chat servers: server-side retention,
identity correlation, and metadata leakage.

The pieces worth naming. Identity becomes a non-deterministic 8-character hex Routing ID, so there is no
phone number field to scrape and no deterministic handle to correlate. Key agreement pairs X25519 with
ML-KEM-768 through HKDF-SHA256, and the Double Ratchet underneath still does the per-message forward secrecy
and post-compromise recovery. Transport is a relay that only moves ciphertext and persists nothing, with
push treated as untrusted blind transport. Backups live in the user's own Drive appData folder, and the vault
key moved from being derived from a Google account ID to being wrapped behind device-held post-quantum key
material, which closed the gap where an account ID alone could reconstruct the key.

- Protocol write-up: https://sednium.com/shield · [Architecture notes](https://sednium.com/onyxchat)
- Builds and system notes: [loid.sednium.com](https://loid.sednium.com)

### Agent context security and quantisation

[![Status published](https://img.shields.io/badge/status-published-111111?style=flat-square)](https://github.com/CoderBhoid/ai-format/blob/main/research.md)
[![Built by Bhoid](https://img.shields.io/badge/built%20by-bhoid-EC5E27?style=flat-square&labelColor=111111)](https://github.com/CoderBhoid)

`research.md` in the ai-format repo is the measurement behind the `.ai` spec. It argues that plain text
context files cost a full forward pass to become usable state, and instead stores pre-computed model state:
serialised activations and KV cache, quantised aggressively (FP16 down toward INT2 and INT4), with gist
tokens or activation beacons collapsing long instruction templates into a handful of vectors. It then
compares an unencrypted general format against a post-quantum keyed one and reports the decryption overhead
as marginal next to ingestion latency, which is why encryption is not optional in the spec.

The same repo holds `brute_force_audit.py` for attacking your own snapshots, plus `agentic-skill/SKILL.md`
and `AGENTS.md` for wiring the format into an agent as a skill.

- Research: https://github.com/CoderBhoid/ai-format/blob/main/research.md · [Source (MIT)](https://github.com/CoderBhoid/ai-format)

### Mobile hardware ceilings

Two studies, both driven by "will it run", that ended up as shipped features.

On the GPU side, Blade Launcher's runtime and renderer matching comes from mapping which Android GPUs handle
desktop OpenGL translation well: GL4ES 1.1.6 for stability on Adreno and Mali, Vulkan Zink where full
Vulkan 1.2 is actually available, VirGL for virtualised setups, plus the Java version each Minecraft release
mandates (8 and 11 for old versions, 17 for 1.17 to 1.20.4, 21 for 1.20.5 and newer). The launcher does this
detection on device instead of shipping a fixed guess. Documented in the [Blade Launcher docs](https://blade-launcher.sednium.com/docs.html).

On the memory side, Oorty's fit matrix measures decode speed, VRAM footprint and crash risk per quantisation
against device RAM (4, 6, 8 and 12 GB classes) with a llama.cpp and LiteRT engine on the same phone, then
refuses to load a model that will be killed. That is where the RAM watchdog came from.

- Details: [Blade Launcher](https://blade-launcher.sednium.com) · [Oorty](https://oorty.sednium.com)

### Browser graphics and offline execution

Continuous experiments with WebGL, Three.js and canvas throughput in mobile browsers, plus the compile and
run pipelines that let a full toolchain live on an Android device (Termux and Linux subsystem work, incremental
parsing, PTY bridges). Krypton's offline execution and Sednicon's edge-rendered SVG work both come out of
this, and the notes are filed against those repositories rather than published as papers.

- Related: [krypton-ide](https://github.com/Sednium-Technologies/krypton-ide) · [SEDNICON](https://github.com/AnkushDas4/SEDNICON) · [CoderBhoid](https://github.com/CoderBhoid)

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
