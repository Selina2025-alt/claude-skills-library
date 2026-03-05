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

| 技能                                    | 触发方式                                          |
| ----------------------------------- | ------------------------------------------------- |
| algorithmic-art                     | 创建算法艺术 / 生成艺术 / 用代码画图              |
| artifacts-builder                   | 创建复杂 HTML 作品 / React 组件                   |
| brand-guidelines                     | 应用品牌风格 / 使用官方颜色和字体                 |
| canvas-design                        | 创建海报 / 艺术作品 / 设计视觉内容                 |
| changelog-generator                 | 生成更新日志 / 版本发布说明                       |
| claymotion-director                  | 黏土动画分镜 / 像素风动画 / 视觉风格导演           |
| competitive-ads-extractor           | 分析竞品广告 / 提取广告库数据                     |
| composition-patterns                | React 组件组合模式 / 重构布尔 props               |
| connect                              | 连接外部应用 / 发邮件建工单                       |
| connect-apps                         | 连接 Gmail/Slack/GitHub                          |
| content-research-writer             | 协作写作 / 添加引用 / 改进内容                    |
| data-insight-orchestrator            | 数据分析 / 数据分析报告                           |
| daily-news (每日资讯日报)            | 每日新闻 / 资讯日报 / 信息监控                     |
| developer-growth-analysis           | 分析编码模式 / 开发者成长报告                     |
| doc-coauthoring                      | 协作文档 / 编写技术规范 / 决策文档                |
| docx                                 | 创建 Word 文档 / 编辑 .docx 文件                  |
| domain-name-brainstormer            | 生成域名创意 / 检查域名可用性                     |
| file-organizer                       | 整理文件 / 智能分类 / 清理重复文件                |
| find-skills                          | 发现技能 / 查找技能 / 安装技能                    |
| frontend-design                      | 设计前端界面 / 网页设计 / 美化 UI                 |
| image-assistant (配图助手)          | 这段内容做个图 / 配几张图 / 我需要配图助手         |
| image-enhancer                       | 增强图片质量 / 提升截图清晰度                     |
| invoice-organizer                    | 整理发票 / 税务准备 / 财务归档                    |
| internal-comms                       | 写状态报告 / 内部通讯 / 工作汇报                  |
| langsmith-fetch                      | 调试 LangChain 代理 / 分析执行追踪                |
| lead-research-assistant              | 寻找潜在客户 / 目标公司研究                       |
| mcp-builder                          | 创建 MCP 服务器 / 构建 Model Context Protocol     |
| meeting-insights-analyzer            | 分析会议记录 / 沟通模式分析                       |
| pdf                                  | 处理 PDF 文件 / 提取内容 / 合并 PDF               |
| pptx                                 | 创建 PPT / 演示文稿 / 编辑 PowerPoint             |
| prd-doc-writer                       | 写 PRD / 梳理需求文档 / 用户故事                  |
| raffle-winner-picker                 | 抽奖选 winner / 随机选择                          |
| react-best-practices                 | React/Next.js 性能优化 / 代码审查                 |
| react-native-skills                  | React Native 开发 / Expo 应用构建                 |
| remotion-best-practices              | Remotion 视频制作 / React 视频生成                |
| req-change-workflow                  | 需求变更 / 改功能 / 重构流程                      |
| skill-creator                        | 创建新技能 / 开发技能 / 编写 Skill 文件            |
| skill-share                          | 创建并分享技能 / Slack 团队协作                   |
| slack-gif-creator                    | 创建 Slack GIF / 制作动画表情                     |
| social-post-writer                   | 写社交媒体帖子 / 发朋友圈 / 写推文                |
| superpowers                          | 软件开发工作流 / TDD / 代码审查 / Git Worktrees   |
| tailored-resume-generator            | 定制简历 / 针对职位优化简历                       |
| theme-factory                        | 应用主题 / 美化幻灯片 / 文档样式                  |
| thought-mining (思维挖掘助手)        | 我想写篇文章 / 整理我的想法                       |
| twitter-algorithm-optimizer          | 优化推文 / 提升推特传播效果                       |
| ui-ux-pro-max                        | UI 设计 / 前端页面设计 / 设计系统                 |
| vercel-deploy-claimable             | 部署到 Vercel / 创建预览部署                      |
| video-downloader                     | 下载 YouTube 视频 / 保存视频                      |
| video-gen                            | AI 生成视频 / 文生视频 / 图生视频                  |
| webapp-testing                       | 测试网页应用 / Web 测试                           |
| web-artifacts-builder                | 创建 HTML 作品 / Web 组件                         |
| web-design-guidelines                | 审查 UI / 检查可访问性 / 设计审计                  |
| xlsx                                 | 创建 Excel 表格 / 电子表格 / 数据分析             |
| 帮我写作                              | 帮我写 / 根据材料写文案                            |
| 爆款标题拆解                          | 拆解这个标题 / 分析标题                            |
| 爆款标题生成器                        | 生成爆款标题 / 帮我想标题 / 起标题                |
| 科技爆款文案生成器                    | 写科技文案 / 科技视频文案                          |
| 来点选题                              | 没有选题灵感 / 推荐选题                            |
| 英文播客自动总结                      | 分析播客 / 总结播客                                |
| 字幕转markdown                        | 字幕转笔记 / SRT 转 Markdown                      |

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

