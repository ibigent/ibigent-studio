# MCP Connection — IBIGENT Studio

**[Docs home](../../README.md)**

IBIGENT Studio exposes a hosted **MCP (Model Context Protocol)** server. Register it in any MCP-capable AI tool to let the AI send HTML into your editor.

## Table of Contents
- [1. Before you start](#1-before-you-start-no-key-needed)
- [2. Server URL](#2-server-url)
- [3. Register in your tool](#3-register-in-your-tool)
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

## Security
- Your key authenticates requests — **treat it like a password.** Do not commit it, share it, or paste it into issues.
- If a key is exposed, revoke/reissue it on the Connection Keys page.

---
**Official docs:** https://www.ibigent.com/docs/ibigent-studio/mcp.html · **Keywords:** MCP, Model Context Protocol, IBIGENT Studio, mcp.ibigent.com
