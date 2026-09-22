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
- Cursor supports OAuth sign-in for remote servers. After registering, sign in to IBIGENT and click **Allow** when the window opens.

---
**Official docs:** https://www.ibigent.com/docs/ibigent-studio/cursor.html · **Keywords:** Cursor MCP, IBIGENT Studio, Model Context Protocol