#### [artifacts-builder](./artifacts-builder)

**描述**: 使用现代前端 Web 技术（React、Tailwind CSS、shadcn/ui）创建复杂的多组件 claude.ai HTML 作品。适用于需要状态管理、路由或 shadcn/ui 组件的复杂作品。

**触发方式**:
```
创建复杂 HTML 作品
构建 React 组件
使用现代前端技术
/artifacts
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

#### [changelog-generator](./changelog-generator)

**描述**: 自动从 git 提交记录创建用户友好的更新日志，通过分析提交历史、分类变更，将技术提交转化为清晰的客户友好的发布说明。

**触发方式**:
```
生成更新日志 / 版本发布说明
创建 changelog / 发布笔记
分析 git 提交生成更新内容
/changelog
```

---

#### [claymotion-director](./claymotion-director) （视觉风格动画导演）

**描述**: 将文案转化为视觉叙事分镜，生成 Veo/Sora 提示词。支持黏土风、毛毡风、像素风、霓虹 Lo-Fi 风、水彩风、布艺风等多种风格。

**适用场景**:
- 需要制作定格动画风格视频
- 文案转视频分镜脚本
- 多种视觉风格探索

**核心功能**:
- 🎬 多种视觉风格：黏土、毛毡、像素、霓虹、水彩、布艺
- 📝 分镜脚本生成：自动转化为视觉叙事
- 🎨 Veo/Sora 提示词：可直接使用的 AI 视频生成提示词

**触发方式**:
```
生成黏土动画分镜
做像素风动画
毛毡风格视频分镜
/claymotion-director
```

---

#### [competitive-ads-extractor](./competitive-ads-extractor)

**描述**: 从广告库（Facebook、LinkedIn 等）提取和分析竞争对手的广告，了解哪些信息、问题和创意方法有效，帮助启发和改进你自己的广告活动。

**触发方式**:
```
分析竞品广告 / 提取广告数据
研究竞争对手广告策略
查看广告库 / 分析广告创意
/competitive-ads
```

---

#### [composition-patterns](./composition-patterns)

**描述**: React 组合模式指南，帮助你构建可扩展的组件。适用于布尔 props 繁殖的组件重构、构建灵活的组件库或设计可复用的 API。

**来源**: [https://github.com/vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills)

**触发方式**:
```
React 组件组合模式
重构布尔 props
构建组件库
复合组件 / 渲染 props
/composition-patterns
```

---

#### [connect](./connect)

**描述**: 将 Claude 连接到任何应用（Gmail、Slack、GitHub、Notion 等 1000+ 服务），直接发送邮件、创建工单、发布消息，而不是只生成文本描述。

**触发方式**:
```
发送邮件 / 创建工单
发布到 Slack / 更新数据库
连接外部应用 / 实际执行操作
/connect
```

---

#### [connect-apps](./connect-apps)

**描述**: 连接 Claude 到 Gmail、Slack、GitHub 等外部应用，真正发送邮件、创建工单、发布消息，而不只是生成关于这些操作的文本。

**触发方式**:
```
连接 Gmail/Slack/GitHub
发送真实邮件 / 创建实际工单
外部应用集成 / 自动化操作
/connect-apps
```

---

#### [content-research-writer](./content-research-writer)

**描述**: 通过研究、添加引用、改进开头、迭代大纲和实时反馈来协助撰写高质量内容，将写作过程从独自努力转变为协作伙伴关系。

**触发方式**:
```
协作写作 / 添加引用
改进文章开头 / 迭代大纲
研究并写作 / 提供内容反馈
/content-writing
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

