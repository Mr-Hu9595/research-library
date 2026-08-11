# 调研成果库系统（Research Library）

> Research Library — 让每次调研都变成项目可复用资产的 Claude Code Skill

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

项目做调研最大的浪费不是"没调研"，而是**调研成果散落在对话和文档里、重复调研、结论没人消费**。

这套系统把调研做成**标准化 + 资产化**的流程：

- **先查后研**：调研前查索引，已有结论直接复用，防重复调研
- **结论优先**：每条调研产出明确推荐 + 可落地清单，不是过程堆砌
- **模式提炼**：找"架构/功能类似"项目（不要求用途一致）提炼可复用模式
- **统一索引**：5 要素索引（主题/日期/路径/结论/决策状态/落地引用/未消费清单），一眼可查
- **闭环可查**：哪些结论落地了、哪些没有，索引即答案

## 核心原则

1. **先查后研** —— 调研前查索引，防重复、可复用
2. **结论优先** —— 推荐 + 可落地清单给到位
3. **模式提炼 > 项目罗列** —— 找架构类似项目提炼模式，不抄名
4. **沉淀入库** —— 标准报告 + 5 要素索引回填
5. **闭环可查** —— 决策状态 + 落地引用 + 未消费清单

## 快速开始

1. 在项目建 `docs/research/`（INDEX.md + 报告 + README）
2. 每次调研走五步流程（见 SKILL.md）：先查后研 → 定目标范围 → 多源执行 → 提炼结论 → 沉淀入库
3. 落地任务完成后，回填索引的「落地引用」列

## 目录结构

```
docs/research/
├── INDEX.md                  # 调研索引（5 要素，SSOT 入口）
├── <YYYY-MM-DD>-<主题>.md    # 调研报告（标准结构）
└── README.md                 # 三库分类说明 + 使用方式
```

## 安装

```bash
# 克隆到 Claude Code 全局 skills 目录
git clone https://github.com/Mr-Hu9595/research-library.git ~/.claude/skills/research-library
```

## 开源

MIT License。欢迎使用、改进、提 PR。

## 与 pm-vs-ai-ssot 的关系

- [pm-vs-ai-ssot](https://github.com/Mr-Hu9595/pm-vs-ai-ssot)：管"任务与协作留痕"（PM 调度 AI 执行者的文档体系）
- **research-library**：管"调研资产与决策反哺"（调研标准化 + 成果库 + 闭环）
- 两者正交、可互相引用：调研库索引可作为 SSOT 项目知识库的一部分；但调研库**不依赖** PM-AI 协作模式，任何项目通用
