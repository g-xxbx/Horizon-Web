---
layout: default
title: "Horizon Summary: 2026-07-27 (ZH)"
date: 2026-07-27
lang: zh
---

> 从 30 条内容中筛选出 10 条重要资讯。

---

1. [Fastjson 1.x 无 Gadget 高危 RCE 漏洞](#item-1) ⭐️ 10.0/10
2. [vLLM v0.26.0 添加 Inkling 模型并提升性能](#item-2) ⭐️ 9.0/10
3. [法官驳回谷歌 DMCA 抓取抗辩](#item-3) ⭐️ 8.0/10
4. [论坛软件从 React 迁移到 HTMX](#item-4) ⭐️ 8.0/10
5. [Paged Out #9：深度技术黑客杂志发布](#item-5) ⭐️ 8.0/10
6. [Bun 用 Rust 重写已投入使用，v1.4 发布延期](#item-6) ⭐️ 8.0/10
7. [用 HTTP 和 JSON 重新构想现代电子邮件](#item-7) ⭐️ 8.0/10
8. [个人研究发现六大前沿语言模型行为左倾](#item-8) ⭐️ 8.0/10
9. [Kimi K3：开源 2.8 万亿参数模型，前端编程排行榜登顶](#item-9) ⭐️ 8.0/10
10. [中芯国际试运行首台国产 DUV 光刻机](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Fastjson 1.x 无 Gadget 高危 RCE 漏洞](https://t.me/zaihuapd/42797) ⭐️ 10.0/10

安全研究人员 Kirill Firsov 披露了 Fastjson 1.x 版本 1.2.68 至 1.2.83 存在高危远程代码执行漏洞。该漏洞无需启用 autoType 或依赖 classpath gadget 链。 此漏洞非常严重，因为 Fastjson 1.x 在 Java 应用中广泛使用且已停止维护，官方不会发布补丁。该漏洞影响 JDK 8、17、21 等多个版本。 该漏洞无需任何 gadget 链或开启 autoTypeSupport 即可利用。推荐的唯一缓解措施是升级到 Fastjson2。

telegram · zaihuapd · 7月27日 10:31

**背景**: Fastjson 是一个流行的 Java JSON 序列化/反序列化库，此前曾出现反序列化安全问题。Gadget 链是反序列化过程中可以链接起来实现代码执行的现有代码片段序列。autoType 是 Fastjson 中允许在反序列化时自动解析类型的特性，通常利用此类漏洞时需要开启该功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@dub-flow/deserialization-what-the-heck-actually-is-a-gadget-chain-1ea35e32df69">Deserialization: What the Heck *Actually* Is a Gadget Chain? | by Florian Walter | Medium</a></li>
<li><a href="https://pentesterlab.com/glossary/gadget-chain">Gadget Chain: Definition & Security Context | PentesterLab Glossary</a></li>

</ul>
</details>

**标签**: `#Fastjson`, `#RCE`, `#Java`, `#security`, `#vulnerability`

---

<a id="item-2"></a>
## [vLLM v0.26.0 添加 Inkling 模型并提升性能](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 9.0/10

vLLM v0.26.0 引入了对新型 Inkling 模型系列的支持、DeepSeek-V4 的优化、fp32 lm_head 和灵活的注意力后端。该版本包含来自 212 位贡献者的 411 次提交。 该版本增强了 vLLM 作为领先的 LLM 推理引擎的地位，能够高效部署像 Inkling（975B 参数）这样的大模型，并提升了 DeepSeek-V4 的性能。灵活的注意力后端和新的模型支持扩展了 vLLM 在多样化硬件和架构上的适用性。 Inkling 模型是一个 975B 参数的混合专家（MoE）Transformer，支持高达 100 万上下文 token，并通过分段 CUDA 图和 Hopper FA4 相对注意力提供支持。DeepSeek-V4 的性能提升包括专用路由内核，端到端 TPOT 提升 2.94%，以及 fused_topk_bias 内核加速 1.5-2 倍。

github · khluu · 7月27日 01:06

**背景**: vLLM 是一个开源的高吞吐量 LLM 推理引擎，广泛用于服务大型语言模型。它支持多种模型架构和优化，如 PagedAttention 和连续批处理。v0.26.0 版本引入了来自 Thinking Machines Lab 的 Inkling 模型系列，这是一个在不到九个月的时间内从头训练的大规模 MoE 模型。该版本还包括针对 DeepSeek-V4 的优化以及用于提高准确性的 fp32 lm_head 等新功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://www.technology.org/2026/07/16/thinking-machines-inkling-open-weights-model/">Thinking Machines Releases Inkling, Its First Open-Weights Model, Trained From Scratch</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#performance optimization`, `#open-source`, `#AI/ML`

---

<a id="item-3"></a>
## [法官驳回谷歌 DMCA 抓取抗辩](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

一位联邦法官裁定，谷歌不能利用《数字千年版权法》（DMCA）来阻止第三方抓取其搜索结果页面。该裁决驳回了谷歌关于抓取行为构成规避技术保护措施的法律论点。 这一裁决明确了 DMCA 反规避条款不适用于单纯抓取公开网络数据，这对数据获取、竞争以及 AI 训练中使用网络数据具有重大影响。它也凸显了版权法与数据抓取之间日益增长的紧张关系。 该案件涉及谷歌起诉 SerpAPI，后者抓取谷歌搜索结果以提供自定义 API。法官发现，谷歌的技术措施（如 CAPTCHA 和 IP 速率限制）并非主要用于版权保护，而这是 DMCA 索赔的必要条件。

hackernews · cdrnsf · 7月27日 18:15 · [社区讨论](https://news.ycombinator.com/item?id=49073513)

**背景**: 《数字千年版权法》（DMCA）包含禁止规避控制访问版权作品的技术措施的条款。在网络抓取领域，一些公司认为单纯抓取网站就规避了这些保护。然而，法院通常对将 DMCA 保护扩展到并非主要用于保护版权的措施持谨慎态度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.quinnemanuel.com/the-firm/publications/the-legal-landscape-of-web-scraping/">The Legal Landscape of Web Scraping</a></li>
<li><a href="https://nortonlaw.com/2026/05/14/dmca-section-1201-claims-the-new-battleground-for-ai-and-data-scraping-litigation/">DMCA Section 1201 Claims: The New Battleground for AI and Data Scraping Litigation - the NORTON law firm</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了不同的反应：一些人批评谷歌的法律策略是大型公司的典型做法（SoftTalker），而另一些人则指出谷歌缺乏良好的搜索结果 API（binarymax）。还有人对欧盟数据库权利与美国版权法进行了讨论（akrymski），以及抓取搜索结果以揭露广告骗局的重要性（jonatron）。

**标签**: `#legal`, `#web scraping`, `#DMCA`, `#Google`, `#search engines`

---

<a id="item-4"></a>
## [论坛软件从 React 迁移到 HTMX](https://misago-project.org/t/removing-reactjs-from-the-codebase-and-adapting-htmx-for-ui-interactivity/1267/) ⭐️ 8.0/10

作者详细介绍了从其论坛软件中移除 React.js 并采用 HTMX 实现服务器驱动交互的过程，指出这带来了更好的性能和更简单的前端架构。 这次迁移代表了更广泛的行业趋势，即针对特定类型的 Web 应用，用服务器驱动的方法取代复杂的前端框架，这可能会影响开发者重新评估他们的前端架构。 HTMX 通过 HTML 属性和服务端推送事件实现动态交互，消除了虚拟 DOM 并降低了 JavaScript 复杂度。

hackernews · Ralfp · 7月27日 09:58 · [社区讨论](https://news.ycombinator.com/item?id=49067301)

**背景**: HTMX 是一个 JavaScript 库，允许开发者使用 HTML 属性而非编写自定义 JavaScript 来构建动态 Web 界面。它通过发送 AJAX 请求并用 HTML 片段更新页面部分来实现服务器驱动的交互，与在浏览器中管理状态和 DOM 更新的客户端框架（如 React）形成对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Htmx">Htmx</a></li>
<li><a href="https://htmx.org/">htmx - high power tools for html</a></li>

</ul>
</details>

**社区讨论**: 社区普遍欢迎转向 HTMX，许多人指出它适合内容密集型的论坛网站。一些用户报告了处理大 HTML 负载时的性能问题，而另一些用户则推荐了 Phoenix LiveView 等替代的服务器驱动方案。

**标签**: `#HTMX`, `#React.js`, `#web development`, `#server-side rendering`, `#frontend architecture`

---

<a id="item-5"></a>
## [Paged Out #9：深度技术黑客杂志发布](https://pagedout.institute/download/PagedOut_009.pdf) ⭐️ 8.0/10

Paged Out #9 已发布，这是一本免费的实验性技术杂志，每篇文章仅一页，涵盖从 C 语言编程到亚像素渲染和可计算平铺等主题。 该杂志在 Hacker News 上因其深度技术内容和类似于 2600 及 Phrack 等经典黑客出版物的风格而备受赞誉，显示出强烈的社区参与度和黑客好奇精神的复兴。 Paged Out #9 包含《C 语言入门》、《亚像素动物园》以及一篇关于可计算平铺的文章，该文章未注明出处地重新发现了王浩在 1960 年代的工作，将平铺问题与停机问题联系起来。

hackernews · laurensr · 7月27日 14:22 · [社区讨论](https://news.ycombinator.com/item?id=49070138)

**背景**: Paged Out 是一本免费的实验性技术杂志，每页只刊登一篇文章，内容涵盖编程、安全、复古计算机等。亚像素渲染是一种利用每个像素的红绿蓝子像素来提高文本和图形显示分辨率的技术。可计算平铺是王浩等人探索的领域，它将平面平铺与可计算性理论联系起来，表明多米诺骨牌问题等价于停机问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Subpixel_rendering">Subpixel rendering</a></li>
<li><a href="https://link.springer.com/chapter/10.1007/978-0-387-09680-3_13">Computability of Tilings | Springer Nature Link</a></li>
<li><a href="https://pagedout.institute/?page=about.php">About ⁂ Paged Out !</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者表达了强烈的正面评价，将 Paged Out #9 比作经典杂志 2600 和 Phrack。他们特别提到了《C 语言入门》和《亚像素动物园》等文章，并对可计算平铺文章提供了背景信息，指出该文章未注明出处地重新发现了王浩的工作。

**标签**: `#technical magazine`, `#programming`, `#computer science`, `#graphics`, `#tilings`

---

<a id="item-6"></a>
## [Bun 用 Rust 重写已投入使用，v1.4 发布延期](https://lockwood.dev/ai/2026/07/27/how-is-the-bun-rewrite-in-rust-going.html) ⭐️ 8.0/10

Bun 的 Rust 重写版本已部署于 Claude Code，v1.4 版本发布推迟，直到通过特定数量的 Node.js 兼容性测试。 用 Rust 重写可能显著提升 Bun 的性能和安全性，而 v1.4 的延期则体现了对 Node.js 兼容性的重视，这对广泛采用至关重要。 整个从 Zig 到 Rust 的 100 万行重写工作仅用 11 天，借助大型语言模型完成；v1.4 版本发布因等待通过目标数量的 Node.js 兼容性测试而推迟。

hackernews · tomlockwood · 7月27日 11:12 · [社区讨论](https://news.ycombinator.com/item?id=49067854)

**背景**: Bun 是一个 JavaScript 运行时，旨在作为 Node.js 的更快速替代方案。它最初用 Zig 编写，但团队决定重写为 Rust，原因在于 Rust 更成熟的生态系统和更强的安全性。这一大规模重写借助 AI 代码翻译在极短时间内完成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bunjs.run/bun-zig-to-rust-rewrite">How Bun Rewrote 1 Million Lines from Zig to Rust in 11 Days Using AI</a></li>
<li><a href="https://www.cosmicjs.com/changelog/bun-rust-rewrite-javascript-runtime">Why Bun is Rewriting in Rust (And What It Means for JavaScript ...)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>

</ul>
</details>

**社区讨论**: 社区讨论中，Jarred 介绍了重写版本的部署和延期情况；SquareWheel 提醒不要仅凭提交指标预测开发速度；benjiro29 批评了在严肃开发中过度依赖 LLM 的做法；bendmorris 提到了一种竞争方法，该法修复了原始 Zig 代码库，实现了亚秒级构建。

**标签**: `#Bun`, `#Rust`, `#JavaScript`, `#Runtime`, `#Node.js`

---

<a id="item-7"></a>
## [用 HTTP 和 JSON 重新构想现代电子邮件](https://en.andros.dev/blog/d7ed8b07/modern-email-can-be-built-from-borrowed-parts/) ⭐️ 8.0/10

一篇文章提出，现代电子邮件可以通过借用 HTTP 和其他协议的组件来重建，从而减少对传统 SMTP 基础设施的依赖。文章强调 JMAP 是一个用标准 HTTP 和 JSON 替代 IMAP 的协议示例。 如果被采用，这种方法可以简化电子邮件基础设施，提高安全性和互操作性，并降低开发成本。这对电子邮件客户端开发者、服务器管理员以及更广泛的通信生态系统具有重要意义。 文章建议利用现有的网络标准，但指出网络效应和与 SMTP 的向后兼容性带来了采用挑战。JMAP 已经证明了使用 HTTP+JSON 进行电子邮件访问的可行性。

hackernews · andros · 7月27日 08:27 · [社区讨论](https://news.ycombinator.com/item?id=49066639)

**背景**: 传统电子邮件依赖于 SMTP 进行传输，使用 IMAP 或 POP3 进行访问，这些协议已有数十年历史。JMAP（JSON 元应用协议）是一个现代开放标准，它用 HTTP 和 JSON 替代 IMAP 和 SMTP 提交，使电子邮件系统更易于开发和安全。MTA-STS（MTA 严格传输安全）是另一个扩展，利用 HTTPS/TLS 来强制执行加密的邮件投递。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/JSON_Meta_Application_Protocol">JSON Meta Application Protocol - Wikipedia</a></li>
<li><a href="https://jmap.io/">JSON Meta Application Protocol Specification ( JMAP )</a></li>
<li><a href="https://datatracker.ietf.org/doc/html/rfc8461">RFC 8461 - SMTP MTA Strict Transport Security ( MTA - STS )</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了历史上关于解决垃圾邮件的提议，一位用户指出了 1990 年代一系列不可行的解决方案。其他人则主张进行根本性变革，比如对电子邮件收费和需要收件人批准，而一些人指出网络效应使得替换电子邮件变得困难。少数人维护当前的技术栈，认为它并没有人们所说的那么糟糕。

**标签**: `#email`, `#SMTP`, `#protocols`, `#web`, `#communication`

---

<a id="item-8"></a>
## [个人研究发现六大前沿语言模型行为左倾](https://www.reddit.com/r/MachineLearning/comments/1v8fnzw/evaluated_6_frontier_llms_gpt54_claude_sonnet_46/) ⭐️ 8.0/10

一项个人评估对六大前沿 LLM（GPT-5.4、Claude Sonnet 4.6、Claude Opus 4.7、Gemini Pro、Gemini Flash 和 Grok 4.3）在八个偏见基准上进行了测试，发现所有模型都表现出左倾行为，其中 Grok 在自我报告（右倾）与实际行为（左倾）之间存在差异。 这项研究揭示了最先进 AI 系统中存在的政治和种族偏见问题，引发了对 LLM 部署中公平性和中立性的担忧。它强调了需要更均衡的训练数据和评估方法，以减少无意的偏见。 在 BBQ 数据集的种族相关问题上，拒绝率显著：GPT-5.4 拒绝 20.3%，Claude Opus 4.7 拒绝 13.8%，Grok 拒绝 9.5%，Claude Sonnet 4.6 和 Gemini Pro 约 5%。局限性包括使用单一提示模板、未进行多轮平均，且评估由一位独立研究人员完成。

reddit · r/MachineLearning · /u/marggggggggg · 7月27日 22:37

**背景**: 偏见基准（如 WinoBias、BBQ、SeeGULL 和 OpinionsQA）用于评估模型在人口统计学刻板印象和政治倾向方面的表现。SeeGULL 是一个大规模刻板印象数据集，覆盖 178 个国家和 23 种语言。cajcodes 政治偏见数据集包含 658 条合成陈述，标注了从保守到自由的程度。OpinionsQA 测试模型与美国人口统计群体在堕胎、移民等话题上的一致性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/google-research-datasets/seegull">GitHub - google-research-datasets/seegull: SeeGULL is a broad-coverage stereotype dataset in English containing stereotypes about identity groups spanning 178 countries across 8 different geo-political regions across 6 continents, as well as state-level identities within the US and India. · GitHub</a></li>
<li><a href="https://huggingface.co/datasets/cajcodes/political-bias">cajcodes/political-bias · Datasets at Hugging Face</a></li>
<li><a href="https://arxiv.org/abs/2303.17548">[2303.17548] Whose Opinions Do Language Models Reflect?</a></li>

</ul>
</details>

**标签**: `#LLM bias`, `#fairness evaluation`, `#political bias`, `#racial bias`, `#frontier models`

---

<a id="item-9"></a>
## [Kimi K3：开源 2.8 万亿参数模型，前端编程排行榜登顶](https://t.me/zaihuapd/42793) ⭐️ 8.0/10

月之暗面发布了 Kimi K3，这是一个开源 2.8 万亿参数模型，在 Frontend Code Arena 中以 1679 分排名第一，超越了 Claude Fable 5。它采用 Kimi Delta Attention 和 Attention Residuals 架构，具备原生视觉能力和 100 万 token 上下文窗口。 Kimi K3 表明，开源模型能够在特定编程基准上与专有前沿模型竞争甚至超越，可能降低开发者和初创公司的门槛。其 2.8 万亿参数使其成为有史以来最大的开源模型之一，标志着开源 AI 规模的新高度。 Kimi K3 在 Frontend Code Arena 中从第 18 名（Kimi k2.6）跃升至第 1 名，在 7 个评测领域中 6 项居首，仅游戏领域落后。模型权重计划于 2025 年 7 月 27 日前发布。

telegram · zaihuapd · 7月27日 06:27

**背景**: Kimi Delta Attention 是一种线性注意力机制，旨在高效处理长上下文，通过更细粒度的门控扩展了 Gated DeltaNet。Attention Residuals 替代了 Transformer 中的标准残差连接，允许各层通过学习的注意力选择性聚合先前输出。Frontend Code Arena 根据真实用户构建应用和网站的 agentic 前端编码任务（HTML 和 React）来评估模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/arena/status/2077824029126504525">Arena.ai on X: "Big news: Kimi-K3 by @Kimi_Moonshot is now #1 in the Frontend Code Arena with 1679 pts, surpassing Claude Fable 5. This is a 17-place jump from Kimi-k2.6 (#18 -> #1). In Frontend, Kimi-K3 ranked #1 in 6 of 7 domains: Brand & Marketing, Reference-Based Design, Data & Analytics, Consumer Product, Simulations, and Content Creation Tools, landing #2 only in Gaming behind Fable 5. The full model weights will be released by July 27. Congrats to the @Kimi_Moonshot team on this major milestone!" / X</a></li>
<li><a href="https://arxiv.org/abs/2510.26692">[2510.26692] Kimi Linear: An Expressive, Efficient Attention Architecture</a></li>
<li><a href="https://arxiv.org/abs/2603.15031">[2603.15031] Attention Residuals</a></li>

</ul>
</details>

**标签**: `#AI`, `#open-source`, `#large language model`, `#coding benchmark`, `#Kimi K3`

---

<a id="item-10"></a>
## [中芯国际试运行首台国产 DUV 光刻机](https://t.me/zaihuapd/42800) ⭐️ 8.0/10

中芯国际正在试运行中国首台由上海初创公司宇量昇研发的先进深紫外（DUV）光刻机，用于 28 纳米芯片生产，并试图通过多重图形化工艺实现 7 纳米甚至 5 纳米制程。 这是中国迈向半导体自主可控的重要一步，有助于减少对荷兰 ASML 的依赖并绕开美国出口限制。如果成功，可能重塑全球芯片供应链，加剧地缘政治竞争。 该设备大部分零部件已国产化，但仍有部分依赖进口。业内人士称量产并达到稳定良率需 1 至 2 年，最快或于 2027 年进入量产。

telegram · zaihuapd · 7月27日 14:10

**背景**: 深紫外（DUV）光刻机使用 193 纳米波长的光源，而极紫外（EUV）光刻机使用 13.5 纳米波长，可制造更精细的电路。为了在 DUV 光刻机上实现 7 纳米及更先进制程，芯片制造商采用多重图形化工艺（如自对准双重图形化）。目前中国先进芯片生产仍依赖荷兰 ASML 的 DUV 光刻机，而 EUV 光刻机因美国出口管制被禁止对华销售。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ime.cas.cn/icac/learning/learning_2/202112/t20211221_6324996.html">DUV 和 EUV 光 刻 机 的 区 别 在哪？- -科普知识</a></li>
<li><a href="https://www.elecfans.com/article/89/2023/202310302282517.html">什么是 EUV 光 刻 ？ EUV 与 DUV 光 刻 的 区 别 - 制造/封装 - 电子发烧友网</a></li>
<li><a href="https://www.researching.cn/ArticlePdf/m00002/2022/59/9/0922027.pdf">亚十纳米导向自组装与深紫外混合光刻技术</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#lithography`, `#SMIC`, `#DUV`, `#China technology`

---