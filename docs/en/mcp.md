# MCP Connection — IBIGENT Studio

**[Docs home](../../README.md)**

IBIGENT Studio exposes a hosted **MCP (Model Context Protocol)** server. Register it in any MCP-capable AI tool to let the AI send HTML into your editor.

## Table of Contents
- [1. Before you start](#1-before-you-start-no-key-needed)
- [2. Server URL](#2-server-url)
- [3. Register in your tool](#3-register-in-your-tool)
- [4. Available tools](#4-available-tools)
- [Security](#security)

## 1. Before you start (no key needed)
> No key is required. Once you register the URL, the IBIGENT sign-in page opens — sign in and click **Allow** once.

## 2. Server URL
Register this URL in your AI tool. No key is needed:

```
https://mcp.ibigent.com/mcp
```

## 3. Register in your tool
| Tool | Guide |
|------|-------|
| Claude Code | [claude-code.md](claude-code.md) |
| Codex CLI | [codex.md](codex.md) |
| Cursor | [cursor.md](cursor.md) |
| Antigravity | [antigravity.md](antigravity.md) |
| VS Code | [vscode.md](vscode.md) (coming soon) |

## 4. Available tools
| Tool | For | What it does |
|------|-----|--------------|
| `list_open_editors` | Both | Finds the editors you have open — no code needed |
| `read_editor_page` | Both | Reads the editor page (each part gets an ID; Builder also returns menus, submenus and footer details) |
| `edit_editor_part` | Both | Changes only the part with that ID — applied immediately, with Undo |
| `get_site_menu` / `set_site_menu` | IBIGENT AI Hosting | Reads and changes the top menu |
| `send_html_to_editor` | Both | Sends an HTML block to the editor |
| `builder_command` | IBIGENT AI Builder Hosting | Changes menus, submenus, boards, pages, logo and footer details, and saves blog posts as drafts — applied immediately, with Undo |

- **IBIGENT AI Hosting and Builder Hosting** need no code. If several editors are open, the AI asks which one.
- Older builders that still show a 6-character code in the editor become code-free after the admin clicks [Get patch]. Until then, put the code in front of your request.
- Editor content goes live **when you save**. Builder menus, pages, logo and footer details go live **immediately** and can be undone with Undo.

## Security
- Connections are authenticated by signing in to IBIGENT (OAuth). There is no key to copy or store.
- Never post your IBIGENT password or personal data in an issue.

---
**Official docs:** https://www.ibigent.com/docs/ibigent-studio/mcp.html · **Keywords:** MCP, Model Context Protocol, IBIGENT Studio, mcp.ibigent.com
