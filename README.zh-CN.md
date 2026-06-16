# Jcble_mam

[English](README.en.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

`jcble-mam` 是一个通用的 Codex skill，用于搭建和运行公司内容管理、文案助理、线上市场推广和多 Agent 协作团队。

支持的 Markdown 语言：

- 简体中文 `zh-CN`
- 英文 `en`
- 西班牙语 `es`
- 日语 `ja`
- 韩语 `ko`

## 适用场景

- 公司文档管理
- 方案策划与方案写作
- 自媒体选题
- 公司 PPT 和方案 PPT 制作
- 产品文案写作
- 产品图、方案图、宣传图的设计简报
- 全球市场信息收集
- 行业新闻追踪
- 海外客户寻找
- 邮件触达草稿
- 每周和每月内容、平台、线索数据复盘
- 持久化多 Agent Codex 会话搭建
- 多语言 Markdown 创建、翻译和本地化

## Skill 名称

可安装的 skill 名称是：

```text
jcble-mam
```

`Jcble_mam` 保留为显示名称和用户可见别名。工作流是通用版本，可适配任何公司。

## 安装

把仓库克隆到 Codex skills 目录：

```bash
git clone https://github.com/Mecil9/jcble-mam.git ~/.agents/skills/jcble-mam
```

然后开启新的 Codex 会话，让 skill 注册表刷新。

## 配置

使用前，把这些占位路径替换为自己的公司工作区：

```text
COMPANY_WORKSPACE=/path/to/company/workspace
COMPANY_KNOWLEDGE_BASE=/path/to/company/knowledge-base
COMPANY_MARKETING_WORKSPACE=/path/to/company/content-marketing-workspace
```

如果你的公司使用不同目录名称，可以更新 reference 文件，或创建等价的索引文件。

## 主要文件

- `SKILL.md` - 触发条件和核心工作流
- `references/agent-team-roles.md` - 多 Agent 角色库
- `references/session-orchestration.md` - Codex 会话创建、命名、同步和消息路由
- `references/company-material-boundaries.md` - 公司资料边界和敏感数据规则
- `references/multilingual-workflow.md` - 多语言 Markdown 规则、本地化边界和检查清单
- `assets/task-card-template.md` - 任务单模板
- `assets/message-template.md` - 消息总线模板
- `assets/retrospective-template.md` - 周报/月报复盘模板

## 安全说明

对外发布前：

- 删除客户、合同、财务、工资、凭证、个人资料等敏感信息
- 用已批准资料核对所有公开声明
- 邮件触达只生成草稿，发送前必须人工确认
- 不要把生成图片描述成真实产品、真实现场或真实客户场景

## License

MIT