---

#### [daily-news](./daily-news) （每日资讯日报生成器）

**描述**: 三阶段工作流自动化生成每日资讯日报：获取元数据 → 生成摘要 → 输出日报

**适用场景**:
- 每日新闻汇总和资讯监控
- 多信源信息聚合与分析
- 个性化新闻日报生成

**核心功能**:
- 📰 多信源抓取：支持 RSS、WebFetch、Browser MCP 三种方式
- 🗄️ SQLite 存储：增量抓取，双层去重机制
- 📝 智能摘要：基于用户画像生成个性化摘要
- 🌐 网站部署：可选自动部署到 Cloudflare Pages
- 📊 日期范围筛选：支持今天、昨天、最近N天、增量抓取等

**触发方式**:
```
生成每日新闻 / 制作资讯日报
信息监控 / 新闻聚合
添加新闻信源
/daily-news
```

---

#### [developer-growth-analysis](./developer-growth-analysis)

**描述**: 分析你最近的 Claude Code 聊天历史，识别编码模式、开发差距和改进领域，策划来自 HackerNews 的相关学习资源，并自动发送个性化成长报告到你的 Slack。

**触发方式**:
```
分析编码模式 / 开发者成长
检查编码习惯 / 识别技术差距
获取个性化学习资源 / 成长报告
/developer-growth
```

---

#### [domain-name-brainstormer](./domain-name-brainstormer)

**描述**: 为你的项目生成创意域名名称，并检查多个 TLD（.com、.io、.dev、.ai 等）的可用性，节省数小时的头脑风暴和手动检查。

**触发方式**:
```
生成域名创意 / 检查域名可用性
为项目起名 / 域名建议
域名头脑风暴 / 查找可用域名
/domain-name
```

---

#### [doc-coauthoring](./doc-coauthoring)

**描述**: 引导用户通过结构化工作流程协作编写文档，适用于编写文档、提案、技术规范、决策文档或类似的结构化内容。

**触发方式**:
```
帮我写文档 / 协作文档
编写提案 / 技术规范
决策文档 / RFC
/doc-coauthoring
```

---

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

#### [file-organizer](./file-organizer)

**描述**: 通过理解上下文、查找重复文件、建议更好的结构和自动化清理任务，智能地组织你计算机上的文件和文件夹，减少认知负担并保持数字工作空间整洁。

**触发方式**:
```
整理文件 / 智能分类
清理重复文件 / 文件归档
优化文件夹结构 / 清理下载文件夹
/file-organizer
```

---

#### [find-skills](./find-skills)

**描述**: 帮助用户发现和安装 agent skills。当用户问"如何做 X"、"找一个能做 X 的技能"、"有没有技能可以..."或表示有兴趣扩展功能时使用。

