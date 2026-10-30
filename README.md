# ORDIMENS

### Local AI Agent Host · Build, Manage & Connect AI Agents

**ORDIMENS** is a locally hosted application for creating, configuring, testing, and connecting AI agents to language models, knowledge bases, speech systems, games, and external software.

It provides a browser-based management interface, so agents and their integrations can be managed from one place rather than building a separate management system for each project. ORDIMENS can be accessed from other devices on your local network when secure access is configured.

> **Current release:** 0.5.88 RC1 · **Platform:** Linux x86-64 · **Distribution:** Compiled application for Patreon members
>
> **Source availability:** ORDIMENS is proprietary and closed-source. This GitHub repository is the public information hub, **not** the application source repository. No source code or compiled application is provided here.

## What can ORDIMENS do?

### AI agents and Playground

- Create and configure multiple agents with individual instructions, parameters, and memory.
- Select the model used by each agent.
- Test configurations and conversations in the integrated Playground.
- Manage agents through a central web interface.

### Local and remote models

ORDIMENS supports configuring model connections through different backends, subject to model and runtime compatibility:

| Backend / connection | Purpose |
| --- | --- |
| **llama.cpp** | Compatible local GGUF models |
| **Transformers** | Compatible local model directories and architectures |
| **OpenAI-compatible APIs** | Local or remote compatible services |
| **Custom HTTP endpoints** | Configurable external model services |

Some vision-enabled GGUF models may require a separate `mmproj` file. Support depends on the model architecture, format, runtime, and available hardware resources.

### Knowledge bases and RAG

- Create document collections using uploaded documents or manually entered text.
- Associate collections with agents.
- Let agents retrieve relevant knowledge during interactions.

### Voice and speech

ORDIMENS includes configuration and integration support for speech capabilities, depending on the installed runtimes and models:

- **Text-to-Speech:** Qwen3-TTS, Chatterbox, Kokoro.
- **Speech-to-Text:** Whisper / Faster-Whisper, Qwen ASR.

Speech models and optional runtimes are **not bundled** with the application.

### APIs, games, and external applications

- Connect external clients to agents through APIs.
- Use permission-scoped access tokens for integrations.
- Import declarative **Character Packs** into the active server, including agent definitions and associated RAG knowledge.

This makes ORDIMENS useful as an external AI host for interactive applications and games, including projects with AI-powered NPCs.

### Administration

- Browser-based configuration and management.
- Initial setup tools.
- Runtime and model connection settings.
- Backup, update, and log management.
- Command-line controls for the installed service.

## Current release — 0.5.88 RC1

| | |
| --- | --- |
| **Operating system** | Linux x86-64 |
| **Status** | First release candidate |
| **Package** | Compiled application with installation/update scripts |
| **Documentation** | User guides distributed with the release |
| **Availability** | Patreon members |

**The application does not include model weights, optional AI runtimes, or GPU drivers.** You must provide and configure compatible components yourself. RAM/VRAM requirements and performance vary with the selected models and settings.

As an early release candidate developed independently, ORDIMENS may contain bugs or incomplete edge-case handling. Issue reports and reproducible feedback are welcome; I will work to provide support and address confirmed problems.

## Download and access

**ORDIMENS 0.5.88 RC1 is available as a compiled Linux release for Patreon members.**

**[Get ORDIMENS on Patreon]([PATREON_RELEASE_URL](https://www.patreon.com/Zetalvx/posts/ordimens-173839463))**

The Patreon release includes the application package and accompanying user documentation. This repository does **not** host the application binary, its source code, or the private build tools.

## In development

The following are **planned / in progress**, not features included in the current Linux release:

- **Windows version:** in the final stages of development, with a streamlined installer intended to make setup possible in just a few clicks.
- **Unity 3D, Unreal Engine, and Godot plugins:** integrations being finalized to connect with ORDIMENS automatically and simplify adding intelligent NPCs to games and interactive applications.

Release dates and final capabilities will be announced when these components are ready.

## Example project — The Lantern Chronicles

**The Lantern Chronicles** is a separate experimental RPG project exploring AI-powered NPCs, agent personalities, and knowledge-driven interactions using an external agent host.

The game, its demos, and its Character Packs are **distributed separately** and are **not included** with ORDIMENS 0.5.88 RC1.

## Project updates and demonstrations

A video walkthrough and further demonstrations are being prepared for the **[ZetaLvX YouTube channel](https://www.youtube.com/@zetalvx)**.

## Licensing and third-party components

ORDIMENS is proprietary software. Public visibility of this repository does not grant permission to redistribute, modify, or reverse engineer the application beyond applicable law and the terms supplied with the release.

AI models, voice models, runtimes, and other third-party components have their **own licenses and requirements**, which users must review separately.

## Feedback and contact

For release feedback, bug reports, and support inquiries:

**zetalvx_contact@proton.me**

**ZetaLvX — AI Automation Lab**  
[YouTube](https://www.youtube.com/@zetalvx) · [Website](https://zetalvx.com)
