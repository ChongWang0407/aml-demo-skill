# aml-demo-skill

AI Muse Lab 专属的 Apple 风格 + Liquid Glass 前端 Demo 工作流 Skill。

这个仓库本身就是一个可下载的 Agent Skill：根目录包含 SKILL.md，其他文件是 UI 元数据和工作流参考。

## 用途

把一个模糊的产品想法快速变成适合给 mentor 展示的前端 Demo：

1. 澄清产品决策、受众、页面范围和展示约束。
2. 整理一份体现 Apple 设计特征的 Liquid Glass 设计方案，并等待确认。
3. 在同一内容和功能范围内制作 2–3 个轻量风格变体。
4. 让用户选择或组合一个方向，再确认关键细节和动效。
5. 完成选定方向、可访问性、响应式和 reduced-motion 检查。

提问数量是自适应的：需求完整时可以不追问；存在关键缺口时才继续提问，直到对意图和偏好达到约 95% 的把握。

## 在 Codex 中调用

直接使用：

$aml-demo-skill Create a mentor-ready frontend demo for <your product idea>. Use Apple style and Liquid Glass.

正在进行的流程可以继续：

$aml-demo-skill Continue the current demo from the last approved direction.

## 支持的底层 Skill

- apple-design：Apple 的层级、排版、材质、触控反馈和克制原则。
- prototype：在一个切换器中制作真正不同的 2–3 个初版方向。
- simple-liquid-glass：Liquid Glass 材质、折射、交互和降级方案。
- animate：在用户选定方向后决定并实现有目的的动效。
- 可用时自动路由 frontend builder 和 frontend testing/debugging Skill。

这些底层 Skill 需要安装在调用方环境中；本 Skill 会自动按阶段路由，不要求用户逐个调用。

## 直接下载与安装

仓库地址：

https://github.com/ChongWang0407/aml-demo-skill

主文件原始下载地址：

https://raw.githubusercontent.com/ChongWang0407/aml-demo-skill/main/SKILL.md

最通用的安装方式是克隆到 Codex 的用户 Skill 目录：

    git clone https://github.com/ChongWang0407/aml-demo-skill.git ~/.codex/skills/aml-demo-skill

也可以下载仓库 ZIP 后，将整个目录放入你的 Agent Skills 目录；请确保 SKILL.md 位于该 Skill 目录的根部。使用支持 GitHub 仓库路径的 Skill 安装器时，填写：

    ChongWang0407/aml-demo-skill

## 仓库结构

- SKILL.md：Skill 主指令。
- agents/openai.yaml：Codex 的展示名称、快捷提示和隐式调用策略。
- references/discovery-and-brief.md：澄清问题和设计 brief 模板。
- references/prototype-and-finish.md：初版对比、动效预算和最终 QA 约定。

## 安全边界

这是公开仓库，只包含工作流指令和参考文档，不包含账号密码、Token、业务数据或私有素材。后续修改 Skill 时请继续保持这一边界。
