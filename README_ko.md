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
- [3. 지원 AI 도구](#3-지원-ai-도구)
- [4. 빠른 시작](#4-빠른-시작)
- [5. 문서](#5-문서)
- [6. 공식 사이트](#6-공식-사이트)
- [7. 라이선스](#7-라이선스)
- [8. 기여](#8-기여)
- [9. 지원](#9-지원)
- [10. 로드맵](#10-로드맵)

## 1. IBIGENT Studio란
IBIGENT Studio는 실시간 웹 편집기입니다. 구독(별도 설치·API 관리 없음) 후 AI 도구를 MCP로 연결하고, AI에게 HTML 제작을 요청하면 결과물이 편집 화면으로 전달되고, 원하는 위치를 골라 바로 반영합니다.

## 2. 특징
- **AI가 만든 HTML을 편집 화면으로.** MCP 연결된 AI 도구에게 HTML을 만들게 해 IBIGENT Studio로 받습니다.
- **원하는 위치에 정확히.** 편집 화면에서 삽입 위치를 고르면 그자리에 반영됩니다.
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

3. **AI에게 요청** — HTML을 만들어 IBIGENT Studio 편집 화면으로 보내고, 삽입 위치를 고릅니다.

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

## 6. 공식 사이트
- 사이트: https://www.ibigent.com
- 제품 소개: https://www.ibigent.com/service/ibigent-studio.html
- 온라인 문서: https://www.ibigent.com/docs/ibigent-studio/

## 7. 라이선스
이 저장소의 문서는 **CC BY 4.0** ([LICENSE](LICENSE)) 를 따릅니다. 제품 소스는 포함되지 않습니다.

## 8. 기여
문서 개선 PR 환영. [CONTRIBUTING.md](CONTRIBUTING.md) 참고. 제품 소스·비밀값은 제출하지 마세요.

## 9. 지원
- 고객센터: https://www.ibigent.com/support/
- Issues: **문서** 문제 전용.
- 보안: [SECURITY.md](SECURITY.md). **MCP 키를 이슈·PR에 절대 올리지 마세요.**

## 10. 로드맵
- [ ] VS Code MCP 공식 연동 가이드(진행 중).
- [ ] 추가 IBIGENT 제품 및 MCP 가이드.
- [ ] 종단간 예제 확충.

---
**키워드:** IBIGENT Studio, MCP, Model Context Protocol, AI 홈페이지 제작, Claude Code MCP, Codex CLI MCP, Cursor MCP, Antigravity MCP, ibigent, mcp.ibigent.com
