# MCP 연결 — IBIGENT Studio

**[문서 홈](../../README_ko.md)**

IBIGENT Studio는 호스팅형 **MCP(Model Context Protocol)** 서버를 제공합니다. MCP를 지원하는 AI 도구에 등록하면 AI가 편집 화면으로 HTML을 보낼 수 있습니다.

## 목차
- [1. 키 발급](#1-키-발급)
- [2. 서버 주소](#2-서버-주소)
- [3. 도구에 등록](#3-도구에-등록)
- [보안](#보안)

## 1. 키 발급
1. **마이페이지 > AI 연동 > 연동 키 관리**: https://www.ibigent.com/mypage/mcp-keys.html
2. **[키 발급]** 클릭. `ibg_…` 키가 생성되고 **1회만** 표시됩니다. 안전하게 보관하세요.

## 2. 서버 주소
AI 도구에 아래 주소를 등록하고 `<내_키>` 를 발급받은 키로 교체:

```
https://mcp.ibigent.com/mcp/<내_키>
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
- 키는 요청을 인증합니다 — **비밀번호처럼 취급.** 커밋·공유·이슈 붙여넣기 금지.
- 키가 노출되면 연동 키 관리 페이지에서 재발급하세요.

---
**공식 문서:** https://www.ibigent.com/docs/ibigent-studio/mcp.html · **키워드:** MCP, Model Context Protocol, IBIGENT Studio, mcp.ibigent.com
