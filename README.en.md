# Jcble_mam

[简体中文](README.zh-CN.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

`jcble-mam` is a general-purpose Codex skill for building and operating company content operations, copywriting workflows, online marketing promotion, and multi-Agent collaboration teams.

Supported Markdown languages:

- Simplified Chinese `zh-CN`
- English `en`
- Spanish `es`
- Japanese `ja`
- Korean `ko`

## Use Cases

- Company document management
- Solution planning and proposal writing
- Social media topic planning
- Company and solution PPT planning
- Product copywriting
- Product, solution, and promotional visual briefs
- Global market intelligence
- Industry-news tracking
- Overseas customer discovery
- Outreach email drafts
- Weekly and monthly content, platform, and lead retrospectives
- Persistent multi-Agent Codex session setup
- Multilingual Markdown creation, translation, and localization

## Skill Name

The installable skill name is:

```text
jcble-mam
```

`Jcble_mam` is kept as the display name and user-facing alias. The workflow is generic and can be adapted to any company.

## Install

Clone this repository into a Codex skills directory:

```bash
git clone https://github.com/Mecil9/jcble-mam.git ~/.agents/skills/jcble-mam
```

Then start a new Codex session so the skill registry can refresh.

## Configuration

Before using the skill, adapt these placeholders to your own workspace:

```text
COMPANY_WORKSPACE=/path/to/company/workspace
COMPANY_KNOWLEDGE_BASE=/path/to/company/knowledge-base
COMPANY_MARKETING_WORKSPACE=/path/to/company/content-marketing-workspace
```

If your company uses different directory names, update the reference files or create equivalent index files.

## Main Files

- `SKILL.md` - trigger conditions and core workflow
- `references/agent-team-roles.md` - multi-Agent role library
- `references/session-orchestration.md` - Codex thread creation, naming, synchronization, and message routing
- `references/company-material-boundaries.md` - company material boundaries and sensitive-data rules
- `references/multilingual-workflow.md` - multilingual Markdown rules, localization boundaries, and review checklist
- `assets/task-card-template.md` - task-card template
- `assets/message-template.md` - message-bus template
- `assets/retrospective-template.md` - weekly/monthly retrospective template

## Safety Notes

Before publishing externally:

- remove confidential customer, contract, finance, payroll, credential, and personal data
- verify all public claims against approved source files
- keep outreach emails as drafts until human approval
- do not represent generated visuals as real products, real sites, or real customer scenes

## License

MIT
