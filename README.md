# LlamaStash — Scoop bucket

![Logo](https://raw.githubusercontent.com/llamastash/llamastash/main/assets/logo-h.jpg)

**Zero-overhead, terminal-native local-LLM launcher.**

A fast TUI **and** CLI with init wizard for launching local LLMs. One Rust binary that's a TUI, a CLI, a daemon, and an OpenAI-compatible proxy. [llama.cpp](https://github.com/ggml-org/llama.cpp) is the direct, zero-overhead backend (vs raw `llama-server`), behind a pluggable backend seam so other engines can plug in.

**This repo holds the [Scoop](https://scoop.sh) bucket for [LlamaStash](https://github.com/llamastash/llamastash).**

## Install

```powershell
scoop bucket add llamastash https://github.com/llamastash/scoop-llamastash
scoop install llamastash
```

Then run `llamastash init` to set up models and detect your GPU.

## How this repo is updated

`llamastash.json` is auto-published on every tagged release of the main repo by the `publish-scoop` job in [`llamastash/llamastash/.github/workflows/release.yml`](https://github.com/llamastash/llamastash/blob/main/.github/workflows/release.yml). The manifest template lives at [`deployment/scoop/llamastash.json.template`](https://github.com/llamastash/llamastash/blob/main/deployment/scoop/llamastash.json.template) in the main repo; don't edit `llamastash.json` here directly — change it upstream.

## License

MIT — see [`LICENSE`](LICENSE).
