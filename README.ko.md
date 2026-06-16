# Jcble_mam

[简体中文](README.zh-CN.md) | [English](README.en.md) | [Español](README.es.md) | [日本語](README.ja.md)

`jcble-mam`은 회사 콘텐츠 운영, 카피라이팅 워크플로, 온라인 마케팅 홍보, multi-Agent 협업 팀을 구축하고 운영하기 위한 범용 Codex skill입니다.

지원하는 Markdown 언어:

- 중국어 간체 `zh-CN`
- 영어 `en`
- 스페인어 `es`
- 일본어 `ja`
- 한국어 `ko`

## 사용 사례

- 회사 문서 관리
- 솔루션 기획 및 제안서 작성
- 소셜 미디어 주제 기획
- 회사 및 솔루션 PPT 기획
- 제품 카피라이팅
- 제품, 솔루션, 홍보 이미지용 비주얼 브리프
- 글로벌 시장 정보 수집
- 업계 뉴스 추적
- 해외 고객 발굴
- 아웃리치 이메일 초안 작성
- 주간 및 월간 콘텐츠, 플랫폼, 리드 회고
- 지속형 multi-Agent Codex 세션 설정
- 다국어 Markdown 작성, 번역, 현지화

## Skill 이름

설치 가능한 skill 이름은 다음과 같습니다:

```text
jcble-mam
```

`Jcble_mam`은 표시 이름과 사용자용 별칭으로 유지됩니다. 이 워크플로는 범용이며 어떤 회사에도 맞게 적용할 수 있습니다.

## 설치

이 저장소를 Codex skills 디렉터리에 클론합니다:

```bash
git clone https://github.com/Mecil9/jcble-mam.git ~/.agents/skills/jcble-mam
```

그런 다음 새 Codex 세션을 시작하여 skill 레지스트리를 새로 고칩니다.

## 설정

사용하기 전에 아래 플레이스홀더를 자신의 회사 작업 공간에 맞게 바꿉니다:

```text
COMPANY_WORKSPACE=/path/to/company/workspace
COMPANY_KNOWLEDGE_BASE=/path/to/company/knowledge-base
COMPANY_MARKETING_WORKSPACE=/path/to/company/content-marketing-workspace
```

회사에서 다른 폴더 이름을 사용하는 경우 reference 파일을 업데이트하거나 동등한 인덱스 파일을 만드세요.

## 주요 파일

- `SKILL.md` - 트리거 조건과 핵심 워크플로
- `references/agent-team-roles.md` - multi-Agent 역할 라이브러리
- `references/session-orchestration.md` - Codex 세션 생성, 이름 지정, 동기화, 메시지 라우팅
- `references/company-material-boundaries.md` - 회사 자료 경계와 민감 데이터 규칙
- `references/multilingual-workflow.md` - 다국어 Markdown 규칙, 현지화 경계, 검토 체크리스트
- `assets/task-card-template.md` - 작업 카드 템플릿
- `assets/message-template.md` - 메시지 버스 템플릿
- `assets/retrospective-template.md` - 주간/월간 회고 템플릿

## 안전 참고 사항

외부에 공개하기 전에:

- 고객, 계약, 재무, 급여, 인증 정보, 개인 데이터 등 기밀 정보를 제거합니다
- 모든 공개 주장을 승인된 원본 파일로 검증합니다
- 아웃리치 이메일은 사람이 승인할 때까지 초안으로 유지합니다
- 생성 이미지를 실제 제품, 실제 현장, 실제 고객 장면으로 표현하지 않습니다

## License

MIT
