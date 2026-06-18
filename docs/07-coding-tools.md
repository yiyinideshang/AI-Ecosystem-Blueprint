# 07 · 编程 AI 专项图谱（专题）

> 编程是 L2-B 智能体最活跃、最成熟的子领域。本页按"运行形态"把主流编程 AI 拆成五类，给你一张选型全景图。
>
> 本篇为专题附录，建立在 [02 · L2 应用深度剖析](./02-l2-analysis.md) 之上。

---

## 一、为什么编程 AI 值得单列？

- **需求最刚性**：代码可验证、可测试，是智能体"自主执行"最理想的试验场。
- **形态最丰富**：从编辑器插件到云端工程师，跑通了多种产品形态。
- **演进最快**：GitHub Copilot 从补全（L2-A）一路长出 Agent Mode（L2-B），是 L2-A→L2-B 演进的活样本。

---

## 二、五大运行形态总览

| 形态 | 运行位置 | 核心特征 | 代表产品 |
| :--- | :--- | :--- | :--- |
| **① AI 原生 IDE** | 整窗编辑器 | AI 深度集成进编辑器内核 | Cursor、Windsurf、Trae |
| **② IDE 插件 / 扩展** | 嵌入现有 IDE | 以插件形式挂载到 VS Code/JetBrains | GitHub Copilot、Cline、Roo Code、Continue、Cody、Amazon Q Developer、Augment Code |
| **③ CLI 终端智能体** | 本地命令行 | 终端运行，直连文件系统与 git | Claude Code、Codex、OpenCode、Aider、Gemini CLI、Qwen Code |
| **④ 云端 SWE Agent** | 云端沙箱 | 全云端自主完成开发任务 | Devin、Codex（云端模式） |
| **⑤ 应用 / UI 生成器（Vibe Coding）** | 浏览器 | 自然语言直出可运行应用，面向非开发者 | Bolt.new、v0、Lovable、Replit Agent |

> 形态①②③ 对应 [02](./02-l2-analysis.md) 里的"本地终端型"，④ 对应"云端沙箱型"，⑤ 是面向终端用户的新分支。

---

## 三、逐类详解

### ① AI 原生 IDE

| 工具 | 厂商 | 开源 | 模型关系 | 说明 |
| :--- | :--- | :--- | :--- | :--- |
| **Cursor** | Anysphere | 否 | 第三方（多模型） | 该品类开创者，深度集成补全 + Agent |
| **Windsurf** | Codeium | 否 | 第三方（多模型） | Cursor 主要竞品，Cascade 智能体 |
| **Trae** | 字节跳动 | 否 | 第三方 | 字节系 AI 原生 IDE |

> 共性：把 AI 做进编辑器内核，而非外挂插件，体验最一体化，但需整体迁移编辑器。

### ② IDE 插件 / 扩展

| 工具 | 厂商 | 开源 | 模型关系 | 层级 | 说明 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **GitHub Copilot** | GitHub/微软 | 否 | 第三方（OpenAI 等） | L2-A→L2-B | 最主流；补全 + 聊天起家，现已有 Agent Mode |
| **Cline**（原 Claude Dev） | 开源社区 | 是 | 模型无关 | L2-B | VS Code 自主代理，社区极活跃 |
| **Roo Code**（原 Roo Cline） | 开源社区 | 是 | 模型无关 | L2-B | Cline 分支，多模式（Architect/Code/Ask/Debug） |
| **Continue.dev** | 开源社区 | 是 | 模型无关 | L2-A→L2-B | VS Code/JetBrains，可自托管 |
| **Cody** | Sourcegraph | 部分开源 | 第三方 | L2-B | 强代码库检索增强 |
| **Amazon Q Developer** | AWS | 否 | 第三方 | L2-A→L2-B | 原 CodeWhisperer，企业级主流 |
| **Augment Code** | Augment | 否 | 第三方 | L2-B | 主打超大代码库上下文 |

