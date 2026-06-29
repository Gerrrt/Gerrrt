<div align="center">

# How'r ya now? 👋

```text
$ whoami
red/blue operator · CLI craftsman · builder of an over-engineered terminal
```

### One terminal. Ten machines. Zero drift. ⌨️

I build a **cross-platform dotfiles fleet** — a unified Zsh · Neovim · Tmux
environment that feels *identical* on macOS, Windows/WSL2, and a rack of Linux
distros, with optional **red** (offensive) and **blue** (defensive) layers
bolted on top.

[![Live showcase](https://img.shields.io/badge/▶-live_showcase-7aa2f7?style=for-the-badge)](https://gerrrt.github.io/dotfiles-web)
[![Core](https://img.shields.io/badge/core-vendored_everywhere-bb9af7?style=for-the-badge)](https://github.com/Gerrrt/dotfiles-core)

</div>

---

### 🧬 The architecture (the part that makes it interesting)

Three layers. One source of truth. No copy-paste.

```text
            ┌─────────────────────────┐
            │      dotfiles-core      │   authored ONCE
            │  zsh · nvim · tmux ·    │
            │   git · starship        │
            └────────────┬────────────┘
                         │  git subtree  (vendored, self-contained)
       ┌─────────┬───────┼───────┬─────────┐
       ▼         ▼       ▼       ▼         ▼
    macOS     Linux ×5  Kali 🔴  Defense 🔵  …each clone stands alone
   (OS layer)         (role layer)
```

- **Core** — identical on every machine, authored once, fanned out via `git subtree`.
- **OS-native** — package manager, clipboard, paths. The only per-OS surface.
- **Role** — offensive (Kali) and defensive (Defense) tradecraft on top.

A green `make audit` in [`dotfiles-core`](https://github.com/Gerrrt/dotfiles-core) gates every change before Core is vendored out. Nothing ships red.

---

### 🗺️ The Fleet

| | Repo | What it is |
|:--|:--|:--|
| 🧬 | **[dotfiles-core](https://github.com/Gerrrt/dotfiles-core)** | The shared core — authored once, vendored everywhere |
| 🍎 | **[dotfiles-MacBook](https://github.com/Gerrrt/dotfiles-MacBook)** | macOS — Homebrew, AeroSpace tiling, desktop tooling |
| 🪟 | **[dotfiles-Windows](https://github.com/Gerrrt/dotfiles-Windows)** | Windows host — PowerShell, Terminal, WSL2 bridge |
| 🐧 | **Linux** | [Arch](https://github.com/Gerrrt/dotfiles-Arch) · [Fedora](https://github.com/Gerrrt/dotfiles-Fedora) · [openSUSE](https://github.com/Gerrrt/dotfiles-openSUSE) · [Gentoo](https://github.com/Gerrrt/dotfiles-Gentoo) · [Alpine](https://github.com/Gerrrt/dotfiles-Alpine) |
| 🔴 | **[dotfiles-Kali](https://github.com/Gerrrt/dotfiles-Kali)** | Offensive role layer — recon → exploit → evasion |
| 🔵 | **[dotfiles-Defense](https://github.com/Gerrrt/dotfiles-Defense)** | Defensive role layer — detection & hunt tooling |
| 🌐 | **[dotfiles-web](https://github.com/Gerrrt/dotfiles-web)** | The public showcase + docs site |

---

### 🔴🔵 The part nobody else has

[**htpx**](https://github.com/Gerrrt/htpx) is a structured, **ATT&CK-tagged,
red↔blue-*paired* corpus** — every attack technique sits beside its detection.
One source of truth drives both the offensive cheatsheet *and* the purple-team
detections. Fast modern-CLI configs are a commodity; a paired methodology corpus
is not. That's the thing worth stealing.

---

<div align="center">

### 📡 Reach me

[![Email](https://img.shields.io/badge/email-garrettallen2-7aa2f7?style=flat-square&logo=gmail&logoColor=white)](mailto:garrettallen2@gmail.com)
[![Showcase](https://img.shields.io/badge/site-dotfiles--web-9ece6a?style=flat-square)](https://gerrrt.github.io/dotfiles-web)

<sub>Built to be stolen from. Or borrowed. Or… whatever.</sub>

</div>
