---
layout: default
title: "Horizon Summary: 2026-07-09 (EN)"
date: 2026-07-09
lang: en
---

> From 40 items, 12 important content pieces were selected

---

1. [OpenAI Releases GPT-5.6 Family: Luna, Terra, Sol](#item-1) ⭐️ 10.0/10
2. [EU Parliament greenlights Chat Control 1.0](#item-2) ⭐️ 9.0/10
3. [Postgres rewritten in Rust passes all regression tests](#item-3) ⭐️ 9.0/10
4. [Bun Rewritten from Zig to Rust Using AI Agents](#item-4) ⭐️ 9.0/10
5. [TypeScript 7.0 Released: Go Rewrite Delivers Up to 12x Speed Boost](#item-5) ⭐️ 9.0/10
6. [Tencent Launches Hy3 Language Model, Rivaling DeepSeek V4 Flash](#item-6) ⭐️ 8.0/10
7. [Meta Releases Muse Spark 1.1 Agentic AI Model](#item-7) ⭐️ 8.0/10
8. [Meta Superintelligence Update: RL Startup, Massive Compute](#item-8) ⭐️ 8.0/10
9. [IMGNet: Face verification using sign patterns, not cosine similarity](#item-9) ⭐️ 8.0/10
10. [Ant LingBot Open Sources LingBot-Video, First MoE Embodied Video Model](#item-10) ⭐️ 8.0/10
11. [DJI EV50 Flies Over Everest at 8,861 Meters](#item-11) ⭐️ 8.0/10
12. [National Supercomputing Internet Core Node Launches in Zhengzhou](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI Releases GPT-5.6 Family: Luna, Terra, Sol](https://simonwillison.net/2026/Jul/9/gpt-5-6/#atom-everything) ⭐️ 10.0/10

OpenAI has launched the GPT-5.6 model family, consisting of three sizes—Luna, Terra, and Sol—with a million-token context window and enhanced agentic capabilities, outperforming Claude Fable 5 on the Agents' Last Exam benchmark. This release marks a significant leap in AI agent performance and cost efficiency, potentially shifting the competitive landscape for large language models, as smaller models in the family offer frontier-level capabilities at a fraction of the cost. The models feature a 128,000 maximum output tokens, new API capabilities like programmatic tool calling and multi-agent support, and prompt cache breakpoints. However, OpenAI also critiqued the SWE-Bench Pro benchmark, where GPT-5.6 lagged behind Claude Fable 5.

rss · Simon Willison · Jul 9, 19:46

**Background**: GPT-5.6 is OpenAI's latest flagship model following the GPT-5 series. It introduces reasoning tokens that allow models to 'think' step-by-step, improving performance on complex tasks. The million-token context window enables processing of very long documents. Agentic benchmarks like Agents' Last Exam evaluate models on long-horizon, real-world tasks with verifiable outcomes.

<details><summary>References</summary>
<ul>
<li><a href="https://agents-last-exam.org/">Agents' Last Exam</a></li>
<li><a href="https://developers.openai.com/api/docs/guides/reasoning">Reasoning models | OpenAI API</a></li>

</ul>
</details>

**Discussion**: The community noted the developer guide's tips on intent understanding, and celebrated GPT-5.6 Sol setting a new SOTA on ARC-AGI-3. There was discussion comparing Claude Code and codex, and some skepticism about OpenAI's benchmark selections. One commenter humorously observed the rivalry between OpenAI and Anthropic.

**Tags**: `#GPT-5.6`, `#OpenAI`, `#AI models`, `#reasoning`, `#agents`

---

<a id="item-2"></a>
## [EU Parliament greenlights Chat Control 1.0](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 9.0/10

The European Parliament has approved the extension of mass scanning of private messages (Chat Control 1.0) until 2028, despite a majority of MEPs voting against it, due to a procedural rule requiring an absolute majority to reject the measure. This decision allows US tech companies to scan private messages without a warrant, undermining encryption and privacy. It sets a concerning precedent for digital surveillance in the EU, affecting millions of users. The measure required an absolute majority of 361 votes to reject; only 314 voted against, with 276 in favor and 113 absent. The scanning applies to platforms like Instagram, Discord, Skype, and Gmail, but does not affect public social media posts or cloud storage files already scannable.

hackernews · rapnie · Jul 9, 11:03 · [Discussion](https://news.ycombinator.com/item?id=48843923)

**Background**: Chat Control is an EU regulation proposed in 2022 aimed at preventing child sexual abuse online by mandating digital platforms to scan private communications. Critics argue it violates fundamental rights to privacy and end-to-end encryption. The first iteration (Chat Control 1.0) was temporary and expired in March 2026, but has now been revived until 2028.

<details><summary>References</summary>
<ul>
<li><a href="https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/">EU Parliament greenlights Chat Control 1.0 – Breyer: "Our children lose out"</a></li>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control_1.0">Chat Control 1.0</a></li>

</ul>
</details>

**Discussion**: Commenters expressed outrage at the procedural manipulation, noting that the vote was held on the last day before summer break with many MEPs absent. They criticized the use of an absolute majority requirement to pass an unpopular law, and warned of the erosion of democracy and legitimacy of the EU.

**Tags**: `#privacy`, `#EU law`, `#surveillance`, `#encryption`, `#technology policy`

---

<a id="item-3"></a>
## [Postgres rewritten in Rust passes all regression tests](https://github.com/malisper/pgrust) ⭐️ 9.0/10

A Rust rewrite of PostgreSQL named pgrust has passed 100% of PostgreSQL's standard regression test suite. The project was developed using LLM-assisted code generation and aims to modernize the legacy database. This demonstrates the potential of modernizing legacy codebases using Rust and LLMs, which could improve safety and performance. The project also sparks discussion about open-source licensing and the feasibility of AI-generated code for critical infrastructure. The project passes the full PostgreSQL regression test suite, indicating high compatibility. However, it changes the license from the PostgreSQL license to AGPL, which may raise compatibility concerns.

hackernews · SweetSoftPillow · Jul 9, 06:18 · [Discussion](https://news.ycombinator.com/item?id=48841676)

**Background**: PostgreSQL is a venerable open-source relational database with a 30-year history. Rust is a systems programming language known for memory safety and concurrency without garbage collection. Recent advances in large language models (LLMs) have enabled automated code generation and translation, which the pgrust project leverages to rewrite C code into Rust.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/malisper/pgrust">GitHub - malisper/pgrust: Postgres rewritten in Rust, now passing 100% of the Postgres regression tests · GitHub</a></li>
<li><a href="https://pgrust.com/">pgrust — postgres, rewritten in rust</a></li>
<li><a href="https://news.ycombinator.com/item?id=48841676">Postgres rewritten in Rust, now passing 100% of the Postgres regression tests | Hacker News</a></li>

</ul>
</details>

**Discussion**: The community reaction is mixed: some are impressed by the technical achievement, while others express concerns about the feasibility of reviewing LLM-generated code, the license change from PostgreSQL to AGPL, and the general reliability of AI-rewritten system software.

**Tags**: `#Rust`, `#PostgreSQL`, `#database`, `#LLM`, `#rewrite`

---

<a id="item-4"></a>
## [Bun Rewritten from Zig to Rust Using AI Agents](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust/#atom-everything) ⭐️ 9.0/10

Jarred Sumner announced that Bun, the JavaScript runtime, has been rewritten from Zig to Rust using AI coding agents, with the new version already deployed in Claude Code since June 17, 2026. This demonstrates that AI coding agents can successfully rewrite large-scale software projects, challenging the long-held belief that rewriting from scratch is too risky. It also showcases how safe Rust's memory management can eliminate entire classes of bugs that plagued the Zig version. The rewrite took 11 days of intensive work and cost an estimated $165,000 in API tokens. The test suite, written in TypeScript, served as a conformance suite to guide the agents, and the new Bun is now powering Claude Code.

rss · Simon Willison · Jul 8, 23:57

**Background**: Bun is a JavaScript runtime known for its performance. Originally written in Zig, it faced memory management issues like use-after-free bugs. Agentic engineering involves using AI coding agents to autonomously perform complex software tasks, while dynamic workflows allow agents to adjust their process in real time based on feedback.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/guides/agentic-engineering-patterns/what-is-agentic-engineering/">What is agentic engineering? - Agentic Engineering Patterns - Simon Willison's Weblog</a></li>
<li><a href="https://claudefa.st/blog/guide/development/dynamic-workflows">Dynamic Workflows in Claude Code: How They Work</a></li>

</ul>
</details>

**Tags**: `#Bun`, `#Rust`, `#Zig`, `#Runtime`, `#Software Engineering`

---

<a id="item-5"></a>
## [TypeScript 7.0 Released: Go Rewrite Delivers Up to 12x Speed Boost](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

Microsoft has officially released TypeScript 7.0, a major version that rewrites the compiler in Go, resulting in build speeds up to 8–12 times faster than the previous JavaScript-based implementation. The new version is available via npm and supports shared-memory multithreading. This performance improvement significantly reduces compile times for large TypeScript codebases, enhancing developer productivity. It also marks a notable shift in the TypeScript ecosystem, as the compiler now leverages Go's concurrency features. TypeScript 7.0 introduces --checkers and --builders flags for customizing parallelism, and provides a compatibility package to coexist with TypeScript 6. However, embedded language tools like Vue and Svelte are not yet supported due to incomplete API.

telegram · zaihuapd · Jul 9, 04:01

**Background**: TypeScript is a typed superset of JavaScript that compiles to plain JavaScript. Its compiler was originally written in TypeScript/JavaScript, which could be slow on large codebases. The decision to rewrite the compiler in Go was made to leverage Go's performance and native multithreading, resulting in dramatic speed improvements. TypeScript 7.0 is the first stable release of this Go-based compiler.

<details><summary>References</summary>
<ul>
<li><a href="https://betterstack.com/community/guides/scaling-nodejs/typescript-7-go-rewrite/">TypeScript 7.0: New Features and the Go-Powered Compiler Rewrite | Better Stack Community</a></li>
<li><a href="https://developers.slashdot.org/story/26/07/05/2335217/go-based-typescript-70-finally-reaches-release-candidate-stage">Go-based TypeScript 7.0 Finally Reaches Release Candidate Stage - Slashdot</a></li>

</ul>
</details>

**Tags**: `#TypeScript`, `#Go`, `#性能`, `#发布`

---

<a id="item-6"></a>
## [Tencent Launches Hy3 Language Model, Rivaling DeepSeek V4 Flash](https://hy.tencent.com/research/hy3) ⭐️ 8.0/10

Tencent has announced Hy3, a new language model that is being offered for free on OpenRouter until July 21. The model is comparable to DeepSeek V4 Flash and has sparked community discussion about its performance and pricing. Hy3 challenges the dominance of models like DeepSeek by offering competitive performance at a smaller model size. Its availability via OpenRouter and potential for local deployment make it an attractive option for developers and researchers. Hy3 is slightly larger than DeepSeek V4 Flash but reportedly matches or exceeds DeepSeek V4 Pro on some benchmarks. The effective input price on OpenRouter is now the same as DeepSeek-hosted Flash V4, and the model can run on systems with around 96GB of RAM.

hackernews · andai · Jul 9, 15:27 · [Discussion](https://news.ycombinator.com/item?id=48847552)

**Background**: Large language models are AI systems trained on vast amounts of text to generate human-like responses. Companies like Tencent and DeepSeek compete to produce capable models that can be accessed via APIs or run locally. OpenRouter is a platform that provides unified access to multiple AI models, including Hy3.

**Discussion**: The community is excited about Hy3's small size and high capability, with some noting it could become a popular local model. There is confusion over pricing, as the effective cost is now similar to DeepSeek Flash V4, and questions about how it handles heavy quantization compared to DeepSeek V4 Flash.

**Tags**: `#machine learning`, `#language models`, `#Tencent`, `#Hy3`, `#AI`

---

<a id="item-7"></a>
## [Meta Releases Muse Spark 1.1 Agentic AI Model](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 8.0/10

Meta has released Muse Spark 1.1, a new agentic AI model available via its API, with community members creating plugins and debating the validity of its benchmark results. This release demonstrates Meta's commitment to competing in the AI model space, potentially commoditizing coding models with aggressive pricing and open-weight availability, while the community critique underscores the need for rigorous evaluation standards. The model is priced at $1.25 per million input tokens and $4.5 per million output tokens, with a cached input rate of $0.15. A community member created a plugin for the LLM tool, allowing terminal usage, while another critique suggests benchmark results may be invalid due to resource cap violations.

hackernews · ot · Jul 9, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48846184)

**Background**: Muse Spark is Meta's series of agentic AI models designed to autonomously complete tasks such as coding and tool interaction. Meta has a history of releasing open-weight models like Llama, and this release includes both API access and open weights. The community discussion focuses on whether the reported benchmark scores are reliable given the testing methodology.

**Discussion**: Community reaction is mixed: some highlight the low pricing and practical integrations (e.g., Simon Willison's LLM plugin), while others question the validity of benchmark results due to potential methodology issues. A user suggests Meta's strategy could be to commoditize AI models, and another notes the surprising competitiveness of Meta and xAI against OpenAI and Anthropic.

**Tags**: `#AI`, `#Meta`, `#Machine Learning`, `#Open Source`, `#Hacker News Discussion`

---

<a id="item-8"></a>
## [Meta Superintelligence Update: RL Startup, Massive Compute](https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence) ⭐️ 8.0/10

Meta's 1-year progress update on superintelligence reveals the emergence of a top-tier RL environment startup, an unprecedented compute scaling plan, and strategic advice for Google DeepMind. This signals Meta's aggressive push toward superintelligence, highlighting the growing importance of reinforcement learning environments and massive compute infrastructure in AI research. The compute ramp is described as the most aggressive ever seen, with scale-across exceeding 2000km, suggesting a massive distributed system. The RL environment startup is considered top-tier yet emerged seemingly out of nowhere.

rss · Semianalysis · Jul 9, 19:16

**Background**: Meta has been investing heavily in AI superintelligence, focusing on large-scale reinforcement learning. RL environments like those used in game AI are crucial for training agents. The "2000km+ scale-across" likely refers to a geographically distributed compute cluster spanning thousands of kilometers.

**Tags**: `#Meta`, `#superintelligence`, `#reinforcement learning`, `#AI infrastructure`, `#compute scaling`

---

<a id="item-9"></a>
## [IMGNet: Face verification using sign patterns, not cosine similarity](https://www.reddit.com/r/MachineLearning/comments/1urxvxh/i_built_imgnet_a_face_verification_model_that/) ⭐️ 8.0/10

IMGNet is a face verification model that replaces cosine similarity with a sliding window sign pattern matching approach, achieving 96.27% on LFW with a compact 10.58 MB model. This introduces a novel metric for face verification that focuses on relational sign patterns rather than global angular similarity, potentially offering better generalization and robustness. The approach also achieves competitive results with a much smaller model, making it suitable for resource-constrained environments. The model uses an SW Block that computes pixel-wise differences to neighbors at prime window sizes, and an IMG Sign MSE Loss that operates purely on sign pattern agreement without amplitude dependency. When applied to ArcFace embeddings without retraining, the IMG Sign Score achieves 99.58% on LFW, only 0.24% below ArcFace+Cosine.

reddit · r/MachineLearning · /u/img-_- · Jul 9, 18:00

**Background**: Face verification is the task of determining whether two face images belong to the same person. Traditional approaches use deep learning to generate embedding vectors and compare them using cosine similarity, which measures the angle between vectors. LFW (Labeled Faces in the Wild) is a standard benchmark dataset for face verification.

**Tags**: `#face verification`, `#computer vision`, `#deep learning`, `#novel approach`, `#efficient model`

---

<a id="item-10"></a>
## [Ant LingBot Open Sources LingBot-Video, First MoE Embodied Video Model](https://www.qbitai.com/2026/07/446458.html) ⭐️ 8.0/10

Ant LingBot has open-sourced LingBot-Video, the first embodied video foundation model based on a Mixture-of-Experts architecture, with 30B total parameters and only 3B activated during inference. This release significantly improves inference efficiency for embodied video generation, achieving about 3x speedup over dense models of similar size, and it is the first open-source model of its kind, which can accelerate research in robotics and world models. The model uses a DiT+MoE design and was trained on a custom dataset of 70,000 hours of embodied data covering dexterous manipulation, robot locomotion, and first-person interaction. It also incorporates a multi-dimensional reinforcement learning reward system focusing on physical plausibility and task completion.

telegram · zaihuapd · Jul 9, 04:30

**Background**: Embodied AI focuses on agents that can perceive and interact with the physical world. Video generation models for embodied tasks must produce physically plausible and task-relevant sequences. MoE (Mixture-of-Experts) architectures allow models to have a large total capacity while only activating a subset of parameters per inference, balancing performance and efficiency.

**Tags**: `#MoE`, `#具身智能`, `#视频生成`, `#开源`, `#AI模型`

---

<a id="item-11"></a>
## [DJI EV50 Flies Over Everest at 8,861 Meters](https://www.163.com/dy/article/L1CUCV940514R9OJ.html) ⭐️ 8.0/10

DJI's unreleased EV50 vertical takeoff and landing cargo drone flew over Mount Everest at 8,861 meters, setting a new altitude record for publicly tested drones of its kind. This achievement demonstrates the EV50's high-altitude performance, which could have significant implications for aerial logistics and scientific research in extreme environments. The EV50 is a composite-wing drone that can vertically take off and land, then switch to fixed-wing flight. During the 12-day mission, it completed 32 sorties, climbed 3,730 meters continuously, and still had 30% battery on return.

telegram · zaihuapd · Jul 9, 06:00

**Background**: Drones typically struggle at high altitudes due to thin air, so achieving flight at over 8,800 meters is a significant engineering challenge. The EV50 is designed for cargo delivery and low-altitude logistics, and this test proves its capabilities in extreme conditions.

**Tags**: `#无人机`, `#珠峰`, `#垂直起降`, `#物流`, `#测试`

---

<a id="item-12"></a>
## [National Supercomputing Internet Core Node Launches in Zhengzhou](https://36kr.com/newsflashes/3887797387344387) ⭐️ 8.0/10

On July 9, 2026, the core node of the National Supercomputing Internet went online in Zhengzhou, providing over 100,000 domestic AI computing cards. This milestone strengthens China's domestic computing infrastructure, reducing dependence on foreign chips and supporting AI and supercomputing advancements. The node serves as the operations and resource scheduling hub for the nationwide computing resource coordination system, also integrating supply-demand matching and industry incubation services.

telegram · zaihuapd · Jul 9, 07:00

**Background**: The National Supercomputing Internet is a project to connect supercomputing centers across China for resource sharing. The core node in Zhengzhou is a key part of this network, and domestic AI computing power uses locally manufactured chips to enhance self-sufficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://dchub.cloud/facility/5667059">国家超算互联网核心节点— , Data Center - DC Hub</a></li>

</ul>
</details>

**Tags**: `#超算互联网`, `#国产算力`, `#人工智能`, `#国家基础设施`

---