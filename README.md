# Corgi IP Illustrations

> 16:9 横版 | 个人柯基 IP | 纯白手绘 | 少量红橙蓝中文批注 | Codex Skill

这是一个本地定制版 Codex Skill，用来为中文文章、帖子、博客、Notion 文档、方法论和工作流内容生成正文配图。

它从 `helloianneo/ian-xiaohei-illustrations` 派生，保留原项目的正文配图工作流、构图方法和 QA 思路，把默认角色替换为个人橙白柯基 IP。

## 核心变化

- skill 名：`corgi-ip-illustrations`
- 默认角色：橙白柯基 IP
- 参考图：`corgi-ip-illustrations/assets/ip-reference/`
- 核心风格：纯白背景、正文插画感、清爽手绘、萌系亲和、大量留白、少量红橙蓝中文手写批注
- 固定角色约束：橙白柯基 IP 没有尾巴
- 禁止方向：3D 渲染、纯贴纸表情包、低幼儿童卡通、宠物写真、PPT 信息图

## 本地安装

复制 skill 主目录到 Codex skills 目录：

```bash
cp -R ./corgi-ip-illustrations "${CODEX_HOME:-$HOME/.codex}/skills/"
```

安装后重启 Codex。

## 使用示例

```text
Use $corgi-ip-illustrations 为这篇中文文章设计并生成 4 张柯基 IP 正文配图。
```

```text
Use $corgi-ip-illustrations 先不要生图，先给这篇文章做配图策略。
每张图写清楚：放在哪段后、主题、核心意思、结构类型、柯基在做什么、建议中文标注词。
```

## 目录

```text
corgi-ip-illustrations/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── assets/
│   └── ip-reference/
│       ├── corgi-front.png
│       ├── corgi-elegant.png
│       └── corgi-online.png
└── references/
    ├── composition-patterns.md
    ├── corgi-ip.md
    ├── prompt-template.md
    ├── qa-checklist.md
    └── style-dna.md
```

## 发布前检查

- 确认测试图已经通过 QA。
- 确认 README、NOTICE、示例提示词不再残留旧 skill 名。
- 确认 Git 远程地址指向自己的仓库。
- 不自动 push，等明确指令后再发布。
