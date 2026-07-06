# Troubleshooting — IBIGENT Studio

**[Docs home](../../README.md)**

### The tool doesn't list `ibigent`
Re-check the URL and key, then verify: `claude mcp list` / `codex mcp list`. Restart the tool after editing config files.

### Codex: registration error
Use `[mcp_servers.ibigent]` (underscore, plural) with only a `url` key. `transport` or `type` keys cause errors.

### Antigravity: server not detected
The key must be `serverUrl` (not `url`/`httpUrl`). Click **Refresh** after editing `~/.gemini/config/mcp_config.json`.

### “initialization did not complete within 60000ms”
Usually caused by an unrelated MCP/connector hanging on startup. Remove or fix other connectors, then retry.

### Authentication fails
Your key may be wrong or revoked. Reissue it on the Connection Keys page (https://www.ibigent.com/mypage/mcp-keys.html) and update the URL.

---
**Keywords:** IBIGENT Studio troubleshooting, MCP errors, serverUrl, config.toml