> 共性：不换编辑器，低成本接入；其中 Cline/Roo Code/Continue 是"模型无关 + 开源"的代表，避免供应商锁定。

### ③ CLI 终端智能体

| 工具 | 厂商 | 开源 | 模型关系 | 说明 |
| :--- | :--- | :--- | :--- | :--- |
| **Claude Code** | Anthropic | 否 | 官方模型 | 封装自家 Claude，L1+L2-B |
| **Codex** | OpenAI | 否 | 官方模型 | 封装自家 GPT，L1+L2-B |
| **OpenCode** | 开源社区 | 是 | 模型无关（75+） | 不锁定供应商 |
| **Aider** | 开源社区 | 是 | 模型无关 | git 友好，每次改动自动提交 |
| **Gemini CLI** | Google | 是 | 官方/第三方 | 2025 新出，对标 Claude Code |
| **Qwen Code** | 阿里 | 是 | 官方/第三方 | 基于 Gemini CLI 衍生 |

> 共性：终端运行，权限直接、git 友好，适合已有本地工程的老手；注意权限与用量控制（见 [06 · 风险](./06-risks.md)）。

### ④ 云端 SWE Agent（自主软件工程师）

| 工具 | 厂商 | 开源 | 模型关系 | 说明 |
| :--- | :--- | :--- | :--- | :--- |
| **Devin** | Cognition | 否 | 第三方 | "首个 AI 软件工程师"，全云端自主完成开发任务 |
| **Codex**（云端模式） | OpenAI | 否 | 官方模型 | 云端沙箱执行 |

> 共性：给目标交付成果，安全隔离、不影响本机；但访问本地环境受限，适合独立任务而非改动现有仓库。

### ⑤ 应用 / UI 生成器（Vibe Coding）

| 工具 | 厂商 | 模型关系 | 说明 |
| :--- | :--- | :--- | :--- |
| **Bolt.new** | StackBlitz | 第三方 | 浏览器内全栈网页应用生成 |
| **v0** | Vercel | 第三方 | UI / 前端组件生成 |
| **Lovable** | 原 GPT Engineer | 第三方 | 自然语言构建完整应用 |
| **Replit Agent** | Replit | 第三方 | 在线 IDE 智能体 |

> 共性：面向非开发者或快速原型，"说话即出应用"；产物偏新项目，深度迭代仍需回到①②③类工具。

---

## 四、案例：GitHub Copilot 的 L2-A → L2-B 演进

```
补全（L2-A）  →  聊天（L2-A）  →  Agent Mode（L2-B）
被动建议          被动问答          自主规划 + 工具调用 + 验证
```

Copilot 是 [02 · L2 应用深度剖析](./02-l2-analysis.md) 中"L2-A→L2-B 演进趋势"的最佳实证：同一个产品随能力升级跨越了分类边界。

---

## 五、选型决策矩阵

| 你的场景 | 推荐形态 | 推荐工具 |
| :--- | :--- | :--- |
| 想整体迁移到 AI 编辑器 | ① AI 原生 IDE | Cursor / Windsurf |
| 不想换编辑器，要轻量接入 | ② IDE 插件 | GitHub Copilot（商用）/ Cline（开源自主） |
| 老手，习惯终端 + git | ③ CLI 终端 | Claude Code（官方）/ OpenCode（开源模型无关） |
| 甩一个独立任务全自动完成 | ④ 云端 SWE | Devin |
| 不会写代码，快速出原型 | ⑤ Vibe Coding | Bolt.new / v0 / Lovable |
| 企业级、需合规与私部署 | ② IDE 插件 | Amazon Q Developer / Continue（自托管） |

> 🛡️ 选型前务必过一遍 [06 · 局限性与风险分析](./06-risks.md) 的自查清单，尤其本地终端型工具的权限边界。

---

← [上一篇：06 · 局限性与风险分析](./06-risks.md) | [返回首页](../README.md) | 相关：[02 · L2 应用深度剖析](./02-l2-analysis.md) · [03 · 混合角色产品](./03-hybrid-roles.md)
