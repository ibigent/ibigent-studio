# Antigravity — IBIGENT Studio (MCP)

**[Docs home](../../README.md) · [MCP](mcp.md)**

Register the IBIGENT Studio MCP server in Antigravity by editing its raw MCP config.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Connect](#connect)
- [Notes](#notes)

## Prerequisites
- An active IBIGENT Studio subscription.
> No key is required. Once you register the URL, the IBIGENT sign-in page opens — sign in and click **Allow** once.

## Connect
### Config file
In the agent panel: **... > MCP Servers > View raw config**, which opens `~/.gemini/config/mcp_config.json` (Windows: `C:\Users\<you>\.gemini\config\mcp_config.json`). Add the entry, then click **Refresh**:

```json
{
  "mcpServers": {
    "ibigent": { "serverUrl": "https://mcp.ibigent.com/mcp" }
  }
}
```

## Notes
- For remote servers the key **must be `serverUrl`** — `url` / `httpUrl` are silently ignored.
- After registering, tools start in an **Ask** state — allow once to proceed.

---
**Official docs:** https://www.ibigent.com/docs/ibigent-studio/antigravity.html · **Keywords:** Antigravity MCP, IBIGENT Studio, Model Context Protocol
