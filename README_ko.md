<!-- SEO: IBIGENT Studio, MCP, 모델 컨텍스트 프로토콜, Claude Code, Codex CLI, Cursor, Antigravity, AI 홈페이지 제작 -->

# IBIGENT Studio — 개발자 문서

**[English](README.md) | 한국어**

AI 기반 홈페이지 제작 플랫폼 **IBIGENT Studio** 의 공식 개발자 문서입니다. Claude Code·Codex CLI·Cursor 등 AI 도구를 **MCP(Model Context Protocol)** 로 연결하면, AI가 만든 HTML을 편집 화면 원하는 위치에 바로 넣을 수 있습니다.

> 이 저장소는 **문서 전용** 입니다 — 제품 소스·비밀값 없음.

- 공식 사이트: https://www.ibigent.com
- 전체 문서: https://www.ibigent.com/docs/ibigent-studio/

## 목차
- [1. IBIGENT Studio란](#1-ibigent-studio란)
- [2. 특징](#2-특징)
- [3. 연결 방법 두 가지](#3-연결-방법-두-가지)
- [4. 지원 AI 도구](#4-지원-ai-도구)
- [5. 빠른 시작](#5-빠른-시작)
- [6. 문서](#6-문서)
- [7. 공식 사이트](#7-공식-사이트)
- [8. 라이선스](#8-라이선스)
- [9. 기여](#9-기여)
- [10. 지원](#10-지원)
- [11. 로드맵](#11-로드맵)

## 1. IBIGENT Studio란
IBIGENT Studio는 실시간 웹 편집기입니다. 구독(별도 설치·API 관리 없음) 후 AI 도구를 MCP로 연결하고, AI에게 HTML 제작을 요청하면 결과물이 편집 화면으로 전달되고, 원하는 위치를 골라 바로 반영합니다.

## 2. 특징
- **AI가 만든 HTML을 편집 화면으로.** MCP 연결된 AI 도구에게 HTML을 만들게 해 IBIGENT Studio로 받습니다.
- **원하는 위치에 정확히.** 편집 화면에서 삽입 위치를 고르면 그자리에 반영됩니다.
- **코드 없이 말로 고치기 (비전트 AI 호스팅 · 빌더 호스팅).** 편집 화면을 열어 두면 AI가 화면을 읽고 말한 부분만 바로 고칩니다. 편집 화면에 바로 반영되고 **[되돌리기]** 로 되돌릴 수 있으며, 저장해야 실제 사이트에 반영됩니다.
- **자료로 새 홈페이지 · 내용페이지 만들기.** AI와 정리한 회사 자료를 보내면 편집 화면의 「새 홈페이지 제작」(빌더) · 「내용페이지 추가」 창에 채워지고, 확인 후 [다음] 을 누르면 아이비전트 디자인으로 만들어집니다.
- **메뉴 · 하위 메뉴 관리.** 빌더는 메뉴 · 서브메뉴 · 게시판 · 로고 · 푸터 회사정보를, 비전트 AI 호스팅은 상단 메뉴와 하위 메뉴(하위 페이지형 홈페이지)를 말로 바꿉니다.
- **코딩·키 발급 없이.** 구독과 아이비전트 로그인만 있으면 됩니다.
- **개방형 MCP** 기반으로 이미 쓰는 도구와 함께 동작합니다.

## 3. 연결 방법 두 가지
| 방법 | 어떤 사람에게 | 도구 |
|---|---|---|
| **방법 A. 커넥터 연결** (Custom Connector) | 터미널을 쓰지 않는 분 (권장) | Claude, ChatGPT |
| **방법 B. 터미널 연결** (MCP server configuration) | 개발 도구를 쓰는 분 | Claude Code, Cursor, Codex, Antigravity |

어느 쪽이든 **주소 등록 → 아이비전트 로그인 → [연결 허용]** 한 번이면 끝입니다. 키 발급·복사는 없습니다.

## 4. 지원 AI 도구
| 도구 | 벤더 | 연결 방법 | 가이드 |
|------|------|------|--------|
| Claude | Anthropic | 커넥터 | [웹 문서](https://www.ibigent.com/docs/ibigent-studio/claude-app.html) |
| ChatGPT | OpenAI | 커넥터 | [웹 문서](https://www.ibigent.com/docs/ibigent-studio/chatgpt.html) |
| Claude Code | Anthropic | 터미널 | [docs/ko/claude-code.md](docs/ko/claude-code.md) |
| Codex CLI | OpenAI | 터미널 | [docs/ko/codex.md](docs/ko/codex.md) |
| Cursor | — | 터미널 | [docs/ko/cursor.md](docs/ko/cursor.md) |
| Antigravity | Google | 터미널 | [docs/ko/antigravity.md](docs/ko/antigravity.md) |
| VS Code | — | 터미널 | [docs/ko/vscode.md](docs/ko/vscode.md) (준비 중) |
| 모든 MCP 클라이언트 | — | — | [docs/ko/mcp.md](docs/ko/mcp.md) |

## 5. 빠른 시작
1. **MCP 서버 등록** — AI 도구에 아래 주소를 넣습니다(키 발급 불필요):

   ```
   https://mcp.ibigent.com/mcp
   ```

   예 — Claude Code:

   ```bash
   claude mcp add --transport http ibigent https://mcp.ibigent.com/mcp
   ```

2. **로그인 → [연결 허용]** — 아이비전트 로그인 창이 한 번 뜹니다. 로그인 후 **[연결 허용]** 을 누릅니다.
3. **AI에게 요청** — 편집 화면을 열어 두고 말로 지시합니다.
   - **비전트 AI 호스팅 · 빌더 호스팅**: 코드 없이 `첫 화면 제목을 바꿔줘` · `회사소개 아래에 오시는 길 페이지 만들어줘` 처럼 말하면 AI가 화면을 읽고 그 부분만 고칩니다.
   - **새 홈페이지 · 내용페이지**: `회사 소개 자료로 홈페이지 새로 만들어줘`(빌더) · `이 자료로 대표 인사말 페이지 만들어줘` 처럼 말하면 자료가 제작 창에 채워집니다. 확인 후 [다음] 을 누르세요.
   - 편집 화면에 6자리 코드가 보이는 예전 빌더는 관리자 화면 [패치 받기] 후 코드 없이 됩니다.

전체 안내: [docs/ko/시작하기.md](docs/ko/시작하기.md).

## 6. 문서
- [시작하기](docs/ko/시작하기.md)
- [설치방법](docs/ko/설치방법.md)
- [MCP 연결](docs/ko/mcp.md)
- [Claude Code](docs/ko/claude-code.md)
- [Codex CLI](docs/ko/codex.md)
- [Cursor](docs/ko/cursor.md)
- [Antigravity](docs/ko/antigravity.md)
- [VS Code](docs/ko/vscode.md)
- [예제](docs/ko/examples.md)
- [FAQ](docs/ko/faq.md)
- [문제 해결](docs/ko/troubleshooting.md)

English documentation: [docs/en/](docs/en/)

## 7. 공식 사이트
- 사이트: https://www.ibigent.com
- 제품 소개: https://www.ibigent.com/service/ibigent-studio.html
- 온라인 문서: https://www.ibigent.com/docs/ibigent-studio/

## 8. 라이선스
이 저장소의 문서는 **CC BY 4.0** ([LICENSE](LICENSE)) 를 따릅니다. 제품 소스는 포함되지 않습니다.

## 9. 기여
문서 개선 PR 환영. [CONTRIBUTING.md](CONTRIBUTING.md) 참고. 제품 소스·비밀값은 제출하지 마세요.

## 10. 지원
- 고객센터: https://www.ibigent.com/support/
- Issues: **문서** 문제 전용.
- 보안: [SECURITY.md](SECURITY.md). **비밀번호·개인정보를 이슈·PR에 절대 올리지 마세요.**

## 11. 로드맵
- [ ] VS Code MCP 공식 연동 가이드(진행 중).
- [ ] 추가 IBIGENT 제품 및 MCP 가이드.
- [ ] 종단간 예제 확충.

---
**키워드:** IBIGENT Studio, MCP, Model Context Protocol, AI 홈페이지 제작, Claude Code MCP, Codex CLI MCP, Cursor MCP, Antigravity MCP, ibigent, mcp.ibigent.com
