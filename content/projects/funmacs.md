---
title: "FunMacs — Modern Emacs, Simplified"
date: 2025-10-21
draft: false
description: "Production-ready Emacs configuration with modern tooling baked in—LSP integration using eglot, tree-sitter parsing, and refined completion experience. Modular architecture for ultimate flexibility."
tags: ["emacs", "productivity", "development-tools", "lsp", "tree-sitter", "elisp"]
github: "https://github.com/mujaxso/funmacs"
showTableOfContents: true
---

![Release](https://img.shields.io/github/v/release/mujaxso/funmacs?style=flat-square)
![Stars](https://img.shields.io/github/stars/mujaxso/funmacs?style=flat-square)
![Forks](https://img.shields.io/github/forks/mujaxso/funmacs?style=flat-square)
![Open Issues](https://img.shields.io/github/issues/mujaxso/funmacs?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/mujaxso/funmacs?style=flat-square)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![Emacs Version](https://img.shields.io/badge/Emacs-29%2B-blue.svg)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)
![Built with Emacs Lisp](https://img.shields.io/badge/Made%20with-Emacs%20Lisp-orange.svg)

**Skip the configuration rabbit hole.** FunMacs is a production-ready Emacs setup with modern tooling baked in—LSP integration using eglot, tree-sitter parsing, and a refined completion experience. Its modular core/ and modules/ architecture means you can extend or strip down features without breaking anything.

{{< youtube "AsHJxMd7Ph0" >}}

## Highlights

- **Zero Setup** — Start coding instantly with pre-configured defaults
- **Modular Design** — Enable or disable features with minimal effort
- **Modern Toolchain** — Tree-sitter, Eglot, and Corfu baked in
- **Optimized for Productivity** — Smart defaults and minimal distractions
- **Clean Aesthetic** — A distraction-free, beautiful interface

## Supported Languages

![C](https://img.shields.io/badge/C-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Python](https://img.shields.io/badge/Python-%2314354C.svg?style=for-the-badge&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![Go](https://img.shields.io/badge/Go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white)
![Zig](https://img.shields.io/badge/Zig-%23000000.svg?style=for-the-badge&logo=zig&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-%23F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JSON](https://img.shields.io/badge/JSON-%23FFF.svg?style=for-the-badge&logo=json&logoColor=black)
![YAML](https://img.shields.io/badge/YAML-%23000000.svg?style=for-the-badge&logo=yaml&logoColor=white)
![Markdown](https://img.shields.io/badge/Markdown-%23000000.svg?style=for-the-badge&logo=markdown&logoColor=white)
![Nix](https://img.shields.io/badge/Nix-%23000000.svg?style=for-the-badge&logo=nixos&logoColor=white)

## UI & Aesthetics

- Minimal interface — no unnecessary menu/tool bars
- **Doom modeline** for rich status info with Nerd Font icons
- **Which-key** integration to guide you through keybindings
- **Custom themes** for both light and dark modes
- Clean typography and layout for long coding sessions

## Editing Experience

- Automatic tag closing in markup and HTML modes
- Relative line numbers for easier navigation
- **Vundo** — tree-structured undo/redo history
- Bell sound disabled (no more beeps!)
- Smooth scrolling and consistent indentation defaults

## Completion System

| Component | Description |
|-----------|-------------|
| **Vertico** | Lightweight and fast minibuffer completion UI |
| **Orderless** | Fuzzy, flexible, and intuitive matching style |
| **Corfu** | Pop-up completion menu for inline suggestions |
| **Embark** | Contextual actions for completion items |
| **Cape** | Adds additional completion sources (symbols, files, etc.) |
| **Nerd Icons Corfu** | Displays icons alongside completion candidates |

The result is a refined, modern completion experience that rivals VS Code or JetBrains IDEs—without leaving Emacs.

## Development Features

- **Eglot (LSP)** – Language Server Protocol integration for code intelligence
- **Tree-sitter** – Modern syntax highlighting and structural parsing
- **Automatic grammar installation** for supported languages
- **Apheleia** – Asynchronous and fast code formatting
- Language-specific **template snippets** included by default
- Intelligent indentation and syntax-aware editing

## Language Support Details

### C / C++

- LSP via `clangd` for autocompletion, diagnostics, and symbol navigation
- Tree-sitter highlighting for precise syntax awareness
- On-save formatting with `clang-format`
- Ready for CMake-based and Makefile projects

### Python

- LSP powered by `pyright` or `pylsp`
- Built-in support for virtual environments
- Automatic formatting with **Black** or **YAPF**
- REPL integration and code navigation included

### Rust

- Uses `rust-analyzer` for advanced IDE features
- Inline diagnostics and code actions
- Built-in formatter (`rustfmt`) and cargo command shortcuts
- Tree-sitter for rich syntax highlighting

### Go

- LSP with `gopls` and on-save formatting
- Auto-imports and completion for packages
- Integrated testing workflow via `go test`

### Zig

- LSP via `zls` (Zig Language Server)
- Tree-sitter grammar for Zig syntax highlighting
- Integrated build and run commands for quick iteration
- Formatter support using `zig fmt`
- Autocompletion for symbols, imports, and built-ins

### JavaScript & TypeScript

- LSP via `typescript-language-server`
- Tree-sitter-based highlighting for JS/TS/JSX/TSX
- Support for ESLint and Prettier formatting
- Module snippets for **React**, **Vue**, and **Svelte** frameworks

### Web Development

- First-class HTML and CSS support
- Autoclosing tags, attribute completion, and live linting
- Framework-specific modules for React, Vue, Svelte, TailwindCSS

### Configuration & Markup

- Syntax highlighting for **JSON**, **YAML**, **Nix**, and more
- Tree-sitter parsing ensures accurate indentation and folding
- LSP and schema validation for configuration files

### Markdown

- `markdown-mode` for writing and syntax highlighting
- `markdown-preview-mode` for real-time preview in another buffer
- Perfect for documentation, notes, and technical writing

## Installation

Clone directly into your Emacs configuration directory:

```bash
git clone https://github.com/mujaxso/funmacs.git ~/.config/emacs
```


Launch Emacs and let the automatic package installation complete on first run.

## Support

If you enjoy FunMacs and want to support ongoing development:

**Buy me a coffee:**  
[![Buy Me A Coffee](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/mujaxso)

**Or become a patron on Patreon:**  
[![Patreon](https://c5.patreon.com/external/logo/become_a_patron_button@2x.png)](https://www.patreon.com/mujaxso)

Your support helps keep FunMacs maintained, updated, and evolving.

## Related Projects

- [**NEOTE**](https://github.com/mujaxso/neote) – Lightweight next-gen text editor
- [**MujaOS**](https://github.com/mujaxso/mujaos) – Modern and secure operating system

## License

FunMacs is released under the **MIT License**. See [LICENSE](https://github.com/mujaxso/funmacs/blob/main/LICENSE) for full details.

---

**FOSS:** [foss.land](https://www.foss.land) • **GitHub:** [@mujaxso](https://github.com/mujaxso) • **Twitter/X:** [@mujaxso](https://twitter.com/mujaxso)

[View on GitHub](https://github.com/mujaxso/funmacs)
