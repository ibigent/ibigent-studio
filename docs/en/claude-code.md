# Claude Code — IBIGENT Studio (MCP)

**[Docs home](../../README.md) · [MCP](mcp.md)**

Register the IBIGENT Studio MCP server in Claude Code with the command below, or by editing your MCP config file.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Connect](#connect)
- [Notes](#notes)

## Prerequisites
- An active IBIGENT Studio subscription.
> No key is required. Once you register the URL, the IBIGENT sign-in page opens — sign in and click **Allow** once.

## Connect
### Command (recommended)
Paste into your terminal and run:

```bash
claude mcp add --transport http ibigent https://mcp.ibigent.com/mcp
```

### Config file
Project scope `.mcp.json` (or `~/.claude.json` for all projects):

```json
{
  "mcpServers": {
    "ibigent": { "type": "http", "url": "https://mcp.ibigent.com/mcp" }
  }
}
```

## Notes
- Verify: run `claude mcp list` and confirm **ibigent** appears.

---
**Official docs:** https://www.ibigent.com/docs/ibigent-studio/claude.html · **Keywords:** Claude Code MCP, IBIGENT Studio, Model Context Protocol
