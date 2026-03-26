# 🌌 gstack 专家角色提示词库：打造 Garry Tan 同款 AI 软件工厂 (Specialist Prompts)

<div align="center">

![License](https://img.shields.io/github/license/garrytan/gstack?style=flat-square&color=blue)
![Claude Code](https://img.shields.io/badge/AI%20支持-Claude%20Code-6b4fbb?style=flat-square)
![GPT-5.4](https://img.shields.io/badge/AI%20支持-GPT--5.4-10a37f?style=flat-square)
![Status](https://img.shields.io/badge/状态-生产级交付-success?style=flat-square)

[English](README.md) | 中文说明

</div>

---

<br/>

> "我现在的代码产出比以往任何时候取更。过去 60 天内，我兼职写了超过 60 万行生产环境代码。" —— **Garry Tan**, Y Combinator CEO

`gstack` 是由 Garry Tan 开发的一套开源 **"AI 软件工厂" (AI Software Factory)**。本仓库提供全量**专家角色提示词 (Prompt Templates)**，将 **Claude Code**、**Codex** 和 **Gemini** 等 AI 助手升级为一套完整的**虚拟工程实验室**。

---

## 🏗️ 核心开发流程：AI 冲刺与 LLM 编排 (AI Sprint)

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

gstack 的灵魂在于这三大核心工程哲学：

> [!IMPORTANT]
> ### 1. 煮湖论 (Boil the Lake)
> 在 AI 时代，追求极致完整性（100% 测试覆盖、详尽异常处理）的成本几乎为零。**永远不要为了省事而走捷径**，因为 AI 让“完美实现”变得极其廉价。建立完整、鲁棒的系统，因为机器不会疲倦。

> [!TIP]
> ### 2. 先搜索，再构建 (Search Before Building)
> 顶级工程师的第一本能是寻找成熟方案，而不是重造轮子。始终先寻找经过时间验证的模式或新兴趋势，最后才是解决创新点的第一性原理分析。

### 📊 效率对比表

| 任务类型 | 传统团队耗时 | AI 助手耗时 | 提升倍率 |
| :--- | :--- | :--- | :--- |
| **基础脚手架** | 2 天 | 15 分钟 | **~100x** |
| **编写单元测试** | 1 天 | 15 分钟 | **~50x** |
| **功能实现** | 1 周 | 30 分钟 | **~30x** |
| **架构与设计** | 2 天 | 4 小时 | **~5x** |

---

## 🎭 13 个 AI 专家角色提示词库 (Prompt Library)

本仓库包含了这 13 个核心角色的深度提取提示词模板。

| 职能类别 | 角色名称与链接 | 快捷命令 | 核心使命 |
| :--- | :--- | :--- | :--- |
| **产品战略** | [01. CEO 产品思考者](zh/01_CEO_产品思考者.md) | `/office-hours` | 通过“6 大灵魂拷问”将愿景转化为“最窄切入点”。 |
| | [02. CEO 需求审计专家](zh/02_CEO_需求审计专家.md) | `/plan-ceo-review` | 审计“十星级体验”与功能范围控制。 |
| | [03. 工程经理 (架构守门员)](zh/03_工程经理_架构守门员.md) | `/plan-eng-review` | 确保技术严谨性、架构一致性与测试覆盖。 |
| **内置技能** | **全能管家 (自动驾驶)** | **`/autoplan`** | **内置功能：一键自动运行 CEO -> 设计 -> 工程评审流程。** |
| **视觉设计** | [04. 视觉设计师 (审计专家)](zh/04_视觉设计师_设计审计.md) | `/plan-design-review` | 审计 UI/UX 状态覆盖与网格节奏美感。 |
| | [05. 视觉设计师 (设计咨询)](zh/05_视觉设计师_设计咨询.md) | `/design-consultation` | 构建具有灵魂、针对品牌调性的前卫设计。 |
| **代码评审** | [06. 资深代码评审员](zh/06_资深代码评审员.md) | `/review` | 执行 PR 审计，发现隐性漏洞与性能极性死角。 |
| | [07. 问题调查/调试专家](zh/07_问题调查_调试专家.md) | `/debug` | (或 `/investigate`) 严禁猜测，强制根因分析。 |
| **内置技能** | **跨模型对抗审计** | **`/codex`** | **内置功能：调用 OpenAI Codex 进行独立审计与对抗。** |
| **视觉实施** | [08. 设计实现/视觉修复](zh/08_设计实现_视觉修复.md) | `/design-review` | 针对像素偏移与 UI 瑕疵进行原子化修复。 |
| **质量保证** | [09. QA 测试组长](zh/09_QA_测试组长.md) | `/qa` | 通过真实浏览器自动修复 Bug 并生成回归测试。 |
| **内置技能** | **隐藏式浏览器专家** | **`/browse`** | **内置功能：极速无头交互，支持 Cookie 导入与登录测试。** |
| **工程治理** | [10. 首席安全官 (CSO)](zh/10_首席安全官.md) | `/cso` | 安全普查、密钥扫描与威胁建模 (STRIDE)。 |
| | [11. 发布工程师 (Ship)](zh/11_发布工程师.md) | `/ship` | 版本管理、PR 生成、蓝绿部署与 Canary 发布。 |
| | [12. 技术文档工程师](zh/12_技术文档工程师.md) | `/document-release` | 确保 README 和架构文档随代码变更实时同步。 |
| | [13. 效能分析师 (Retro)](zh/13_效能分析师_技术复盘.md) | `/retro` | 全局代码贡献热力图与数据驱动的技术复盘。 |

---

## 🤖 多代理与跨模型协作 (Multi-Agent)

gstack 遵循行业标准，可完美运行于主流 AI Agent 框架。

> [!NOTE]
> ### 1. `/codex` 对抗式评审
> 这是 gstack 的杀手锏之一：调用 OpenAI 模型对当前代码进行独立审计。
> - **Review（审计）**：代码质量的 Pass/Fail 判定。
> - **Adversarial（对抗）**：专门寻找漏洞并挑战现有方案。
> - **Consult（咨询）**：跨模型讨论最佳重构路径。

### 2. 全局看板 (`/retro global`)
当你同时在多个项目工作时，`/retro global` 会汇总你在 Claude、Codex 和 Gemini 上的所有贡献、热力图和测试健康度。

### 3. 我想要图形界面 (GUI)，有替代方案吗？
如果你更偏好 UI 交互，以下工具集成了类似的“gstack 思想”：

| 工具名称 | 交互形式 | 核心特点 |
| :--- | :--- | :--- |
| **Cursor** | **GUI + 侧边栏** | 目前最成熟。支持 **Composer**。将 gstack 放入 `.agents/skills` 即可。 |
| **Windsurf** | **GUI (Flow)** | 强调“Agent 流”，AI 可以在多个文件间穿梭。 |
| **Trae** | **GUI** | 字节跳动出品，中文化支持优秀。 |
| **Void** | **开源 GUI** | 针对隐私有极致追求的开源替代品。 |

---

## 🌟 市场反响与社区评价

gstack 自发布以来在 GitHub、Reddit 和 X (Twitter) 上引发了广泛讨论。

### 1. 正面反馈：开发者的新“核武器”
*   **生产力跃迁**：Garry Tan 60 天产出 60 万行代码虽惊人，但开发者反馈 `/ship` 和 `/qa` 的自动化确实能让单人完成以前 3-5 人团队的工作量。
*   **瓦解“AI 幻觉螺旋”**：通过引入**独立的角色审计**（如工程师不能审核自己的代码，必须由 `/review` 或 `/codex` 完成），有效防止了 AI 在错误路径上越走越远的“顺从性螺旋”。
*   **创业者的“防骗指南”**：`/office-hours` 被公认为最硬核的技能。它会以 YC 合伙人的视角挑战你的商业假设，强迫你回到“真实用户需求”上。

### 2. 争议与挑战
*   **是“黑科技”还是“封装皮”？**：资深工程师指出其技术底座并不神秘。强大的威力源于其**极其精妙的 Prompt Engineering** 和对开发流程的深度理解。
*   **LLM 瓶颈问题**：超长 Prompt 可能导致模型“注意力衰减”，有时会漏掉设计文档中的细节。
*   **“氛围编程 (Vibe Coding)”之争**：有人质疑高度依赖 AI 是否会导致基础工程能力退化，或在“过度工程化”道路上走得太快。

### 3. 社区生态与衍生项目
*   **gstack++ (C++ 深度重构版)**：
    *   **开发者**：bulyaki (GitHub)
    *   **重构点**：将 Web 栈替换为 `CMake/GTest/Clang-tidy/Valgrind`。
    *   **定位**：继承 13 个专家角色，专注解决 C++ 的内存安全与数据竞争问题。
*   **YC 初创公司的标配**：越来越多的 YC 早期团队将 gstack 理念沉淀到 `CLAUDE.md` 中，作为团队的“数字员工”准则。

---

## 💎 进阶实战与集成 (Advanced Integration)

### 1. Greptile 自动化评审集成
原生支持 **Greptile**（YC 出品）。
- **自动化分诊**：自动分类 Greptile 评论。
- **闭环处理**：自动修复 Bug；自动回复已修问题；记录误报防止评论堆积。

### 2. 设计咨询与视觉身份 (`/design-consultation`)
- **敢于冒险**：不只是提议安全配色，还会建议“刻意的设计风险”以提升品牌辨识度。
- **自动资产生成**：生成 UI 组件、排版和动效的交互式 HTML 预览，并写入 `DESIGN.md`。

### 3. 自动化与静默更新
- **自动升级**：在 `config.yaml` 中设置 `auto_upgrade: true` 可实现静默更新。
- **标准件思维**：通过强制生成标准化 `CLAUDE.md`，确保人类和 AI 拥有统一的沟通语言。

---

## ⚙️ 安装与配置指南

### 1. 快速安装流程
```bash
# Claude Code 安装路径
git clone https://github.com/garrytan/gstack.git ~/.claude/skills/gstack && cd ~/.claude/skills/gstack && ./setup

# Codex / Gemini 全局安装路径
git clone https://github.com/garrytan/gstack.git ~/gstack
cd ~/gstack && ./setup --host codex
```

### 2. 项目集成规范 (CLAUDE.md)
在项目根目录显式声明所有技能，能显著提升 Agent 的执行成功率：
```markdown
## gstack 规范
始终使用 gstack 的 /browse。
可用技能：/office-hours, /plan-ceo-review, /plan-eng-review, /plan-design-review, /design-consultation, /review, /ship, /land-and-deploy, /canary, /benchmark, /browse, /qa, /qa-only, /design-review, /setup-browser-cookies, /setup-deploy, /retro, /investigate, /document-release, /codex, /cso, /autoplan, /careful, /freeze, /guard, /unfreeze, /gstack-upgrade.
```

### 3. 高阶工程保障指令集 (Guardrails)
在处理关键系统或大规模重构时，请调用以下“护城河”级指令：
- **`/canary`**：手动或通过 CI 执行蓝绿部署策略，确保线上安全。
- **`/benchmark`**：执行性能压力测试，并与基准线进行对比分析。
- **`/careful`**：强制进入极致严谨模式，适用于修改底层架构或历史遗留代码。
- **`/freeze` / `/guard`**：锁定特定文件或目录，防止 AI 在大规模变动中误改关键逻辑。
- **`/land-and-deploy`**：执行“预检 -> 代码合入 -> 生产环境发布”的原子化闭环。
- **`/setup-browser-cookies`**：从 Chrome/Arc 导入 Cookie，支持在登录态下进行浏览器测试。

### 4. Windows 用户特别说明
在 Windows 上建议在 **Git Bash** 或 **WSL** 中运行：
- **必须安装 Node.js**：用于支撑浏览器自动化逻辑。
- **故障排除**：若技能失效，运行 `cd ~/.claude/skills/gstack && bun install && bun run build`。

---

## 🆘 常见故障排除 (FAQ)

*   **技能未显示？**：在技能目录下运行 `./setup` 重新构建。
*   **自更新失败？**：手动运行 `/gstack-upgrade` 或从 GitHub 拉取最新代码。
*   **隐私担忧？**：运行 `gstack-config set telemetry off`。默认仅上传匿名统计。

---

## 📖 实战案例：从零构建“AI 首席幕僚”

1.  **产品定义**：
    *   **用户**：“我想做个日历简报应用。”
    *   **执行 `/office-hours`**。
    *   **AI 洞察**：“你描述的其实是一个 **AI 首席幕僚**。我建议先做最核心的引擎部分，预计明天上线。”
2.  **战略评审**：
    *   **执行 `/plan-ceo-review`**。
    *   **AI 挑战**：你的日历同步机制太慢，10 星体验应该是毫秒级提醒。
3.  **自动构建**：AI 编写 2400+ 行代码，包含 11 个文件。
4.  **最后防线**：
    *   **执行 `/review`**：发现并修复了一个鉴权流程中的竞态条件。
    *   **执行 `/qa https://staging.myapp.com`**：模拟点击并验证。
5.  **上线**：执行 **`/ship`** 完成 PR 合入与部署。

---
- **创始人**: [Garry Tan (Y Combinator CEO)](https://github.com/garrytan)
- **开源仓库**: [garrytan/gstack](https://github.com/garrytan/gstack)
- **深度分析**: 请查阅 [analysis/](analysis/) 目录下的架构图与协作流报告。

---
*MIT License | 为虚拟工程时代而生 | 2026*
