# Antigravity 연결 — IBIGENT Studio (MCP)

**[문서 홈](../../README_ko.md) · [MCP](mcp.md)**

Antigravity의 raw MCP 설정에 IBIGENT Studio MCP 서버를 등록합니다.

## 목차
- [준비물](#준비물)
- [연결](#연결)
- [참고](#참고)

## 준비물
- IBIGENT Studio 구독(활성).
- [마이페이지 > AI 연동 > 연동 키 관리](https://www.ibigent.com/mypage/mcp-keys.html) 에서 발급받은 키 `ibg_…`. [MCP](mcp.md) 참고.
- URL의 `<내_키>` 를 발급받은 키로 교체. **키는 비밀번호처럼 노출 금지.**

## 연결
### 설정 파일
에이전트 패널 **··· > MCP Servers > View raw config** 로 `~/.gemini/config/mcp_config.json` (Windows: `C:\Users\사용자\.gemini\config\mcp_config.json`) 에 추가 후 **Refresh**:

```json
{
  "mcpServers": {
    "ibigent": { "serverUrl": "https://mcp.ibigent.com/mcp/<내_키>" }
  }
}
```

## 참고
- 원격 서버는 반드시 키 이름 **`serverUrl`** — `url`·`httpUrl` 은 조용히 무시됩니다.
- 등록 후 도구는 처음 **확인 요청(Ask)** 상태 — 한 번 허용하면 됩니다.

---
**공식 문서:** https://www.ibigent.com/docs/ibigent-studio/antigravity.html · **키워드:** Antigravity MCP, IBIGENT Studio, Model Context Protocol
