# job-hunt-coach

一个面向 Claude（Claude Code / Claude.ai）的求职教练 **Agent Skill**。基于"**面试是博弈，不是证明自己**"的方法论，覆盖求职全链条：简历优化、自我介绍、高频难题应对、gap 与转行叙事、薪资谈判。

它给的是**表达策略和博弈框架**——帮你把真实的本事讲清楚、在求职中掌握主动权，同时坚守"**不造假、不过度包装**"的诚实底线。

## 它能帮你做什么
- 把简历从"自传"改成"广告"（动作 + 数据 + 价值、过 ATS、一岗一份）
- 设计自我介绍（锚定核心标签、留追问钩子）
- 应对"你的缺点 / 为什么离职 / 为什么适合"等高频难题
- 把 gap 空窗期和转行讲成优势
- 薪资谈判（调研定区间、不先报价、三种报价逻辑、24h 缓冲）
- 模拟面试、陪练追问

## 安装

> 前提：需要装了 `git`。

### 方式一：让 AI agent 帮你装（最省事，推荐）

如果你用 Claude Code（或其它能跑命令的编码 agent），**把下面这段话整段贴给它**，它会帮你克隆并装好：

```text
帮我装一个 Claude Code 的 skill（一个求职面试教练，叫 job-hunt-coach）。

请用 git 把这个公开仓库克隆到我的个人 skills 目录：
  仓库：https://github.com/forestlii/job-hunt-coach.git
  目标：~/.claude/skills/job-hunt-coach
  （Windows 就是 %USERPROFILE%\.claude\skills\job-hunt-coach；
   如果 .claude\skills 目录还没有，先建好它。）

装完帮我确认 SKILL.md 在 ~/.claude/skills/job-hunt-coach/ 下，
并告诉我是不是要新开一个会话它才生效、以及我该怎么触发它。
```

> 💡 agent 跑 `git clone` 时可能弹一次权限确认，点允许即可。

### 方式二：自己用 git 装

```bash
# macOS / Linux
git clone https://github.com/forestlii/job-hunt-coach.git ~/.claude/skills/job-hunt-coach
```
```powershell
# Windows PowerShell
git clone https://github.com/forestlii/job-hunt-coach.git $env:USERPROFILE\.claude\skills\job-hunt-coach
```

也可以装在某个项目内：`<项目>/.claude/skills/job-hunt-coach/`。

### 装完怎么生效

skill 列表是在**会话启动时**加载的，所以装完要**新开一个会话**（或重启 Claude Code）它才会出现。之后提到任何求职 / 面试 / 简历 / 谈薪相关的事，skill 会自动触发；也可以直接说"用 job-hunt-coach 帮我准备面试"。

## 怎么用
直接说你的诉求，并尽量提供：
- 目标**岗位 / JD**（贴原文最好）
- 你的**真实经历**（做过什么、有什么成果 / 数字）
- 你的**目标和顾虑**

越具体，教练给的越是为你定制、能落地的东西，而不是通用模板。

## 结构
```
job-hunt-coach/
├── SKILL.md                  # 核心：博弈论内核 + 诚实底线 + 工作流 + 路由
└── references/
    ├── resume.md             # 简历优化（广告思维四步）
    ├── self-introduction.md  # 自我介绍（锚定法则）
    ├── tough-questions.md    # 高频难题（缺点 / 离职 / 适配）
    ├── gap-and-pivot.md      # gap 与转行叙事
    └── salary-negotiation.md # 薪资谈判
```

## 来源
方法论提炼自公开的求职经验分享内容，整理成结构化的 skill。它不替你造假——教练的价值在于帮人把真本事讲清楚。

## License
MIT。可按需修改 / 再分发。
