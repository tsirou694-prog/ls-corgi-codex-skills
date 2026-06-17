# Corgi IP Illustrations 目录规范

## 定位

这是从 `ian-xiaohei-illustrations` 派生的本地定制版仓库，用于沉淀个人柯基 IP 的中文正文配图 skill。

## 结构

- `corgi-ip-illustrations/`：Codex 可安装的 skill 主目录。
- `corgi-ip-illustrations/SKILL.md`：skill 触发说明和工作流。
- `corgi-ip-illustrations/references/`：风格、IP、构图、提示词和 QA 规则。
- `corgi-ip-illustrations/assets/ip-reference/`：个人 IP 原始参考图，只作风格识别和提示词校准。
- `examples/`：示例图和示例提示词，发布前按实际测试结果再更新。

## 命名

- skill 名使用英文小写短横线：`corgi-ip-illustrations`。
- 生成图片按 `01-topic-name.png` 命名。
- 参考文件使用英文名，正文说明可以用中文。

## 清理

- 临时测试图、失败图、截图放到任务临时目录，确认无用后清理。
- 不把密钥、账号信息、未公开个人隐私写进仓库。
- 发布 GitHub 前先检查 README、NOTICE、示例和远程仓库地址。

## Git

- 本地可以修改和测试。
- 不自动 `git push`。
- 测试成功并得到明确指令后，再绑定用户自己的 GitHub 仓库。
