# MCP 연결 — IBIGENT Studio

**[문서 홈](../../README_ko.md)**

IBIGENT Studio는 호스팅형 **MCP(Model Context Protocol)** 서버를 제공합니다. MCP를 지원하는 AI 도구에 등록하면 AI가 편집 화면으로 HTML을 보낼 수 있습니다.

## 목차
- [1. 준비](#1-준비-키-발급-불필요)
- [2. 서버 주소](#2-서버-주소)
- [3. 도구에 등록](#3-도구에-등록)
- [보안](#보안)

## 1. 준비 (키 발급 불필요)
> 키 발급은 더 이상 필요하지 않습니다. 주소를 등록하면 아이비전트 로그인 → [연결 허용] 한 번으로 연결됩니다.

## 2. 서버 주소
AI 도구에 아래 주소를 등록합니다. 키 발급·복사는 필요 없습니다:

```
https://mcp.ibigent.com/mcp
```

## 3. 도구에 등록
| 도구 | 가이드 |
|------|--------|
| Claude Code | [claude-code.md](claude-code.md) |
| Codex CLI | [codex.md](codex.md) |
| Cursor | [cursor.md](cursor.md) |
| Antigravity | [antigravity.md](antigravity.md) |
| VS Code | [vscode.md](vscode.md) (준비 중) |

## 보안
- 연결은 아이비전트 로그인(OAuth)으로 인증합니다. 복사·보관할 키가 없습니다.
- 아이비전트 비밀번호·개인정보를 이슈에 올리지 마세요.

---
**공식 문서:** https://www.ibigent.com/docs/ibigent-studio/mcp.html · **키워드:** MCP, Model Context Protocol, IBIGENT Studio, mcp.ibigent.com
