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
把整个 `job-hunt-coach/` 目录放到你的 Claude skills 目录下：

- **个人全局（推荐）**
  - macOS / Linux：`~/.claude/skills/job-hunt-coach/`
  - Windows：`%USERPROFILE%\.claude\skills\job-hunt-coach\`
- 或放某个项目内：`<项目>/.claude/skills/job-hunt-coach/`

用 git：
```bash
cd ~/.claude/skills
git clone <仓库地址> job-hunt-coach
```

放好后，新开一个 Claude 会话，提到任何求职 / 面试 / 简历 / 谈薪相关的事，skill 会自动触发。也可以直接说"用 job-hunt-coach 帮我准备面试"。

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
