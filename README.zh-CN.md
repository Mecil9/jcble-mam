# Jcble_mam

[English](README.md) | 简体中文 | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

`jcble-mam` 是一个面向 Codex 的 skill，用于公司内容运营、文案工作流、线上市场推广和多 Agent 会话协作。

它可以让 Codex 像一个协同的内容与市场团队一样工作，覆盖文档管理、方案写作、产品文案、自媒体选题、视觉设计简报、市场调研、客户寻找、邮件触达草稿，以及周报/月报复盘。

## 主要能力

- 创建可复用的公司内容与市场推广 Agent 团队。
- 定义主控总编、文档管理、方案策划、文案写作、产品文案、PPT 制作、视觉设计、市场情报、客户挖掘、邮件触达、审核合规和复盘分析等角色。
- 支持持久化 Codex 角色会话和消息总线协作流程。
- 支持简体中文、英文、西班牙语、日语、韩语 Markdown 输出。
- 对外内容必须基于已批准证据，并保留人工审核边界。

## Codex 安装方式

把这个仓库克隆到 Codex skills 目录：

```bash
git clone https://github.com/Mecil9/jcble-mam.git ~/.agents/skills/jcble-mam
```

然后开启一个新的 Codex 会话，让 skill 注册表刷新。

如果你的 Codex 使用不同的 skills 目录，把仓库克隆到对应目录，并保持文件夹名称为：

```text
jcble-mam
```

## 使用方法简介

安装后，直接用自然语言让 Codex 调用。示例：

```text
使用 jcble-mam 为我的公司创建一个内容与市场推广 Agent 团队。
```

```text
使用 jcble-mam 把这份产品资料改写成官网文案和邮件触达草稿。
```

```text
使用 jcble-mam 创建主控总编、文案、市场情报、视觉设计和审核 Agent 的独立 Codex 会话。
```

```text
使用 jcble-mam 把这份方案摘要写成英文、西班牙语、日语和韩语版本。
```

## 工作区配置

在使用公司资料前，把这些占位路径映射到你自己的工作区：

```text
COMPANY_WORKSPACE=/path/to/company/workspace
COMPANY_KNOWLEDGE_BASE=/path/to/company/knowledge-base
COMPANY_MARKETING_WORKSPACE=/path/to/company/content-marketing-workspace
```

如果你的公司使用不同目录名称，可以更新 reference 文件，或创建等价索引文件。

## 包含文件

- `SKILL.md` - 触发条件和核心工作流
- `references/agent-team-roles.md` - 多 Agent 角色库
- `references/session-orchestration.md` - Codex 会话创建、命名、同步和消息路由
- `references/company-material-boundaries.md` - 公司资料边界和敏感数据规则
- `references/multilingual-workflow.md` - 多语言 Markdown 规则、本地化边界和检查清单
- `assets/task-card-template.md` - 任务单模板
- `assets/message-template.md` - 消息总线模板
- `assets/retrospective-template.md` - 周报/月报复盘模板

## 安全说明

对外发布或发送前：

- 删除客户、合同、财务、工资、凭证、个人资料等敏感信息
- 用已批准资料核对所有公开声明
- 邮件触达只生成草稿，发送前必须人工确认
- 不要把生成图片描述成真实产品、真实现场或真实客户场景

## License

MIT
