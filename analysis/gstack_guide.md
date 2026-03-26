# gstack: AI 虚拟精英工程团队全指南 🚀

> "我现在的代码产出比以往任何时候都多。过去 60 天内，我兼职写了超过 60 万行生产环境代码。" —— **Garry Tan**, Y Combinator CEO

`gstack` 是 Garry Tan 开发的开源“软件工厂”。它将 AI 助手（Claude Code, Codex, Cursor 等）从单纯的“副驾驶”升级为一套完整的**虚拟工程团队**。通过 28+ 种专业技能（Slash Commands），它模拟了从 CEO、架构师到 QA 工程师的全流程协作。

---

## 🏗️ 核心开发流程：AI 冲刺 (AI Sprint)

gstack 不仅仅是工具，而是一套严谨的软件开发流程。

```text
    [ 需求输入 ]
         |
         v
    [/office-hours] (产品构思) ----> [ 产生: DESIGN.md & 计划 ]
         |                                |
         +---------------|----------------+
                         v
                [ 三重联合审计门禁 ]
      +------------------+------------------+
      | [/plan-ceo]      | [/plan-eng]      | [/plan-design]
      | (战略/范围)       | (架构/测试)       | (UI/UX 灵魂)
      +------------------+------------------+
                         |
                         v
                  [ 开发实施阶段 ] <-------- [/debug] (调查/复现)
                         |         <-------- [/design-review] (视觉微调)
                         v
                  [ 合并前审计漏斗 ]
      +------------------+------------------+
      | [/review]        | [/cso]           | [/qa]
      | (逻辑漏洞)        | (安全官)         | (浏览器测试)
                         |
                         v
                  [ /ship发布 & /retro复盘 ]
```

---

## 🧠 开发者精神 (Builder Ethos)

gstack 的灵魂在于这三大哲学：

### 1. 煮湖论 (Boil the Lake)
> **理念**：AI 辅助下，极致的完整性成本几乎为零。
*   如果一个功能需要 100% 的测试覆盖率和全路径错误处理，以前需要 2 天，现在只需 15 分钟。
*   **格言**：永远不要为了省事而走捷径，因为 AI 让“完美实现”变得极其廉价。

### 2. 先搜索，再构建 (Search Before Building)
*   1000x 工程师的第一本能是搜索现有的成熟方案，而不是从零设计。
*   **Layer 1**：经久考验的标准模式。
*   **Layer 2**：新兴的流行趋势。
*   **Layer 3**：解决特定问题的第一性原理（真正的创新点）。

### 3. 效率对比表 (Compression Ratio)

| 任务类型 | 传统团队耗时 | AI 助手耗时 | 提升倍率 |
| :--- | :--- | :--- | :--- |
| **基础脚手架** | 2 天 | 15 分钟 | ~100x |
| **编写单元测试** | 1 天 | 15 分钟 | ~50x |
| **功能实现** | 1 周 | 30 分钟 | ~30x |
| **架构与设计** | 2 天 | 4 小时 | ~5x |

---

## 🛠️ 全能技能矩阵 (The Skill Matrix)

gstack 提供了 28 个专业角色，按开发生命周期分类：

### 🧬 定义与规划 (Think & Plan)
| 命令 | 角色 | 核心任务 |
| :--- | :--- | :--- |
| `/office-hours` | **YC 专家** | 通过 6 个“灵魂拷问”重构你的产品思路，生成设计文档。 |
| `/plan-ceo-review` | **创始人** | 以 Brian Chesky 式的审美评审设计，追求 10 星级体验。 |
| `/plan-eng-review` | **工程经理** | 生成数据流 ASCII 图、状态机，锁定测试矩阵。 |
| `/autoplan` | **全能管家** | 一键自动运行 CEO → 设计 → 工程评审流程。 |

