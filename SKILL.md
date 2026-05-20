---
name: EmaoNovel
description: 小说创作助手，写小说、码字、网文写作、轻小说创作都用得上。帮你整理角色设定和世界观、初始化小说项目、批量修订小说内容（把XX改成YY）、继续上次写作、归档素材、管理剧情大纲。也适用于需要Git版本管理的创作场景。典型触发：整理这些设定、初始化小说项目、把门派改成学院、继续上次写、今天先到这、帮我归档世界观、写角色设定、修订大纲。
user-invocable: true
version: 1.0.0
metadata:
  openclaw:
    requires:
      bins: ["git"]
    os: ["darwin", "linux", "win32"]
---

# 基于 Git 的小说创作工作流

## 概述

以 Git 为版本管理核心、AI 助手为执行层的小说创作工作流。作者负责"写什么"，AI 负责"怎么存"。

## 任务目标

- 本 Skill 用于：小说创作项目的高效管理与迭代
- 能力包含：原始素材归档、四类设定文件生成、Git 版本管理、批量修订、断点续写
- 触发条件：开始新项目、口述设定、整理角色、修订正文

## 执行方式

触发本技能后，按顺序加载以下资源并执行：

1. 读取 [references/workflow.md](references/workflow.md) — 完整执行流程：项目初始化、素材整理、写作、续写、修订、存档的操作指南
2. 读取 [references/rules.md](references/rules.md) — 规则引擎：规则架构、加载优先级、冲突处理、文风分析的执行规范
3. 按需读取 [references/usage-examples.md](references/usage-examples.md) — 典型场景示例
4. 按需读取 [references/templates/](references/templates/) — 规则与设定模板

## 资源索引

| 文件 | 内容 |
|------|------|
| [references/workflow.md](references/workflow.md) | 工作流程、命令参考、意图映射表 |
| [references/rules.md](references/rules.md) | 规则引擎详解、commit 规范 |
| [references/usage-examples.md](references/usage-examples.md) | 典型使用场景 |
| [references/templates/](references/templates/) | 全套规则模板（总规则、版本管理、结构、内容、禁止词库等） |
