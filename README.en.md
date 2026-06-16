# Jcble_mam

[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

`jcble-mam` is a Codex skill for company content operations, copywriting workflows, online marketing promotion, and multi-Agent session orchestration.

It helps Codex work as a coordinated content and marketing team for document management, proposal writing, product copy, social media topics, visual briefs, market research, customer discovery, email outreach drafts, and weekly or monthly retrospectives.

## What It Does

- Creates a reusable company content and marketing Agent team.
- Defines role Agents for editorial coordination, document management, proposal planning, copywriting, product copy, PPT planning, visual briefs, market intelligence, customer discovery, email drafting, review, and retrospectives.
- Supports persistent Codex role sessions and a message-bus workflow.
- Supports Markdown output in Simplified Chinese, English, Spanish, Japanese, and Korean.
- Keeps external-facing content tied to approved evidence and human review.

## Install For Codex

Clone this repository into your Codex skills directory:

```bash
git clone https://github.com/Mecil9/jcble-mam.git ~/.agents/skills/jcble-mam
```

Then start a new Codex session so the skill registry can refresh.

If your Codex setup uses a different skills directory, clone the repository there and keep the folder name as:

```text
jcble-mam
```

## Basic Usage

After installation, ask Codex in natural language. Examples:

```text
Use jcble-mam to create a content and marketing Agent team for my company.
```

```text
Use jcble-mam to turn this product document into website copy and an outreach email draft.
```

```text
Use jcble-mam to create independent Codex sessions for the editor, copywriter, market research, visual brief, and review Agents.
```

```text
Use jcble-mam to write this proposal summary in English, Spanish, Japanese, and Korean.
```

## Workspace Configuration

Before using the skill with company files, map these placeholders to your own workspace:

```text
COMPANY_WORKSPACE=/path/to/company/workspace
COMPANY_KNOWLEDGE_BASE=/path/to/company/knowledge-base
COMPANY_MARKETING_WORKSPACE=/path/to/company/content-marketing-workspace
```

If your company uses different directory names, update the reference files or create equivalent index files.

## Included Files

- `SKILL.md` - trigger conditions and core workflow
- `references/agent-team-roles.md` - multi-Agent role library
- `references/session-orchestration.md` - Codex session creation, naming, synchronization, and message routing
- `references/company-material-boundaries.md` - company material boundaries and sensitive-data rules
- `references/multilingual-workflow.md` - multilingual Markdown rules, localization boundaries, and review checklist
- `assets/task-card-template.md` - task-card template
- `assets/message-template.md` - message-bus template
- `assets/retrospective-template.md` - weekly/monthly retrospective template

## Safety Notes

Before publishing or sending anything externally:

- remove confidential customer, contract, finance, payroll, credential, and personal data
- verify all public claims against approved source files
- keep outreach emails as drafts until human approval
- do not represent generated visuals as real products, real sites, or real customer scenes

## License

MIT
