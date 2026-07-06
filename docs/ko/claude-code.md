# Claude Code 연결 — IBIGENT Studio (MCP)

**[문서 홈](../../README_ko.md) · [MCP](mcp.md)**

아래 명령 또는 MCP 설정 파일로 Claude Code에 IBIGENT Studio MCP 서버를 등록합니다.

## 목차
- [준비물](#준비물)
- [연결](#연결)
- [참고](#참고)

## 준비물
- IBIGENT Studio 구독(활성).
- [마이페이지 > AI 연동 > 연동 키 관리](https://www.ibigent.com/mypage/mcp-keys.html) 에서 발급받은 키 `ibg_…`. [MCP](mcp.md) 참고.
- URL의 `<내_키>` 를 발급받은 키로 교체. **키는 비밀번호처럼 노출 금지.**

## 연결
### 명령어 (권장)
터미널에 붙여넣고 실행:

```bash
claude mcp add --transport http ibigent https://mcp.ibigent.com/mcp/<내_키>
```

### 설정 파일
작업 폴더의 `.mcp.json` (전체 적용은 홈의 `~/.claude.json`):

```json
{
  "mcpServers": {
    "ibigent": { "type": "http", "url": "https://mcp.ibigent.com/mcp/<내_키>" }
  }
}
```

## 참고
- 확인: `claude mcp list` 에 **ibigent** 이 보이면 완료.

---
**공식 문서:** https://www.ibigent.com/docs/ibigent-studio/claude.html · **키워드:** Claude Code MCP, IBIGENT Studio, Model Context Protocol
