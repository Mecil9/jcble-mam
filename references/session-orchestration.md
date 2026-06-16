# Company Content Marketing Session Orchestration

Use this guide when creating, renaming, synchronizing, or coordinating independent Codex sessions for a company content and marketing Agent team.

## Required Thread Tools

Load Codex thread tools through `tool_search` when they are not already available. Search for:

```text
create_thread set_thread_title send_message_to_thread list_threads read_thread
```

Use:

- `create_thread` to create user-owned persistent role sessions.
- `set_thread_title` to enforce naming.
- `send_message_to_thread` to assign or synchronize work.
- `list_threads` to verify titles and statuses.
- `read_thread` to inspect recent status if needed.

## Thread Naming

Name threads with this exact pattern:

```text
<CompanyOrTeamName>-<Role>Agent
```

Default long-running roles:

- CompanyContent-主控总编Agent
- CompanyContent-文档管理Agent
- CompanyContent-方案策划Agent
- CompanyContent-方案写作Agent
- CompanyContent-文案写作Agent
- CompanyContent-自媒体选题Agent
- CompanyContent-产品文案Agent
- CompanyContent-PPT制作Agent
- CompanyContent-视觉设计Agent
- CompanyContent-市场情报Agent
- CompanyContent-行业新闻Agent
- CompanyContent-客户挖掘Agent
- CompanyContent-邮件触达Agent
- CompanyContent-复盘分析Agent
- CompanyContent-审核合规Agent

## Creation Procedure

1. Read existing session index if present:
   `COMPANY_MARKETING_WORKSPACE/agent-sessions/00.agent-session-index.md`
2. Reuse existing threads when the requested team already exists and thread IDs are valid.
3. Create missing threads using the local company project target when possible.
4. Send each new thread a role-specific initialization prompt:
   - State the role.
   - State the working language: `zh-CN`, `en`, `es`, `ja`, or `ko`.
   - Use Simplified Chinese by default when no language is specified.
   - Require reading `COMPANY_WORKSPACE/AGENTS.md` or equivalent workspace instructions when available.
   - Require reading the company team manual, session index, message bus, and collaboration protocol.
   - Say not to change files and not to execute business tasks during initialization.
   - Require a one-line readiness reply.
5. Rename each thread with `set_thread_title`.
6. Write thread IDs into the session index.
7. Send a synchronization message after all IDs are written so each thread can read the updated index.
8. Verify with `list_threads` and the local session-index file.

## Communication Model

Do not claim that Codex threads automatically listen to each other. Explain this operational model:

- Main editor or 主控总编 sends explicit messages to role threads.
- Role threads respond in their own sessions.
- Role threads use the task's target language for deliverables and status replies unless the assignment says otherwise.
- Persistent collaboration state is recorded in the local message bus.
- The 主控总编 Agent tracks open, acknowledged, done, and blocked messages.

## Message Bus Location

Use:

```text
COMPANY_MARKETING_WORKSPACE/agent-sessions/01.message-bus.md
```

Use this message format:

```markdown
## MSG-YYYYMMDD-HHMM-序号

- 状态：open / acknowledged / done / blocked
- 发件 Agent：
- 收件 Agent：
- 抄送：
- 关联任务：
- 目标语言：zh-CN / en / es / ja / ko
- 优先级：高 / 中 / 低
- 截止时间：
- 请求：
- 输入资料：
- 期望输出：
- 回复：
- 处理记录：
```

## Assignment Prompt Template

```text
按公司文案与市场推广团队协作协议处理以下子任务。

角色：
关联任务：
目标语言：
目标：
输入资料：
禁止使用资料：
输出格式：
截止时间：
验收标准：

只处理本角色职责范围内的内容。需要其它 Agent 协助时，说明要发给谁、需要什么。
```
