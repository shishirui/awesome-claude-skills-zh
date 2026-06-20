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

- **[yunshu_skillshub](https://github.com/yunshu0909/yunshu_skillshub)** — 云舒整理的 Claude Code skill 集合，覆盖周报、PRD、UI 设计、需求分析等开发与产品工作流。
  **什么时候用：** 需要从 git commit / 会议记录自动生成周报，或做产品需求文档与 UI 风格迭代时。
  **作者：** [@yunshu0909](https://github.com/yunshu0909)　**标签：** `合集` `周报` `PRD` `产品管理`

- **[everything-claude-code-zh](https://github.com/xu-xiang/everything-claude-code-zh)** — Anthropic 黑客松冠军方案的中文化，50+ skill 覆盖 TDD、安全审查、Docker、CI/CD 等工程化场景。
  **什么时候用：** 想搭一套生产级 Claude Code 工程化配置（agents + skills + hooks + commands + MCP）时。
  **作者：** [@xu-xiang](https://github.com/xu-xiang)　**标签：** `工程化` `TDD` `安全审查` `黑客松冠军`

- **[embeddedskills](https://github.com/zhinkgit/embeddedskills)** — 嵌入式开发 11 skill：Keil/GCC 编译 + J-Link/OpenOCD 调试 + 串口/CAN/网络通信 + 工作流编排。
  **什么时候用：** 做单片机、RTOS、硬件验证全流程自动化时——填补"嵌入式 + Claude Code"空白。
  **作者：** [@zhinkgit](https://github.com/zhinkgit)　**标签：** `嵌入式` `单片机` `Keil` `OpenOCD`

- **[huangshu](https://github.com/Backtthefuture/huangshu)** — 黄叔的 Claude Code 工具合集：12 专家智囊团、社交人格、视频转录、本地 Skill Hub 管理 UI。
  **什么时候用：** 想做商业决策模拟、视频字幕，或本地有大量 skill 需要 UI 化管理时。
  **作者：** [@Backtthefuture](https://github.com/Backtthefuture) (黄叔)　**标签：** `合集` `智囊团` `Skill Hub` `视频转录`

- **[claude-code-skills-zh](https://github.com/laolaoshiren/claude-code-skills-zh)** — 精选 100+ Claude Code skill 的中文合集，含 18 个原创可直接安装的中文 skill（zh-code-reviewer、zh-readme 等）。
  **什么时候用：** 想用中文母语做代码 review 或生成中文 README，避免英文 skill 的"翻译腔"输出时。
  **作者：** [@laolaoshiren](https://github.com/laolaoshiren)　**标签：** `合集` `代码审查` `README` `中文输出`

- **[huangwb8/skills](https://github.com/huangwb8/skills)** — Claude Code & Codex 通用 skill 开发流水线脚手架，含项目初始化、测试、Git 自动化模板。
  **什么时候用：** 自己写新 skill 时不想从零搭基础结构，或想跨 Claude Code / Codex 平台时。
  **作者：** [@huangwb8](https://github.com/huangwb8)　**标签：** `脚手架` `开发流水线` `Codex 兼容`

- **[ax-extract-workflow](https://github.com/Necmttn/ax/tree/main/skills/ax-extract-workflow)** — 基于本地 ax 会话、提交记录、skill 使用和 sub-agent 活动，还原 PR、功能或报告的交付过程。
  **什么时候用：** 需要复盘一次交付、提炼可复用流程，或梳理 agent 协作过程时。
  **作者：** [@Necmttn](https://github.com/Necmttn)　**标签：** `工作流复盘` `agent协作` `本地记录` `Claude Code`

- **[claude-skills-suite](https://github.com/joneqian/claude-skills-suite)** — 全栈 skill 套件：14 个 Agents + 16 个 Commands + 40 个 Skills，含 D3 可视化、PostgreSQL/MySQL、微信小程序等国内技术栈。
  **什么时候用：** 想要一个开箱即用的大套件，尤其是涉及国内技术栈（微信小程序、TDesign）时。
  **作者：** [@joneqian](https://github.com/joneqian)　**标签：** `合集` `全栈` `微信小程序` `数据库`

### 文档与写作

> 技术文档、PR 描述、commit 信息、周报、README 生成等写作场景。

- **[baoyu-skills](https://github.com/JimLiu/baoyu-skills)** — 宝玉的 20+ 内容创作 skill 合集，含小红书卡片、信息图、SVG 图解、文章插图，以及公众号/微博/X 一键发布。
  **什么时候用：** 做自媒体内容、技术博客配图、社交平台多平台分发时——中文创作生态目前最成熟的工具集。
  **作者：** [@JimLiu](https://github.com/JimLiu)　**标签：** `合集` `自媒体` `小红书` `公众号` `配图`

- **[webnovel-writer](https://github.com/lingfengQAQ/webnovel-writer)** — 长篇网文辅助系统，支持 200 万字量级，RAG + 实体图 + 长期记忆解决"AI 遗忘/幻觉"。
  **什么时候用：** 连载长篇小说、要保证人物/世界观跨章节一致性时。
  **作者：** [@lingfengQAQ](https://github.com/lingfengQAQ)　**标签：** `长篇网文` `RAG` `长期记忆` `连载`

- **[qiaomu-anything-to-notebooklm](https://github.com/joeseesun/qiaomu-anything-to-notebooklm)** — 乔木的多源内容处理 skill，把微信文章、网页、YouTube、PDF 转成 NotebookLM 播客、PPT、思维导图、测验。
  **什么时候用：** 想把零散学习材料（公众号收藏 / 长视频 / 论文）自动整理成播客或学习卡片时。
  **作者：** [@joeseesun](https://github.com/joeseesun)　**标签：** `NotebookLM` `内容转换` `微信文章` `播客`

- **[XiaohongshuSkills](https://github.com/white0dew/XiaohongshuSkills)** — 小红书自动发布、评论、检索 skill，支持多账号与无头模式，兼容 OpenClaw / Codex / Claude Code。
  **什么时候用：** 做小红书运营需要批量发笔记、自动回复评论、抓取数据时。
  **作者：** [@white0dew](https://github.com/white0dew)　**标签：** `小红书` `自动化` `多账号` `运营`

- **[md2wechat-skill](https://github.com/geekjourneyx/md2wechat-skill)** — Markdown 转公众号排版，40+ 主题与 43 个版式组件，支持 AI 配图与一键推送草稿。
  **什么时候用：** 公众号文章排版调样式调到崩溃时——给它一个 Markdown 文件，剩下交给它。
  **作者：** [@geekjourneyx](https://github.com/geekjourneyx)　**标签：** `公众号` `排版` `Markdown`

- **[wewrite](https://github.com/oaker-io/wewrite)** — 公众号文章全流程 skill：热点抓取 → 选题 → 写作 → SEO → AI 配图 → 排版 → 微信草稿箱推送。
  **什么时候用：** 自媒体作者想一句命令跑完整公众号发文流水线时。
  **作者：** [@oaker-io](https://github.com/oaker-io)　**标签：** `公众号` `全流程` `自媒体` `选题`

- **[chinese-novelist-skill](https://github.com/PenglongHuang/chinese-novelist-skill)** — 三层递进式问答 + 跨会话偏好记忆 + 章末悬念钩子，可一次性产出整本长篇。
  **什么时候用：** 想"一句话开始一本小说"的休闲创作场景、对配置简单度有要求时。
  **作者：** [@PenglongHuang](https://github.com/PenglongHuang)　**标签：** `长篇小说` `偏好记忆` `中断续写` `休闲创作`

- **[oh-story-claudecode](https://github.com/worldwonderer/oh-story-claudecode)** — 网文小说全流程 skill 包：扫榜 → 拆文 → 写作 → 去 AI 味 → 封面，覆盖长篇短篇。
  **什么时候用：** 网络文学作者要做番茄/晋江/起点商业化写作时——商业化方法论 + 反 AI 味输出。
  **作者：** [@worldwonderer](https://github.com/worldwonderer)　**标签：** `网文` `商业写作` `去AI味` `封面`

- **[translate-book](https://github.com/deusyu/translate-book)** — 整本书翻译（PDF/DOCX/EPUB），8 个并行 sub-agent + 术语表 + SHA-256 校验，覆盖中日韩英法德西。
  **什么时候用：** 要批量翻译技术书、报告、合同时——超出段落级翻译的工程化方案。
  **作者：** [@deusyu](https://github.com/deusyu)　**标签：** `整书翻译` `并行Agent` `术语表` `EPUB`

- **[Viral_Writer_Skill](https://github.com/nashsu/Viral_Writer_Skill)** — 基于 11 个内容洞见维度的自媒体创作 skill，输入主题输出完整文章 + 5 个备选标题 + 每张配图的生成 prompt。
  **什么时候用：** 写自媒体爆款标题困难、或想要系统化的内容创作方法论时。
  **作者：** [@nashsu](https://github.com/nashsu)　**标签：** `爆款` `自媒体` `标题党` `配图 prompt`

- **[makeownsrt](https://github.com/joshhu/makeownsrt)** — MKV/MP4 抽字幕 → 翻译成繁中双语 SRT，无字幕时 Whisper 兜底，支持 19 语对。
  **什么时候用：** 海外剧/纪录片做双语字幕、或做语言学习用的对照字幕时。
  **作者：** [@joshhu](https://github.com/joshhu)　**标签：** `字幕` `双语SRT` `Whisper` `繁中`

- **[video-to-subtitle-summary-skill](https://github.com/imlewc/video-to-subtitle-summary-skill)** — 抖音/小红书/B 站/YouTube 视频转字幕 + AI 总结，本地 faster-whisper 或火山引擎双后端。
  **什么时候用：** 批量做短视频字幕、信息流摘要时——中文短视频平台全覆盖。
  **作者：** [@imlewc](https://github.com/imlewc)　**标签：** `视频字幕` `Whisper` `抖音` `B站`

### 数据处理

> CSV/Excel 处理、SQL 查询、数据清洗、可视化、报表生成等。

- **[duckdb-skills](https://github.com/duckdb/duckdb-skills)** — DuckDB 官方 skill 合集，用 SQL 直接查询本地 CSV / Parquet / JSON / Excel / SQLite，支持 S3 / GCS 远程文件。（英文项目）
  **什么时候用：** 不想 import pandas、但想用 SQL 快速对一堆本地数据文件做分析时。
  **作者：** [@duckdb](https://github.com/duckdb)　**标签：** `SQL` `DuckDB` `CSV` `Parquet` `官方`

- **[xhs-claude-skills](https://github.com/chenxiachan/xhs-claude-skills)** — 小红书帖子抓取 → 结构化 Obsidian 笔记 + 视频本地 mlx-whisper 转写。
  **什么时候用：** 把小红书种草内容沉淀到第二大脑、或建本地内容素材库时。
  **作者：** [@chenxiachan](https://github.com/chenxiachan)　**标签：** `小红书` `Obsidian` `素材库` `Whisper`

- **[skills_collection](https://github.com/wwwzhouhui/skills_collection)** — 个人开发的 Claude Code skill 集合，其中 excel-report-generator 可从 CSV/DataFrame/数据库自动生成带图表样式的专业 Excel 报表。
  **什么时候用：** 需要给老板出报表、把数据库查询结果整理成可发邮件的 Excel 时。
  **作者：** [@wwwzhouhui](https://github.com/wwwzhouhui)　**标签：** `合集` `Excel` `报表` `办公自动化`

- **[finance-quant-skills](https://github.com/lzwme/finance-quant-skills)** — A 股量化交易 11 skill，覆盖 BaoStock/AKShare/Tushare/Backtrader/RQAlpha 等中文金融数据生态。
  **什么时候用：** 做 A 股量化策略、回测、因子研究、券商接口对接时——中文金融场景独此一家。
  **作者：** [@lzwme](https://github.com/lzwme)　**标签：** `量化` `A股` `回测` `金融`

### 运维部署

> CI/CD、Docker、Kubernetes、云服务配置、日志分析、监控告警等。

- **[full-stack-skills](https://github.com/partme-ai/full-stack-skills)** — 421 个 SKILL.md 跨 42 组，覆盖 Spring/Node/Go/Vue/React/Docker/数据库/测试等基础设施。
  **什么时候用：** 需要一站式拿到运维 + 后端 + 前端 + 测试成熟模板时——同时覆盖开发辅助。
  **作者：** [@partme-ai](https://github.com/partme-ai)　**标签：** `合集` `全栈` `Docker` `数据库`

- **[kubernetes-skill](https://github.com/LukasNiessen/kubernetes-skill)** — failure-mode-first 生成 K8s manifest，覆盖 NSA/CISA/CIS 安全基准与 Helm/Kustomize。（英文项目）
  **什么时候用：** 让 Claude 写 K8s YAML 但担心幻觉、或需要满足合规基准时。
  **作者：** [@LukasNiessen](https://github.com/LukasNiessen)　**标签：** `K8s` `Helm` `Kustomize` `合规`

- **[jeecgboot/skills](https://github.com/jeecgboot/skills)** — JeecgBoot × 积木报表官方 skill，一句话生成代码/表单/流程/报表/大屏。
  **什么时候用：** 基于 JeecgBoot 低代码平台做企业应用、报表、大屏开发时。
  **作者：** [@jeecgboot](https://github.com/jeecgboot)　**标签：** `低代码` `企业开发` `报表` `大屏`

- **[Commonly-used-high-value-skills](https://github.com/seaworld008/Commonly-used-high-value-skills)** — 289 个高价值 skill 横跨 16 类，含 observability-designer、senior-devops、incident-commander 等 SRE 角色。
  **什么时候用：** 需要可观测性方案、应急响应 runbook、SRE 日常自动化时——中文 SRE 维度最完整。
  **作者：** [@seaworld008](https://github.com/seaworld008)　**标签：** `合集` `SRE` `可观测性` `应急响应`

### 学习研究

> 论文阅读、知识整理、笔记生成、概念解释、学习计划等。

- **[Auto-claude-code-research-in-sleep](https://github.com/wanshuiyin/Auto-claude-code-research-in-sleep)** — "睡觉时跑科研"：5 阶段流水线（idea/实验/审稿/论文/rebuttal），74 个 skill，支持 Kimi/DeepSeek/GLM/MiniMax。
  **什么时候用：** ML 实验需要长时间无人值守、想 Claude + 国产模型协作时——中文科研自动化最高 star。
  **作者：** [@wanshuiyin](https://github.com/wanshuiyin)　**标签：** `自动科研` `跨模型协作` `ML实验` `Overleaf`

- **[claude-scholar](https://github.com/Galaxy-Dawn/claude-scholar)** — CS/AI 方向研究生工具包：25 skill + 2 agent + 30+ command，含 paper-miner、kaggle-miner、Nature 风格润色、rebuttal。
  **什么时候用：** 做 ML 文献综述、跑 Kaggle 实验、写论文、回审意见时。
  **作者：** [@Galaxy-Dawn](https://github.com/Galaxy-Dawn)　**标签：** `学术` `Kaggle` `论文写作` `审稿回复`

- **[obsidian-ai-orange-book](https://github.com/alchaincyf/obsidian-ai-orange-book)** — 花叔《Obsidian × Claude Code 重建第二大脑》方法论 PDF + 工具：7 个工作流、vault 架构、Git 版本控制。
  **什么时候用：** 从零搭一个 AI 友好的 Obsidian 知识库时。
  **作者：** [@alchaincyf](https://github.com/alchaincyf) (花叔)　**标签：** `Obsidian` `第二大脑` `知识管理` `橙皮书`

- **[dailypaper-skills](https://github.com/huangkiki/dailypaper-skills)** — 每日 HuggingFace/arXiv 论文流水线：扫单 → 分级 → 解读 → 概念笔记 → 落地 Obsidian，跨日去重。
  **什么时候用：** 每天/每周想被自动喂论文、有 Obsidian/Zotero 知识库的研究者。
  **作者：** [@huangkiki](https://github.com/huangkiki)　**标签：** `论文` `每日推送` `Obsidian` `Zotero`

- **[gs-skills](https://github.com/cookjohn/gs-skills)** — Google Scholar 完整集成：检索、引用追踪、全文链接抓取、BibTeX 导 Zotero，全部通过 Chrome DevTools MCP。
  **什么时候用：** 需要程序化跑 Google Scholar、批量同步引用到 Zotero 时——纯 DOM 方案稳定。
  **作者：** [@cookjohn](https://github.com/cookjohn)　**标签：** `Google Scholar` `Zotero` `引用追踪` `MCP`

- **[paper-craft-skills](https://github.com/zsyggg/paper-craft-skills)** — 把论文做成深度解读文章、10 页教学漫画、速览总结，附公式拆解和源码对照。
  **什么时候用：** 科普作者、读书会、把论文做成可分发内容时。
  **作者：** [@zsyggg](https://github.com/zsyggg)　**标签：** `论文解读` `漫画` `科普` `教学`

- **[paper-glance-skill](https://github.com/CatVinci-Studio/paper-glance-skill)** — 论文深度报告 + Mermaid 思维导图 + 同行评议 + 推广文案 + 播客脚本五合一。
  **什么时候用：** 要把论文变成多种二次传播形态时——无需付费 API。
  **作者：** [@CatVinci-Studio](https://github.com/CatVinci-Studio)　**标签：** `论文` `思维导图` `同行评议` `播客脚本`

- **[qinyan-academic-skills](https://github.com/LeonChaoX/qinyan-academic-skills)** — 沁言学术：177+ 学术 skill，17 大分类涵盖论文检索、生信、药物发现、临床医学、NSFC 申报。
  **什么时候用：** 理工/医学/生命科学科研人员需要细分领域专家方法论时——医学/生信方向覆盖最深。
  **作者：** [@LeonChaoX](https://github.com/LeonChaoX)　**标签：** `学术` `生物信息` `临床医学` `NSFC`

- **[codex-claude-academic-skills](https://github.com/zLanqing/codex-claude-academic-skills)** — 中文科研工作流三件套：论文阅读 + 学术 PPT 生成、写作润色与审稿回复、MATLAB/Python 科学计算与期刊级绘图。
  **什么时候用：** 国内高校与科研人员做文献综述、写论文、回审稿意见、画发表用图表时。
  **作者：** [@zLanqing](https://github.com/zLanqing)　**标签：** `科研` `论文` `学术写作` `MATLAB` `Python`

- **[claude-code-interview](https://github.com/huifer/claude-code-interview)** — 8 个面试求职 skill：JD 分析、ATS 简历优化、模拟面试、薪资谈判、LinkedIn 导入、市场情报看板。
  **什么时候用：** 技术求职准备、简历对标 JD、想看市场情报看板时——与 interview-master-skill 互补。
  **作者：** [@huifer](https://github.com/huifer)　**标签：** `求职` `ATS` `面试` `市场情报`

- **[interview-master-skill](https://github.com/chen3tu/interview-master-skill)** — 求职面试全流程 skill：公司七维分析 + STAR-R 法则简历 + 模拟面试 + 薪资谈判。
  **什么时候用：** 准备面试、复盘 offer、谈判薪资时——比通用建议更结构化。
  **作者：** [@chen3tu](https://github.com/chen3tu)　**标签：** `求职` `面试` `STAR-R` `薪资谈判`

- **[awesome-obsidian-skills](https://github.com/BCS1037/awesome-obsidian-skills)** — 精选 Obsidian × Claude Code skill 子列表，含 kepano 官方 obsidian-skills、Claudian、Claudesidian MCP 等。
  **什么时候用：** 找 Obsidian 生态里所有可用 Claude skill 的入口时——专项 awesome 子列表。
  **作者：** [@BCS1037](https://github.com/BCS1037)　**标签：** `Obsidian` `精选列表` `MCP` `子awesome`

- **[literature-review-skill](https://github.com/YANZHANLIN/literature-review-skill)** — 文献综述全流程 5 子 skill：检索（PICO/SPIDER）→ 获取 → 精读（Keshav 三遍法）→ 综述写作 → 学位论文章节。
  **什么时候用：** 写学位论文文献综述、需要 GB/T 7714 或 APA/PRISMA 规范时。
  **作者：** [@YANZHANLIN](https://github.com/YANZHANLIN)　**标签：** `文献综述` `学位论文` `PRISMA` `GB/T 7714`

### 设计与创意

> UI/UX 评审、文案创作、命名建议、配色与排版、原型生成等。

- **[huashu-design](https://github.com/alchaincyf/huashu-design)** — 花叔的 HTML 原生设计 skill，一句话产出高保真原型、幻灯片、动画、印刷级海报，内置 20 套设计哲学。
  **什么时候用：** 想要 Claude 生成不像"AI 默认审美"的视觉作品时——产品发布动画、可点击 App 原型、印刷信息图都能搞定。
  **作者：** [@alchaincyf](https://github.com/alchaincyf) (花叔)　**标签：** `HTML` `原型` `动画` `海报` `印刷级`

- **[guizang-ppt-skill](https://github.com/op7418/guizang-ppt-skill)** — 归藏的 HTML 幻灯片 skill：编辑杂志 / Swiss 设计两套体系，22 锁定布局，WebGL 演示运行时。
  **什么时候用：** 做发布会/作品集/汇报需要强设计感时——与 NanoBanana-PPT-Skills 体系完全不同。
  **作者：** [@op7418](https://github.com/op7418) (归藏)　**标签：** `PPT` `HTML` `Swiss设计` `WebGL`

- **[axton-obsidian-visual-skills](https://github.com/axtonliu/axton-obsidian-visual-skills)** — Obsidian 可视化三件套：Excalidraw 手绘图 + Mermaid 专业图表 + Canvas 思维导图，原生中文触发词。
  **什么时候用：** 在 Obsidian 里要把笔记/流程变成可视化图时。
  **作者：** [@axtonliu](https://github.com/axtonliu) (Axton Liu)　**标签：** `Obsidian` `Excalidraw` `Mermaid` `Canvas`

- **[NanoBanana-PPT-Skills](https://github.com/op7418/NanoBanana-PPT-Skills)** — 归藏的 AI 自动 PPT 工具，生成 2K/4K 杂志风 / 科研汇报 PPT 图片，支持智能转场视频与交互式播放。
  **什么时候用：** 临时要 PPT 但没设计感、或想做 AI 风格的杂志级幻灯片时。
  **作者：** [@op7418](https://github.com/op7418) (归藏)　**标签：** `PPT` `Gemini` `转场动画` `4K`

- **[claude-design-skill](https://github.com/jiji262/claude-design-skill)** — 复刻 Claude.ai 内部 Design 系统 prompt，让 Claude 输出 HTML deck、landing page、原型、动画、海报。
  **什么时候用：** 想要 Claude 生成不像"AI 默认审美"的视觉输出时——能产出更接近 Claude.ai 官方风格的设计。
  **作者：** [@jiji262](https://github.com/jiji262)　**标签：** `HTML` `原型` `landing page` `海报`

---

## 通用 Prompt 模板

> 这部分收录跟具体 agent 无关、能在 Claude / ChatGPT / Gemini 等多个平台通用的精选 prompt 模板。

- **[claude-code-system-prompts](https://github.com/Piebald-AI/claude-code-system-prompts)** — Claude Code 官方系统 prompt 完整反汇编：27 个内置工具描述、Plan/Explore/Task 子 agent prompt，每版本跟踪。（英文项目）
  **什么时候用：** 研究 Claude Code 内部工作机制、自己写 agent/skill 时参考官方 prompt 写法。
  **作者：** [@Piebald-AI](https://github.com/Piebald-AI)　**标签：** `系统Prompt` `逆向` `工具描述` `子Agent`

- **[awesome-claude-prompts](https://github.com/langgptai/awesome-claude-prompts)** — LangGPT 团队整理的 Claude 通用 prompt 精选，覆盖编程、写作、营销、商业、学习。
  **什么时候用：** 找跨场景 Claude prompt 启发、做提示词学习参考时——LangGPT 作者云中江树出品。
  **作者：** [@langgptai](https://github.com/langgptai) (云中江树)　**标签：** `Prompt` `精选` `LangGPT` `跨场景`

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
