---
layout: default
title: "Horizon Summary: 2026-07-27 (EN)"
date: 2026-07-27
lang: en
---

> From 30 items, 10 important content pieces were selected

---

1. [Critical RCE in Fastjson 1.x without Gadget or autoType](#item-1) ⭐️ 10.0/10
2. [vLLM v0.26.0 Adds Inkling Models and Performance Boosts](#item-2) ⭐️ 9.0/10
3. [Judge Rejects Google's DMCA Scraping Defense](#item-3) ⭐️ 8.0/10
4. [Forum Software Migrates from React to HTMX](#item-4) ⭐️ 8.0/10
5. [Paged Out #9: Deeply Technical Hacker Magazine Released](#item-5) ⭐️ 8.0/10
6. [Bun Rust Rewrite Shipped in Claude Code, v1.4 Delayed](#item-6) ⭐️ 8.0/10
7. [Modern Email Reimagined with HTTP and JSON](#item-7) ⭐️ 8.0/10
8. [Solo Study Finds All 6 Frontier LLMs Lean Left in Behavior](#item-8) ⭐️ 8.0/10
9. [Kimi K3: Open-Source 2.8T Model Tops Frontend Code Arena](#item-9) ⭐️ 8.0/10
10. [SMIC Tests China's First Domestic DUV Lithography Machine](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Critical RCE in Fastjson 1.x without Gadget or autoType](https://t.me/zaihuapd/42797) ⭐️ 10.0/10

Security researcher Kirill Firsov disclosed a high-severity remote code execution vulnerability in Fastjson 1.x versions 1.2.68 to 1.2.83. The exploit does not require enabling autoType or any classpath gadget chains. This is critical because Fastjson 1.x is widely used in Java applications and is no longer maintained, meaning no official patch will be released. The vulnerability affects multiple JDK versions, including 8, 17, and 21. The vulnerability is exploitable without needing any gadget chains or enabling autoTypeSupport. The only recommended mitigation is upgrading to Fastjson2.

telegram · zaihuapd · Jul 27, 10:31

**Background**: Fastjson is a popular Java library for JSON serialization and deserialization, which has had prior deserialization security issues. A gadget chain is a sequence of existing code fragments that can be chained together during deserialization to achieve code execution. autoType is a feature in Fastjson that enables automatic type resolution during deserialization, often required for exploitation of such vulnerabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@dub-flow/deserialization-what-the-heck-actually-is-a-gadget-chain-1ea35e32df69">Deserialization: What the Heck *Actually* Is a Gadget Chain? | by Florian Walter | Medium</a></li>
<li><a href="https://pentesterlab.com/glossary/gadget-chain">Gadget Chain: Definition & Security Context | PentesterLab Glossary</a></li>

</ul>
</details>

**Tags**: `#Fastjson`, `#RCE`, `#Java`, `#security`, `#vulnerability`

---

<a id="item-2"></a>
## [vLLM v0.26.0 Adds Inkling Models and Performance Boosts](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 9.0/10

vLLM v0.26.0 introduces support for the new Inkling model family, optimizations for DeepSeek-V4, fp32 lm_head, and flexible attention backends. The release features 411 commits from 212 contributors. This release enhances vLLM as a leading LLM inference engine, enabling efficient deployment of large models like Inkling (975B parameters) and improving performance on DeepSeek-V4. The flexible attention backend and new model support expand vLLM's applicability across diverse hardware and architectures. The Inkling model is a 975B-parameter Mixture-of-Experts transformer with up to 1M context tokens, supported by piecewise CUDA graphs and Hopper FA4 relative attention. DeepSeek-V4 performance gains include a specialized routing kernel with 2.94% end-to-end TPOT improvement and fused_topk_bias kernel speedups of 1.5-2x.

github · khluu · Jul 27, 01:06

**Background**: vLLM is an open-source high-throughput LLM inference engine widely used for serving large language models. It supports various model architectures and optimizations like PagedAttention and continuous batching. The release of v0.26.0 comes with the introduction of the Inkling model family from Thinking Machines Lab, which is a large MoE model trained from scratch in under nine months. The version also includes optimizations for DeepSeek-V4 and new features like fp32 lm_head for better accuracy.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://www.technology.org/2026/07/16/thinking-machines-inkling-open-weights-model/">Thinking Machines Releases Inkling, Its First Open-Weights Model, Trained From Scratch</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#performance optimization`, `#open-source`, `#AI/ML`

---

<a id="item-3"></a>
## [Judge Rejects Google's DMCA Scraping Defense](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

A federal judge has ruled that Google cannot use the Digital Millennium Copyright Act (DMCA) to prevent third parties from scraping its search engine results pages (SERPs). The decision rejects Google's legal theory that scraping constitutes circumvention of a technological protection measure. This ruling clarifies that DMCA anti-circumvention provisions do not apply to mere scraping of publicly available web data, which could have significant implications for data access, competition, and the use of web data for AI training. It also highlights the growing tension between copyright law and data scraping. The case involved Google suing SerpAPI, a service that scrapes Google search results to provide custom APIs. The judge found that Google's technical measures (such as CAPTCHAs and IP rate limits) were not primarily for copyright protection, which is required for DMCA claims.

hackernews · cdrnsf · Jul 27, 18:15 · [Discussion](https://news.ycombinator.com/item?id=49073513)

**Background**: The Digital Millennium Copyright Act (DMCA) includes provisions that prohibit circumvention of technological measures that control access to copyrighted works. In the context of web scraping, some companies have argued that the mere act of scraping a website circumvents these protections. However, courts have generally been cautious about extending DMCA protections to measures that are not primarily designed to protect copyright.

<details><summary>References</summary>
<ul>
<li><a href="https://www.quinnemanuel.com/the-firm/publications/the-legal-landscape-of-web-scraping/">The Legal Landscape of Web Scraping</a></li>
<li><a href="https://nortonlaw.com/2026/05/14/dmca-section-1201-claims-the-new-battleground-for-ai-and-data-scraping-litigation/">DMCA Section 1201 Claims: The New Battleground for AI and Data Scraping Litigation - the NORTON law firm</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed reactions: some criticized Google's legal strategy as typical of large companies (SoftTalker), while others noted the lack of a good API for search results (binarymax). There was also discussion about EU database rights versus US copyright law (akrymski), and the importance of being able to scrape search results to expose advertising scams (jonatron).

**Tags**: `#legal`, `#web scraping`, `#DMCA`, `#Google`, `#search engines`

---

<a id="item-4"></a>
## [Forum Software Migrates from React to HTMX](https://misago-project.org/t/removing-reactjs-from-the-codebase-and-adapting-htmx-for-ui-interactivity/1267/) ⭐️ 8.0/10

The author describes removing React.js from their forum software and adopting HTMX for server-driven UI interactivity, citing better performance and a simpler frontend architecture. This migration represents a broader industry trend of replacing complex client-side frameworks with server-driven approaches for certain types of web applications, potentially influencing developers to reevaluate their frontend architecture. HTMX enables dynamic web interactions through HTML attributes and server-sent events, eliminating the virtual DOM and reducing JavaScript complexity.

hackernews · Ralfp · Jul 27, 09:58 · [Discussion](https://news.ycombinator.com/item?id=49067301)

**Background**: HTMX is a JavaScript library that allows developers to build dynamic web interfaces using HTML attributes instead of writing custom JavaScript. It enables server-driven interactivity by sending AJAX requests and updating parts of the page with HTML fragments, contrasting with client-side frameworks like React that manage state and DOM updates on the browser.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Htmx">Htmx</a></li>
<li><a href="https://htmx.org/">htmx - high power tools for html</a></li>

</ul>
</details>

**Discussion**: The community largely welcomes the move to HTMX, with many noting its suitability for content-heavy sites like forums. Some users report performance issues with large HTML payloads, while others suggest alternative server-driven approaches like Phoenix LiveView.

**Tags**: `#HTMX`, `#React.js`, `#web development`, `#server-side rendering`, `#frontend architecture`

---

<a id="item-5"></a>
## [Paged Out #9: Deeply Technical Hacker Magazine Released](https://pagedout.institute/download/PagedOut_009.pdf) ⭐️ 8.0/10

Paged Out #9, a free experimental technical magazine featuring one-page articles on topics from C programming to subpixel rendering and computable tilings, has been released as a PDF. The magazine has been highly praised on Hacker News for its deep technical content and resemblance to classic hacker publications like 2600 and Phrack, indicating strong community engagement and a revival of hacker-curious spirit. Paged Out #9 includes articles such as 'Baby Steps in C', 'The Subpixel Zoo', and a piece on computable tilings, which is an uncredited rediscovery of Hao Wang's 1960s work linking tilings to the halting problem.

hackernews · laurensr · Jul 27, 14:22 · [Discussion](https://news.ycombinator.com/item?id=49070138)

**Background**: Paged Out is a free experimental technical magazine that publishes one article per page, covering programming, security, retro computing, and more. Subpixel rendering is a technique that uses individual red, green, and blue subpixels to increase the apparent resolution of text and graphics on displays. Computable tilings, as explored by Hao Wang and others, connect tilings of the plane to computability theory, showing that the domino problem is equivalent to the halting problem.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Subpixel_rendering">Subpixel rendering</a></li>
<li><a href="https://link.springer.com/chapter/10.1007/978-0-387-09680-3_13">Computability of Tilings | Springer Nature Link</a></li>
<li><a href="https://pagedout.institute/?page=about.php">About ⁂ Paged Out !</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News expressed strong positive sentiment, comparing Paged Out #9 to classic zines 2600 and Phrack. They highlighted specific articles like 'Baby Steps in C' and 'The Subpixel Zoo', and provided context on the computable tilings piece, noting it is an uncredited rediscovery of Wang's work.

**Tags**: `#technical magazine`, `#programming`, `#computer science`, `#graphics`, `#tilings`

---

<a id="item-6"></a>
## [Bun Rust Rewrite Shipped in Claude Code, v1.4 Delayed](https://lockwood.dev/ai/2026/07/27/how-is-the-bun-rewrite-in-rust-going.html) ⭐️ 8.0/10

Bun's Rust rewrite has been shipped in Claude Code, with the v1.4 release postponed until a specific number of Node.js compatibility tests pass. The rewrite in Rust could significantly improve Bun's performance and safety, while the delay in v1.4 demonstrates a focus on Node.js compatibility, which is crucial for adoption. The entire rewrite of 1 million lines from Zig to Rust was accomplished in 11 days using large language models, and the v1.4 release is held back pending the passing of a target number of Node.js compatibility tests.

hackernews · tomlockwood · Jul 27, 11:12 · [Discussion](https://news.ycombinator.com/item?id=49067854)

**Background**: Bun is a JavaScript runtime created as a faster alternative to Node.js. It was originally written in Zig, but the team decided to rewrite it in Rust due to Rust's stronger ecosystem and safety guarantees. The massive rewrite was completed in a remarkably short time using AI-powered code translation.

<details><summary>References</summary>
<ul>
<li><a href="https://bunjs.run/bun-zig-to-rust-rewrite">How Bun Rewrote 1 Million Lines from Zig to Rust in 11 Days Using AI</a></li>
<li><a href="https://www.cosmicjs.com/changelog/bun-rust-rewrite-javascript-runtime">Why Bun is Rewriting in Rust (And What It Means for JavaScript ...)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>

</ul>
</details>

**Discussion**: The community discussion includes Jarred's update on the rewrite's deployment and delay; SquareWheel cautions about predicting development speed from commit metrics; benjiro29 criticizes over-reliance on LLMs for serious development; bendmorris notes a competing approach that fixed the original Zig codebase, achieving sub-second builds.

**Tags**: `#Bun`, `#Rust`, `#JavaScript`, `#Runtime`, `#Node.js`

---

<a id="item-7"></a>
## [Modern Email Reimagined with HTTP and JSON](https://en.andros.dev/blog/d7ed8b07/modern-email-can-be-built-from-borrowed-parts/) ⭐️ 8.0/10

An article proposes that modern email can be rebuilt by borrowing components from HTTP and other protocols, reducing reliance on legacy SMTP infrastructure. It highlights JMAP as an example of a protocol that replaces IMAP with standard HTTP and JSON. If adopted, this approach could simplify email infrastructure, improve security and interoperability, and reduce development costs. It matters for email client developers, server administrators, and the broader communication ecosystem. The article suggests leveraging existing web standards, but notes that network effects and backward compatibility with SMTP pose adoption challenges. JMAP already demonstrates the feasibility of using HTTP+JSON for email access.

hackernews · andros · Jul 27, 08:27 · [Discussion](https://news.ycombinator.com/item?id=49066639)

**Background**: Traditional email relies on SMTP for transfer and IMAP or POP3 for access, protocols that are decades old. JMAP (JSON Meta Application Protocol) is a modern open standard that replaces IMAP and SMTP submission with HTTP and JSON, making email systems easier to develop and secure. MTA-STS (MTA Strict Transport Security) is another extension that uses HTTPS/TLS to enforce encrypted email delivery.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/JSON_Meta_Application_Protocol">JSON Meta Application Protocol - Wikipedia</a></li>
<li><a href="https://jmap.io/">JSON Meta Application Protocol Specification ( JMAP )</a></li>
<li><a href="https://datatracker.ietf.org/doc/html/rfc8461">RFC 8461 - SMTP MTA Strict Transport Security ( MTA - STS )</a></li>

</ul>
</details>

**Discussion**: Commenters discussed historical proposals to fix spam, with one user pointing to a list of unworkable solutions from the 1990s. Others argued for fundamental changes like charging for emails and requiring recipient approval, while some noted that network effects make email replacement difficult. A few defended the current stack, suggesting it is not as broken as claimed.

**Tags**: `#email`, `#SMTP`, `#protocols`, `#web`, `#communication`

---

<a id="item-8"></a>
## [Solo Study Finds All 6 Frontier LLMs Lean Left in Behavior](https://www.reddit.com/r/MachineLearning/comments/1v8fnzw/evaluated_6_frontier_llms_gpt54_claude_sonnet_46/) ⭐️ 8.0/10

A solo evaluation of six frontier LLMs (GPT-5.4, Claude Sonnet 4.6, Claude Opus 4.7, Gemini Pro, Gemini Flash, and Grok 4.3) across eight bias benchmarks found all models exhibit left-leaning behavior, with Grok showing a discrepancy between its self-reported right-leaning stance and left-leaning behavior. This study underscores persistent political and racial biases in state-of-the-art AI systems, raising concerns about fairness and neutrality in LLM deployment. It highlights the need for more balanced training data and evaluation methods to mitigate unintended bias. Notable refusal rates on race-based questions from the BBQ dataset: GPT-5.4 refused 20.3%, Claude Opus 4.7 13.8%, Grok 9.5%, Claude Sonnet 4.6 and Gemini Pro about 5%. Limitations include single prompt templates and no multi-run averaging, and the evaluation was conducted by a single non-affiliated researcher.

reddit · r/MachineLearning · /u/marggggggggg · Jul 27, 22:37

**Background**: Bias benchmarks like WinoBias, BBQ, SeeGULL, and OpinionsQA evaluate models for demographic stereotypes and political leanings. SeeGULL is a large-scale stereotype dataset covering 178 countries and 23 languages. The cajcodes political bias dataset contains 658 synthetic statements annotated on a conservative-liberal spectrum. OpinionsQA tests alignment with US demographic groups on topics like abortion and immigration.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/google-research-datasets/seegull">GitHub - google-research-datasets/seegull: SeeGULL is a broad-coverage stereotype dataset in English containing stereotypes about identity groups spanning 178 countries across 8 different geo-political regions across 6 continents, as well as state-level identities within the US and India. · GitHub</a></li>
<li><a href="https://huggingface.co/datasets/cajcodes/political-bias">cajcodes/political-bias · Datasets at Hugging Face</a></li>
<li><a href="https://arxiv.org/abs/2303.17548">[2303.17548] Whose Opinions Do Language Models Reflect?</a></li>

</ul>
</details>

**Tags**: `#LLM bias`, `#fairness evaluation`, `#political bias`, `#racial bias`, `#frontier models`

---

<a id="item-9"></a>
## [Kimi K3: Open-Source 2.8T Model Tops Frontend Code Arena](https://t.me/zaihuapd/42793) ⭐️ 8.0/10

Moonshot AI released Kimi K3, an open-source 2.8 trillion parameter model that achieved first place in Frontend Code Arena with 1679 points, surpassing Claude Fable 5. It utilizes Kimi Delta Attention and Attention Residuals architectures and features native vision support and a 1 million token context window. Kimi K3 demonstrates that open-source models can compete with and surpass proprietary frontier models in specialized coding benchmarks, potentially lowering barriers for developers and startups. Its 2.8 trillion parameters make it one of the largest open-source models ever released, signaling a new scale in open-weight AI. Kimi K3 jumped from 18th place (Kimi k2.6) to 1st in the Frontend Code Arena, ranking first in 6 out of 7 domains, only behind in Gaming. The model weights are scheduled to be released by July 27, 2025.

telegram · zaihuapd · Jul 27, 06:27

**Background**: Kimi Delta Attention is a linear attention mechanism designed for efficient long-context processing, extending Gated DeltaNet with finer-grained gating. Attention Residuals replace standard residual connections in transformers, allowing layers to selectively aggregate previous outputs via learned attention. Frontend Code Arena evaluates models on agentic frontend coding tasks from real users building apps and websites in HTML and React.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/arena/status/2077824029126504525">Arena.ai on X: "Big news: Kimi-K3 by @Kimi_Moonshot is now #1 in the Frontend Code Arena with 1679 pts, surpassing Claude Fable 5. This is a 17-place jump from Kimi-k2.6 (#18 -> #1). In Frontend, Kimi-K3 ranked #1 in 6 of 7 domains: Brand & Marketing, Reference-Based Design, Data & Analytics, Consumer Product, Simulations, and Content Creation Tools, landing #2 only in Gaming behind Fable 5. The full model weights will be released by July 27. Congrats to the @Kimi_Moonshot team on this major milestone!" / X</a></li>
<li><a href="https://arxiv.org/abs/2510.26692">[2510.26692] Kimi Linear: An Expressive, Efficient Attention Architecture</a></li>
<li><a href="https://arxiv.org/abs/2603.15031">[2603.15031] Attention Residuals</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-source`, `#large language model`, `#coding benchmark`, `#Kimi K3`

---

<a id="item-10"></a>
## [SMIC Tests China's First Domestic DUV Lithography Machine](https://t.me/zaihuapd/42800) ⭐️ 8.0/10

SMIC is testing China's first domestically developed DUV lithography machine, built by Shanghai startup Yuliangsheng, for 28nm chip production and aims to achieve 7nm and 5nm nodes using multi-patterning techniques. This marks a significant step toward China's semiconductor self-sufficiency, reducing dependence on ASML and circumventing US export restrictions. Success could reshape global chip supply chains and intensify geopolitical competition. Most components of the machine are domestically sourced, but some remain imported. Industry insiders estimate mass production with stable yield will take one to two years, with commercial production possibly by 2027.

telegram · zaihuapd · Jul 27, 14:10

**Background**: DUV lithography uses 193nm wavelength light, while EUV uses 13.5nm for finer features. To achieve sub-7nm nodes, multi-patterning techniques like self-aligned double patterning are used with DUV. China currently relies on ASML's DUV machines for advanced chips, as EUV exports are banned due to US export controls.

<details><summary>References</summary>
<ul>
<li><a href="https://ime.cas.cn/icac/learning/learning_2/202112/t20211221_6324996.html">DUV 和 EUV 光 刻 机 的 区 别 在哪？- -科普知识</a></li>
<li><a href="https://www.elecfans.com/article/89/2023/202310302282517.html">什么是 EUV 光 刻 ？ EUV 与 DUV 光 刻 的 区 别 - 制造/封装 - 电子发烧友网</a></li>
<li><a href="https://www.researching.cn/ArticlePdf/m00002/2022/59/9/0922027.pdf">亚十纳米导向自组装与深紫外混合光刻技术</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#lithography`, `#SMIC`, `#DUV`, `#China technology`

---