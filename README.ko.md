# Jcble_mam

[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [日本語](README.ja.md) | 한국어

`jcble-mam`은 회사 콘텐츠 운영, 카피라이팅 워크플로, 온라인 마케팅 홍보, multi-Agent 세션 오케스트레이션을 Codex에서 다루기 위한 skill입니다.

Codex가 문서 관리, 제안서 작성, 제품 카피, 소셜 미디어 주제 기획, 비주얼 브리프, 시장 조사, 고객 발굴, 아웃리치 이메일 초안, 주간 및 월간 회고를 수행하는 콘텐츠 및 마케팅 팀처럼 작동하도록 돕습니다.

## 주요 기능

- 재사용 가능한 회사 콘텐츠 및 마케팅 Agent 팀을 만듭니다.
- 편집 조정, 문서 관리, 제안 기획, 카피라이팅, 제품 카피, PPT 기획, 비주얼 브리프, 시장 정보, 고객 발굴, 이메일 초안, 검토, 회고 역할을 정의합니다.
- 역할별 지속형 Codex 세션과 메시지 버스 워크플로를 지원합니다.
- 중국어 간체, 영어, 스페인어, 일본어, 한국어 Markdown 출력을 지원합니다.
- 외부 공개 콘텐츠를 승인된 근거와 사람의 검토에 연결합니다.

## Codex 설치

이 저장소를 Codex skills 디렉터리에 클론합니다:

```bash
git clone https://github.com/Mecil9/jcble-mam.git ~/.agents/skills/jcble-mam
```

그런 다음 새 Codex 세션을 시작하여 skill 레지스트리를 새로 고칩니다.

Codex 설정에서 다른 skills 디렉터리를 사용하는 경우 그 위치에 클론하고 폴더 이름은 다음과 같이 유지하세요:

```text
jcble-mam
```

## 기본 사용법

설치 후 Codex에 자연어로 요청합니다. 예:

```text
jcble-mam을 사용해 우리 회사를 위한 콘텐츠 및 마케팅 Agent 팀을 만들어 주세요.
```

```text
jcble-mam을 사용해 이 제품 문서를 웹사이트 카피와 아웃리치 이메일 초안으로 바꿔 주세요.
```

```text
jcble-mam을 사용해 편집자, 카피라이터, 시장 조사, 비주얼 브리프, 검토 Agent의 독립 Codex 세션을 만들어 주세요.
```

```text
jcble-mam을 사용해 이 제안 요약을 영어, 스페인어, 일본어, 한국어로 작성해 주세요.
```

## 작업 공간 설정

회사 파일과 함께 사용하기 전에 아래 플레이스홀더를 자신의 작업 공간에 맞게 지정합니다:

```text
COMPANY_WORKSPACE=/path/to/company/workspace
COMPANY_KNOWLEDGE_BASE=/path/to/company/knowledge-base
COMPANY_MARKETING_WORKSPACE=/path/to/company/content-marketing-workspace
```

회사에서 다른 폴더 이름을 사용하는 경우 reference 파일을 업데이트하거나 동등한 인덱스 파일을 만드세요.

## 포함 파일

- `SKILL.md` - 트리거 조건과 핵심 워크플로
- `references/agent-team-roles.md` - multi-Agent 역할 라이브러리
- `references/session-orchestration.md` - Codex 세션 생성, 이름 지정, 동기화, 메시지 라우팅
- `references/company-material-boundaries.md` - 회사 자료 경계와 민감 데이터 규칙
- `references/multilingual-workflow.md` - 다국어 Markdown 규칙, 현지화 경계, 검토 체크리스트
- `assets/task-card-template.md` - 작업 카드 템플릿
- `assets/message-template.md` - 메시지 버스 템플릿
- `assets/retrospective-template.md` - 주간/월간 회고 템플릿

## 안전 참고 사항

외부에 게시하거나 보내기 전에:

- 고객, 계약, 재무, 급여, 인증 정보, 개인 데이터 등 기밀 정보를 제거합니다
- 모든 공개 주장을 승인된 원본 파일로 검증합니다
- 아웃리치 이메일은 사람이 승인할 때까지 초안으로 유지합니다
- 생성 이미지를 실제 제품, 실제 현장, 실제 고객 장면으로 표현하지 않습니다

## License

MIT
