# Cursor — IBIGENT Studio (MCP)

**[Docs home](../../README.md) · [MCP](mcp.md)**

Register the IBIGENT Studio MCP server in Cursor from Settings, or by editing `mcp.json`.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Connect](#connect)
- [Notes](#notes)

## Prerequisites
- An active IBIGENT Studio subscription.
> No key is required. Once you register the URL, the IBIGENT sign-in page opens — sign in and click **Allow** once.
- Replace the address above in the URL with your issued key. **Never share the key** — treat it like a password.

## Connect
### Settings UI
Settings (gear) > Tools & Integrations > **Add custom MCP**. Type: HTTP (URL). Name: **ibigent**. URL:

```text
https://mcp.ibigent.com/mcp
```

### Config file
`~/.cursor/mcp.json` (Windows: `C:\Users\<you>\.cursor\mcp.json`):

```json
{
  "mcpServers": {
    "ibigent": { "url": "https://mcp.ibigent.com/mcp" }
  }
}
```

## Notes
- When you issue a key on My Page, a one-click Cursor deep link is also offered.

---
**Official docs:** https://www.ibigent.com/docs/ibigent-studio/cursor.html · **Keywords:** Cursor MCP, IBIGENT Studio, Model Context Protocol
