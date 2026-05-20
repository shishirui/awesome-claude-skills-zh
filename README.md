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

_暂无收录，欢迎通过 [PR](CONTRIBUTING.md) 或 [issue](../../issues/new/choose) 推荐你知道的优秀 skill。_

### 文档与写作

> 技术文档、PR 描述、commit 信息、周报、README 生成等写作场景。

_暂无收录，欢迎通过 [PR](CONTRIBUTING.md) 或 [issue](../../issues/new/choose) 推荐你知道的优秀 skill。_

### 数据处理

> CSV/Excel 处理、SQL 查询、数据清洗、可视化、报表生成等。

_暂无收录，欢迎通过 [PR](CONTRIBUTING.md) 或 [issue](../../issues/new/choose) 推荐你知道的优秀 skill。_

### 运维部署

> CI/CD、Docker、Kubernetes、云服务配置、日志分析、监控告警等。

_暂无收录，欢迎通过 [PR](CONTRIBUTING.md) 或 [issue](../../issues/new/choose) 推荐你知道的优秀 skill。_

### 学习研究

> 论文阅读、知识整理、笔记生成、概念解释、学习计划等。

_暂无收录，欢迎通过 [PR](CONTRIBUTING.md) 或 [issue](../../issues/new/choose) 推荐你知道的优秀 skill。_

### 设计与创意

> UI/UX 评审、文案创作、命名建议、配色与排版、原型生成等。

_暂无收录，欢迎通过 [PR](CONTRIBUTING.md) 或 [issue](../../issues/new/choose) 推荐你知道的优秀 skill。_

---

## 通用 Prompt 模板

> 这部分收录跟具体 agent 无关、能在 Claude / ChatGPT / Gemini 等多个平台通用的精选 prompt 模板。

_暂无收录，欢迎贡献你常用且效果好的 prompt 模板。_

---

## 相关资源

**官方文档**

- [Claude Code 官方文档](https://docs.claude.com/claude-code)
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
