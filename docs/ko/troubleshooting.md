# 문제 해결 — IBIGENT Studio

**[문서 홈](../../README_ko.md)**

### 도구에 `ibigent` 이 안 보임
URL·키 재확인 후 `claude mcp list` / `codex mcp list` 로 확인. 설정 파일 수정 후 도구 재시작.

### Codex: 등록 오류
`[mcp_servers.ibigent]` (밑줄·복수) + `url` 키만 사용. `transport`·`type` 키는 오류.

### Antigravity: 서버 인식 안 됨
키는 `serverUrl` 이어야 합니다(`url`/`httpUrl` 아님). `~/.gemini/config/mcp_config.json` 수정 후 **Refresh**.

### “initialization did not complete within 60000ms”
보통 관련 없는 다른 MCP/커넥터가 시작 시 멈추면 발생. 다른 커넥터를 정리·수정 후 재시도.

### 인증 실패
키가 틀렸거나 폐기됐을 수 있습니다. 연동 키 관리 페이지(https://www.ibigent.com/mypage/mcp-keys.html)에서 재발급 후 URL 갱신.

---
**키워드:** IBIGENT Studio 문제 해결, MCP 오류, serverUrl, config.toml
