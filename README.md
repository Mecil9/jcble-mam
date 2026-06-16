# Jcble_mam

`jcble-mam` is a Codex skill for building and operating a general company content, copywriting assistant, and online market-promotion Agent team.

It packages a reusable workflow for:

- company document management
- solution planning and proposal writing
- social media topic planning
- company and solution PPT planning
- product copywriting
- product, solution, and promotional visual briefs
- global market intelligence
- industry-news tracking
- overseas customer discovery
- outreach email drafting
- weekly and monthly content or funnel retrospectives
- persistent multi-Agent Codex session setup

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

The references describe recommended files and folders. If a company uses different names, update the reference files or create equivalent index files.

## Main Files

- `SKILL.md` - trigger conditions and core workflow
- `references/agent-team-roles.md` - multi-Agent role library
- `references/session-orchestration.md` - Codex thread creation, naming, synchronization, and message routing
- `references/company-material-boundaries.md` - company material source map and sensitive-data boundaries
- `assets/task-card-template.md` - reusable task card
- `assets/message-template.md` - message-bus entry template
- `assets/retrospective-template.md` - weekly/monthly review template

## Safety Notes

This skill is designed for internal company workflows. Before sharing outputs externally:

- remove confidential customer, contract, finance, payroll, credential, and personal data
- verify all public claims against approved source files
- keep email outreach as drafts until human approval
- do not represent generated visuals as real field photos or real products

## License

MIT
