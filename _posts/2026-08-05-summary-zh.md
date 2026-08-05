---
layout: default
title: "Horizon Summary: 2026-08-05 (ZH)"
date: 2026-08-05
lang: zh
---

> 从 31 条内容中筛选出 12 条重要资讯。

---

1. [谷歌 DeepMind 重大调整：哈萨比斯转任董事长，杰夫·迪恩离职](#item-1) ⭐️ 9.0/10
2. [ChainDrop 蠕虫攻陷 npm 逾 1300 个包](#item-2) ⭐️ 9.0/10
3. [杰夫·迪恩离开谷歌，创办 Discovery Loop](#item-3) ⭐️ 8.0/10
4. [专用开源模型以 100 倍更低成本击败 GPT-5.6 Sol](#item-4) ⭐️ 8.0/10
5. [Meta 投放含 AI 生成儿童性虐待图像的广告](#item-5) ⭐️ 8.0/10
6. [Cloudflare 发布面向智能体、应用与工作的开源 OS](#item-6) ⭐️ 8.0/10
7. [Claude Fable 5 仅凭一条推文构建出可玩的《Raccoon Heist》游戏](#item-7) ⭐️ 8.0/10
8. [LLM 0.32 发布：新增推理痕迹、Responses API 和服务端工具](#item-8) ⭐️ 8.0/10
9. [Monodratic：学习式乘积哈希路由实现稀疏因果注意力](#item-9) ⭐️ 8.0/10
10. [马斯克宣布 SpaceX 将独家采用英伟达 AI 架构](#item-10) ⭐️ 8.0/10
11. [DeepSeek 重启第二轮融资，投前估值 5000 亿元](#item-11) ⭐️ 8.0/10
12. [FFmpeg 9.0 发布，新增动画 WebP 与 Vulkan 滤镜及 AI 辅助开发](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [谷歌 DeepMind 重大调整：哈萨比斯转任董事长，杰夫·迪恩离职](https://blog.google/company-news/inside-google/message-ceo/next-chapter-ai-momentum/) ⭐️ 9.0/10

2026 年 8 月 5 日，谷歌 DeepMind 宣布重大领导层调整：德米斯·哈萨比斯将卸任 CEO 并转任董事长，而杰夫·迪恩和桑贾伊·格马瓦特将离开谷歌，共同创立一家专注于机器学习、科学和工程的独立公共福利公司。 这标志着谷歌 DeepMind 一个黄金时代的结束，因为两位最具标志性的技术领袖离开了。杰夫·迪恩和桑贾伊·格马瓦特的离去，加上近期一波资深 AI 研究人员的离职潮，引发了人们对谷歌留住顶尖人才并保持 AI 竞争优势能力的严重担忧。 杰夫·迪恩已在谷歌工作 27 年，桑贾伊·格马瓦特则是谷歌高级研究员；两人将共同创办一家独立的公共福利公司。社区观察者指出，哈萨比斯的职位调整可能实际上使他成为 Alphabet 的首席科学家，而消息公布后谷歌股价据报下跌了 5%。

hackernews · colesantiago · 8月5日 16:05 · [社区讨论](https://news.ycombinator.com/item?id=49184755)

**背景**: 谷歌 DeepMind 是由 DeepMind 与谷歌大脑合并而成的 AI 研究实验室，德米斯·哈萨比斯作为 CEO 领导其前沿 AI 研究。杰夫·迪恩是传奇的谷歌研究员，曾共同设计 MapReduce 和 TensorFlow 等基础系统，因此他的离开对公司来说既是象征性也是实质性的损失。这一消息反映了更广泛的行业趋势：资深 AI 研究人员正纷纷离开大型科技公司，去创办自己的企业或独立研究机构。

**社区讨论**: Hacker News 评论者对两人的离开表示惋惜，称这是“一个黄金时代的真正终结”，并指出许多财务自由的资深工程师之所以继续留任，部分原因就是“杰夫和桑贾伊还在”。还有人列举了谷歌近几个月流失的一长串知名 AI 研究人员，却没有引入同等级别的人才，认为谷歌营造了敌视人才的环境并出现战略偏离。部分评论还强调了市场的即时反应——谷歌股价下跌约 5%，可见这对组合在人们心中的价值巨大。

**标签**: `#google-deepmind`, `#ai-leadership`, `#jeff-dean`, `#organizational-change`, `#tech-industry`

---

<a id="item-2"></a>
## [ChainDrop 蠕虫攻陷 npm 逾 1300 个包](https://www.bleepingcomputer.com/news/security/massive-chaindrop-npm-supply-chain-attack-infects-hundreds-of-packages/) ⭐️ 9.0/10

自我传播的 ChainDrop 蠕虫已入侵 npm 仓库上超过 1300 个包，包括 Keyv、Cacheable 等热门缓存工具，通过攻破维护者账号并滥用 GitHub Actions 发布恶意版本。受影响包的合计月下载量达数十亿次，构成一次大规模供应链攻击。 这是 npm 历史上最大规模的供应链攻击之一，涉及月下载量达数十亿的软件包，对整个 JavaScript 生态构成严重威胁。任何安装过受影响版本的开发者都应视系统为已失陷，并立即轮换凭证。 恶意版本中的 setup.mjs 投放器和 Math_Symbol.js 窃密脚本会在 npm install 时自动执行，窃取 GitHub、npm、AWS 和 Kubernetes 等凭证。域名 npm-cache[.]com 可作为失陷指标（IoC），且攻击仍在持续扩散，受影响包数量预计还会增加。

telegram · zaihuapd · 8月5日 03:04

**背景**: 供应链攻击针对软件供应链中安全性较弱的环节（如开源软件包）注入恶意代码，进而感染下游用户。在此次事件中，ChainDrop 蠕虫通过攻破维护者账号并利用 GitHub Actions 等受信任的 CI 流程发布恶意版本来自我传播，使其更难被发现。失陷指标（IoC）是用于确认系统是否已被入侵的取证痕迹。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/08/04/chaindrop-supply-chain-compromise-anatomy-self-propagating-worm/">ChainDrop supply chain compromise: Anatomy of a self ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack</a></li>
<li><a href="https://en.wikipedia.org/wiki/Indicator_of_compromise">Indicator of compromise</a></li>

</ul>
</details>

**标签**: `#npm`, `#supply-chain`, `#security`, `#malware`, `#worm`

---

<a id="item-3"></a>
## [杰夫·迪恩离开谷歌，创办 Discovery Loop](https://www.discoveryloop.com/) ⭐️ 8.0/10

杰夫·迪恩（Jeff Dean）与几位资深谷歌 AI 研究员离开谷歌，共同创办了 Discovery Loop，一家旨在自动化机器学习研究与工程中实验循环的初创公司。该项目初期聚焦 AI/ML，但计划扩展到更广泛的科学发现与工程挑战。 这件事意义重大，因为它标志着“由 AI 驱动的全自动化科研”这一方向正获得越来越多的关注与投入，该方向因安德烈·卡尔帕西（Andrej Karpathy）的“autoresearch”概念而广为人知。若取得成功，它可能极大加速药物研发、芯片设计乃至更多科学与工程领域的发现进程。 该公司的公开策略是自动化实验循环，并同时构建机器学习与大规模系统方面的专业能力。目前尚不清楚物理实验将如何被自动化，因为 AI 可以在数字领域高速迭代，但在现实世界中仍受制于实体实验设施。

hackernews · xtreak29 · 8月5日 16:19 · [社区讨论](https://news.ycombinator.com/item?id=49184960)

**背景**: “自动化实验循环”指的是让 AI 智能体在最少人类干预下提出假设、设计实验、执行实验并分析结果。2026 年，安德烈·卡尔帕西发布了“autoresearch”，一个 600 行的 Python 脚本，展示了在安全护栏内运行的自主实验循环。Discovery Loop 希望大规模推广这一理念，并借助创始团队在谷歌构建 TensorFlow 及大语言模型基础设施等大规模系统时积累的经验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/08/05/technology/google-researchers-ai-startup.html">Four Top Google A.I. Researchers Form New Start-Up</a></li>
<li><a href="https://www.wired.com/story/jeff-dean-google-discovery-loop-startup/">Google’s Top AI Brains Are Leaving to Launch Discovery Loop ...</a></li>
<li><a href="https://www.discoveryloop.com/">Discovery Loop — Continuous Exploration</a></li>

</ul>
</details>

**社区讨论**: 评论者很快将 Discovery Loop 与卡尔帕西的 autoresearch 相提并论，称其为“机构化、大规模扩展版”的 autoresearch。也有人对自动化物理实验表示怀疑，指出 AI 缺乏实体；更有评论开玩笑说，谷歌是在为资深人才打造“养老院”，好让他们不被竞争对手挖走。

**标签**: `#AI/ML`, `#Research Automation`, `#Experimental Loop`, `#Large-Scale Systems`, `#Scientific Discovery`

---

<a id="item-4"></a>
## [专用开源模型以 100 倍更低成本击败 GPT-5.6 Sol](https://neon.com/blog/how-castform-neon-beats-frontier-models-on-price-and-efficiency) ⭐️ 8.0/10

Neon 的 Castform 专用开源模型据称在检索任务上超越了 OpenAI 的 GPT-5.6 Sol，而成本仅为后者的 1/100。这一说法出自 neon.com 的博客文章，在社区引发了关于专用模型的讨论。 这一结果挑战了前沿通用模型总是最优选择的假设，表明针对特定任务的专用开源模型可以大幅降低成本、提升效率。它也凸显了模型路由（即系统将每个请求分配给最合适模型）日益重要。 该博客未公布具体性能指标，仅称 Castform 在检索任务上以 100 倍的更低推理成本胜过 GPT-5.6 Sol。这里的成本比较通常指推理成本，而检索是指从文档或数据库中找出相关信息。

hackernews · moonikakiss · 8月5日 18:18 · [社区讨论](https://news.ycombinator.com/item?id=49186762)

**背景**: GPT-5.6 是 OpenAI 于 2026 年 7 月发布的系列大语言模型，包含 Luna、Terra 和 Sol 三个版本，其中 Sol 能力最强。模型路由是一种将每个查询分配给最合适模型的优化技术，已成为降低成本的行业做法。像 Castform 这样的开源模型可以自由下载和部署，比按 API 调用的前沿模型更具成本优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6_Sol">GPT-5.6 Sol</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT‑5.6 Sol: a next-generation model - OpenAI</a></li>
<li><a href="https://www.braintrust.dev/articles/best-llm-routers-2026">Best LLM routers and model routing platforms in 2026 - Articles - Braintrust</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍对专用模型表示认同，将其比作“使用合适的数据结构”，并指出小型模型在事实检索上可能超越更大的同类模型。也有用户提出方法学问题，例如检索在大规模数据上的表现，以及是否应对比较小的 GPT-5.6 Luna 变体。整体态度积极，同时关注评测设计和模型选择的合理性。

**标签**: `#AI/ML`, `#retrieval`, `#model-efficiency`, `#open-models`, `#LLM`

---

<a id="item-5"></a>
## [Meta 投放含 AI 生成儿童性虐待图像的广告](https://www.wired.com/story/meta-ran-ads-that-contained-ai-generated-child-sexual-abuse-imagery/) ⭐️ 8.0/10

《连线》杂志报道称，Meta 投放了包含 AI 生成儿童性虐待图像的广告，这表明其内容审核系统存在严重失职。尽管 Meta 有禁止此类内容的政策，这些广告据称仍通过了审查。 这一事件凸显了 AI 生成儿童性虐待材料日益严峻的挑战，以及大型平台无法可靠地在大规模范围内检测此类内容的问题。它引发了关于平台责任、监管执法以及生成式 AI 工具安全性的紧迫质疑。 《连线》的报道指出 Meta 广告生态系统中存在系统性的审核漏洞，AI 生成的儿童性虐待材料得以上架。社区评论还提到 YouTube 等其他平台存在类似问题，并指出用户举报后公司响应耗时漫长。

hackernews · malshe · 8月5日 19:47 · [社区讨论](https://news.ycombinator.com/item?id=49187977)

**背景**: AI 生成的儿童性虐待材料（AI CSAM）是指完全由生成式 AI 系统创建或在其辅助下创建的儿童性虐待图像。这些逼真的合成图像越来越难以与真实虐待材料区分，而检测技术仍在发展之中。像 Meta 这样的平台依赖自动化审核工具和人工审核相结合，但 AI 生成内容的数量级和复杂程度可能压垮这些系统。法律框架也正在追赶，许多州和国家已将创建和传播 AI 辅助的儿童性虐待材料定为犯罪。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.iwf.org.uk/about-us/why-we-exist/our-research/how-ai-is-being-abused-to-create-child-sexual-abuse-imagery">AI CSAM Report 2026: Harm Without Limits | IWF</a></li>
<li><a href="https://link.springer.com/article/10.1007/s42452-025-08174-9">Deepfake detection: critical review of state-of-the-art ...</a></li>

</ul>
</details>

**社区讨论**: 评论者对平台审核表示失望，有人指出 Meta 还投放煽动针对政客暴力的广告，还有人说在 YouTube 上看到露骨广告。有人认为罚款只是被当作经营成本，不会改变企业行为；也有人将现状与有人工编辑把关的地方报纸进行对比并表达不满。还有用户回忆，多年前向大公司举报类似内容，花了数月才得到处理。

**标签**: `#AI-safety`, `#content-moderation`, `#Meta`, `#ethics`, `#advertising`

---

<a id="item-6"></a>
## [Cloudflare 发布面向智能体、应用与工作的开源 OS](https://blog.cloudflare.com/cloudflare-os/) ⭐️ 8.0/10

Cloudflare 发布了 Cloudflare OS——一个基于 Cloudflare Workers 构建智能体、应用和工作的开源平台。它包含一个智能体工作区（提供可编写和运行代码的隔离运行时），以及一套用于安全访问内部系统的安全与治理框架。 这一发布标志着 Cloudflare 平台方向的重大转变：将 AI 智能体与无服务器 Workers 融合，并重拾创造者早前的 Sandstorm 愿景。它可能影响企业构建和治理 AI 内部工具的方式，不过一些用户可能担心被锁定。 Cloudflare OS 是开源的，以每家公司在平台中整理的上下文和技能为基础，智能体可在隔离运行时中执行代码。评论者指出，它直接使用了 pi-agent，而非 Cloudflare 自研的 Agents SDK、Think 或 Flue 框架。

hackernews · speckx · 8月5日 13:58 · [社区讨论](https://news.ycombinator.com/item?id=49182996)

**背景**: Cloudflare Workers 是 Cloudflare 的无服务器执行平台，可让代码在其全球边缘网络上运行。Cloudflare OS 的创造者 Kenton Varda 曾于 2014 年推出 Sandstorm，一个面向自托管 Web 应用的平台；Cloudflare OS 被描述为基于 Workers 重构并深度融入 AI 的 Sandstorm。Cloudflare 将这款产品定位为开源的 AI 操作系统，企业可以围绕自己的上下文、工具和规则加以塑造。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/cloudflare-os/">Cloudflare OS: an open platform for agents, apps, and work | The Cloudflare Blog</a></li>
<li><a href="https://www.phoronix.com/news/Cloudflare-OS">Cloudflare Announces Open-Source Cloudflare OS As AI "Operating System" - Phoronix</a></li>
<li><a href="https://www.cloudflare.com/products/workers/">Cloudflare Workers - Global Serverless Functions Platform</a></li>

</ul>
</details>

**社区讨论**: 社区评价褒贬不一：有人欢迎 Sandstorm 的回归，但也有不少人担心被厂商锁定，并批评“OS”这个叫法没有实际意义。技术型用户还质疑，为什么 Cloudflare 使用 pi-agent，而不是自研的 Agents SDK、Think 或 Flue 框架。

**标签**: `#cloudflare`, `#agents`, `#platform`, `#workers`, `#ai`

---

<a id="item-7"></a>
## [Claude Fable 5 仅凭一条推文构建出可玩的《Raccoon Heist》游戏](https://simonwillison.net/2026/Aug/5/raccoon-heist/#atom-everything) ⭐️ 8.0/10

西蒙·威利森（Simon Willison）使用运行在 Claude Code for web 中的 Claude Fable 5，仅凭其 2022 年 8 月一条推文中的文字和概念图，就构建出了一款完整可玩的浏览器游戏《Raccoon Heist》（浣熊大劫案）。该游戏已上线 GitHub Pages，完整源代码也已发布在 GitHub 上。 这表明 Mythos 级别的模型可以在没有人工指导的情况下，把一个仅有百余字的模糊概念变成可运行的游戏，标志着 AI 辅助软件开发的一个重要里程碑。对于想了解前沿编程智能体能在多大程度上端到端承担开发流程的 AI 研究者和开发者来说，这件事很有参考价值。 为了绕开 Claude Code for web 难以实时测试的问题，威利森采用了 GitHub Pages 的方案：先创建仓库，让 Claude 尽快提交一个 index.html，然后在生成的 claude/... 分支上启用 Pages，以便在智能体工作时实时观察进度。文章也强调，这只是一个演示，而非系统性的基准测试。

rss · Simon Willison · 8月5日 19:42

**背景**: Claude Fable 5 是 Anthropic 于 2026 年 6 月 9 日发布的“Mythos 级”模型，是对限制更严格的 Claude Mythos 5 的通用安全版本，并在网络安全、生物与化学、模型蒸馏等提示词上增加了安全规则。Claude Code 是 Anthropic 的智能体式编码工具，可在终端、IDE 或网页端编辑文件、运行命令并配合 GitHub 仓库工作。原推文本是 2022 年 8 月一次“60 秒原型”实验的产物：GPT-3 采用文本补全方式写出了游戏描述，DALL-E 则生成了概念图。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable_5">Claude Fable 5</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**标签**: `#AI`, `#Claude`, `#game development`, `#generative AI`, `#coding assistant`

---

<a id="item-8"></a>
## [LLM 0.32 发布：新增推理痕迹、Responses API 和服务端工具](https://simonwillison.net/2026/Aug/4/new-release-of-llm/#atom-everything) ⭐️ 8.0/10

Simon Willison 发布了 LLM 0.32，这是该项目自启动以来最重要的一次更新，新增了可见的推理痕迹、对 OpenAI Responses API 的支持、CodeInterpreter 和 WebSearch 等服务端工具，以及重新设计的内容可寻址 SQLite 日志。新的 llm openai endpoint 命令可以对任意兼容 OpenAI 的端点执行一次性提示。 此次发布通过将推理模型的中间「思考」过程输出到标准错误，显著改善了开发者体验，同时保持标准输出干净以便管道处理。它还使 LLM 跟上现代提供商的功能，如服务端工具和 Responses API，扩展了其作为通用 LLM 命令行工具的角色。 推理痕迹会输出到标准错误，并可通过 -R/--hide-reasoning 选项隐藏。新的默认模型是 GPT-5.6 Luna；OpenAI 的服务端工具包括 CodeInterpreter 和 WebSearch，而 llm-anthropic 插件新增了 WebSearch、WebFetch、CodeExecution 和 AnthropicMCP。

rss · Simon Willison · 8月4日 23:58

**背景**: LLM 是 Simon Willison 推出的一个开源命令行工具，用于与各种大语言模型交互。推理痕迹是指 AI 模型在生成最终答案之前产生的中间推理步骤；内容可寻址存储使用加密哈希作为键，以确保数据的唯一性和完整性。OpenAI Responses API 于 2025 年 3 月发布，将聊天补全与高级工具调用能力相结合，而服务端工具允许模型在单次请求中调用提供商托管的函数，如代码执行或网络搜索。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/OpenAI_Responses_API">OpenAI Responses API</a></li>
<li><a href="https://jumpcloud.com/it-index/what-are-reasoning-traces-in-ai">What Are Reasoning Traces in AI ? - JumpCloud</a></li>
<li><a href="https://en.wikipedia.org/wiki/Content-addressable_storage">Content-addressable storage</a></li>

</ul>
</details>

**标签**: `#LLM`, `#OpenAI`, `#CLI`, `#SQLite`, `#plugins`

---

<a id="item-9"></a>
## [Monodratic：学习式乘积哈希路由实现稀疏因果注意力](https://www.reddit.com/r/MachineLearning/comments/1vg3jda/monodratic_learned_producthash_routing_for_sparse/) ⭐️ 8.0/10

一位独立研究者发布了 Monodratic，这是一种稀疏因果注意力架构，利用学习式乘积哈希路由选取固定数量的远程源块，然后执行精确 softmax。在合成关联回忆基准上，仅从 5 个候选远程块中选取 2 个，其平均准确率达 99.35%。 稀疏注意力是扩展 Transformer 以处理更长上下文的关键方向，而 Monodratic 表明，学习式路由可以在限制注意力预算的同时保持很强的回忆能力。它的发布可能会推动更多关于用学习式索引结构替代固定启发式规则来组织注意力的研究。 实验是合成数据上的测试，实现是可移植的 PyTorch 而非融合内核，因此论文没有声称具备自然语言质量或部署速度上的优势。稀疏选定集合注意力与密集选定掩码基准的最大绝对误差为 1.43e-6；在 4,096 到 32,768 token 范围内，打包的 CPU 路由实现拟合缩放指数为 0.993。

reddit · r/MachineLearning · /u/dttdrv · 8月5日 10:28

**背景**: 标准因果注意力允许每个 token 关注所有之前的 token，因此复杂度随序列长度 n 呈 O(n²) 增长；稀疏注意力只对一部分键计算注意力，以减少计算成本。Monodratic 在旋转位置编码（RoPE）之后使用学习式乘积哈希路由，把源块分配到有界的 posting list，并让每个查询探测乘积地址。之后，模型对选中的远程块和保证包含的本地块执行精确的因果 softmax。关联回忆是一种合成任务，要求模型从上下文中回忆与某个键相关联的值，常用于检验序列模型的记忆与检索能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Misul-Computing/Monodratic">GitHub - Misul-Computing/Monodratic: Learned product-hash ...</a></li>
<li><a href="https://arxiv.org/abs/2312.04927">[2312.04927] Zoology: Measuring and Improving Recall in ... Associative memory (psychology) - Wikipedia Revisiting associative recall in modern recurrent models Associative Recall Task Associative Recall Task - Psychological Scales & Instruments ... Associative Recall: Mechanisms & Models - emergentmind.com Associative Recall in Memory Systems - emergentmind.com</a></li>

</ul>
</details>

**标签**: `#sparse attention`, `#efficient transformers`, `#associative recall`, `#machine learning research`, `#product hashing`

---

<a id="item-10"></a>
## [马斯克宣布 SpaceX 将独家采用英伟达 AI 架构](https://wccftech.com/elon-musk-commits-spacex-exclusively-to-nvidia-gpus-citing-theyre-the-best/) ⭐️ 8.0/10

马斯克在 8 月 4 日 SpaceX 首次财报电话会上宣布，SpaceX 的 AI 服务将独家采用英伟达 AI 架构，包括 Vera Rubin 平台。SpaceX 计划在地面和轨道数据中心部署英伟达 Vera Rubin NVL72 机架系统，目标是在今年年底前超过 2 吉瓦的 AI 算力，并在 2027 年前接近 10 吉瓦。 这一独家承诺使英伟达成为 SpaceX 不断扩展的太空 AI 计划（包括 Starmind 轨道数据中心项目）的基础 AI 计算供应商。这标志着英伟达在 AI 加速器市场上对竞争对手的重大胜利，也凸显了 AI 算力在太空领域日益增长的重要性。 SpaceX 将采用英伟达 Vera Rubin NVL72 机架系统，这是一种包含 72 个通过 NVLink 互连的 GPU 的机架级架构。这些系统将用于 Starmind 卫星项目，相关卫星计划明年开始发射；英伟达此前已推出面向太空的 Space-1 Vera Rubin 模块，支持在轨 AI 推理。

telegram · zaihuapd · 8月5日 02:04

**背景**: 英伟达 Vera Rubin 平台是其下一代 AI 架构，接替 Blackwell，Rubin GPU 在 FP4 精度下提供高达 50 稀疏 petaflops 的性能。NVL72 机架级设计最初随 Blackwell（GB200 NVL72）推出，是单个机架内的百亿亿次级系统，专为万亿参数 AI 训练和推理而设计。SpaceX 的 Starmind 项目由马斯克于 2026 年 6 月确认，标志着其从 Starlink 互联网星座转向轨道 AI 数据中心网络。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rubin_(microarchitecture)">Rubin (microarchitecture) - Wikipedia</a></li>
<li><a href="https://developer.nvidia.com/blog/inside-the-nvidia-rubin-platform-six-new-chips-one-ai-supercomputer/">Inside the NVIDIA Vera Rubin Platform: Six New Chips, One AI ...</a></li>
<li><a href="https://cryptobriefing.com/spacex-starmind-ai-satellite-network/">SpaceX plans Starmind , an AI network powered by satellites in orbit</a></li>

</ul>
</details>

**标签**: `#AI`, `#NVIDIA`, `#SpaceX`, `#Space Computing`, `#Hardware`

---

<a id="item-11"></a>
## [DeepSeek 重启第二轮融资，投前估值 5000 亿元](https://finance.sina.com.cn/wm/2026-08-05/doc-inimfmyv1554159.shtml) ⭐️ 8.0/10

DeepSeek 已重启第二轮融资，计划募资 500 亿元，投前估值约 5000 亿元，预计 8 月下旬完成签约。本轮融资于 7 月中旬开启、7 月底暂停，如今在创始人梁文锋对疑似泄露的“投资者会议实录”表达不满之后重新启动。 本轮融资体现了市场对 DeepSeek 的强烈信心，投前估值较首轮提升约 43%，达到 5000 亿元。若顺利完成，两轮合计募资将达 1000 亿元，使 DeepSeek 成为资金最充裕的 AI 创业公司之一，并加剧中国 AI 领域的融资竞争。 暂停据称源于创始人梁文锋对网上流传的疑似泄露“面向投资者的会议实录”不满，投资方希望融资重启后低调进行。部分此前积极接触的机构表示尚未接到重启消息，说明融资通道仍处于部分暂缓状态。

telegram · zaihuapd · 8月5日 02:46

**背景**: DeepSeek 是中国领先的人工智能公司。“投前估值”指公司获得新一轮投资前的价值；按本轮 5000 亿元投前估值计算，投资方投入 500 亿元将获得约 9% 的股份。DeepSeek 首轮融资于 4 月开启、6 月完成交割，募资 500 亿元、估值超 3500 亿元，因此本轮估值提升约 43%。此次暂停与重启也反映出融资进程对创始人态度和投资方关系的敏感性。

**标签**: `#DeepSeek`, `#AI funding`, `#venture capital`, `#valuation`

---

<a id="item-12"></a>
## [FFmpeg 9.0 发布，新增动画 WebP 与 Vulkan 滤镜及 AI 辅助开发](https://news.ycombinator.com/item?id=49166202) ⭐️ 8.0/10

FFmpeg 9.0 正式发布，新增了动画 WebP 解码器与分离器、v360_vulkan 滤镜、Playdate 视频编码器与封装器、HE-AAC 960 解码、transpose_cuda 滤镜、AMF 帧率转换器，以及 ONNX Runtime DNN 后端。开发团队还通过 Anthropic 的 Claude for Open Source Program 免费使用了六个月的 Claude Max，用于帮助查找缺失的向后移植。 FFmpeg 是多媒体处理领域的基石，本次发布带来了现代格式支持和 GPU 加速滤镜，确保其继续成为视频处理的首选工具。在开源维护中使用 Claude 也标志着 AI 辅助在关键基础设施项目中的趋势日益增长，既带来了机遇，也引发了安全方面的担忧。 由 Lynne 开发的 v360_vulkan 滤镜是一个基于 Vulkan 计算的 360 度视频转换滤镜，支持等距柱状投影和立方体贴图投影，已于 2026 年 4 月合入。AMD 贡献的 ONNX Runtime 后端利用 GPU 和 NPU 增强了 DNN 滤镜中的 AI 模型执行能力。Playdate 编码器生成的 .pdv 文件可通过 Playdate SDK 或 Playorama 播放器在 Playdate 设备上播放。

telegram · zaihuapd · 8月5日 10:32

**背景**: FFmpeg 是领先的开源多媒体框架，用于处理音视频的解码、编码、滤镜和转码。动画 WebP 是一种支持动画的图像格式，压缩率优于 GIF。Vulkan 是低开销的 GPU API，ONNX Runtime 是跨平台的机器学习模型推理引擎。Playdate 是一款掌上游戏机，Claude 是 Anthropic 的 AI 助手，通过专门计划免费提供给开源维护者使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.ffmpeg.org/FFmpeg/FFmpeg/pulls/22725">#22725 - lavfi/v360: add a Vulkan-compute based filter ...</a></li>
<li><a href="https://github.com/hteumeuleu/pdv">GitHub - hteumeuleu/pdv: Playdate PDV encoder</a></li>
<li><a href="https://thelinuxcamp.com/news/amd-introduces-onnx-runtime-backend-for-ffmpeg-s-dnn-filter-mqte6kmz">AMD Introduces ONNX Runtime Backend for FFmpeg 's DNN Filter</a></li>

</ul>
</details>

**社区讨论**: 新闻中提到，一些社区成员对 AI 辅助开发的安全审查流程表达了担忧，尤其是对 FFmpeg 使用 Claude 这一做法。这反映出在开源项目中，如何在 AI 带来的效率提升与严格的安全审计需求之间取得平衡，是一个更广泛的讨论话题。

**标签**: `#FFmpeg`, `#multimedia`, `#open-source`, `#AI-assisted development`, `#video encoding`

---