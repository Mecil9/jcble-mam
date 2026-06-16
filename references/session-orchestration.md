# JCBLE Session Orchestration

Use this guide when creating, renaming, synchronizing, or coordinating independent Codex sessions for the JCBLE Agent team.

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
JCBLE文案团队-<角色>Agent
```

Default long-running roles:

- JCBLE文案团队-主控总编Agent
- JCBLE文案团队-文档管理Agent
- JCBLE文案团队-方案策划Agent
- JCBLE文案团队-方案写作Agent
- JCBLE文案团队-文案写作Agent
- JCBLE文案团队-自媒体选题Agent
- JCBLE文案团队-产品文案Agent
- JCBLE文案团队-PPT制作Agent
- JCBLE文案团队-视觉设计Agent
- JCBLE文案团队-市场情报Agent
- JCBLE文案团队-行业新闻Agent
- JCBLE文案团队-全球客户挖掘Agent
- JCBLE文案团队-邮件触达Agent
- JCBLE文案团队-复盘分析Agent
- JCBLE文案团队-审核合规Agent

## Creation Procedure

1. Read existing session index if present:
   `JCBLE_WORKSPACE/08.团队管理/JCBLE文案团队/07.Agent会话与消息总线/00.Agent会话索引.md`
2. Reuse existing threads when the requested team already exists and thread IDs are valid.
3. Create missing threads using the local JCBLE project target when possible.
4. Send each new thread a role-specific initialization prompt:
   - State the role.
   - Require Chinese by default.
   - Require reading `JCBLE_WORKSPACE/AGENTS.md`.
   - Require reading the JCBLE team manual, session index, message bus, and collaboration protocol.
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
- Persistent collaboration state is recorded in the local message bus.
- The 主控总编 Agent tracks open, acknowledged, done, and blocked messages.

## Message Bus Location

Use:

```text
JCBLE_WORKSPACE/08.团队管理/JCBLE文案团队/07.Agent会话与消息总线/01.消息总线.md
```

Use this message format:

```markdown
## MSG-YYYYMMDD-HHMM-序号

- 状态：open / acknowledged / done / blocked
- 发件 Agent：
- 收件 Agent：
- 抄送：
- 关联任务：
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
按 JCBLE 文案团队协作协议处理以下子任务。

角色：
关联任务：
目标：
输入资料：
禁止使用资料：
输出格式：
截止时间：
验收标准：

只处理本角色职责范围内的内容。需要其它 Agent 协助时，说明要发给谁、需要什么。
```
