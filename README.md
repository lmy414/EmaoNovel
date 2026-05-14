# novel-writing-workflow

基于 Git + GitHub 的小说创作版本管理技能。作者自然对话即触发，AI 负责执行层。

## 触发方式

投喂设定 / 整理项目 / 修订设定 / 续写正文 / 搁置存档——在对话中自然说出意图即可。

## 核心流程

1. 用户触发 → 检查项目文件夹
2. 新项目 → 初始化完整目录结构 → 读取素材归档
3. 已有项目 → 优先读取 `.rules/` → 按规则执行用户指令
4. 每次修改自动 commit + push，永久可回溯

## 文件结构

```
novel-writing-workflow/
├── SKILL.md
└── references/
    ├── rules.md
    ├── workflow.md
    ├── usage-examples.md
    └── templates/
```

## 安装

将 `.skill` 文件放入 `~/.openclaw/plugin-skills/`。
