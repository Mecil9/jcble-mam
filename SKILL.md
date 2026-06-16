---
name: jcble-mam
description: This skill should be used for JCBLE company management, copywriting assistant operations, online market promotion, and multi-Agent content team setup. Use it when creating or running the Jcble_mam Agent team, building independent Codex role sessions, coordinating document management, solution writing, product copy, PPT work, visual briefs, global market research, customer discovery, email outreach drafts, and weekly or monthly performance reviews.
---

# Jcble_mam

## Overview

Operate JCBLE's management, copywriting, and online market-promotion Agent team. Create and coordinate a reusable multi-Agent system for document management, solution planning, content production, product copy, PPT preparation, visual design briefs, market intelligence, industry-news tracking, overseas customer discovery, email outreach drafting, review checks, and platform-data retrospectives.

## When To Use

Use this skill when the task asks to:

- Create or update the JCBLE content, management, marketing, or copywriting Agent team.
- Build independent Codex sessions for JCBLE role Agents and name those sessions.
- Coordinate multiple JCBLE writing, solution, market, visual, email, or review Agents.
- Produce JCBLE task cards, evidence packs, content drafts, customer outreach drafts, or weekly/monthly review outputs.
- Set up or maintain the JCBLE Agent session index, message bus, and collaboration protocol.

## First Checks

Before planning or writing:

1. Read `JCBLE_WORKSPACE/AGENTS.md`.
2. Read `JCBLE_WORKSPACE/00.JCBLE资料库-Obsidian关联索引.md` when company material, solutions, products, market work, or business planning is involved.
3. Read `JCBLE_WORKSPACE/08.团队管理/JCBLE文案团队/01.JCBLE文案团队运行手册.md` when it exists.
4. Read the session index and communication files when coordinating existing Agents:
   - `JCBLE_WORKSPACE/08.团队管理/JCBLE文案团队/07.Agent会话与消息总线/00.Agent会话索引.md`
   - `JCBLE_WORKSPACE/08.团队管理/JCBLE文案团队/07.Agent会话与消息总线/01.消息总线.md`
   - `JCBLE_WORKSPACE/08.团队管理/JCBLE文案团队/07.Agent会话与消息总线/02.协作协议.md`

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
2. Create one thread per role using the local JCBLE project target when available.
3. Name every thread with the pattern `JCBLE文案团队-<角色>Agent`.
4. Write every thread ID into the session index.
5. Send each thread an initialization prompt that says to read the JCBLE rules, role index, message bus, and collaboration protocol, then stay idle until assigned.
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
- `references/jcble-material-boundaries.md` - JCBLE source map, evidence rules, and sensitive-data boundaries.
- `assets/task-card-template.md` - Task-card template for new work.
- `assets/message-template.md` - Message-bus entry template.
- `assets/retrospective-template.md` - Weekly/monthly review template.
