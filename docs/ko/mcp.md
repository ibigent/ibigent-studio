# MCP 연결 — IBIGENT Studio

**[문서 홈](../../README_ko.md)**

IBIGENT Studio는 호스팅형 **MCP(Model Context Protocol)** 서버를 제공합니다. MCP를 지원하는 AI 도구에 등록하면 AI가 편집 화면으로 HTML을 보낼 수 있습니다.

## 목차
- [1. 준비](#1-준비-키-발급-불필요)
- [2. 서버 주소](#2-서버-주소)
- [3. 도구에 등록](#3-도구에-등록)
- [4. 사용할 수 있는 도구](#4-사용할-수-있는-도구)
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

## 4. 사용할 수 있는 도구
| 도구 | 대상 | 하는 일 |
|------|------|---------|
| `list_open_editors` | 비전트 AI 호스팅 | 코드 없이 지금 열려 있는 편집 화면을 찾습니다 |
| `read_editor_page` | 비전트 AI 호스팅 | 편집 화면을 읽습니다(부분마다 번호가 붙음) |
| `edit_editor_part` | 비전트 AI 호스팅 | 번호로 고른 부분만 고칩니다 — 바로 반영, [되돌리기] 가능 |
| `get_site_menu` / `set_site_menu` | 비전트 AI 호스팅 | 상단 메뉴를 읽고 바꿉니다 |
| `send_html_to_editor` | 공용 | HTML 블록을 편집 화면으로 보냅니다(빌더는 6자리 코드 필요) |
| `builder_command` | 비전트 AI 빌더 호스팅 | 메뉴·게시판·로고를 바꿉니다(6자리 코드 필요) |

- **비전트 AI 호스팅**은 코드가 필요 없습니다. 편집 화면이 여러 개 열려 있으면 AI가 어느 화면인지 묻습니다.
- 어느 경우든 **저장하기 전에는 실제 사이트가 바뀌지 않습니다.**
- 말로 지시하는 방법 전체: https://www.ibigent.com/docs/ibigent-studio/commands.html

## 보안
- 연결은 아이비전트 로그인(OAuth)으로 인증합니다. 복사·보관할 키가 없습니다.
- 아이비전트 비밀번호·개인정보를 이슈에 올리지 마세요.

---
**공식 문서:** https://www.ibigent.com/docs/ibigent-studio/mcp.html · **키워드:** MCP, Model Context Protocol, IBIGENT Studio, mcp.ibigent.com
