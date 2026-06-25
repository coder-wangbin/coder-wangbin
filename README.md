<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&duration=3000&pause=1000&color=0969DA&center=true&vCenter=true&width=680&lines=Hi%2C+I%27m+coder-wangbin;Go+Backend+Developer+%C2%B7+7%2B+Years;AI-Driven+Full-Chain+Workflow+Builder;K8s+%2B+DevOps+Toolchain+Designer" alt="Typing SVG" />
</p>

<p align="center">
</p>

<p align="center"><i>"瓶颈不在模型，在模型外的工程系统。"</i></p>

<p align="center">
  <a href="mailto:coder.wangbin@gmail.com"><img src="https://img.shields.io/badge/Email-coder.wangbin%40gmail.com-blue?style=flat-square&logo=gmail" /></a>
  <a href="https://coder-wangbin.github.io"><img src="https://img.shields.io/badge/Portfolio-coder--wangbin.github.io-green?style=flat-square" /></a>
  <img src="https://komarev.com/ghpvc/?username=coder-wangbin&style=flat-square&color=blue" />
</p>

---

## 👨‍💻 关于我

Go 后端开发，7+ 年。专注把 AI 真正接入研发全流程——从需求分析到自动部署、从代码生成到故障自愈。

花了半年时间设计并落地了一套 AI 驱动全链路工具链，把需求分析、方案设计、编码自验证、K8s 自动部署、日志诊断、Bug 自动修复串成了可执行、可回流的闭环。

---

## 🏗️ AI 全链路研发管线

**1 需求分析** → **2 方案设计** → **3 编码开发** → **4 Oracle 审核** → **5 自动部署** → **6 健康检查** → **7 自愈 & 告警**

| 环节 | 以前（人工） | 现在（AI 驱动） | 提效 |
|------|-------------|----------------|------|
| **需求分析** | 下载 PRD 逐字读，漏洞靠经验 | AI 自动读取、查漏补缺 | 半天→10-60min |
| **方案设计** | 手写文档，复制粘贴，文档总滞后 | AI 生成方案并同步到文档 | 1-2天→对话中产出 |
| **数据库配置** | 切分支手动改 DSN，忘了就切错库 | Git hook 自动同步，热重载 | 手动→零操作 |
| **编码开发** | 写→编译→部署→测试全靠手 | ulw-loop 编译→测试→审核循环 | 2-3天→自验证 |
| **部署上线** | 打开 Kuboard → 手动更新镜像 | push → CI → lb 自动部署 | 30min→全自动 |
| **故障排查** | 复制 CI/K8s 日志贴给 AI 分析 | AI 直接读日志，自动诊断 | 1-2h→Agent 诊断 |
| **Bug 修复** | 改代码 5 分钟，走流程 4 小时 | AI 监控 Bug 列表→自动修→部署 | 半天→自动闭环 |
| **代码搜索** | grep + read 链，耗 token | CodeGraph 语义搜索 MCP | token↓ 调用↓ |

---

## 🔧 核心工具链

### lb CLI + MCP Server — K8s 运维
11 个 MCP 工具（list_pods / get_logs / diagnose / events / restart / pipeline / job_logs / ingress / tls / status / notify）让 AI 能直接操作 K8s 和 GitLab CI。Kuboard SSO 5 步认证 + Strategic Merge Patch 滚动更新 + 关联部署 + 通知。

### dbhub MCP + Git Hook — 数据库自动切换
post-checkout hook 检测分支切换 → 读 conf.yml → Go DSN 转 MySQL DSN → 写 dbhub.toml → config-watcher 热重载。多项目扩展。

### CodeGraph — 代码知识图谱
10 个 MCP 工具：context / search / explore / trace / callers / callees / impact / node / files / status。支持 20+ 语言，多分支增量同步，Go 框架路由识别。

### CCX — 多模型路由
CodeX + CCX 接入 DeepSeek + DashScope。双通道（文本推理 + 多模态视觉），视觉路由机制，3 个常见配置错误排坑。

### OpenCode 环境
ulw-loop 自验证循环 · Ghostty + yazi · 多轮上下文管理 · 插件生态（CodeGraph/dbhub/lb/lark-cli/fmt）· 配置自动更新。

---

## 🚀 项目

| 项目 | 说明 |
|------|------|
| [📄 AI 全链路工作流文档](https://github.com/coder-wangbin/ai-driven-dev-workflow) | 完整工程文档：从需求到交付的闭环实践，含 Mermaid 图 |
| [📚 知识库](https://github.com/coder-wangbin/knowledge-base) | OpenCode · CodeGraph · CCX · lb DevOps · Go工具 · RAG |
| [🌍 Skill 描述本地化](https://github.com/coder-wangbin/opencode-skill-localizer) | git skip-worktree 保护翻译不改被覆盖 |
| [🎯 并行任务分解](https://github.com/coder-wangbin/codex-goal-parallel) | CodeX skill：自动并行拆解任务 |

---

## 🧰 技术栈

| 领域 | 技术 |
|------|------|
| 语言 | Go · Python · Shell |
| 云原生 | Kubernetes · Docker · Kuboard |
| CI/CD | GitLab CI · 自研 CLI |
| AI & MCP | OpenCode · Codex · CodeGraph · lark-cli |
| 数据库 | MySQL · Redis · dbhub MCP |
| 知识管理 | CodeGraph · AGENTS.md · CHANGELOG.md |

---

## 📚 知识积累

| 主题 | 涵盖内容 |
|------|---------|
| OpenCode 全配置 | ulw-loop · Ghostty+yazi · 上下文策略 · 插件生态 · 自动更新 · handoff |
| CodeGraph 实践 | MCP 接入 · 10 工具 · 多分支 · Go 配置 · 框架路由 · 索引 |
| 多模型路由 | CCX+DS+DashScope · 视觉路由 · 3 个坑 · 验证方法 |
| Go 开发 | Air 热编译 · AGENTS.md · worktree · TDD · subagent |
| RAG & 搜索 | SearchRAG · SearchApi 实践 |
| DevOps 设计 | 三层架构 · SSO · CI 模板 · MCP Server · 通知 |

---

## 📊 动态

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=coder-wangbin&show_icons=true&hide_title=true&hide_border=true&count_private=true" height="150" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=coder-wangbin&layout=compact&hide_title=true&hide_border=true" height="150" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=coder-wangbin&theme=github-light&hide_border=true&area=true" width="90%" />
</p>

---

<p align="center"><i>"瓶颈不在模型，在模型外的工程系统。"</i></p>
