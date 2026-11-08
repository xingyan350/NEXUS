# NEXUS 团队协作规范

## 基本原则

- 三位成员都可以参与程序、关卡、剧情、测试和设计讨论。
- 项目负责人负责协调架构与集成，不意味着其他成员不能提交代码。
- 开始任务前先确认负责人、交付内容和验收标准。
- 不要把尚未讨论确定的设计当作正式设定。

## 分支建议

- `main`：保持可运行，尽量只通过 Pull Request 合并。
- `feature/<topic>`：新功能，例如 `feature/player-movement`。
- `fix/<topic>`：问题修复，例如 `fix/weapon-reload`。
- `docs/<topic>`：文档修改，例如 `docs/story-outline`。

## 提交规范

建议使用简短、明确的提交信息：

- `feat: add player movement`
- `fix: correct hit detection`
- `docs: update story outline`
- `art: add infected character sprites`
- `refactor: split weapon controller`

## Pull Request 检查

提交 PR 前：

1. 确认项目可以在团队约定的 Godot 版本中打开。
2. 检查是否误提交缓存、导出文件或个人配置。
3. 说明改动目的、主要文件和测试方式。
4. 涉及玩法或剧情的改动，更新对应设计文档。
5. 至少由另一位成员检查后再合并。

## Godot 资源协作

- 场景、脚本和资源使用清晰且稳定的文件名。
- 避免多人同时编辑同一个大型场景文件。
- 修改共享资源前先同步团队。
- 不要随意移动或重命名已被场景引用的资源。
- 资源导入设置和项目配置变更需要在 PR 中说明。

## Definition of Done

一个任务只有在实现、基本测试、必要文档更新和代码审查完成后，才算完成。
