<h1 align="center">👋 王彬 · coder-wangbin</h1>
<p align="center"><b>Go Backend Developer · AI-Driven Full-Chain Workflow Builder · K8s + DevOps Toolchain Designer</b></p>

<p align="center">
  <a href="mailto:coder.wangbin@gmail.com"><img src="https://img.shields.io/badge/Email-coder.wangbin%40gmail.com-blue?style=flat-square&logo=gmail" /></a>
  <a href="https://coder-wangbin.github.io"><img src="https://img.shields.io/badge/Portfolio-coder--wangbin.github.io-green?style=flat-square" /></a>
  <img src="https://komarev.com/ghpvc/?username=coder-wangbin&style=flat-square&color=blue" />
</p>

---

## 👨‍💻 About Me

**Go 后端开发工程师 · 6+ 年经验**

我花了半年时间把 AI 从"只会写代码"变成了"能跟着研发链路从头走到尾"——设计并落地了一套 AI 驱动的全链路研发工具链，覆盖需求分析、方案设计、编码自验证、K8s 自动部署、日志诊断、Bug 自修复。

- ⚡ 自研 DevOps 工具链（CLI + MCP Server，11 个工具），让 AI Agent 能直接操作 K8s 和 GitLab CI
- 🧩 打通 CLI ＋ 数据库 MCP ＋ 代码知识图谱，形成从需求到交付的完整闭环
- 🌱 深度使用 **OpenCode ulw-loop / Codex goal** 做 AI 辅助开发
- 🪝 设计 Git post-checkout hook 驱动分支切换自动同步数据库配置

---

## 🏗️ AI-Driven Full-Chain Workflow

| Stage | Before (Manual) | After (AI-Driven) |
|-------|-----------------|-------------------|
| **Req Analysis** | Download PRD, read line-by-line, catch gaps by experience | Agent reads docs, auto-flags gaps & inconsistencies |
| **Design Spec** | Write manually, copy-paste; docs lag behind code | Agent generates spec & syncs in real-time |
| **DB Config** | Manually switch per git branch; forgot once → wrong DB | Git hook auto-syncs DSN on checkout, hot-reload |
| **Coding** | Write → compile → deploy → test (manual) | ulw-loop: code → build → test → **Oracle review** → redo on fail |
| **Deploy** | Open Kuboard → find Deployment → update image → wait | `git push` → CI → auto-deploy → health check → notify |
| **Diagnosis** | Copy CI/K8s logs → paste to AI → human fixes | Agent reads logs via MCP, diagnoses, self-heals |
| **Bug Fix** | QA reports → locate → fix → deploy (fix 5 min, workflow 4 hr) | Agent monitors → auto-fix → verify → deploy → notify |

### ulw-loop: Oracle Review Gate

```
Set Goal → Agent Implements → Self-Verify (build/test/LSP) → Oracle Review
  ├─ Pass → Deliver
  └─ Reject → Redo from start (continuous loop)
```

---

## 🧰 Tech Stack

| Domain | Technologies |
|--------|-------------|
| **Languages** | Go · Python · Shell |
| **Cloud Native** | Kubernetes · Docker · Kuboard |
| **CI/CD** | GitLab CI · Self-built CLI |
| **AI & MCP** | OpenCode · Codex · CodeGraph · lark-cli |
| **Databases** | MySQL · Redis · dbhub MCP |
| **Infra** | Linux · macOS · Nginx |

---

## 🚀 Projects

| Project | Description |
|---------|-------------|
| [📄 ai-driven-dev-workflow](https://github.com/coder-wangbin/ai-driven-dev-workflow) | 完整工程文档：AI 全链路开发工作流 —— 从需求到交付的闭环实践 |
| [🌍 skill-localizer](https://github.com/coder-wangbin/opencode-skill-localizer) | Skill 描述本地化工具 — git skip-worktree 保护翻译 |
| [🎯 codex-goal-parallel](https://github.com/coder-wangbin/codex-goal-parallel) | CodeX 并行任务分解 + 子 Agent 生命周期管理 |

### 🔧 Internal Toolchain
- **K8s MCP Server**: 11 tools — list_pods, get_logs, diagnose, events, restart_deployment, get_pipeline, get_job_logs, get_ingress, patch_ingress_tls, deployment_status, send_notification
- **DB MCP Server**: Agent-driven DB queries with branch-switch auto-sync via Git hooks
- **Deploy CLI**: Kuboard SSO, Strategic Merge Patch, rolling updates, notifications

---

## 📚 Knowledge Base

| Topic | Key Points |
|-------|-----------|
| **OpenCode** | ulw-loop mode, multi-turn context, Ghostty + yazi, Skills & MCP ecosystem |
| **CodeGraph** | MCP integration, 10 tools, multi-branch practice, Go specifics |
| **Multi-Model Routing** | CCX + DeepSeek + DashScope, vision routing, common pitfalls |
| **Go DevTools** | Hot-reload with Air, modern Go idioms |
| **DevOps Design** | K8s auto-deploy, Kuboard SSO, CI templates, MCP Server architecture |
| **RAG & Search** | SearchRAG, SearchApi practical experience |

---

## 📊 Activity

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=coder-wangbin&show_icons=true&hide_title=true&hide_border=true&count_private=true" height="150" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=coder-wangbin&layout=compact&hide_title=true&hide_border=true" height="150" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=coder-wangbin&theme=github-light&hide_border=true&area=true" width="90%" />
</p>

---

<p align="center">
  <i>"The bottleneck is not the model — it's the engineering system outside the model."</i>
</p>
