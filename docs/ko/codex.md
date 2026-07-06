# Codex CLI 연결 — IBIGENT Studio (MCP)

**[문서 홈](../../README_ko.md) · [MCP](mcp.md)**

아래 명령 또는 `config.toml` 로 Codex CLI에 IBIGENT Studio MCP 서버를 등록합니다.

## 목차
- [준비물](#준비물)
- [연결](#연결)
- [참고](#참고)

## 준비물
- IBIGENT Studio 구독(활성).
- [마이페이지 > AI 연동 > 연동 키 관리](https://www.ibigent.com/mypage/mcp-keys.html) 에서 발급받은 키 `ibg_…`. [MCP](mcp.md) 참고.
- URL의 `<내_키>` 를 발급받은 키로 교체. **키는 비밀번호처럼 노출 금지.**

## 연결
### 명령어
터미널에 붙여넣고 실행:

```bash
codex mcp add ibigent --url https://mcp.ibigent.com/mcp/<내_키>
```

### 설정 파일
`~/.codex/config.toml` (Windows: `C:\Users\사용자\.codex\config.toml`):

```toml
[mcp_servers.ibigent]
url = "https://mcp.ibigent.com/mcp/<내_키>"
```

## 참고
- 표 이름은 밑줄·복수형 `[mcp_servers.ibigent]`.
- `transport`·`type` 키는 **금지**(오류).
- 확인: `codex mcp list` 에 **ibigent** 표시.

---
**공식 문서:** https://www.ibigent.com/docs/ibigent-studio/codex.html · **키워드:** Codex CLI MCP, IBIGENT Studio, Model Context Protocol
