<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&duration=3000&pause=1000&color=0969DA&center=true&vCenter=true&width=650&lines=Hi%2C+I'm+%E7%8E%8B%E5%BD%AC+(coder-wangbin);Go+Backend+Developer;AI-Driven+Full-Chain+Workflow+Builder;K8s+%2B+DevOps+Toolchain+Designer" alt="Typing SVG" />
</p>

---

## 👨‍💻 About Me

Go 后端开发工程师。我花了半年时间把 AI 从"只会写代码"变成了"能跟着研发链路从头走到尾"——设计并落地了一套 AI 驱动的全链路研发工具链，覆盖需求分析、方案设计、编码自验证、K8s 自动部署、日志诊断、Bug 自修复。

- ⚡ 自研 **lb CLI + MCP Server**（11 个 MCP 工具），让 AI Agent 能直接操作 K8s 和 GitLab CI
- 🧩 打通 **lark-cli ＋ dbhub MCP ＋ CodeGraph**，形成从需求到交付的完整闭环
- 🌱 深度使用 **OpenCode ulw-loop / Codex goal** 做 AI 辅助开发
- 🪝 设计 **Git post-checkout hook ＋ dbhub**，分支切换自动同步数据库配置

---

## 🏗️ AI-Driven Full-Chain Development Workflow

我把传统研发流程中 AI 帮不上忙的环节逐个击破，串成了一条可执行、可回流的管线：

```mermaid
flowchart LR
    A["PRD Doc"] -->|Agent reads| B["Requirement Analysis"]
    B -->|Agent writes| C["Design Spec"]
    C -->|CodeGraph context| D["Coding"]
    D -->|ulw-loop self-verify| E{"Tests Pass?"}
    E -->|Yes| F["Git Push"]
    F -->|lb-CLI| G["K8s Auto Deploy"]
    G -->|lb-diagnose| H{"Healthy?"}
    H -->|Yes| I["Done"]
    H -->|No| J["Alert"]
    K["Bug Report"] -->|Agent monitors| L["Auto Fix"]
    L -->|CodeGraph + lb logs| D
```

### Key Capabilities Built

| Stage | Before | After |
|-------|--------|-------|
| **Requirement Analysis** | Manual PRD reading, missed edge cases | AI reads docs automatically, flags gaps & inconsistencies |
| **Design Spec** | Write manually, copy-paste to docs | AI generates spec & syncs to cloud doc |
| **Coding** | Write → compile → deploy → test (manual) | ulw-loop: plan → code → build → test → Oracle review → redo on fail |
| **DB Config** | Manually switch config per branch | Git hook auto-syncs DSN on checkout |
| **Deploy** | Open Kuboard → update image → wait → check logs | `git push` → CI → lb auto-deploy → health check → notify |
| **Diagnosis** | Copy GitLab CI / K8s logs → paste to AI | Agent reads logs directly via lb MCP, diagnoses, self-heals simple issues |
| **Bug Fix** | QA reports → manual locate → fix → deploy | Agent monitors bug list → auto-fix → verify → deploy → notify |

### ulw-loop: Continuous Self-Verification with Oracle Gate

```
Set Goal → Agent Implements → Self-Verify (build/test/LSP) → Oracle Review
                                                              ├─ Reject → Redo from start
                                                              └─ Pass → Deliver
```

The Oracle review gate is the critical last step — AI doesn't ship until a separate reviewer agent approves. No approval = kicked back for redo. This loop continues until all checks pass **and** the reviewer signs off.

---

## 🧰 Tech Stack

| Domain | Technologies |
|--------|-------------|
| **Languages** | Go · Python · Shell |
| **Cloud Native** | Kubernetes · Docker · Kuboard |
| **CI/CD** | GitLab CI · lb CLI (self-built) |
| **AI Coding** | OpenCode · Codex · Claude Code · lark-cli |
| **Databases** | MySQL · Redis · dbhub MCP |
| **Infra** | Linux · macOS · Nginx · CodeGraph |

---

## 🚀 Featured Projects

### 🔧 lb CLI + MCP Server
> K8s deploy, diagnose & operate — all from AI Agent

- **11 MCP tools**: list_pods · get_logs · diagnose · events · restart_deployment · get_pipeline · get_job_logs · get_ingress · patch_ingress_tls · send_feishu_notification · deployment_status
- Kuboard SSO auth (5-step auto)
- Strategic Merge Patch for rolling updates
- Built-in Feishu notification (one aggregated message per push)

### 🗄️ dbhub MCP + Git Hook Auto-Sync
> Never manually switch database config on branch change again

- `post-checkout` hook detects branch switch → reads `conf.yml` DSN
- Auto-converts Go-format DSN → MySQL format
- Writes to `dbhub.toml` → config-watcher hot-reloads
- Multi-project support via `<project>-current` source IDs

### 🌍 [opencode-skill-localizer](https://github.com/coder-wangbin/opencode-skill-localizer)
> Localize AI assistant skill descriptions without losing changes on `git pull`

- Uses `git update-index --skip-worktree` to protect local translations
- Batch replace `description` fields in `SKILL.md` files
- Symbolic links for skill discovery across directories

### 🎯 [codex-goal-parallel](https://github.com/coder-wangbin/codex-goal-parallel)
> CodeX skill: automatic parallel task decomposition with sub-agent lifecycle management

---

## 📊 Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=coder-wangbin&show_icons=true&hide_border=true&count_private=true" height="150" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=coder-wangbin&layout=compact&hide_border=true" height="150" />
</p>

---

<p align="center">
  <i>"The bottleneck is not the model — it's the engineering system outside the model."</i>
</p>
