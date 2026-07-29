<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&duration=3000&pause=1000&color=0969DA&center=true&vCenter=true&width=680&lines=Hi%2C+I%27m+coder-wangbin;Go+Backend+Developer+%C2%B7+7%2B+Years;AI-Driven+Full-Chain+Workflow+Builder;K8s+%2B+DevOps+Toolchain+Designer" alt="Typing SVG" />
</p>

<p align="center"><i>"瓶颈不在模型，在模型外的工程系统。"</i></p>

<p align="center">
  <a href="mailto:coder.wangbin@gmail.com"><img src="https://img.shields.io/badge/Email-coder.wangbin%40gmail.com-blue?style=flat-square&logo=gmail" /></a>
  <a href="https://coder-wangbin.github.io"><img src="https://img.shields.io/badge/Portfolio-coder--wangbin.github.io-green?style=flat-square" /></a>
</p>

---

## 👨‍💻 关于我

Go 后端开发，7+ 年。专注 **Agentic Engineering**——把 AI Agent 真正接入研发全流程，从需求分析到自动部署、从代码生成到故障自愈。

花了半年时间设计并落地了一套 AI 驱动全链路工具链，串起了需求分析、方案设计、编码自验证、K8s 自动部署、日志诊断、Bug 自动修复的完整闭环。

---

## 🏗️ AI 全链路研发管线

**1 需求分析** → **2 方案设计** → **3 编码开发** → **4 Goal 审核** → **5 自动部署** → **6 健康检查** → **7 自愈 & 告警**

| 环节 | 以前（人工） | 现在（AI 驱动） | 提效 |
|------|-------------|----------------|------|
| **需求分析** | 下载 PRD 逐字读，漏洞靠经验 | Agent 自动读取、查漏补缺 | 半天→10-60min |
| **方案设计** | 手写文档，复制粘贴，文档总滞后 | Agent 生成方案并同步到文档 | 1-2天→对话中产出 |
| **数据库配置** | 切分支手动改 DSN，忘了就切错库 | Git hook 自动同步，热重载 | 手动→零操作 |
| **编码开发** | 写→编译→部署→测试全靠手 |  编译→测试→审核循环 | 2-3天→自验证 |
| **部署上线** | 打开 Kuboard → 手动更新镜像 | push → CI → lb 自动部署 | 30min→全自动 |
| **故障排查** | 复制 CI/K8s 日志贴给 AI 分析 | Agent 直接读日志，自动诊断 | 1-2h→Agent 诊断 |
| **Bug 修复** | 改代码 5 分钟，走流程 4 小时 | Agent 监控 Bug 列表→自动修→部署 | 半天→自动闭环 |
| **代码搜索** | grep + read 链，耗 token | CodeGraph 语义搜索 MCP | token↓ 调用↓ |

### 🎯 /goal 目标驱动开发

> oh-my-openagent v4.19 起，`/goal` 取代 ulw-loop，成为标准的 Agent 目标驱动模式。

| 特性 | 说明 |
|------|------|
| 🎯 **/goal 命令** | 设定目标 → Agent 自动实现 → 自验证（编译/测试/诊断） → Goal 审核 → 不通过打回重做 → 通过交付 |
| 🧠 **模型工具** | `create_goal` / `update_goal` / `get_goal` — Agent 可自主管理目标 |
| 💾 **持久化状态** | 目标状态持久化到 `.omo/goal/`，会话恢复自动继续 |
| 🔄 **持续 Loop** | Goal 审核（GPT-5.6 Sol）不通过就打回重做，循环直到审核批准 |

---

## 🔧 核心工具链

| 工具 | 核心能力 |
|------|---------|
| **lb CLI + MCP Server** | 11 个 MCP 工具让 Agent 直操作 K8s 和 GitLab CI。Kuboard SSO 5 步认证 + Strategic Merge Patch 滚动更新 + 关联部署 |
| **dbhub MCP + Git Hook** | post-checkout hook 检测分支切换 → 读 conf.yml → DSN 自动转换 → 热重载 |
| **CodeGraph MCP** | 代码知识图谱，10 个 MCP 工具（context / search / trace / callers / impact 等），20+ 语言，多分支增量同步 |
| **CCX 多模型路由** | CodeX + CCX 接入 DeepSeek + DashScope。双通道（文本 + 视觉），视觉路由 |
| **OpenCode + Codex** | `/goal` 目标驱动 · Ghostty + yazi · 多轮上下文 · 插件生态 |
| **codex-swarm** | 三支柱并行智能体编排：第一性原理 × 对抗式审查 × 防作弊护栏 |

### 🔌 MCP 2026-07-28 · Agentic Engineering

| 概念 | 说明 |
|------|------|
| 🔌 **MCP 2026-07-28** | Stateless Core · MRTR 多轮请求 · MCP Apps/Tasks 扩展 · 250M+ 周下载 |
| 🔗 **标准接口** | Agent 通过统一 MCP 连接数据库、搜索引擎、云 API、内部工具 |
| 🏗️ **Agentic Engineering** | Vibe Coding 进化为系统化工程实践 |

> **Spec 先行 → Review 把关 → Test 验证**：同一套"描述意图 → Agent 构建"的本能，加上完整的工程纪律。

---

## 🚀 项目

| 项目 | 说明 | 关键词 |
|------|------|--------|
| [🐝 codex-swarm](https://github.com/coder-wangbin/codex-swarm) | 三支柱并行智能体编排 | CodeX · Agent · Security |
| [📄 AI 全链路工作流](https://github.com/coder-wangbin/ai-driven-dev-workflow) | 从需求到交付的闭环工程文档 | Docs · Mermaid · DevOps |
| [📚 知识库](https://github.com/coder-wangbin/knowledge-base) | 6 大主题经验沉淀 | OpenCode · K8s · CCX |
| [🌍 Skill 本地化](https://github.com/coder-wangbin/opencode-skill-localizer) | git skip-worktree 保护翻译 | Shell · Git · OpenCode |
| [🎯 并行任务分解](https://github.com/coder-wangbin/codex-goal-parallel) | 自动拆解 + 子 Agent 管理 | CodeX · Agent |

---

## 🧰 技术栈 & 📚 知识积累

| 领域 | 技术栈 | 知识深度 |
|------|--------|---------|
| **语言** | Go · Python · Shell | — |
| **云原生 / DevOps** | Kubernetes · Docker · Kuboard · GitLab CI | K8s 自动部署 · SSO · CI 模板 · MCP Server · 三层架构 |
| **AI & MCP** | OpenCode · Codex · CodeGraph · lark-cli · CCX | MCP 2026-07-28 · Stateless Core · MRTR · /goal 目标驱动 |
| **Agent 编排** | codex-swarm 多智能体 | 第一性原理 · 对抗式审查 · 防作弊护栏 |
| **数据库** | MySQL · Redis · dbhub MCP | Git Hook DSN 自动同步 · 热重载 |
| **Go 开发** | Air 热编译 · AGENTS.md · worktree · TDD | subagent · 会话健康检查 · 多轮上下文管理 |
| **多模型** | CCX + DeepSeek + DashScope | 视觉路由 · 3 个配置错误 · 验证方法 |
| **知识管理** | CodeGraph · AGENTS.md · CHANGELOG.md | 10 MCP 工具 · 多分支增量 · Go 路由识别 |

---

## 📊 项目总览

- **6** 个公开仓库
- 核心领域：Go · K8s DevOps · MCP 协议 · AI Agent 编排
- 主力工作在私有仓库，公开仓库为技术分享和开源项目

---

<p align="center"><i>"瓶颈不在模型，在模型外的工程系统。"</i></p>
