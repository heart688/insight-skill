# Paper Storytelling · 论文故事

让读者理解真实问题、记住核心 insight，并看懂方法与证据怎样回应它。

这是一套可跨研究领域使用的 Agent Skill，用于论文故事梳理、章节改写和逻辑审读。

## 它解决什么

- **问题可信：** 说明任务需要什么、现有做法依赖什么，以及真实约束为何带来困难。
- **Insight 清楚：** 从核心矛盾提炼可理解、可检验的判断。
- **记忆点统一：** 用稳定术语贯穿摘要、引言、相关工作、方法、实验和结论。
- **方法自然：** 让设计从约束和信息需求中逐步出现。
- **证据闭环：** 用关键对照检验同一个核心判断，并保留结论范围。

## 开始使用

入口是 [SKILL.md](SKILL.md)。提供当前稿件、真实方法和结果，再说明需要故事框架、审读意见还是原位修改。

```text
使用 $paper-storytelling 审读这篇论文。
先确定真实问题、核心矛盾和 insight，再检查方法与实验是否持续回应它。
用稳定术语强化核心记忆点。
先列出具体修改位置和建议，暂不修改原文。
```

## 安装

在 Codex 中首次安装：

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/heart688/insight-skill.git ~/.codex/skills/paper-storytelling
```

其他支持 Agent Skills 的工具可按其安装方式使用。与其他写作 AI 配合时，提供 `SKILL.md` 及它链接的相关参考文件。此 skill 为纯文本，无需安装运行时依赖。

## 内容

```text
SKILL.md
agents/openai.yaml
references/
├── problem-insight-memory.md
├── section-patterns.md
├── story-review.md
└── top-conference-patterns.md
```

- [问题、insight 与记忆点](references/problem-insight-memory.md)：核心矛盾、问题依据、固定术语和全文贯穿。
- [章节写作模式](references/section-patterns.md)：从问题到方法、实验与结论的递进。
- [故事审读](references/story-review.md)：检查读者能否记住问题、认识和最强证据。
- [十篇公开论文的论证分析](references/top-conference-patterns.md)：比较不同贡献类型的写法，附来源与版本。

## 原则

先让问题成立，再提出 insight。核心术语保持稳定，每次复现承担新的论证任务。结构随贡献类型调整，真实方法、协议和结果决定结论范围。

需要进一步组织实验部分时，可配合使用[论文实验写作 skill](https://github.com/heart688/exp-skill)。
