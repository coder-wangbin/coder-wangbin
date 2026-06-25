<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&duration=3000&pause=1000&color=0969DA&center=true&vCenter=true&width=680&lines=Hi%2C+I'm+%E7%8E%8B%E5%BD%AC+(coder-wangbin);Go+Backend+Developer+·+6%2B+Years;AI-Driven+Full-Chain+Workflow+Builder;K8s+%2B+DevOps+Toolchain+Designer" alt="Typing SVG" />
</p>

<p align="center">
  <a href="mailto:coder.wangbin@gmail.com"><img src="https://img.shields.io/badge/Email-coder.wangbin%40gmail.com-blue?style=flat-square&logo=gmail" /></a>
  <a href="https://github.com/coder-wangbin"><img src="https://img.shields.io/badge/GitHub-coder--wangbin-black?style=flat-square&logo=github" /></a>
  <img src="https://komarev.com/ghpvc/?username=coder-wangbin&style=flat-square&color=blue" />
</p>

---

## 👨‍💻 About Me

**Go 后端开发工程师 · 6+ 年经验 · 当前就职于 Langboat（浪舟）**

我花了半年时间把 AI 从"只会写代码"变成了"能跟着研发链路从头走到尾"——设计并落地了一套 AI 驱动的全链路研发工具链，覆盖需求分析、方案设计、编码自验证、K8s 自动部署、日志诊断、Bug 自修复。

- ⚡ 自研 DevOps 工具链（CLI + MCP Server，11 个工具），让 AI Agent 能直接操作 K8s 和 GitLab CI
- 🧩 打通飞书 CLI ＋ 数据库 MCP ＋ 代码知识图谱，形成从需求到交付的完整闭环
- 🌱 深度使用 **OpenCode ulw-loop / Codex goal** 做 AI 辅助开发
- 🪝 设计 Git post-checkout hook 驱动分支切换自动同步数据库配置

---

## 🏗️ AI-Driven Full-Chain Development Workflow

把传统研发流程中 AI 帮不上忙的环节逐个击破，串成一条可执行、可回流的管线：

```mermaid
flowchart LR
    A["PRD Doc"] -->|Agent reads| B["Req Analysis"]
    B -->|Agent writes| C["Design Spec"]
    C -->|CodeGraph context| D["Coding"]
    D -->|ulw-loop verify| E{"Tests Pass?"}
    E -->|Yes| F["Git Push"]
    F -->|lb-CLI| G["K8s Deploy"]
    G -->|diagnose| H{"Healthy?"}
    H -->|Yes| I["Done"]
    H -->|No| J["Alert"]
    K["Bug Report"] -->|Agent monitors| L["Auto Fix"]
    L -->|logs + context| D
```

### Before vs After — 7 Stages Transformed

| Stage | Before (Manual) | After (AI-Driven) |
|-------|-----------------|-------------------|
| **Req Analysis** | Download PRD, read line-by-line, catch gaps by experience | Agent reads docs via CLI, auto-flags gaps & inconsistencies |
| **Design Spec** | Write manually, copy-paste to cloud doc; frontend complains docs lag behind code | Agent generates spec & syncs to cloud doc in real-time |
| **DB Config** | Manually switch config per git branch; forgot once → operated wrong DB | Git hook auto-syncs DSN on checkout, hot-reload |
| **Coding** | Write → compile → deploy → test (all manual); AI writes code but doesn't verify | ulw-loop: plan → code → build → test → **Oracle review** → redo on fail |
| **Deploy** | Open Kuboard → find Deployment → update image → wait → check logs | `git push` → CI → auto-deploy → health check → notify |
| **Diagnosis** | Copy GitLab CI / K8s logs → paste to AI → AI tells problem → human fixes | Agent reads logs directly via MCP, diagnoses, self-heals simple issues |
| **Bug Fix** | QA reports → locate → fix → deploy → notify (fix 5 min, workflow 4 hours) | Agent monitors bug list → auto-fix → verify → deploy → notify |

### ulw-loop: Self-Verification with Oracle Gate

```
Set Goal → Agent Implements → Self-Verify (build / test / LSP)
                                    ↓
                              Oracle Review
                               ↓         ↓
                            Pass       Reject → Redo from start
```

AI 写完代码不是终点。**Oracle 审核是最后一道门禁**——审核不通过就打回重做，持续 loop 直到通过。这确保了 AI 的输出质量有人把关，而不是"生成即交付"。

---

## 🧰 Tech Stack

| Domain | Technologies |
|--------|-------------|
| **Languages** | Go · Python · Shell |
| **Cloud Native** | Kubernetes · Docker · Kuboard |
| **CI/CD** | GitLab CI · Self-built CLI tools |
| **AI Coding** | OpenCode · Codex · Claude Code · Lark CLI |
| **Databases** | MySQL · Redis · MCP Server |
| **Knowledge** | CodeGraph · MCP Protocol |
| **Infra** | Linux · macOS · Nginx |

---

## 🚀 Open Source Projects

### 🌍 [opencode-skill-localizer](https://github.com/coder-wangbin/opencode-skill-localizer)
> Localize AI assistant skill descriptions without losing changes on `git pull`

- Uses `git update-index --skip-worktree` to protect local translations
- Batch replace `description` fields in `SKILL.md` files
- Symbolic link support for cross-directory skill discovery
- MIT License

### 🎯 [codex-goal-parallel](https://github.com/coder-wangbin/codex-goal-parallel)
> CodeX skill: automatic parallel task decomposition with sub-agent lifecycle management

### 🔧 DevOps Toolchain (Internal)

Built and maintain a full DevOps toolchain for the team:
- **K8s Operations MCP Server**: 11 tools — list_pods, get_logs, diagnose, events, restart_deployment, get_pipeline, get_job_logs, get_ingress, patch_ingress_tls, deployment_status, send_feishu_notification
- **Database MCP Server**: Agent-driven database queries with branch-switch auto-sync via Git hooks
- **Deploy CLI**: Kuboard SSO auth, Strategic Merge Patch, rolling updates, Feishu notifications
- **CodeGraph Integration**: Semantic code search via MCP — reduced token usage and tool calls

---

## 📊 GitHub Activity

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
