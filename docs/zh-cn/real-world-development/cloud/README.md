---
slug: zh-cn/real-world-development/cloud
title: "GitHub Copilot 云端智能体"
authors:
  - geektrainer
lastUpdated: 2026-06-30
---

**[GitHub Copilot 云端智能体](https://docs.github.com/copilot/concepts/agents/cloud-agent/about-cloud-agent)** 可让 GitHub Copilot 在云端异步工作。你可以在 GitHub 上分配任务，云端智能体会在后台处理：探索仓库、进行更改并创建拉取请求，让你可以继续处理其他事务。

在这些练习中，你将添加云端智能体要遵循的自定义指令，然后分配一个 GitHub issue，让它实现相应工作。你将审查并使用自定义智能体来调整它的工作方式，在智能体仪表板中监控并引导会话，最后审查它创建的拉取请求并迭代改进结果。

## 练习

| 练习 | 主题 | 说明 |
|----------|-------|-------------|
| [0. 准备工作][ex0] | 设置 | 创建仓库和 Codespace |
| [1. 自定义指令][ex1] | 上下文 | 添加云端智能体要遵循的自定义指令 |
| [2. 云端智能体][ex2] | 异步智能体 | 将 issue 分配给 GitHub Copilot 云端智能体 |
| [3. 自定义智能体][ex3] | 专业智能体 | 审查并使用自定义智能体 |
| [4. 管理智能体][ex4] | 监控 | 监控并引导智能体会话 |
| [5. 迭代改进][ex5] | 审查 | 审查拉取请求、迭代改进 Copilot 的工作并选择后续步骤 |

## 准备工作

参加此 workshop 前，请确保你具备以下条件：

- [ ] 拥有有效的 **Copilot Student、Pro、Pro+、Business 或 Enterprise** 计划的 GitHub 帐户
- [ ] 已为你的帐户或组织启用 GitHub Copilot 云端智能体

> [!TIP]
> 没有付费计划？通过验证的学生可以从 [GitHub Education][callout-student-plan-education] 免费获取 GitHub Copilot。**Copilot Student** 计划包含此 workshop 使用的智能体、MCP、代码审查和 Copilot CLI 功能，因此可以用它完成所有开发环境中的练习。

[callout-student-plan-education]: https://github.com/education/students

> [!NOTE]
> 云端智能体适用于 **Copilot Student、Pro、Pro+、Business 和 Enterprise** 计划，Copilot Free 除外。对于 Copilot Business 或 Enterprise，管理员必须为组织启用该功能。

> [!NOTE]
> 此开发环境不介绍 MCP。若要了解如何将 MCP 服务器与 Copilot 配合使用，请参阅 [CLI 开发环境][cli]或 [VS Code 开发环境][vscode]。

## 开始

**[从练习 0：准备工作开始 →][ex0]**

[ex0]: 0-prerequisites/
[ex1]: 1-custom-instructions/
[ex2]: 2-cloud-agent/
[ex3]: 3-custom-agents/
[ex4]: 4-managing-agents/
[ex5]: 5-iterating/
[cli]: ../cli/
[vscode]: ../vscode/
