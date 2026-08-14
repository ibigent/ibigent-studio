# Cursor 연결 — IBIGENT Studio (MCP)

**[문서 홈](../../README_ko.md) · [MCP](mcp.md)**

설정 화면 또는 `mcp.json` 으로 Cursor에 IBIGENT Studio MCP 서버를 등록합니다.

## 목차
- [준비물](#준비물)
- [연결](#연결)
- [참고](#참고)

## 준비물
- IBIGENT Studio 구독(활성).
> 키 발급은 더 이상 필요하지 않습니다. 주소를 등록하면 아이비전트 로그인 → [연결 허용] 한 번으로 연결됩니다.
- URL의 위 주소 를 발급받은 키로 교체. **키는 비밀번호처럼 노출 금지.**

## 연결
### 설정 화면
설정(⚙) > Tools & Integrations > **Add custom MCP**. 종류 HTTP(URL), 이름 **ibigent**, 주소:

```text
https://mcp.ibigent.com/mcp
```

### 설정 파일
`~/.cursor/mcp.json` (Windows: `C:\Users\사용자\.cursor\mcp.json`):

```json
{
  "mcpServers": {
    "ibigent": { "url": "https://mcp.ibigent.com/mcp" }
  }
}
```

## 참고

---
**공식 문서:** https://www.ibigent.com/docs/ibigent-studio/cursor.html · **키워드:** Cursor MCP, IBIGENT Studio, Model Context Protocol
