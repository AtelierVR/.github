<div align="center">
  <img src="logo.png" width="360" alt="NoxVR" />

  <br />
  <br />

  <p>
    <strong>A federated, open-source Social VR platform</strong><br />
    <sub>Own your identity. Share your worlds. Connect across servers.</sub>
  </p>

  <br />

  <p>
    <a href="https://github.com/AtelierVR/front">
      <img src="https://img.shields.io/badge/Front-Next.js%2FReact-000000?style=for-the-badge&logo=next.js&logoColor=white" alt="Front" />
    </a>
    &nbsp;
    <a href="https://github.com/AtelierVR/node">
      <img src="https://img.shields.io/badge/Node-NestJS%2FTypeScript-e0234e?style=for-the-badge&logo=nestjs&logoColor=white" alt="Node" />
    </a>
    &nbsp;
    <a href="https://github.com/AtelierVR/relay">
      <img src="https://img.shields.io/badge/Relay-Rust%2FQUIC-f74c00?style=for-the-badge&logo=rust&logoColor=white" alt="Relay" />
    </a>
    &nbsp;
    <a href="https://github.com/AtelierVR/runtime">
      <img src="https://img.shields.io/badge/Runtime-Unity%2FC%23-000000?style=for-the-badge&logo=unity&logoColor=white" alt="Runtime" />
    </a>
    &nbsp;
    <a href="https://github.com/AtelierVR/docs">
      <img src="https://img.shields.io/badge/Docs-MDX%2FNext.js-f97316?style=for-the-badge" alt="Docs" />
    </a>
  </p>

  <p>
    <img src="https://img.shields.io/badge/License-AGPL--3.0-22c55e?style=flat-square" alt="License" />
    <img src="https://img.shields.io/badge/Status-In%20Development-facc15?style=flat-square" alt="Status" />
    <img src="https://img.shields.io/badge/Federation-ActivityPub--inspired-6366f1?style=flat-square" alt="Federation" />
  </p>
</div>

<br />

---

## What is NoxVR?

NoxVR is a **federated social VR platform** — think ActivityPub, but for virtual reality. Each server is independent and can communicate with others. Users own their identity and content is shared across the network without a central authority.

<br />

## Philosophy

**Free & open, by design — not by promise.**

NoxVR is built on three core principles:

- **Open-source under AGPL-3.0** — every part of the platform is fully open-source. The AGPL license ensures that any server running NoxVR must publish its source code, including modifications. This guarantees that the platform stays free, transparent, and auditable — no hidden code, no black-box servers.

- **Federated by architecture** — there is no central authority. Anyone can run their own NoxVR server and join the network. Users keep their identity across servers. No single company controls the platform.

- **Modding-oriented** — the platform is designed to be extended. The Unity runtime exposes a modding API so players and creators can add new content, mechanics, and interactions.

<br />

## 🔷 Core Projects

| Repository | Description | Stack |
|:---|:---|:---:|
| [**front**](https://github.com/AtelierVR/front) | Web frontend — user interface, dashboard, settings | TypeScript / Next.js |
| [**node**](https://github.com/AtelierVR/node) | Central API server — auth, users, worlds, avatars, federation | TypeScript / NestJS |
| [**relay**](https://github.com/AtelierVR/relay) | Real-time QUIC relay for multiplayer game sessions | Rust |
| [**runtime**](https://github.com/AtelierVR/runtime) | Unity client runtime — rendering, networking, interaction | C# / Unity |
| [**docs**](https://github.com/AtelierVR/docs) | Official documentation — API reference, guides, technical specs | MDX / Next.js |
| [**bot**](https://github.com/AtelierVR/bot) | Load testing bot for relay servers | Rust |

<br />

---

<div align="center">
  <sub>Made with ♥ by <a href="https://github.com/AtelierVR">AtelierVR</a> &nbsp;·&nbsp; <a href="https://www.gnu.org/licenses/agpl-3.0">AGPL-3.0</a></sub>
</div>
