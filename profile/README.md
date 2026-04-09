
<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/AtelierVR/node/development/public/logo.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/AtelierVR/node/development/public/logo.png" />
    <img src="https://raw.githubusercontent.com/AtelierVR/node/development/public/logo.png" width="360" alt="NoxVR" />
  </picture>

  <p><strong>A federated, open-source Social VR platform.</strong></p>

  <p>
    <a href="https://github.com/AtelierVR/node"><img src="https://img.shields.io/badge/NestJS-Backend-e0234e?logo=nestjs&logoColor=white" alt="Backend" /></a>
    <a href="https://github.com/AtelierVR/relay"><img src="https://img.shields.io/badge/Rust-Relay-f74c00?logo=rust&logoColor=white" alt="Relay" /></a>
    <a href="https://github.com/AtelierVR/runtime"><img src="https://img.shields.io/badge/Unity-Runtime-000000?logo=unity&logoColor=white" alt="Unity" /></a>
    <a href="https://github.com/AtelierVR/docs"><img src="https://img.shields.io/badge/Docs-Fumadocs-f97316" alt="Docs" /></a>
    <img src="https://img.shields.io/badge/License-AGPL--3.0-22c55e" alt="License" />
  </p>
</div>

---

NoxVR is a **federated social VR platform** — think ActivityPub, but for virtual reality. Servers are independent and interconnected. Users own their identity. Content is shared across the network.

## Core Projects

| Repository | Description | Stack |
|---|---|---|
| [node](https://github.com/AtelierVR/node) | Central API server — auth, users, worlds, avatars, federation | TypeScript / NestJS |
| [relay](https://github.com/AtelierVR/relay) | Real-time QUIC relay for multiplayer game sessions | Rust |
| [runtime](https://github.com/AtelierVR/runtime) | Unity client runtime — rendering, networking, avatar system | C# / Unity |
| [docs](https://github.com/AtelierVR/docs) | Official documentation — API reference, guides, technical specs | MDX / Next.js |
| [nox.desktop](https://github.com/AtelierVR/nox.desktop) | Desktop overlay controller | C# |
| [bot](https://github.com/AtelierVR/bot) | Load testing bot for relay servers | Rust |

## Unity Packages

| Package | Description |
|---|---|
| [nox.cck](https://github.com/AtelierVR/nox.cck) | Content Creation Kit — build avatars & worlds for NoxVR |
| [nox.xr](https://github.com/AtelierVR/nox.xr) | XR input and tracking integration |
| [nox.controllers](https://github.com/AtelierVR/nox.controllers) | Controller input API |
| [nox.microphone](https://github.com/AtelierVR/nox.microphone) | Microphone / voice capture |
| [nox.ffmpeg](https://github.com/AtelierVR/nox.ffmpeg) | FFmpeg bindings for media playback |
| [nox.offline](https://github.com/AtelierVR/nox.offline) | Offline / local play support |

## Architecture

```
  Unity Client  ──QUIC──▶  Relay  ──WebSocket──▶  Node (API)
                                                      │
  Browser Client ──HTTP──────────────────────────────▶│
                                                      │
                                            PostgreSQL + Storage
```

- Each **Node** server is independent and federates with others via `.well-known/nox`
- **Relay** servers register to a Node and handle real-time player sessions
- **Unity clients** authenticate via Node and connect to Relay via QUIC

## Documentation

📖 [docs.ateliervr.fr](https://github.com/AtelierVR/docs) — API reference, avatar guides, relay protocol

---

<div align="center">
  <p>Made with ♥ by <a href="https://github.com/AtelierVR">AtelierVR</a> &nbsp;·&nbsp; <a href="https://www.gnu.org/licenses/agpl-3.0">AGPL-3.0</a></p>
</div>
