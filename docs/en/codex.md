# Codex CLI — IBIGENT Studio (MCP)

**[Docs home](../../README.md) · [MCP](mcp.md)**

Register the IBIGENT Studio MCP server in Codex CLI with the command below, or by editing `config.toml`.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Connect](#connect)
- [Notes](#notes)

## Prerequisites
- An active IBIGENT Studio subscription.
- Your MCP key `ibg_…` from [My Page > AI Integration > Connection Keys](https://www.ibigent.com/mypage/mcp-keys.html). See [MCP](mcp.md).
- Replace `<YOUR_KEY>` in the URL with your issued key. **Never share the key** — treat it like a password.

## Connect
### Command
Paste into your terminal and run:

```bash
codex mcp add ibigent --url https://mcp.ibigent.com/mcp/<YOUR_KEY>
```

### Config file
`~/.codex/config.toml` (Windows: `C:\Users\<you>\.codex\config.toml`):

```toml
[mcp_servers.ibigent]
url = "https://mcp.ibigent.com/mcp/<YOUR_KEY>"
```

## Notes
- The table name uses an underscore and plural: `[mcp_servers.ibigent]`.
- Do **not** add `transport` or `type` keys — they cause errors.
- Verify: run `codex mcp list` and confirm **ibigent** appears.

---
**Official docs:** https://www.ibigent.com/docs/ibigent-studio/codex.html · **Keywords:** Codex CLI MCP, IBIGENT Studio, Model Context Protocol
