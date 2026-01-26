> **Note:** This repository contains Anthropic's implementation of skills for Claude. For information about the Agent Skills standard, see [agentskills.io](http://agentskills.io).

# Skills

Skills are folders of instructions, scripts, and resources that Claude loads dynamically to improve performance on specialized tasks. Skills teach Claude how to complete specific tasks in a repeatable way, whether that's creating documents with your company's brand guidelines, analyzing data using your organization's specific workflows, or automating personal tasks.

For more information, check out:

- [What are skills?](https://support.claude.com/en/articles/12512176-what-are-skills)
- [Using skills in Claude](https://support.claude.com/en/articles/12512180-using-skills-in-claude)
- [How to create custom skills](https://support.claude.com/en/articles/12512198-creating-custom-skills)
- [Equipping agents for the real world with Agent Skills](https://anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills)

---

## 📚 本库 Skills 目录

本目录包含所有已安装的 Claude Code Skills，按字母顺序排列。

| 技能                                 | 触发方式                                   |
| ------------------------------------ | ------------------------------------------ |
| algorithmic-art                      | 创建算法艺术 / 生成艺术 / 用代码画图       |
| brand-guidelines                     | 使用品牌风格 / 应用官方颜色                |
| canvas-design                        | 创建海报 / 艺术作品 / 视觉设计             |
| data-insight-orchestrator            | 分析数据 / 数据分析报告                    |
| doc-coauthoring                      | 帮我写文档 / 协作文档 / 编写提案           |
| docx                                 | 创建 Word 文档 / 编辑 Word                 |
| frontend-design                      | 设计前端界面 / 网页设计 / 美化 UI          |
| image-assistant (配图助手)           | 这段内容做个图 / 配几张图 / 我需要配图助手 |
| internal-comms                       | 写状态报告 / 工作汇报 / 内部通讯           |
| mcp-builder                          | 创建 MCP 服务器 / 开发 MCP 工具            |
| pdf                                  | 处理 PDF 文件 / 提取 PDF 内容              |
| pptx                                 | 创建 PPT / 演示文稿 / 编辑 PowerPoint      |
| prd-doc-writer (PRD 文档撰写助手)    | 帮我写 PRD / 梳理需求文档                  |
| req-change-workflow (需求变更工作流) | 改需求 / 需求变更 / 调整交互               |
| skill-creator                        | 创建新技能 / 开发技能                      |
| slack-gif-creator                    | 创建 Slack GIF / 制作动画表情              |
| social-post-writer                   | 写社交媒体帖子 / 发朋友圈 / 写推文         |
| theme-factory                        | 应用主题 / 美化幻灯片 / 文档样式           |
| thought-mining (思维挖掘助手)        | 我想写篇文章 / 整理我的想法                |
| webapp-testing                       | 测试网页应用 / Web 测试                    |
| web-artifacts-builder                | 创建 HTML 作品 / Web 组件                  |
| xlsx                                 | 创建 Excel 表格 / 电子表格 / 数据分析      |
| 帮我写作                             | 帮我写 / 根据材料写文案                    |
| 爆款标题拆解                         | 拆解这个标题 / 分析标题                    |
| 爆款标题生成器                       | 生成爆款标题 / 帮我想标题 / 起标题         |
| 科技爆款文案生成器                   | 写科技文案 / 科技视频文案                  |
| 来点选题                             | 没有选题灵感 / 推荐选题                    |
| 英文播客自动总结                     | 分析播客 / 总结播客                        |
| 字幕转markdown                       | 字幕转笔记 / SRT 转 Markdown               |

### A

#### [algorithmic-art](./algorithmic-art)

**描述**: 使用 p5.js 创建算法艺术，支持种子随机性和交互式参数探索。适用于代码艺术、生成艺术、算法艺术、流场或粒子系统等场景。

**触发方式**:

```
创建算法艺术 / 生成艺术
用代码画图 / 生成艺术作品
创建流场 / 粒子系统效果
/algorithmic-art
```

---

### B

#### [brand-guidelines](./brand-guidelines)

**描述**: 应用 Anthropic 官方品牌颜色和排版到任何需要品牌风格的文档或作品中。

**触发方式**:

```
使用 Anthropic 品牌风格
应用官方颜色和字体
使用品牌指南
/brand-guidelines
```

---

### C

#### [canvas-design](./canvas-design)

**描述**: 使用设计哲学在 .png 和 .pdf 文档中创建精美的视觉艺术。适用于创建海报、艺术作品、设计或其他静态作品。

**触发方式**:

```
创建海报 / 艺术作品
设计视觉内容
生成设计图 / canvas
/canvas-design
```

---

### D

#### [data-insight-orchestrator](./data-insight-orchestrator)

**描述**: Data Dive - 完整开发规范。智能数据分析系统，能够接收多种格式的数据文件（Excel、PDF、Word、CSV、TXT），通过交互式对话了解用户的分析侧重点。

**触发方式**:

```
分析数据 / 数据分析报告
数据分析助手
处理数据文件 / 生成数据报告
/data-insight
```

#### [doc-coauthoring](./doc-coauthoring)

**描述**: 引导用户通过结构化工作流程协作编写文档，适用于编写文档、提案、技术规范、决策文档或类似的结构化内容。

**触发方式**:

```
帮我写文档 / 协作文档
编写提案 / 技术规范
决策文档 / RFC
/doc-coauthoring
```

#### [docx](./docx)

**描述**: 综合文档创建、编辑和分析工具，支持跟踪更改、评论、格式保留和文本提取。

**触发方式**:

```
创建 Word 文档 / .docx 文件
编辑 Word 文档
处理 Word 文件格式
/docx
```

---

### F

#### [frontend-design](./frontend-design)

**描述**: 创建具有高质量设计的独特生产级前端界面。适用于构建网页组件、页面、作品、海报或应用程序。

**触发方式**:

```
设计前端界面 / 网页设计
创建网页组件 / 页面
美化 UI / 前端设计
/frontend-design
```

---

### I

#### [image-assistant](./image-assistant) （配图助手）

**描述**: 把文章/模块内容转成统一风格、少字高可读的 16:9 信息图提示词

**适用场景**:

- 文章需要配图但不知道怎么设计
- PPT、海报、社媒图需要统一风格
- 内容太多字，想要更趣味、更好读的视觉呈现
- 需要批量生成配图提示词

**核心功能**:

- 📋 需求澄清：挖掘内容、场景、受众和字数偏好
- 🗂️ 配图规划：拆分内容，定义图清单（几张图/每张讲什么）
- ✍️ 文案定稿：逐字定稿"图上写什么"（Copy Spec）
- 🎯 提示词封装：生成可复制的生图提示词，支持批量出图
- 🔄 迭代润色：根据反馈减字、换隐喻、提升可读性

**触发方式**:

```
这段内容做个图/配几张图
给我两张出图提示词
字太多不好看，帮我更趣味、更好读
/image /配图 /出图
```

#### [internal-comms](./internal-comms)

**描述**: 用于编写各类内部沟通内容的资源集，包括状态报告、领导层更新、3P 更新、公司通讯、常见问题解答、事件报告、项目更新等。

**触发方式**:

```
写状态报告 / 工作汇报
写内部通讯 / 领导层更新
3P 更新 / 项目更新
/internal-comms
```

---

### M

#### [mcp-builder](./mcp-builder)

**描述**: 创建高质量 MCP（模型上下文协议）服务器的指南，使 LLM 能够通过精心设计的工具与外部服务交互。

**触发方式**:

```
创建 MCP 服务器
构建 Model Context Protocol 服务
开发 MCP 工具
/mcp-builder
```

---

### P

#### [pdf](./pdf)

**描述**: 综合的 PDF 处理工具包，用于提取文本和表格、创建新 PDF、合并/拆分文档以及处理表单。

**触发方式**:

```
处理 PDF 文件
提取 PDF 内容 / 合并 PDF
创建 PDF / 填写 PDF 表单
/pdf
```

#### [pptx](./pptx)

**描述**: 演示文稿创建、编辑和分析。处理演示文稿（.pptx 文件）的创建、修改、布局、评论或演讲者备注。

**触发方式**:

```
创建 PPT / 演示文稿
编辑 PowerPoint 文件
处理 .pptx 文件
/pptx
```

#### [prd-doc-writer](./prd-doc-writer) （PRD 文档撰写助手）

**描述**: 以故事驱动的方式，帮助你撰写和迭代完善 PRD/需求文档

**适用场景**:

- 需要撰写产品需求文档
- 想用用户故事的方式梳理需求
- 需要用图表减少需求歧义

**核心功能**:

- 🗺️ 用户旅程地图：构建宏观业务流程
- 📖 故事化需求：每个功能点都是一个完整的用户故事
- 🎨 ASCII 线框图：可视化页面布局
- 📊 Mermaid 图表：流程图/状态图/时序图
- ✅ 阶段性确认：确保每一步都与你达成共识

**触发方式**:

```
帮我写 PRD
梳理需求文档
/prd-doc-writer
```

---

### R

#### [req-change-workflow](./req-change-workflow) （需求变更工作流）

**描述**: 标准化需求变更流程，避免改需求时的混乱和代码崩溃

**适用场景**:

- 需要修改现有功能的需求
- 改需求时经常出现意外 bug
- 需要一个可靠的变更验证流程
- 特别适合 Chrome 扩展等复杂项目

**核心功能**:

- 📝 需求澄清：锁定变更范围和验收标准
- 🔍 现状基线：从代码中确认当前行为
- ⚠️ 影响评估：评估风险和变更范围
- 🎯 设计方案：提出新设计并获得批准
- 🛠️ 最小化实现：小范围、局部化的代码修改
- ✅ 回归测试：固定的验证清单
- 📚 文档维护：决策日志和文档更新

**触发方式**:

```
改需求/需求变更
调整交互/改功能
/req-change-workflow
```

---

### S

#### [skill-creator](./skill-creator)

**描述**: 创建有效技能的指南。当用户想要创建新技能（或更新现有技能）以扩展 Claude 的功能时使用。

**触发方式**:

```
创建新技能 / 开发技能
编写 Skill 文件
/skill-creator
```

#### [slack-gif-creator](./slack-gif-creator)

**描述**: 为 Slack 创建优化动画 GIF 的知识和工具集。提供约束、验证工具和动画概念。

**触发方式**:

```
创建 Slack GIF / 制作动画表情
生成 Slack 表情
/slack-gif
```

#### [social-post-writer](./social-post-writer)

**描述**: 社交媒体帖子撰写助手。适用于将模糊想法转化为社交帖子、改写帖子、为各平台撰写内容、优化帖子表达。

**触发方式**:

```
写社交媒体帖子 / 发朋友圈
写推文 / 小红书文案
改写帖子 / 优化文案
/social-post
```

---

### T

#### [theme-factory](./theme-factory)

**描述**: 使用主题样式化作品集的工具包。包含 10 个预设的颜色/字体主题，适用于幻灯片、文档、报告、HTML 登陆页等。

**触发方式**:

```
应用主题 / 使用主题样式
美化幻灯片 / 文档样式
/theme-factory
```

#### [thought-mining](./thought-mining) （思维挖掘助手）

**描述**: 通过对话帮助你把脑子里的零散想法倒出来、记录下来、整理成文章

**适用场景**:

- 想写文章但思路不清晰
- 有很多零散想法需要整理
- 需要从混乱的思考中提炼核心观点

**核心功能**:

- 📝 思维挖掘：引导式对话，帮你说出并记录想法
- 🎯 选题确定：从洞察中找到核心观点
- ✅ 观点验证：联网搜索验证理解是否正确
- ✍️ 写作辅助：逻辑检查、文字润色、金句提炼
- 🔍 最终审核：发布前的全面检查

**触发方式**:

```
我想写一篇关于 XX 的文章
帮我整理一下我的想法
/thought-mining
```

---

### W

#### [webapp-testing](./webapp-testing)

**描述**: 使用 Playwright 与本地 Web 应用程序交互和测试的工具包。支持验证前端功能、调试 UI 行为、捕获浏览器截图和查看浏览器日志。

**触发方式**:

```
测试网页应用 / Web 测试
使用 Playwright 测试
调试前端功能
/webapp-testing
```

#### [web-artifacts-builder](./web-artifacts-builder)

**描述**: 使用现代前端 Web 技术（React、Tailwind CSS、shadcn/ui）创建复杂的多组件 claude.ai HTML 作品的工具套件。

**触发方式**:

```
创建 HTML 作品 / Web 组件
构建复杂前端界面
/web-artifacts
```

---

### X

#### [xlsx](./xlsx)

**描述**: 综合电子表格创建、编辑和分析，支持公式、格式化、数据分析和可视化。

**触发方式**:

```
创建 Excel 表格 / 电子表格
处理 .xlsx 文件
数据分析 / 表格可视化
/xlsx
```

---

### 中文技能

#### [帮我写作](./帮我写作)

**描述**: 结合用户提供的材料进行文案写作。

**触发方式**:

```
帮我写 / 帮我写作
根据材料写文案
结合材料写文章
```

#### [爆款标题拆解](./爆款标题拆解)

**描述**: 拥有千万级爆款经验的新媒体内容专家，擅长"逆向工程"和"第一性原理"，能逆向工程任何一个高点击率标题。

**触发方式**:

```
拆解这个标题 / 分析标题
这个标题为什么火
标题逆向分析
```

#### [爆款标题生成器](./爆款标题生成器)

**描述**: 基于84个千万级播放AI视频标题的逆向工程拆解，提供6大核心策略、万能模板和标题组合公式。

**触发方式**:

```
生成爆款标题 / 帮我想标题
起标题 / 写标题
/爆款标题
```

#### [科技爆款文案生成器](./科技爆款生成器)

**描述**: 基于4篇百万播放科技视频拆解，提炼出的通用爆款要素和可复用模板，包含5种爆款打法、万能句式模板和口语化表达词库。

**触发方式**:

```
写科技文案 / 科技视频文案
生成科技类内容
/科技文案
```

#### [来点选题](./来点选题)

**描述**: 当用户视频创作选题枯竭的时候，为用户提供选题思路。

**触发方式**:

```
没有选题灵感 / 给我选题思路
推荐选题 / 来点选题
/选题
```

#### [英文播客自动总结](./英文播客自动总结)

**描述**: 一键完成播客的抓取、转录和智能分析。自动执行 RSS 抓取 → Deepgram 转录 → Claude 分析 → 保存结果全流程。

**触发方式**:

```
分析播客 / 总结播客
/podcast-analyze
```

#### [字幕转markdown](./字幕转markdown)

**描述**: 把srt字幕文件转换成markdown笔记。

**触发方式**:

```
字幕转笔记 / SRT 转 Markdown
转换字幕文件
/字幕转md
```

---

## 📊 统计

| 类别           | 数量                     |
| -------------- | ------------------------ |
| 英文技能       | 19                       |
| 中文技能       | 7                        |
| 无 SKILL.md    | 2 (pm-practice, 剪口播/) |
| **总计** | **28**             |

---

*最后更新: 2026-01-22*

---

# About This Repository

This repository contains skills that demonstrate what's possible with Claude's skills system. These skills range from creative applications (art, music, design) to technical tasks (testing web apps, MCP server generation) to enterprise workflows (communications, branding, etc.).

Each skill is self-contained in its own folder with a `SKILL.md` file containing the instructions and metadata that Claude uses. Browse through these skills to get inspiration for your own skills or to understand different patterns and approaches.

Many skills in this repo are open source (Apache 2.0). We've also included the document creation & editing skills that power [Claude&#39;s document capabilities](https://www.anthropic.com/news/create-files) under the hood in the [`docx`](./docx), [`pdf`](./pdf), [`pptx`](./pptx), and [`xlsx`](./xlsx) subfolders. These are source-available, not open source, but we wanted to share these with developers as a reference for more complex skills that are actively used in a production AI application.

## Disclaimer

**These skills are provided for demonstration and educational purposes only.** While some of these capabilities may be available in Claude, the implementations and behaviors you receive from Claude may differ from what is shown in these skills. These skills are meant to illustrate patterns and possibilities. Always test skills thoroughly in your own environment before relying on them for critical tasks.

# Skill Sets

- [./](./): All available skills
- [../spec](../spec): The Agent Skills specification
- [../template](../template): Skill template

# Try in Claude Code, Claude.ai, and the API

## Claude Code

You can register this repository as a Claude Code Plugin marketplace by running the following command in Claude Code:

```
/plugin marketplace add anthropics/skills
```

Then, to install a specific set of skills:

1. Select `Browse and install plugins`
2. Select `anthropic-agent-skills`
3. Select `document-skills` or `example-skills`
4. Select `Install now`

Alternatively, directly install either Plugin via:

```
/plugin install document-skills@anthropic-agent-skills
/plugin install example-skills@anthropic-agent-skills
```

After installing the plugin, you can use the skill by just mentioning it. For instance, if you install the `document-skills` plugin from the marketplace, you can ask Claude Code to do something like: "Use the PDF skill to extract the form fields from `path/to/some-file.pdf`"

## Claude.ai

These example skills are all already available to paid plans in Claude.ai.

To use any skill from this repository or upload custom skills, follow the instructions in [Using skills in Claude](https://support.claude.com/en/articles/12512180-using-skills-in-claude#h_a4222fa77b).

## Claude API

You can use Anthropic's pre-built skills, and upload custom skills, via the Claude API. See the [Skills API Quickstart](https://docs.claude.com/en/api/skills-guide#creating-a-skill) for more.

# Creating a Basic Skill

Skills are simple to create - just a folder with a `SKILL.md` file containing YAML frontmatter and instructions. You can use the **template-skill** in this repository as a starting point:

```markdown
---
name: my-skill-name
description: A clear description of what this skill does and when to use it
---

# My Skill Name

[Add your instructions here that Claude will follow when this skill is active]

## Examples
- Example usage 1
- Example usage 2

## Guidelines
- Guideline 1
- Guideline 2
```

The frontmatter requires only two fields:

- `name` - A unique identifier for your skill (lowercase, hyphens for spaces)
- `description` - A complete description of what the skill does and when to use it

The markdown content below contains the instructions, examples, and guidelines that Claude will follow. For more details, see [How to create custom skills](https://support.claude.com/en/articles/12512198-creating-custom-skills).

# Partner Skills

Skills are a great way to teach Claude how to get better at using specific pieces of software. As we see awesome example skills from partners, we may highlight some of them here:

- **Notion** - [Notion Skills for Claude](https://www.notion.so/notiondevs/Notion-Skills-for-Claude-28da4445d27180c7af1df7d8615723d0)
