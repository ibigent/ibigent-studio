<!-- SEO: IBIGENT Studio, MCP, Model Context Protocol, Claude Code, Codex CLI, Cursor, Antigravity, AI website builder -->

# IBIGENT Studio — Developer Documentation

**English | [한국어](README_ko.md)**

Official developer documentation for **IBIGENT Studio**, an AI-powered website building platform. Connect your AI coding tool (Claude Code, Codex CLI, Cursor, and more) to IBIGENT Studio over the **Model Context Protocol (MCP)** so the AI can generate HTML and place it directly into your live editor.

> This repository contains **documentation only** — no product source code, no secrets.

- Official website: https://www.ibigent.com
- Full documentation: https://www.ibigent.com/docs/ibigent-studio/

## Table of Contents
- [1. What is IBIGENT Studio](#1-what-is-ibigent-studio)
- [2. Features](#2-features)
- [3. Supported AI tools](#3-supported-ai-tools)
- [4. Quick Start](#4-quick-start)
- [5. Documentation](#5-documentation)
- [6. Official Website](#6-official-website)
- [7. License](#7-license)
- [8. Contributing](#8-contributing)
- [9. Support](#9-support)
- [10. Roadmap](#10-roadmap)

## 1. What is IBIGENT Studio
IBIGENT Studio is a real-time web editor. You subscribe (no API keys to manage, nothing to install locally), connect your AI tool over MCP, and ask the AI to build HTML. The generated HTML is delivered to your editor, where you choose the exact position to insert it — and it appears immediately.

## 2. Features
- **Send AI-generated HTML into the editor.** Ask any MCP-connected AI tool to produce HTML and receive it in IBIGENT Studio.
- **Place it exactly where you want.** Choose the insertion point in the editor; the HTML is applied in place.
- **No coding, no API wiring.** A subscription and an MCP key are all you need.
- **Uses the open Model Context Protocol**, so it works with the tools you already use.

## 3. Supported AI tools
| Tool | Vendor | Guide |
|------|--------|-------|
| Claude Code | Anthropic | [docs/en/claude-code.md](docs/en/claude-code.md) |
| Codex CLI | OpenAI | [docs/en/codex.md](docs/en/codex.md) |
| Cursor | — | [docs/en/cursor.md](docs/en/cursor.md) |
| Antigravity | Google | [docs/en/antigravity.md](docs/en/antigravity.md) |
| VS Code | — | [docs/en/vscode.md](docs/en/vscode.md) (coming soon) |
| Any MCP client | — | [docs/en/mcp.md](docs/en/mcp.md) |

## 4. Quick Start
1. **Get your key.** Open **My Page > AI Integration > Connection Keys** (https://www.ibigent.com/mypage/mcp-keys.html) and click **Issue Key**. Your key `ibg_…` is shown only once — treat it like a password.
2. **Register the MCP server** in your AI tool, replacing `<YOUR_KEY>`:

   ```
   https://mcp.ibigent.com/mcp/<YOUR_KEY>
   ```

   Example — Claude Code:

   ```bash
   claude mcp add --transport http ibigent https://mcp.ibigent.com/mcp/<YOUR_KEY>
   ```

3. **Ask the AI** to generate HTML and send it to your IBIGENT Studio editor, then pick where to insert it.

Full walkthrough: [docs/en/getting-started.md](docs/en/getting-started.md).

## 5. Documentation
- [Getting Started](docs/en/getting-started.md)
- [Installation](docs/en/installation.md)
- [MCP Connection](docs/en/mcp.md)
- [Claude Code](docs/en/claude-code.md)
- [Codex CLI](docs/en/codex.md)
- [Cursor](docs/en/cursor.md)
- [Antigravity](docs/en/antigravity.md)
- [VS Code](docs/en/vscode.md)
- [Examples](docs/en/examples.md)
- [FAQ](docs/en/faq.md)
- [Troubleshooting](docs/en/troubleshooting.md)

Korean documentation: [docs/ko/](docs/ko/)

## 6. Official Website
- Website: https://www.ibigent.com
- Product page: https://www.ibigent.com/service/ibigent-studio.html
- Online docs: https://www.ibigent.com/docs/ibigent-studio/

## 7. License
Documentation in this repository is licensed under **CC BY 4.0** (see [LICENSE](LICENSE)). No product source code is included.

## 8. Contributing
Documentation fixes are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md). Please do not submit product source code or secrets.

## 9. Support
- Help center: https://www.ibigent.com/support/
- Issues: use this repository's Issues for **documentation** problems only.
- Security: see [SECURITY.md](SECURITY.md). **Never post your MCP key** in an issue or PR.

## 10. Roadmap
- [ ] Official VS Code MCP integration guide (in progress).
- [ ] Additional IBIGENT products and their MCP guides.
- [ ] More end-to-end examples.

---
**Keywords:** IBIGENT Studio, MCP, Model Context Protocol, AI website builder, Claude Code MCP, Codex CLI MCP, Cursor MCP, Antigravity MCP, ibigent, mcp.ibigent.com
