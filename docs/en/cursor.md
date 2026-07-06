# Cursor — IBIGENT Studio (MCP)

**[Docs home](../../README.md) · [MCP](mcp.md)**

Register the IBIGENT Studio MCP server in Cursor from Settings, or by editing `mcp.json`.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Connect](#connect)
- [Notes](#notes)

## Prerequisites
- An active IBIGENT Studio subscription.
- Your MCP key `ibg_…` from [My Page > AI Integration > Connection Keys](https://www.ibigent.com/mypage/mcp-keys.html). See [MCP](mcp.md).
- Replace `<YOUR_KEY>` in the URL with your issued key. **Never share the key** — treat it like a password.

## Connect
### Settings UI
Settings (gear) > Tools & Integrations > **Add custom MCP**. Type: HTTP (URL). Name: **ibigent**. URL:

```text
https://mcp.ibigent.com/mcp/<YOUR_KEY>
```

### Config file
`~/.cursor/mcp.json` (Windows: `C:\Users\<you>\.cursor\mcp.json`):

```json
{
  "mcpServers": {
    "ibigent": { "url": "https://mcp.ibigent.com/mcp/<YOUR_KEY>" }
  }
}
```

## Notes
- When you issue a key on My Page, a one-click Cursor deep link is also offered.

---
**Official docs:** https://www.ibigent.com/docs/ibigent-studio/cursor.html · **Keywords:** Cursor MCP, IBIGENT Studio, Model Context Protocol
