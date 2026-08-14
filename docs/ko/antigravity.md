# Antigravity 연결 — IBIGENT Studio (MCP)

**[문서 홈](../../README_ko.md) · [MCP](mcp.md)**

Antigravity의 raw MCP 설정에 IBIGENT Studio MCP 서버를 등록합니다.

## 목차
- [준비물](#준비물)
- [연결](#연결)
- [참고](#참고)

## 준비물
- IBIGENT Studio 구독(활성).
> 키 발급은 더 이상 필요하지 않습니다. 주소를 등록하면 아이비전트 로그인 → [연결 허용] 한 번으로 연결됩니다.
- URL의 위 주소 를 발급받은 키로 교체. **키는 비밀번호처럼 노출 금지.**

## 연결
### 설정 파일
에이전트 패널 **··· > MCP Servers > View raw config** 로 `~/.gemini/config/mcp_config.json` (Windows: `C:\Users\사용자\.gemini\config\mcp_config.json`) 에 추가 후 **Refresh**:

```json
{
  "mcpServers": {
    "ibigent": { "serverUrl": "https://mcp.ibigent.com/mcp" }
  }
}
```

## 참고
- 원격 서버는 반드시 키 이름 **`serverUrl`** — `url`·`httpUrl` 은 조용히 무시됩니다.
- 등록 후 도구는 처음 **확인 요청(Ask)** 상태 — 한 번 허용하면 됩니다.

---
**공식 문서:** https://www.ibigent.com/docs/ibigent-studio/antigravity.html · **키워드:** Antigravity MCP, IBIGENT Studio, Model Context Protocol
