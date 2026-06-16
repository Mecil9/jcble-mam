# Multilingual Markdown Workflow

Use this guide when creating, translating, or localizing Markdown files for company content, marketing, outreach, proposals, reviews, and Agent coordination.

## Supported Languages

| Code | Language | Use For |
|---|---|---|
| `zh-CN` | 简体中文 | Default internal work, Chinese marketing copy, Chinese task coordination |
| `en` | English | Global public content, international sales materials, outreach drafts |
| `es` | Español | Spanish-language public content, market notes, outreach drafts |
| `ja` | 日本語 | Japanese-language public content, market notes, outreach drafts |
| `ko` | 한국어 | Korean-language public content, market notes, outreach drafts |

## Language Selection

1. Use the language explicitly requested by the user.
2. If no language is requested, use the user's workspace default or Simplified Chinese.
3. For international outreach, ask for the target region when tone or wording may differ.
4. For one multilingual file, create sections in this order: `zh-CN`, `en`, `es`, `ja`, `ko`.
5. For separate language files, use suffixes such as `proposal.zh-CN.md`, `proposal.en.md`, `proposal.es.md`, `proposal.ja.md`, and `proposal.ko.md`.

## Markdown Structure

Keep Markdown stable across languages:

- Preserve heading hierarchy, tables, links, IDs, task numbers, dates, metrics, and source paths.
- Translate headings, labels, body copy, calls to action, and review notes into the target language.
- Keep product model names, company legal names, file paths, URLs, email addresses, version numbers, standards, and certifications unchanged unless an approved official translation exists.
- Use UTF-8 Markdown.
- Avoid mixing languages inside one section except for proper nouns, model names, source citations, and required glossary terms.

## Template Localization

When localizing `assets/*.md` templates, keep the same fields and replace labels with the target language. Use this core label glossary:

| Field | `zh-CN` | `en` | `es` | `ja` | `ko` |
|---|---|---|---|---|---|
| Task card | 任务单 | Task Card | Ficha de tarea | タスクカード | 작업 카드 |
| Task ID | 任务编号 | Task ID | ID de tarea | タスクID | 작업 ID |
| Created date | 创建日期 | Created Date | Fecha de creación | 作成日 | 생성일 |
| Owner | 负责人 | Owner | Responsable | 担当者 | 담당자 |
| Target language | 目标语言 | Target Language | Idioma objetivo | 対象言語 | 대상 언어 |
| Audience | 目标受众 | Target Audience | Público objetivo | 対象読者 | 대상 독자 |
| Channel | 使用渠道 | Channel | Canal | チャネル | 채널 |
| Deadline | 截止时间 | Deadline | Fecha límite | 期限 | 마감일 |
| Input | 输入 | Input | Entrada | 入力 | 입력 |
| Output | 输出 | Output | Entregable | 出力 | 출력 |
| Reviewer | 审核人 | Reviewer | Revisor | レビュー担当 | 검토자 |
| Archive location | 归档位置 | Archive Location | Ubicación de archivo | アーカイブ先 | 보관 위치 |
| Message bus | 消息总线 | Message Bus | Bus de mensajes | メッセージバス | 메시지 버스 |
| Status | 状态 | Status | Estado | ステータス | 상태 |
| Sender Agent | 发件 Agent | Sender Agent | Agent remitente | 送信 Agent | 발신 Agent |
| Receiver Agent | 收件 Agent | Receiver Agent | Agent destinatario | 受信 Agent | 수신 Agent |
| Request | 请求 | Request | Solicitud | 依頼 | 요청 |
| Reply | 回复 | Reply | Respuesta | 返信 | 답변 |
| Retrospective | 复盘 | Retrospective | Retrospectiva | 振り返り | 회고 |
| Data source | 数据来源 | Data Source | Fuente de datos | データソース | 데이터 출처 |
| Changes | 变化 | Changes | Cambios | 変化 | 변화 |
| Cause analysis | 原因判断 | Cause Analysis | Análisis de causas | 原因分析 | 원인 분석 |
| Next actions | 下周期动作 | Next Actions | Próximas acciones | 次のアクション | 다음 작업 |

## Localization Rules

### Chinese `zh-CN`

- Use concise Simplified Chinese.
- Prefer clear business wording over slogans.
- Keep claims tied to evidence and avoid exaggerated guarantees.

### English `en`

- Use plain international business English.
- Prefer direct sentences and specific benefits.
- Avoid idioms that may not translate well across regions.

### Spanish `es`

- Use neutral international Spanish.
- Avoid region-specific slang.
- Keep business tone clear, professional, and specific.

### Japanese `ja`

- Use polite business Japanese.
- Prefer clear `です / ます` style for external-facing content.
- Avoid overstatement, excessive urgency, and unsupported superiority claims.

### Korean `ko`

- Use formal business Korean.
- Prefer `-습니다 / -합니다` style for external-facing content.
- Avoid excessive honorifics and unsupported superiority claims.

## Translation Boundaries

- Do not translate or localize unverified customer claims, pricing, certifications, compliance statements, or technical parameters without checking the approved source.
- Mark uncertain terms with a review note instead of guessing.
- Preserve source citations from the original Markdown.
- When translating outreach emails, keep them as drafts and require human approval before sending.
- When generated images or visual prompts are included, do not present generated visuals as real products, real sites, or real customer scenes.

## Review Checklist

Before finalizing multilingual Markdown:

- Confirm the target language code is shown in the task card or file name.
- Confirm all numbers, dates, source paths, URLs, and product identifiers match the source.
- Confirm sensitive content is not exposed in external-facing translations.
- Confirm the tone fits the target language and channel.
- Confirm tables still render correctly after translation.
- Confirm all language sections are complete when producing one multilingual file.
