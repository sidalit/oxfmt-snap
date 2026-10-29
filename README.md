<div align="center">

<img src="snap/gui/oxfmt.png" alt="Oxfmt logo" width="128" />

# Oxfmt

**A fast formatter for JavaScript and TypeScript projects**

[![oxfmt](https://snapcraft.io/oxfmt/badge.svg)](https://snapcraft.io/oxfmt)
[![Base: core26](https://img.shields.io/badge/Base-core26-2C8C3C?logo=canonical&logoColor=white)](https://snapcraft.io/core26)
![Confinement: strict](https://img.shields.io/badge/Confinement-strict-2C8C3C)
[![Maintainer: sidaliteir](https://img.shields.io/badge/Maintainer-sidaliteir-2C8C3C?logo=snapcraft&logoColor=white)](https://snapcraft.io/publisher/sidaliteir)
![Architectures: amd64 and arm64](https://img.shields.io/badge/Architectures-amd64%20%7C%20arm64-2C8C3C?logo=linux&logoColor=white)

[Getting Started](#getting-started) · [Configure](#configure) · [Limitations](#limitations) · [Build](#build) · [Support](#support) · [License](#license)

Unofficial snap packaging for [Oxfmt](https://github.com/oxc-project/oxc), a formatter for JavaScript, TypeScript, JSON, CSS, Markdown and other project files.

</div>

---

## Getting Started

<a href="https://snapcraft.io/oxfmt"><img alt="Get it from the Snap Store" src="https://snapcraft.io/en/dark/install.svg" width="180"></a>

```bash
sudo snap install oxfmt
cd ~/project/my-project
oxfmt --write .
```

Use `oxfmt --check .` to check formatting without changing files.

## Configure

Use your project's `.oxfmtrc.json`. See the [upstream documentation](https://oxc.rs/docs/guide/usage/formatter.html) for settings.

```bash
sudo snap connect oxfmt:removable-media   # optional: /media, /mnt
```

## Limitations

- Projects must be in non-hidden home folders or connected removable storage.
- Standalone release: no LSP, stdin formatting, JS/TS configuration, init/migration commands or Prettier/Tailwind integrations.

## Build

```bash
git clone https://github.com/sidalit/oxfmt-snap.git
cd oxfmt-snap
sudo snap install snapcraft --classic
snapcraft pack
```

## Support

- **Installation or snap issues:** [open a packaging issue](https://github.com/sidalit/oxfmt-snap/issues).
- **Application bugs:** [report them upstream](https://github.com/oxc-project/oxc/issues).

## License

Snap packaging: [MIT](https://github.com/sidalit/oxfmt-snap/blob/main/LICENSE).
