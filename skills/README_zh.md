# 🌌 gstack-ai-roles: 精英工程引擎 (Elite Engineering Engine)

<div align="center">

![工作流封面](assets/skills_cover.png)

</div>

本目录包含了 **“gstack-ai-roles 精英工程引擎”**。这是一个深受 gstack 哲学启发、并针对通用 AI Agent 规范进行极致优化的 6 阶段生产系统。

## 🏗️ 6 阶段架构

```text
  [ Think ] --(DESIGN.md)--> [ Plan ] --(PLAN.md)--> [ Build ]
                                                       |
                                                  (代码与测试)
                                                       |
     [ Ship ] <--(合并 PR)--- [ Test ] <--(审计通过)--- [ Review ]
```

## 🛠️ 核心组件

- **[SKILL.md](SKILL.md)**: 技能的“大脑”。定义了元数据、触发条件以及 AI 代理的高级执行逻辑。
- **[references/prompts.md](references/prompts.md)**: 为每个阶段（Think, Plan, Build, Review, Test, Ship）深度提取的角色提示词。

## 🚀 安装指南

### 离线手动安装 (本地开发)
克隆本仓库并将其中的 `skills` 目录复制到你的 Agent 技能路径下：

```bash
# 克隆仓库
git clone https://github.com/lee-jet/gstack-ai-roles.git

# 安装至 Claude Code
cp -r gstack-ai-roles/skills ~/.claude/skills/gstack-ai-roles

# 安装至 Codex / 通用工具
cp -r gstack-ai-roles/skills ~/.codex/skills/gstack-ai-roles

# 针对 Cursor / Windsurf / Trae
# 直接在工具中加载本仓库的 /skills 目录即可。
```

## 🎮 引擎驱动 (使用方法)

`gstack-ai-roles` 引擎通过自然语言意联或显式的斜杠命令启动。

### 🖥️ 全量编排：自动化工厂流水线 (End-to-End)
从高层愿景到生产交付，自动化运行完整的 6 个运营单元。
- “从零构建一个 [功能名称]”
- “针对 [项目想法] 启动 gstack-ai-roles 工程工厂”
- “初始化生产级 [模块] 并运行所有审计门禁”

### 🚦 智能状态恢复：零损耗工作流 (State-Based)
引擎会自动探测已存在的 `DESIGN.md` 或 `PLAN.md` 产出物，并仅从必要阶段续作。
- “架构蓝图已锁定，直接开始编码与评审”
- “实施已完成，执行对抗性审计并发布上线”
- “接管此分支：审计当前代码并生成回归测试”

### 🧩 手动单元调用 (Manual Unit)
直接触发特定领域的子代理进行专项工程任务：
- `/think [概念]` — 深度第一性原理分析与 `DESIGN.md`
- `/plan` — 系统拓扑与状态机设计 (`PLAN.md`)
- `/review` — 严格的逻辑与安全审计（资深架构师/CSO 模式）
- `/ship` — 最终治理、Rebase 与发布同步

---
*本技能由 Garry Tan 的 gstack 理念启发，针对快速闭环开发冲刺进行了极致优化。*
