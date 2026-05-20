# Awesome Claude Skills 中文版

> 精选优质 Claude skills 收录，中文社区优先。
> A curated, Chinese-first list of high-quality Claude skills.

---

## 是什么？

**Claude Skill** 是给 Claude 的一项可复用、可组合的"专长"——例如让它按团队规范写 commit、阅读某种格式的日志、自动化某个开发工作流。每个 skill 通常是一个目录，包含 `SKILL.md` 描述文件和相关脚本/模板，放在 `~/.claude/skills/` 下即可被 Claude Code 自动识别。

国内开发者在寻找好用的 Claude skill 时，常常被英文资料和分散的 marketplace 劝退。本仓库的目标是：

- 用**中文**为每个 skill 写清楚"是什么、什么时候用、怎么用"
- 按**使用场景**而不是字母分类，让你能直接找到对路的工具
- 只收**真正有人用过、能跑通**的 skill，宁缺毋滥

收录范围：

- **Claude Code Skills**：`SKILL.md` 格式 skill（主体）
- **通用 Prompt 模板**：跨 agent 可用的精选 prompt（附录）

---

## 目录

- [开发辅助](#开发辅助)
- [文档与写作](#文档与写作)
- [数据处理](#数据处理)
- [运维部署](#运维部署)
- [学习研究](#学习研究)
- [设计与创意](#设计与创意)
- [通用 Prompt 模板](#通用-prompt-模板)
- [相关资源](#相关资源)
- [如何贡献](#如何贡献)

---

## Claude Code Skills

每条收录使用如下格式：

> **[Skill 名称](链接)** — 一句话中文介绍。
> **什么时候用：** 适用场景。
> **作者：** [@username](链接)　**标签：** `tag1` `tag2`

### 开发辅助

> 代码 review、调试、重构、测试生成、版本管理等开发流程中的辅助技能。

- **[claude-code-skills-zh](https://github.com/laolaoshiren/claude-code-skills-zh)** — 精选 100+ Claude Code skill 的中文合集，含 18 个原创可直接安装的中文 skill（zh-code-reviewer、zh-readme 等）。
  **什么时候用：** 想用中文母语做代码 review 或生成中文 README，避免英文 skill 的"翻译腔"输出时。
  **作者：** [@laolaoshiren](https://github.com/laolaoshiren)　**标签：** `合集` `代码审查` `README` `中文输出`

- **[yunshu_skillshub](https://github.com/yunshu0909/yunshu_skillshub)** — 云舒整理的 Claude Code skill 集合，覆盖周报、PRD、UI 设计、需求分析等开发与产品工作流。
  **什么时候用：** 需要从 git commit / 会议记录自动生成周报，或做产品需求文档与 UI 风格迭代时。
  **作者：** [@yunshu0909](https://github.com/yunshu0909)　**标签：** `合集` `周报` `PRD` `产品管理`

- **[claude-skills-suite](https://github.com/joneqian/claude-skills-suite)** — 全栈 skill 套件：14 个 Agents + 16 个 Commands + 40 个 Skills，含 D3 可视化、PostgreSQL/MySQL、微信小程序等国内技术栈。
  **什么时候用：** 想要一个开箱即用的大套件，尤其是涉及国内技术栈（微信小程序、TDesign）时。
  **作者：** [@joneqian](https://github.com/joneqian)　**标签：** `合集` `全栈` `微信小程序` `数据库`

- **[huangwb8/skills](https://github.com/huangwb8/skills)** — Claude Code & Codex 通用 skill 开发流水线脚手架，含项目初始化、测试、Git 自动化模板。
  **什么时候用：** 自己写新 skill 时不想从零搭基础结构，或想跨 Claude Code / Codex 平台时。
  **作者：** [@huangwb8](https://github.com/huangwb8)　**标签：** `脚手架` `开发流水线` `Codex 兼容`

### 文档与写作

> 技术文档、PR 描述、commit 信息、周报、README 生成等写作场景。

- **[baoyu-skills](https://github.com/JimLiu/baoyu-skills)** — 宝玉的 20+ 内容创作 skill 合集，含小红书卡片、信息图、SVG 图解、文章插图，以及公众号/微博/X 一键发布。
  **什么时候用：** 做自媒体内容、技术博客配图、社交平台多平台分发时——中文创作生态目前最成熟的工具集。
  **作者：** [@JimLiu](https://github.com/JimLiu)　**标签：** `合集` `自媒体` `小红书` `公众号` `配图`

- **[md2wechat-skill](https://github.com/geekjourneyx/md2wechat-skill)** — Markdown 转公众号排版，40+ 主题与 43 个版式组件，支持 AI 配图与一键推送草稿。
  **什么时候用：** 公众号文章排版调样式调到崩溃时——给它一个 Markdown 文件，剩下交给它。
  **作者：** [@geekjourneyx](https://github.com/geekjourneyx)　**标签：** `公众号` `排版` `Markdown`

- **[qiaomu-anything-to-notebooklm](https://github.com/joeseesun/qiaomu-anything-to-notebooklm)** — 乔木的多源内容处理 skill，把微信文章、网页、YouTube、PDF 转成 NotebookLM 播客、PPT、思维导图、测验。
  **什么时候用：** 想把零散学习材料（公众号收藏 / 长视频 / 论文）自动整理成播客或学习卡片时。
  **作者：** [@joeseesun](https://github.com/joeseesun)　**标签：** `NotebookLM` `内容转换` `微信文章` `播客`

- **[wewrite](https://github.com/oaker-io/wewrite)** — 公众号文章全流程 skill：热点抓取 → 选题 → 写作 → SEO → AI 配图 → 排版 → 微信草稿箱推送。
  **什么时候用：** 自媒体作者想一句命令跑完整公众号发文流水线时。
  **作者：** [@oaker-io](https://github.com/oaker-io)　**标签：** `公众号` `全流程` `自媒体` `选题`

- **[XiaohongshuSkills](https://github.com/white0dew/XiaohongshuSkills)** — 小红书自动发布、评论、检索 skill，支持多账号与无头模式，兼容 OpenClaw / Codex / Claude Code。
  **什么时候用：** 做小红书运营需要批量发笔记、自动回复评论、抓取数据时。
  **作者：** [@white0dew](https://github.com/white0dew)　**标签：** `小红书` `自动化` `多账号` `运营`

- **[Viral_Writer_Skill](https://github.com/nashsu/Viral_Writer_Skill)** — 基于 11 个内容洞见维度的自媒体创作 skill，输入主题输出完整文章 + 5 个备选标题 + 每张配图的生成 prompt。
  **什么时候用：** 写自媒体爆款标题困难、或想要系统化的内容创作方法论时。
  **作者：** [@nashsu](https://github.com/nashsu)　**标签：** `爆款` `自媒体` `标题党` `配图 prompt`

### 数据处理

> CSV/Excel 处理、SQL 查询、数据清洗、可视化、报表生成等。

- **[skills_collection](https://github.com/wwwzhouhui/skills_collection)** — 个人开发的 Claude Code skill 集合，其中 excel-report-generator 可从 CSV/DataFrame/数据库自动生成带图表样式的专业 Excel 报表。
  **什么时候用：** 需要给老板出报表、把数据库查询结果整理成可发邮件的 Excel 时。
  **作者：** [@wwwzhouhui](https://github.com/wwwzhouhui)　**标签：** `合集` `Excel` `报表` `办公自动化`

- **[duckdb-skills](https://github.com/duckdb/duckdb-skills)** — DuckDB 官方 skill 合集，用 SQL 直接查询本地 CSV / Parquet / JSON / Excel / SQLite，支持 S3 / GCS 远程文件。（英文项目）
  **什么时候用：** 不想 import pandas、但想用 SQL 快速对一堆本地数据文件做分析时。
  **作者：** [@duckdb](https://github.com/duckdb)　**标签：** `SQL` `DuckDB` `CSV` `Parquet` `官方`

### 运维部署

> CI/CD、Docker、Kubernetes、云服务配置、日志分析、监控告警等。

- **[kubernetes-skill](https://github.com/LukasNiessen/kubernetes-skill)** — failure-mode-first 生成 K8s manifest，覆盖 NSA/CISA/CIS 安全基准与 Helm/Kustomize。（英文项目）
  **什么时候用：** 让 Claude 写 K8s YAML 但担心幻觉、或需要满足合规基准时。
  **作者：** [@LukasNiessen](https://github.com/LukasNiessen)　**标签：** `K8s` `Helm` `Kustomize` `合规`

> 📢 **本分类仍在招募中文社区原创**：目前条目以英文项目为主。如果你写过或用过好用的 K8s / CI/CD / 监控类**中文** skill，欢迎通过 [PR](CONTRIBUTING.md) 或 [issue](../../issues/new/choose) 推荐。

### 学习研究

> 论文阅读、知识整理、笔记生成、概念解释、学习计划等。

- **[codex-claude-academic-skills](https://github.com/zLanqing/codex-claude-academic-skills)** — 中文科研工作流三件套：论文阅读 + 学术 PPT 生成、写作润色与审稿回复、MATLAB/Python 科学计算与期刊级绘图。
  **什么时候用：** 国内高校与科研人员做文献综述、写论文、回审稿意见、画发表用图表时。
  **作者：** [@zLanqing](https://github.com/zLanqing)　**标签：** `科研` `论文` `学术写作` `MATLAB` `Python`

- **[interview-master-skill](https://github.com/chen3tu/interview-master-skill)** — 求职面试全流程 skill：公司七维分析 + STAR-R 法则简历 + 模拟面试 + 薪资谈判。
  **什么时候用：** 准备面试、复盘 offer、谈判薪资时——比通用建议更结构化。
  **作者：** [@chen3tu](https://github.com/chen3tu)　**标签：** `求职` `面试` `STAR-R` `薪资谈判`

### 设计与创意

> UI/UX 评审、文案创作、命名建议、配色与排版、原型生成等。

- **[huashu-design](https://github.com/alchaincyf/huashu-design)** — 花叔的 HTML 原生设计 skill，一句话产出高保真原型、幻灯片、动画、印刷级海报，内置 20 套设计哲学。
  **什么时候用：** 想要 Claude 生成不像"AI 默认审美"的视觉作品时——产品发布动画、可点击 App 原型、印刷信息图都能搞定。
  **作者：** [@alchaincyf](https://github.com/alchaincyf) (花叔)　**标签：** `HTML` `原型` `动画` `海报` `印刷级`

- **[NanoBanana-PPT-Skills](https://github.com/op7418/NanoBanana-PPT-Skills)** — 归藏的 AI 自动 PPT 工具，生成 2K/4K 杂志风 / 科研汇报 PPT 图片，支持智能转场视频与交互式播放。
  **什么时候用：** 临时要 PPT 但没设计感、或想做 AI 风格的杂志级幻灯片时。
  **作者：** [@op7418](https://github.com/op7418) (归藏)　**标签：** `PPT` `Gemini` `转场动画` `4K`

- **[claude-design-skill](https://github.com/jiji262/claude-design-skill)** — 复刻 Claude.ai 内部 Design 系统 prompt，让 Claude 输出 HTML deck、landing page、原型、动画、海报。
  **什么时候用：** 想要 Claude 生成不像"AI 默认审美"的视觉输出时——能产出更接近 Claude.ai 官方风格的设计。
  **作者：** [@jiji262](https://github.com/jiji262)　**标签：** `HTML` `原型` `landing page` `海报`

---

## 通用 Prompt 模板

> 这部分收录跟具体 agent 无关、能在 Claude / ChatGPT / Gemini 等多个平台通用的精选 prompt 模板。

_暂无收录，欢迎贡献你常用且效果好的 prompt 模板。_

---

## 相关资源

**官方文档与仓库**

- [Claude Code 官方文档](https://docs.claude.com/claude-code)
- [anthropics/skills](https://github.com/anthropics/skills) — Anthropic 官方 skills 仓库（13.7 万 ★），含 canvas-design、pdf 等基线 skill，可视为所有 Claude skill 的"标准库"
- [Anthropic 官方 plugins 仓库](https://github.com/anthropics/claude-plugins-official)

**其他优秀的 skills 收集项目**（英文为主，欢迎参考）

- [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) — 综合性 AI agent skills 列表
- [travisvn/awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills) — Claude 专属 awesome 列表
- [tech-leads-club/agent-skills](https://github.com/tech-leads-club/agent-skills) — agent skills 收集

如果你知道更多优秀的中文/英文 skill 项目，欢迎通过 PR 补充到这里。

---

## 如何贡献

我们欢迎两种贡献方式：

1. **PR**：直接编辑 README.md，按格式补充 skill 条目。请阅读 [CONTRIBUTING.md](CONTRIBUTING.md) 了解收录标准和格式规范。
2. **Issue 推荐**：如果你只是知道一个不错的 skill 但不想自己写描述，[开一个 issue](../../issues/new/choose) 告诉我们就好，我们会整理。

收录标准简述：

- 必须真实可用，能在 Claude Code 里跑通
- 有清晰的 `SKILL.md` 或等价说明文档
- 解决具体问题，而不是"hello world"级示例
- 作者活跃维护（最近 6 个月有更新优先）

完整规范见 [CONTRIBUTING.md](CONTRIBUTING.md)。

---

## License

本仓库内容采用 [CC0 1.0 公共领域贡献](LICENSE) 协议——你可以自由使用、修改、分发，无需署名。

被收录的各 skill 项目本身遵循其各自的开源协议，请前往原仓库查看。
