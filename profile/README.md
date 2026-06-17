<div align="center">

# BLINC

**Native User Interface and Interaction Systems**

A declarative, reactive UI framework written in Rust — with first-class state machines, spring-physics animation, and GPU-accelerated rendering.

[Website](https://blinc.rs) · [Core Framework](https://github.com/project-blinc/Blinc) · [crates.io](https://crates.io/crates/blinc_app) · [Discord](https://discord.gg/WXADUBBgzP) · [Apache-2.0](https://github.com/project-blinc/Blinc/blob/main/LICENSE)

</div>

---

## Blinc

[**Blinc**](https://github.com/project-blinc/Blinc) is the core UI system everything here builds on. It treats interfaces as declarative, reactive descriptions of state rather than imperative trees of widgets, so your UI stays in sync with your data automatically.

- 🧩 **Declarative & reactive** — describe what the UI should be; Blinc keeps it consistent as state changes
- 🔁 **First-class state machines** — model interaction and view logic as explicit, inspectable states
- 🌊 **Spring-physics animation** — natural, interruptible motion instead of fixed-duration tweens
- ⚡ **GPU-accelerated rendering** — fast, hardware-backed drawing at the core
- 🦀 **Pure Rust** — memory-safe, portable, and dependency-light

```toml
[dependencies]
blinc_app = "0.5"
```

> See the [Blinc repository](https://github.com/project-blinc/Blinc) for documentation, examples, and getting-started guides.

---

## Packages

Blinc is extended by a set of focused crates. Each one is independent — pull in only what your project needs.

### Canvas & scene authoring

| Package | What it does |
| --- | --- |
| [**blinc_canvas_kit**](https://github.com/project-blinc/blinc_canvas_kit) | Canvas authoring toolkit: interactive scene graphs (pan, zoom, selection, grid), a 3D scene kit, and p5.js-style immediate-mode sketching over Blinc's `DrawContext`. |
| [**blinc_portal_ui**](https://github.com/project-blinc/blinc_portal_ui) | Immediate-mode widget toolkit for canvas closures — render real interactive widgets and free-form painting inside a Canvas. |
| [**blinc_node_editor**](https://github.com/project-blinc/blinc_node_editor) | A metadata-driven node-graph editor toolkit built on [`blinc_canvas_kit`](https://github.com/project-blinc/blinc_canvas_kit). Typed ports, bezier connectors with drag-to-connect, immediate-mode content widgets inside node bodies, group chrome, theme-aware rendering, frustum-culled paint, and a signal + event API designed for reactive Blinc hosts. |

### Animation & assets

| Package | What it does |
| --- | --- |
| [**blinc_skeleton**](https://github.com/project-blinc/blinc_skeleton) | Runtime poser for Blinc 2D/3D canvases. |
| [**blinc_gltf**](https://github.com/project-blinc/blinc_gltf) | glTF 2.0 loader for Blinc. |
| [**blinc_lottie**](https://github.com/project-blinc/blinc_lottie) | Lottie animation player for Blinc sketches. |

### Input

| Package | What it does |
| --- | --- |
| [**blinc_input**](https://github.com/project-blinc/blinc_input) | Polling-style input state for Blinc sketches and canvases. |

---

## Ecosystem

```
                        ┌─────────────┐
                        │    Blinc    │   declarative · reactive · GPU
                        │  core UI    │
                        └──────┬──────┘
                               │
        ┌──────────────────────┼──────────────────────┐
        │                      │                       │
  Canvas & scene         Animation & assets          Input
  ─────────────          ──────────────────        ─────────
  canvas_kit             skeleton                   input
  portal_ui              gltf
  node_editor            lottie
```

---

## Getting started

1. Start with [**Blinc**](https://github.com/project-blinc/Blinc) — the core framework.
2. Add the extension crates your project needs (canvas tooling, asset loaders, input, etc.).
3. Visit [**blinc.rs**](https://blinc.rs) for guides and reference material.

## Contributing

Contributions are welcome across the ecosystem. Open an issue or PR on the relevant repository, and check each project's README for setup and contribution notes.

<div align="center">

Built with 🦀 by the BLINC project · [blinc.rs](https://blinc.rs)

</div>