**来源**: [https://github.com/vercel-labs/skills](https://github.com/vercel-labs/skills)

**如何使用**:

| 你的问题 | 触发时机 |
|---------|---------|
| "有没有做 X 的技能？" | 查找特定功能的技能 |
| "如何做 Y？" | 自动检测相关技能 |
| "帮我找一个能处理 Z 的技能" | 搜索技能库 |
| "有没有技能可以扩展这个功能" | 发现新能力 |

**触发方式**:
```
找一个能做 X 的技能
有没有技能可以...
帮我发现技能
如何做...
/find-skills
```

---

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

---

#### [image-enhancer](./image-enhancer)

**描述**: 通过增强分辨率、锐度和清晰度来提高图像质量（尤其是截图），非常适合为演示文稿、文档或社交媒体帖子准备图像。

**触发方式**:
```
增强图片质量 / 提升截图清晰度
优化图像 / 改善图片效果
图片增强 / 提高分辨率
/image-enhance
```

---

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

#### [invoice-organizer](./invoice-organizer)

**描述**: 通过读取杂乱的文件、提取关键信息、一致地重命名并分类到逻辑文件夹中，自动整理发票和收据以备税务准备，将数小时的手动记账变成几分钟的自动整理。

**触发方式**:
```
整理发票 / 税务准备
财务归档 / 发票分类
处理收据 / 财务文档整理
/invoice-organizer
```

---

### L

#### [langsmith-fetch](./langsmith-fetch)

**描述**: 通过从 LangSmith Studio 获取执行追踪来调试 LangChain 和 LangGraph 代理，自动获取最新追踪并分析执行模式。

**触发方式**:
```
调试 LangChain 代理 / 查看追踪
分析代理行为 / 检查错误
LangSmith 调试 / 执行分析
/langsmith
```

---

#### [lead-research-assistant](./lead-research-assistant)

**描述**: 通过分析业务、搜索目标公司并提供可操作的联系方式，为产品或服务识别高质量的潜在客户，非常适合销售、业务拓展和营销专业人士。

**触发方式**:
```
寻找潜在客户 / 目标公司研究
客户分析 / 销售线索
业务拓展 / 寻找目标客户
/lead-research
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

#### [meeting-insights-analyzer](./meeting-insights-analyzer)

**描述**: 分析会议记录和录音以揭示行为模式、沟通见解和可操作反馈，识别何时回避冲突、使用填充词、主导对话或错失倾听机会。

**触发方式**:
```
分析会议记录 / 沟通模式分析
会议洞察 / 沟通技巧改进
会议行为分析 / 领导力反馈
/meeting-insights
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

---

#### [pptx](./pptx)

**描述**: 演示文稿创建、编辑和分析。处理演示文稿（.pptx 文件）的创建、修改、布局、评论或演讲者备注。

**触发方式**:
```
创建 PPT / 演示文稿
编辑 PowerPoint 文件
处理 .pptx 文件
/pptx
```

---

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

#### [react-best-practices](./react-best-practices)

**描述**: React 和 Next.js 性能优化指南，来自 Vercel Engineering。在编写、审查或重构 React/Next.js 代码时使用，确保最佳性能模式。

**来源**: [https://github.com/vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills)

**触发方式**:
```
React/Next.js 性能优化
代码审查 / 重构组件
数据获取优化 / Bundle 优化
性能改进
/react-best-practices
```

---

#### [react-native-skills](./react-native-skills)

**描述**: React Native 和 Expo 最佳实践，用于构建高性能移动应用。在构建 React Native 组件、优化列表性能、实现动画或使用原生模块时使用。

**来源**: [https://github.com/vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills)

**触发方式**:
```
React Native 开发
Expo 应用构建
移动应用性能优化
原生模块集成
/react-native-skills
```

---

#### [raffle-winner-picker](./raffle-winner-picker)

**描述**: 从列表、电子表格或 Google Sheets 中随机选择抽奖、赠品和竞赛的获奖者，确保公平、无偏见的选择和透明度。

**触发方式**:
```
抽奖选 winner / 随机选择
抽取获奖者 / 公平抽奖
随机选择 / 抽奖工具
/raffle
```

---

#### [remotion-best-practices](./remotion-best-practices)

**描述**: Remotion 最佳实践 - 使用 React 创建视频。

**触发方式**:
```
Remotion 视频制作
React 视频生成
/remotion-best-practices
```

---

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

---

#### [skill-share](./skill-share)

**描述**: 创建新的 Claude 技能并使用 Rube 自动在 Slack 上分享，实现无缝团队协作和技能发现。

**触发方式**:
```
创建并分享技能 / Slack 团队协作
技能打包分发 / 团队技能管理
技能创建与分享 / 团队通知
/skill-share
```

---

#### [superpowers](./superpowers) （软件开发工作流）

**描述**: 完整的软件开发工作流，基于可组合的"技能"系统，让你的 AI 编程代理拥有真正的超能力。

**来源**: [https://github.com/obra/superpowers](https://github.com/obra/superpowers)

**核心工作流**:
1. **brainstorming** - 在编写代码前激活，通过对话细化需求，探索替代方案
2. **using-git-worktrees** - 设计批准后创建隔离工作空间，运行项目设置
3. **writing-plans** - 将工作分解为小任务（2-5分钟），包含精确路径和验证步骤
4. **subagent-driven-development** - 派遣子代理处理每个任务，两阶段审查（规范合规性 + 代码质量）
5. **test-driven-development** - 强制 RED-GREEN-REFACTOR：先写失败测试，再写最少代码
6. **requesting-code-review** - 按计划审查，按严重程度报告问题
7. **finishing-a-development-branch** - 验证测试，提供合并/PR/保留/丢弃选项

**包含技能**:
- **测试**: test-driven-development
- **调试**: systematic-debugging, verification-before-completion
- **协作**: brainstorming, writing-plans, executing-plans, dispatching-parallel-agents, requesting-code-review, receiving-code-review, using-git-worktrees, finishing-a-development-branch, subagent-driven-development
- **元技能**: writing-skills, using-superpowers

**触发方式**:
```
帮助我规划这个功能
让我们调试这个问题
软件开发的完整工作流
使用 superpowers
```

---

#### [slack-gif-creator](./slack-gif-creator)

**描述**: 为 Slack 创建优化动画 GIF 的知识和工具集。提供约束、验证工具和动画概念。

**触发方式**:
```
创建 Slack GIF / 制作动画表情
生成 Slack 表情
/slack-gif
```

---

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

#### [tailored-resume-generator](./tailored-resume-generator)

**描述**: 分析职位描述并生成定制简历，突出相关经验、技能和成就以最大化面试机会。

**触发方式**:
```
定制简历 / 针对职位优化简历
生成求职简历 / 简历优化
职位分析 / 简历定制
/resume-generator
```

---

#### [theme-factory](./theme-factory)

**描述**: 使用主题样式化作品集的工具包。包含 10 个预设的颜色/字体主题，适用于幻灯片、文档、报告、HTML 登陆页等。

**触发方式**:
```
应用主题 / 使用主题样式
美化幻灯片 / 文档样式
/theme-factory
```

---

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

#### [twitter-algorithm-optimizer](./twitter-algorithm-optimizer)

**描述**: 使用 Twitter 的开源算法见解分析和优化推文以获得最大覆盖面，根据推荐系统对内容的排名方式重写和编辑用户推文。

**触发方式**:
```
优化推文 / 提升推特传播
推特算法优化 / 改进推文效果
最大化推文触达 / 内容策略优化
/twitter-optimize
```

---

### V

#### [video-gen](./video-gen)

**描述**: 使用 AI 生成视频，支持 Veo/Sora 模型。适用于文生视频、图生视频等场景。

**触发方式**:
```
AI 生成视频 / 文生视频
图生视频 / create video
做一个视频 / 视频生成
/video-gen
```

---

#### [vercel-deploy-claimable](./vercel-deploy-claimable)

**描述**: 部署应用到 Vercel。无需认证，返回预览 URL 和可认领的部署链接。

**来源**: [https://github.com/vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills)

**触发方式**:
```
部署应用到 Vercel
部署到生产环境
创建预览部署
给我部署链接
/deploy-vercel
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

---

#### [web-artifacts-builder](./web-artifacts-builder)

**描述**: 使用现代前端 Web 技术（React、Tailwind CSS、shadcn/ui）创建复杂的多组件 claude.ai HTML 作品的工具套件。

**触发方式**:
```
创建 HTML 作品 / Web 组件
构建复杂前端界面
/web-artifacts
```

---

#### [web-design-guidelines](./web-design-guidelines)

**描述**: 审查 UI 代码是否符合 Web 界面指南规范。当被要求"审查我的 UI"、"检查可访问性"、"设计审计"、"审查 UX"或"根据最佳实践检查我的网站"时使用。

**来源**: [https://github.com/vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills)

**触发方式**:
```
审查我的 UI / 检查可访问性
设计审计 / 审查 UX
检查网站最佳实践
/web-design-guidelines
```

---

### U

#### [ui-ux-pro-max](./ui-ux-pro-max-skill)

**描述**: UI/UX 设计智能工具包。包含 50+ 种风格、97 个配色方案、57 种字体搭配、99 条 UX 指南和 25 种图表类型，支持 9 种技术栈。可搜索数据库，提供优先级推荐。

**来源**: [https://github.com/nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)

**添加日期**: 2026-01-28

**触发方式**:
```
设计前端页面 / UI 设计
设计登录页 / Dashboard 设计
优化 UI/UX / 设计系统
/ui-ux-pro-max
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

#### [yt-dlp](./yt-dlp)

**描述**: 使用 yt-dlp 下载视频，支持 YouTube、Bilibili、Vimeo、Twitter 等 1000+ 网站。支持下载视频、音频、指定格式等。

**来源**: [https://github.com/yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp)

**添加日期**: 2026-01-28

**触发方式**:
```
下载视频 / 保存视频
视频下载 / 保存在线视频
YouTube 下载器 / B站下载
下载这个视频 / 视频保存
/yt-dlp
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

---

#### [爆款标题拆解](./爆款标题拆解)

**描述**: 拥有千万级爆款经验的新媒体内容专家，擅长"逆向工程"和"第一性原理"，能逆向工程任何一个高点击率标题。

**触发方式**:
```
拆解这个标题 / 分析标题
这个标题为什么火
标题逆向分析
```

---

#### [爆款标题生成器](./爆款标题生成器)

**描述**: 基于84个千万级播放AI视频标题的逆向工程拆解，提供6大核心策略、万能模板和标题组合公式。

**触发方式**:
```
生成爆款标题 / 帮我想标题
起标题 / 写标题
/爆款标题
```

---

#### [科技爆款文案生成器](./科技爆款生成器)

**描述**: 基于4篇百万播放科技视频拆解，提炼出的通用爆款要素和可复用模板，包含5种爆款打法、万能句式模板和口语化表达词库。

**触发方式**:
```
写科技文案 / 科技视频文案
生成科技类内容
/科技文案
```

---

#### [来点选题](./来点选题)

**描述**: 当用户视频创作选题枯竭的时候，为用户提供选题思路。

**触发方式**:
```
没有选题灵感 / 给我选题思路
推荐选题 / 来点选题
/选题
```

---

#### [英文播客自动总结](./英文播客自动总结)

**描述**: 一键完成播客的抓取、转录和智能分析。自动执行 RSS 抓取 → Deepgram 转录 → Claude 分析 → 保存结果全流程。

**触发方式**:
```
分析播客 / 总结播客
/podcast-analyze
```

---

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

| 类别           | 数量                        |
| -------------- | --------------------------- |
| 英文技能       | 47                          |
| 中文技能       | 8                           |
| 无 SKILL.md    | 2 (pm-practice, 剪口播/)    |
| **总计** | **57**                |

---

*最后更新: 2026-03-02*

---

# About This Repository

This repository contains skills that demonstrate what's possible with Claude's skills system. These skills range from creative applications (art, music, design) to technical tasks (testing web apps, MCP server generation) to enterprise workflows (communications, branding, etc.).

Each skill is self-contained in its own folder with a `SKILL.md` file containing the instructions and metadata that Claude uses. Browse through these skills to get inspiration for your own skills or to understand different patterns and approaches.

Many skills in this repo are open source (Apache 2.0). We've also included the document creation & editing skills that power [Claude's document capabilities](https://www.anthropic.com/news/create-files) under the hood in the [`docx`](./docx), [`pdf`](./pdf), [`pptx`](./pptx), and [`xlsx`](./xlsx) subfolders. These are source-available, not open source, but we wanted to share these with developers as a reference for more complex skills that are actively used in a production AI application.

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
