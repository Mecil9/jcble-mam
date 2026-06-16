---
name: jcble-mam
description: This skill should be used for company content operations, copywriting assistant workflows, online market promotion, and multi-Agent marketing team setup. Use it when creating or running a reusable company content and marketing Agent team, building independent Codex role sessions, coordinating document management, solution writing, product copy, PPT work, visual briefs, market research, customer discovery, email outreach drafts, and weekly or monthly performance reviews.
---

# Jcble_mam

## Overview

Operate a company's content, copywriting, and online market-promotion Agent team. Create and coordinate a reusable multi-Agent system for document management, solution planning, content production, product copy, PPT preparation, visual design briefs, market intelligence, industry-news tracking, customer discovery, outreach email drafting, review checks, and platform-data retrospectives.

## When To Use

Use this skill when the task asks to:

- Create or update a company content, marketing, or copywriting Agent team.
- Build independent Codex sessions for role Agents and name those sessions.
- Coordinate multiple writing, solution, market, visual, email, or review Agents.
- Produce task cards, evidence packs, content drafts, customer outreach drafts, or weekly/monthly review outputs.
- Set up or maintain an Agent session index, message bus, and collaboration protocol.

## First Checks

Before planning or writing:

1. Read `COMPANY_WORKSPACE/AGENTS.md` or equivalent workspace instructions when available.
2. Read `COMPANY_WORKSPACE/00.company-material-index.md` or equivalent company-material index when company material, solutions, products, market work, or business planning is involved.
3. Read `COMPANY_MARKETING_WORKSPACE/01.company-content-marketing-team-manual.md` when an existing team manual exists.
4. Read the session index and communication files when coordinating existing Agents:
   - `COMPANY_MARKETING_WORKSPACE/agent-sessions/00.agent-session-index.md`
   - `COMPANY_MARKETING_WORKSPACE/agent-sessions/01.message-bus.md`
   - `COMPANY_MARKETING_WORKSPACE/agent-sessions/02.collaboration-protocol.md`

## Core Workflow

1. Classify the request as one of three output types: internal management, external-facing content, or technical/product material.
2. Define the task card: objective, audience, channel, output format, required sources, forbidden sources, deadline, and approval owner.
3. Build an evidence pack before drafting. Mark each source as public, internal, restricted, or forbidden.
4. Select the minimum necessary Agents from the role library in `references/agent-team-roles.md`.
5. For persistent multi-Agent work, create or reuse independent Codex threads using `references/session-orchestration.md`.
6. Coordinate through the main editor Agent plus the shared message bus. Do not assume threads automatically monitor each other.
7. Route drafts through review before external use. Require human approval for publishing, email sending, customer-list export, customer-case claims, and pricing.
8. Archive the task card, evidence pack, draft, review notes, final output, and retrospective.

## Session Setup Workflow

When asked to create independent Agent sessions:

1. Search for Codex thread tools with `tool_search` using terms such as `create_thread set_thread_title send_message_to_thread list_threads`.
2. Create one thread per role using the local company project target when available.
3. Name every thread with the pattern `<CompanyOrTeamName>-<Role>Agent`.
4. Write every thread ID into the session index.
5. Send each thread an initialization prompt that says to read the company rules, role index, message bus, and collaboration protocol, then stay idle until assigned.
6. Explain that cross-thread work is coordinated by explicit messages and the shared message bus, not by automatic always-on listening.

Load `references/session-orchestration.md` before creating or updating threads.

## Safety Boundaries

- Treat payroll, equity, banking, contracts, quotes, invoices, credentials, personal resumes, private customer details, and raw financial worksheets as internal or forbidden by default.
- Use only approved public-safe materials for websites, social posts, sales decks, product brochures, public cases, and overseas outreach.
- Preserve company files. Do not move, rename, delete, deduplicate, or bulk-edit historical documents unless explicitly asked.
- Separate facts, interpretation, and recommended action in internal outputs.
- Cite source file paths and dates or versions for product parameters, customer names, case results, certifications, prices, and market claims.
- Draft emails only. Send no email and export no customer list without explicit human approval.

## Resources

- `references/agent-team-roles.md` - Role library, responsibilities, outputs, and acceptance criteria.
- `references/session-orchestration.md` - Independent Codex thread creation, naming, synchronization, and communication workflow.
- `references/company-material-boundaries.md` - Company source map, evidence rules, and sensitive-data boundaries.
- `assets/task-card-template.md` - Task-card template for new work.
- `assets/message-template.md` - Message-bus entry template.
- `assets/retrospective-template.md` - Weekly/monthly review template.