### 🔍 评审与调试 (Review & Debug)
| 命令 | 角色 | 核心任务 |
| :--- | :--- | :--- |
| `/review` | **资深架构师** | 扫描 N+1 查询、死锁、逃逸 Bug 等深层问题，自动修复低级错误。 |
| `/investigate` | **调试专家** | 严禁在不调查的情况下修复 Bug，强制执行根因分析。 |
| `/codex` | **外援** | 调用 OpenAI Codex 进行独立评审，多模型对抗以发现隐性漏洞。 |

### 🧪 自动化 QA (Automated Testing)
| 命令 | 角色 | 核心任务 |
| :--- | :--- | :--- |
| `/browse` | **隐身人** | 极速 Chromium 浏览器，100ms 级别响应，真实交互。 |
| `/qa` | **QA 指挥官** | 遍历页面流程，发现 Bug 后自动修复并**生成回归测试**。 |
| `/setup-browser-cookies` | **合伙人** | 从你常用的浏览器（Chrome/Arc等）导入 Cookie，测试**登录后页面**。 |

---

## 🤖 多代理与跨模型协作 (Multi-Agent Support)

gstack 不仅限于 Claude Code，它遵循 [SKILL.md](https://github.com/anthropics/claude-code) 行业标准，可以无缝运行在多个 AI 代理上。

### 1. 支持的 AI 代理
*   **Claude Code**：官方推荐，支持最全。
*   **Codex (OpenAI)**：通过 `--host codex` 参数集成。
*   **Gemini CLI**：通过 Google 的 AI 代理运行。
*   **Cursor**：将 gstack 放入项目根目录的 `.agents/skills/` 即可被自动发现。

### 2. 为 Codex / Gemini 安装 gstack
如果你使用 Codex 或 Gemini CLI，安装时需要指定主机参数：

*   **单项目本地安装**：
    ```bash
    git clone https://github.com/garrytan/gstack.git .agents/skills/gstack
    cd .agents/skills/gstack && ./setup --host codex
    ```
*   **用户全局安装**：
    ```bash
    git clone https://github.com/garrytan/gstack.git ~/gstack
    cd ~/gstack && ./setup --host codex
    ```
    > [!TIP]
    > `--host codex` 会将环境配置在 `~/.codex/skills/gstack`，避免与 Claude 的路径冲突。

### 3. 使用 `/codex` 获取“第二意见”
这是 gstack 的杀手锏之一：**跨模型对抗评审**。

在 Claude Code 中运行 **`/codex`**，它会唤起 OpenAI 的模型对当前代码进行独立审计。
*   **Review 模式**：通过/拒绝门禁，确保代码质量。
*   **Adversarial 模式**：模型会专门找茬，挑战你的实现路径。
*   **Consult 模式**：开放式咨询，探讨多种模型下的最佳方案。

### 4. 跨项目看板 (`/retro global`)
当你同时在多个项目（或使用不同 Agent）工作时，可以使用：
`/retro global`
它会扫描所有 gstack 记录，汇总你在 Claude、Codex 和 Gemini 上的所有代码贡献、提交热力图和测试健康度。

---

---

## 🖥️ 交互形式：一定要在终端执行吗？

很多用户习惯了图形界面 (GUI)，而 `gstack` 及其背后的 AI Agent (如 Claude Code) 看起来更像黑框框。

### 1. 为什么是命令行 (CLI)？
`gstack` 被设计为一套 **Agent 技能集**。像 Claude Code 这样的 Agent 需要直接操控你的本地文件系统、运行测试脚本、执行 Git 命令。命令行是目前这类“自主型 Agent”最高效、权限最完整的交互方式。

### 2. Windows 用户的使用方式
在 Windows 上，目前没有官方的 gstack GUI 窗口。你**必须**通过控制台调用。
*   **推荐环境**：建议使用 `Git Bash` 或 `WSL (Ubuntu)`。
*   **交互逻辑**：你通过终端给 Claude 发指令 (如 `/review`)，Claude 在后台调用 gstack 的代码逻辑。

### 3. 我想要 GUI，有替代方案吗？
如果你更偏好图形界面，市面上有几款集成了类似“gstack 思想”的 AI IDE：

| 工具名称 | 交互形式 | 核心特点 |
| :--- | :--- | :--- |
| **Cursor** | **GUI + 侧边栏** | 目前最成熟的 AI IDE。支持 **Composer** 大规模重构。可以把 gstack 技能放入 `.agents/skills` 供其调用。 |
| **Windsurf** | **GUI (Flow-based)** | 强调“Agent 流”，AI 可以自主在多个文件间穿梭，有非常丝滑的悬浮窗交互。 |
| **Trae** | **GUI** | 字节跳动出品，界面友好，针对中文化支持较好。 |
| **Void** | **Open Source GUI** | Cursor 的开源替代品，适合对隐私和开源有极致追求的人。 |

### 4. 选型建议
*   **选 gstack (CLI)**：如果你已经是命令行高手，或者需要极高的自定义能力（比如想让 Claude 调用你写的特定脚本），或者需要 Claude Code 这样极强的文件系统操控能力。
*   **选 Cursor/Windsurf (GUI)**：如果你想要开箱即用的“现代编辑器”体验，喜欢用鼠标点击来进行对比、撤销和预览。

---

## ⚙️ 保姆级安装与配置指南

### 1. 基础安装 (30 秒)
在你的 AI 工具终端（推荐 Claude Code）执行：
```bash
git clone https://github.com/garrytan/gstack.git ~/.claude/skills/gstack && cd ~/.claude/skills/gstack && ./setup
```

### 2. 项目集成 (关键一步)
为了让 AI 助手识别这些技能，你必须在项目根目录的 `CLAUDE.md` 中添加以下内容。

> [!IMPORTANT]
> 必须显式告诉助手使用 gstack 的浏览器，而不是 Claude 原生的。

```markdown
## gstack 规范
始终使用 gstack 的 /browse 技能进行所有网页浏览，严禁使用 mcp__claude-in-chrome__*。
可用技能列表：/office-hours, /plan-ceo-review, /plan-eng-review, /plan-design-review, /design-consultation, /review, /ship, /land-and-deploy, /canary, /benchmark, /browse, /qa, /qa-only, /design-review, /setup-browser-cookies, /setup-deploy, /retro, /investigate, /document-release, /codex, /cso, /autoplan, /careful, /freeze, /guard, /unfreeze, /gstack-upgrade.
```

### 3. Windows 环境特别注意
Windows 用户建议在 Git Bash 或 WSL 中运行：
*   **必须安装 Node.js**：Bun 在 Windows 上存在 Playwright 兼容性 Bug，gstack 会自动回退到 Node.js。
*   **修复浏览器**：如果 `/browse` 失败，运行 `cd ~/.claude/skills/gstack && bun install && bun run build`。

---

## 📖 实战案例：从零构建“AI 首席幕僚”

1.  **产品定义**：
    *   用户：“我想做个日历简报应用。”
    *   执行 **`/office-hours`**。
    *   AI 反馈：“你描述的其实是一个 AI 个人幕僚。我建议先做最核心的部分，预计明天上线。”
2.  **战略评审**：
    *   执行 **`/plan-ceo-review`**。
    *   AI 挑战：你的日历同步机制太慢，10 星体验应该是毫秒级提醒。
3.  **自动构建**：AI 编写 2400+ 行代码，包含 11 个文件。
4.  **最后防线**：
    *   执行 **`/review`**：发现并修复了一个竞态条件。
    *   执行 **`/qa https://staging.myapp.com`**：模拟点击并验证。
5.  **上线**：执行 **`/ship`**。

---

## 🆘 常见故障排除 (Troubleshooting)

*   **技能未显示？** 执行 `./setup` 重新构建二进制。
*   **自更新失败？** 手动运行 `/gstack-upgrade`。
*   **隐私担忧？** 执行 `gstack-config set telemetry off`。gstack 默认不上传任何代码，仅上传匿名统计。

---

## 🌟 市场反响与用户评价

gstack 自发布以来在 GitHub、Reddit 和 X (Twitter) 上引发了广泛讨论。以下是开发者社区的真实反馈汇总：

### 1. 正面反馈：开发者的新“核武器”
*   **生产力跃迁**：Garry Tan 本人 60 天产出 60 万行代码的数据虽然惊人，但许多开发者反馈通过 `/ship` 和 `/qa` 的自动化，确实能让单人完成以前需要 3-5 人团队的工作量。
*   **瓦解“AI 幻觉螺旋”**：gstack 通过引入**独立的角色审计**（如工程师不能审核自己的代码，必须由 `/review` 或 `/codex` 完成），有效防止了单个 AI 助手在错误路径上越走越远的“顺从性螺旋”。
*   **创业者的“防骗指南”**：`/office-hours` 被公认为最硬核的技能。它不仅帮你写代码，还会以 YC 合伙人的视角挑战你的商业假设，强迫你回到“真实用户需求”上。

### 2. 争议与挑战：冷静的思考
*   **是“黑科技”还是“封装皮”？**：有资深工程师指出，gstack 的技术底座（如 Playwright 封装、Markdown 提示词注入）并不神秘。它的强大更多地源于其**极其精妙的 Prompt Engineering (提示词工程)** 和对开发流程的深度理解。
*   **LLM 瓶颈问题**：随着项目规模扩大，超长 Prompt 可能导致模型的“注意力衰减”。部分用户反馈 AI 有时会默默漏掉设计文档中的细节。
*   **“氛围编程 (Vibe Coding)”之争**：有人质疑这种高度依赖 AI 的方式是否会导致基础工程能力的退化，或者在过度工程化 (Overengineering) 的道路上走得太快。

### 3. 社区生态与衍生项目
*   **gstack++ (C++ 深度重构版)**：
    *   **开发者**：bulyaki (GitHub)
    *   **重构点**：将原本面向 Web 的 Web 技术栈全量替换为 C++ 基建：
        *   **构建系统**：`npm/Bun` → `CMake`, `Make`, `Ninja`。
        *   **测试框架**：`Playwright` → `CTtest`, `GTest`, `Catch2`。
        *   **静态分析**：`ESLint` → `clang-tidy`, `cppcheck`。
        *   **动态分析**：利用 `ASan`, `UBSan`, `TSan` 和 `Valgrind` 替换浏览器控制台日志。
    *   **定位**：继承了 gstack 的 13 个专家角色，但专注于解决 C++ 的内存安全、未定义行为和数据竞争问题。
*   **YC 初创公司的标配**：越来越多的 YC 早期团队开始将 gstack 及其理念沉淀到 `CLAUDE.md` 中，作为团队的“数字员工”准则。

---

## 💎 进阶实战与集成 (Advanced Integration)

根据 **Junia.ai** 等技术博客的实战总结，gstack 的威力在于其“流程封装”能力：

### 1. Greptile 自动化评审集成
gstack 的 `/review` 和 `/ship` 命令原生支持 **Greptile**（YC 出品的一款 PR 自动评审工具）。
*   **自动化分诊**：gstack 会读取 Greptile 的评论，自动对问题进行分类。
*   **闭环处理**：合法的 bug 会被自动修复；已修复的问题会自动回复；误报 (False Positive) 会被记录并推回，防止评论堆积。

### 2. 设计咨询与视觉身份 (`/design-consultation`)
不仅仅是写代码，gstack 还能帮你从零构建**视觉身份**：
*   **敢于冒险**：它不只是提议安全的配色，还会建议“刻意的设计风险”以提升品牌辨识度。
*   **自动生成设计资产**：自动生成包含 UI 组件、排版和动效的交互式 HTML 预览，并写入 `DESIGN.md`。

### 3. 自动化与静默更新
*   **自动升级**：在 `~/.gstack/config.yaml` 中设置 `auto_upgrade: true`，gstack 会在每次启动时静默检查并更新，确保你使用的是最新的专家提示词。
*   **标准件思维**：通过 `/office-hours` 强制生成标准化的 `CLAUDE.md` 和设计文档，确保团队间（人类和 AI）拥有统一的沟通语言。

---

*MIT License | [GitHub 仓库原文](https://github.com/garrytan/gstack)*
