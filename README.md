<div align="center">

# 🗺️ AI Ecosystem Blueprint
# AI 生态架构蓝图：L1 → L2 → L3 全局认知指南

在 AI 大模型爆发、工具层出不穷的当下，你是否也感到困惑：ChatGPT、Claude Code、Cursor、OpenRouter 这些 AI 工具到底是什么关系？谁在提供大脑？谁在做执行？

**本项目旨在：建立全局认知，告别概念混淆。**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](./CONTRIBUTING.md)
[![Stars](https://img.shields.io/github/stars/yiyinideshang/AI-Ecosystem-Blueprint?style=social)](https://github.com/yiyinideshang/AI-Ecosystem-Blueprint)

</div>

---

# 🧠 核心分层速览

| 层级 | 角色定义 | 代表产品 |
| :--- | :--- | :--- |
| **L1：AI 模型** | 提供"大脑"（自研模型 + API） | Agnes-2.0、GLM、DeepSeek、Claude |
| **L2：AI 应用软件** | 提供"躯干与工具"（供用户使用） | Chatbox、Cursor、Claude Code、OpenCode |
| **L3：AI 网关 / 聚合** | 提供"调度网络"（多模型路由） | OpenRouter、ZenMux、CCSwitch |

---

# 🤔 为什么有这个项目？

如今 AI 产品满天飞，很多概念被混为一谈。例如：
- Claude Code 到底是模型还是应用？
- OpenRouter 和 ChatGPT 什么关系？
- Cursor 属于哪一层？

本项目通过一套清晰的 **L1（模型）→ L2（应用）→ L3（网关）** 分层架构，帮助开发者、产品经理和投资人快速建立 AI 行业认知坐标系。既适合作为**个人入门指南**，也可作为**团队内部分享材料**。

---

# 📚 快速导航

本项目将内容模块化，方便按需阅读：

| # | 模块 | 内容要点 |
| :---: | :--- | :--- |
| 01 | [核心分层框架](./docs/01-framework.md) | L1 / L2 / L3 的精确定义、判定标准与"三问法" |
| 02 | [L2 应用深度剖析](./docs/02-l2-analysis.md) | 区分 L2-A（传统对话）与 L2-B（自主智能体 Agent） |
| 03 | [混合角色产品](./docs/03-hybrid-roles.md) | 现实中横跨多层的产品案例（八种组合形态） |
| 04 | [横向维度扩展](./docs/04-extensions.md) | 模态、开源属性、网关演进方向 |
| 05 | [商业模式与数据流向](./docs/05-business.md) | 钱怎么赚？数据怎么流？（含 Mermaid 流程图） |
| 06 | [局限性与风险分析](./docs/06-risks.md) | 每一层级的脆弱点与选型自查清单 |
| 07 | [编程 AI 专项图谱](./docs/07-coding-tools.md) | 专题：AI 原生 IDE / IDE 插件 / CLI / 云端 SWE / Vibe Coding 五类全景 + 选型矩阵 |

> 🕐 全文阅读约 25 分钟（含专题）。建议按 01 → 06 顺序通读建立坐标系，再按需查阅 07 专题。

---

# 🚀 快速开始

1. **通读建立认知**：按上面快速导航顺序阅读 6 个模块。
2. **按需查阅**：遇到具体产品，回到 [03 · 混合角色产品](./docs/03-hybrid-roles.md) 查"基因"。
3. **选型决策**：采购 / 选型前过一遍 [06 · 局限性与风险分析](./docs/06-risks.md) 的自查清单。
4. **内部分享**：可直接基于 `docs/` 目录组织分享 PPT，每篇即一个章节。

---

# 🎯 适合人群

- **AI 初学者**：被各种名词绕晕，想理清"谁是谁"。
- **开发者**：选模型、选工具、设计架构时需要全局视角。
- **产品经理 / 创业者**：判断赛道与竞品定位，避开同质化红海。
- **投资人**：快速给项目"挂号"，看懂商业模式的层级逻辑。
- **团队 Leader**：需要一份可直接用于内部分享的 AI 行业入门材料。

---

# 📂 项目结构

```
AI-Ecosystem-Blueprint/
├── README.md                  # 项目入口（你正在看的这篇）
├── LICENSE                    # MIT 开源协议
├── CONTRIBUTING.md            # 贡献指南
├── AI关系.md                  # 原始素材 / 速查表
└── docs/                      # 分模块深度内容
    ├── 01-framework.md        # 核心分层框架 L1/L2/L3
    ├── 02-l2-analysis.md      # L2 应用深度剖析（L2-A / L2-B）
    ├── 03-hybrid-roles.md     # 混合角色产品（八种组合形态）
    ├── 04-extensions.md       # 横向维度扩展（模态 / 开源 / 网关演进）
    ├── 05-business.md         # 商业模式与数据流向（含流程图）
    ├── 06-risks.md            # 局限性与风险分析（含选型自查清单）
    └── 07-coding-tools.md     # 编程 AI 专项图谱（五类工具 + 选型矩阵）
```

---

# 🤝 贡献

AI 生态日新月异，欢迎通过 Pull Request 补充新案例或修正分类！

- 新增产品案例：请按 [03 · 混合角色产品](./docs/03-hybrid-roles.md) 的格式标注其覆盖层级。
- 修正分类错误：欢迎直接提 PR 或 Issue。
- 分享实践：欢迎补充各层级真实使用经验与踩坑记录。

请先阅读 [贡献指南](./CONTRIBUTING.md)。

---

# 📌 内容时效性声明

AI 行业迭代极快，本项目内容反映 **2025–2026** 年的生态快照，产品分类与商业模式会随时间演变。欢迎共同维护更新。

---

<div align="center">
  <sub>Built with ❤️ for AI Learners</sub>
</div>
