# Codex CLI 연결 — IBIGENT Studio (MCP)

**[문서 홈](../../README_ko.md) · [MCP](mcp.md)**

아래 명령 또는 `config.toml` 로 Codex CLI에 IBIGENT Studio MCP 서버를 등록합니다.

## 목차
- [준비물](#준비물)
- [연결](#연결)
- [참고](#참고)

## 준비물
- IBIGENT Studio 구독(활성).
> 키 발급은 더 이상 필요하지 않습니다. 주소를 등록하면 아이비전트 로그인 → [연결 허용] 한 번으로 연결됩니다.
- URL의 위 주소 를 발급받은 키로 교체. **키는 비밀번호처럼 노출 금지.**

## 연결
### 명령어
터미널에 붙여넣고 실행:

```bash
codex mcp add ibigent --url https://mcp.ibigent.com/mcp
```

### 설정 파일
`~/.codex/config.toml` (Windows: `C:\Users\사용자\.codex\config.toml`):

```toml
[mcp_servers.ibigent]
url = "https://mcp.ibigent.com/mcp"
```

## 참고
- 표 이름은 밑줄·복수형 `[mcp_servers.ibigent]`.
- `transport`·`type` 키는 **금지**(오류).
- 확인: `codex mcp list` 에 **ibigent** 표시.

---
**공식 문서:** https://www.ibigent.com/docs/ibigent-studio/codex.html · **키워드:** Codex CLI MCP, IBIGENT Studio, Model Context Protocol
