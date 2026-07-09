---
layout: default
title: "Horizon Summary: 2026-07-09 (ZH)"
date: 2026-07-09
lang: zh
---

> 从 40 条内容中筛选出 12 条重要资讯。

---

1. [OpenAI 发布 GPT-5.6 系列：Luna、Terra、Sol](#item-1) ⭐️ 10.0/10
2. [欧盟议会批准聊天控制 1.0](#item-2) ⭐️ 9.0/10
3. [用 Rust 重写的 PostgreSQL 通过全部回归测试](#item-3) ⭐️ 9.0/10
4. [Bun 运行时从 Zig 重写为 Rust，借助 AI 代理](#item-4) ⭐️ 9.0/10
5. [TypeScript 7.0 正式发布：Go 重写带来最高 12 倍速度提升](#item-5) ⭐️ 9.0/10
6. [腾讯发布 Hy3 语言模型，与 DeepSeek V4 Flash 竞争](#item-6) ⭐️ 8.0/10
7. [Meta 发布 Muse Spark 1.1 智能体 AI 模型](#item-7) ⭐️ 8.0/10
8. [Meta 超级智能更新：RL 初创公司与大规模算力](#item-8) ⭐️ 8.0/10
9. [IMGNet：使用符号模式而非余弦相似度的人脸验证模型](#item-9) ⭐️ 8.0/10
10. [蚂蚁灵波开源全球首个 MoE 具身视频基模 LingBot-Video](#item-10) ⭐️ 8.0/10
11. [大疆 EV50 飞越珠峰至 8861 米](#item-11) ⭐️ 8.0/10
12. [国家超算互联网核心节点在郑州上线](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 发布 GPT-5.6 系列：Luna、Terra、Sol](https://simonwillison.net/2026/Jul/9/gpt-5-6/#atom-everything) ⭐️ 10.0/10

OpenAI 发布了 GPT-5.6 模型系列，包括 Luna、Terra 和 Sol 三种尺寸，具有百万标记上下文窗口和增强的代理能力，在 Agent 最后考试基准测试中优于 Claude Fable 5。 此次发布标志着 AI 代理性能及成本效益的重大飞跃，可能改变大型语言模型的竞争格局，因为系列中的较小模型以极低的成本提供前沿能力。 这些模型具有 128,000 个最大输出标记、新的 API 功能（如程序化工具调用和多代理支持）以及提示缓存断点。不过，OpenAI 也批评了 SWE-Bench Pro 基准测试，在该测试中 GPT-5.6 落后于 Claude Fable 5。

rss · Simon Willison · 7月9日 19:46

**背景**: GPT-5.6 是 OpenAI 继 GPT-5 系列之后的最新旗舰模型。它引入了推理标记，使模型能够逐步“思考”，从而提高复杂任务的性能。百万标记上下文窗口允许处理非常长的文档。像 Agent 最后考试这样的代理基准测试评估模型在长期、现实世界任务中的表现，结果可验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://agents-last-exam.org/">Agents' Last Exam</a></li>
<li><a href="https://developers.openai.com/api/docs/guides/reasoning">Reasoning models | OpenAI API</a></li>

</ul>
</details>

**社区讨论**: 社区注意到开发者指南中关于意图理解的提示，并庆祝 GPT-5.6 Sol 在 ARC-AGI-3 上树立新的 SOTA。大家讨论了 Claude Code 和 codex 的比较，并对 OpenAI 的基准测试选择有些怀疑。一位评论者幽默地观察了 OpenAI 和 Anthropic 之间的竞争。

**标签**: `#GPT-5.6`, `#OpenAI`, `#AI models`, `#reasoning`, `#agents`

---

<a id="item-2"></a>
## [欧盟议会批准聊天控制 1.0](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 9.0/10

欧洲议会批准将私人消息大规模扫描（聊天控制 1.0）延长至 2028 年，尽管大多数议员投了反对票，但由于程序规则要求绝对多数才能否决该措施。 这一决定允许美国科技公司在没有授权的情况下扫描私人消息，破坏了加密和隐私。这为欧盟的数字监控树立了一个令人担忧的先例，影响数百万用户。 该措施需要绝对多数（361 票）才能否决；只有 314 票反对，276 票赞成，113 票缺席。扫描适用于 Instagram、Discord、Skype 和 Gmail 等平台，但不影响已经可扫描的公开社交媒体帖子或云存储文件。

hackernews · rapnie · 7月9日 11:03 · [社区讨论](https://news.ycombinator.com/item?id=48843923)

**背景**: 聊天控制是欧盟 2022 年提出的一项法规，旨在通过强制数字平台扫描私人通信来防止在线儿童性虐待。批评者认为它侵犯了隐私和端到端加密的基本权利。第一次迭代（聊天控制 1.0）是临时性的，于 2026 年 3 月到期，但现在已恢复至 2028 年。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/">EU Parliament greenlights Chat Control 1.0 – Breyer: "Our children lose out"</a></li>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control_1.0">Chat Control 1.0</a></li>

</ul>
</details>

**社区讨论**: 评论者对程序操纵表示愤怒，指出投票安排在暑假前的最后一天，许多议员缺席。他们批评使用绝对多数要求来通过一项不受欢迎的法律，并警告民主和欧盟合法性的侵蚀。

**标签**: `#privacy`, `#EU law`, `#surveillance`, `#encryption`, `#technology policy`

---

<a id="item-3"></a>
## [用 Rust 重写的 PostgreSQL 通过全部回归测试](https://github.com/malisper/pgrust) ⭐️ 9.0/10

名为 pgrust 的 Rust 重写版 PostgreSQL 已通过全部 PostgreSQL 标准回归测试。该项目采用 LLM 辅助代码生成，旨在实现传统数据库的现代化。 这展示了使用 Rust 和 LLM 实现遗留代码库现代化的潜力，有望提升安全性和性能。该项目还引发了关于开源许可证以及 AI 生成代码用于关键基础设施可行性的讨论。 该项目通过了完整的 PostgreSQL 回归测试套件，表明高度兼容。但许可证从 PostgreSQL 许可证改为 AGPL，可能引发兼容性问题。

hackernews · SweetSoftPillow · 7月9日 06:18 · [社区讨论](https://news.ycombinator.com/item?id=48841676)

**背景**: PostgreSQL 是一款历史悠久的开源关系型数据库，已有 30 年历史。Rust 是一种以内存安全著称的系统编程语言，无需垃圾回收即可实现并发。近期大语言模型（LLM）的进步实现了自动化代码生成与翻译，pgrust 项目正是利用这一点将 C 代码重写为 Rust。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/malisper/pgrust">GitHub - malisper/pgrust: Postgres rewritten in Rust, now passing 100% of the Postgres regression tests · GitHub</a></li>
<li><a href="https://pgrust.com/">pgrust — postgres, rewritten in rust</a></li>
<li><a href="https://news.ycombinator.com/item?id=48841676">Postgres rewritten in Rust, now passing 100% of the Postgres regression tests | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些人对此技术成就印象深刻，而另一些人对审查 LLM 生成代码的可行性、许可证从 PostgreSQL 改为 AGPL 以及 AI 重写系统软件的可靠性表示担忧。

**标签**: `#Rust`, `#PostgreSQL`, `#database`, `#LLM`, `#rewrite`

---

<a id="item-4"></a>
## [Bun 运行时从 Zig 重写为 Rust，借助 AI 代理](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust/#atom-everything) ⭐️ 9.0/10

Jarred Sumner 宣布，JavaScript 运行时 Bun 已借助 AI 编程代理从 Zig 重写为 Rust，新版本自 2026 年 6 月 17 日起已在 Claude Code 中部署。 这证明了 AI 编程代理能够成功重写大规模软件项目，挑战了长期以来认为从头重写风险过高的观念。它还展示了 Rust 的安全内存管理如何消除困扰 Zig 版本的整类错误。 重写工作历时 11 天，估算消耗了 16.5 万美元的 API 令牌费用。用 TypeScript 编写的测试套件作为一致性测试集指导代理，新的 Bun 现已用于驱动 Claude Code。

rss · Simon Willison · 7月8日 23:57

**背景**: Bun 是一个以性能著称的 JavaScript 运行时。最初用 Zig 编写，但面临释放后使用等内存管理问题。代理工程（agentic engineering）指利用 AI 编程代理自主执行复杂软件任务，而动态工作流（dynamic workflows）让代理能根据反馈实时调整流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/guides/agentic-engineering-patterns/what-is-agentic-engineering/">What is agentic engineering? - Agentic Engineering Patterns - Simon Willison's Weblog</a></li>
<li><a href="https://claudefa.st/blog/guide/development/dynamic-workflows">Dynamic Workflows in Claude Code: How They Work</a></li>

</ul>
</details>

**标签**: `#Bun`, `#Rust`, `#Zig`, `#Runtime`, `#Software Engineering`

---

<a id="item-5"></a>
## [TypeScript 7.0 正式发布：Go 重写带来最高 12 倍速度提升](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

微软正式发布了 TypeScript 7.0，该版本用 Go 语言重写了编译器，构建速度比旧版 JavaScript 实现快 8 到 12 倍。用户现可通过 npm 安装，并支持共享内存多线程。 这一性能提升显著缩短了大型 TypeScript 代码库的编译时间，提高了开发效率。同时标志着 TypeScript 生态的重大转变，编译器开始利用 Go 的并发特性。 TypeScript 7.0 引入了 --checkers 和 --builders 参数以自定义并行度，并提供了兼容包以便与 TypeScript 6 共存。但 Vue、Svelte 等嵌入式语言工具链因 API 尚未就绪，目前仍需使用旧版本。

telegram · zaihuapd · 7月9日 04:01

**背景**: TypeScript 是 JavaScript 的类型超集，可编译为普通 JavaScript。其编译器最初用 TypeScript/JavaScript 编写，在大型代码库上可能很慢。决定用 Go 重写编译器是为了利用 Go 的性能和原生多线程，从而带来显著的加速。TypeScript 7.0 是基于 Go 的编译器的首个稳定版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://betterstack.com/community/guides/scaling-nodejs/typescript-7-go-rewrite/">TypeScript 7.0: New Features and the Go-Powered Compiler Rewrite | Better Stack Community</a></li>
<li><a href="https://developers.slashdot.org/story/26/07/05/2335217/go-based-typescript-70-finally-reaches-release-candidate-stage">Go-based TypeScript 7.0 Finally Reaches Release Candidate Stage - Slashdot</a></li>

</ul>
</details>

**标签**: `#TypeScript`, `#Go`, `#性能`, `#发布`

---

<a id="item-6"></a>
## [腾讯发布 Hy3 语言模型，与 DeepSeek V4 Flash 竞争](https://hy.tencent.com/research/hy3) ⭐️ 8.0/10

腾讯发布了新的语言模型 Hy3，该模型在 OpenRouter 上免费提供至 7 月 21 日。该模型与 DeepSeek V4 Flash 相当，引发了社区对其性能和定价的讨论。 Hy3 通过以更小的模型尺寸提供有竞争力的性能，挑战了 DeepSeek 等模型的主导地位。它通过 OpenRouter 提供，并且具备本地部署的潜力，使其成为开发者和研究人员有吸引力的选择。 Hy3 比 DeepSeek V4 Flash 稍大，但据报道在某些基准测试中能够匹敌甚至超越 DeepSeek V4 Pro。在 OpenRouter 上的有效输入价格现在与 DeepSeek 托管的 Flash V4 相同，并且该模型可以在约 96GB RAM 的系统上运行。

hackernews · andai · 7月9日 15:27 · [社区讨论](https://news.ycombinator.com/item?id=48847552)

**背景**: 大型语言模型是在大量文本上训练的人工智能系统，用于生成类似人类的回应。腾讯和 DeepSeek 等公司竞争生产强大的模型，这些模型可以通过 API 访问或在本地运行。OpenRouter 是一个提供统一访问多个 AI 模型的平台，包括 Hy3。

**社区讨论**: 社区对 Hy3 的小尺寸和高能力感到兴奋，一些人认为它可能成为流行的本地模型。关于定价存在困惑，因为有效成本现在与 DeepSeek Flash V4 相似，并且有关于它如何处理与 DeepSeek V4 Flash 相比的重重量化的疑问。

**标签**: `#machine learning`, `#language models`, `#Tencent`, `#Hy3`, `#AI`

---

<a id="item-7"></a>
## [Meta 发布 Muse Spark 1.1 智能体 AI 模型](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 8.0/10

Meta 发布了 Muse Spark 1.1，这是一个新的智能体 AI 模型，通过 API 提供。社区成员已为其创建插件，并对基准测试结果的有效性展开讨论。 此次发布展示了 Meta 在 AI 模型领域的竞争决心，通过激进定价和开源权重可能使编程模型商品化；同时社区批评凸显了严格评估标准的必要性。 该模型定价为每百万输入 token 1.25 美元，每百万输出 token 4.5 美元，缓存输入仅为 0.15 美元。社区成员为 LLM 工具创建了插件，支持终端使用；同时有批评指出基准测试结果可能因超出资源限制而无效。

hackernews · ot · 7月9日 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48846184)

**背景**: Muse Spark 是 Meta 推出的智能体 AI 模型系列，旨在自主完成编程和工具交互等任务。Meta 曾有发布 Llama 等开源权重模型的历史。此次发布包括 API 访问和开源权重。社区讨论集中在基准测试分数因测试方法而是否可靠。

**社区讨论**: 社区反应复杂：有人强调定价低廉和实际集成（如 Simon Willison 的 LLM 插件），也有人质疑基准测试结果因方法问题而有效性。有用户认为 Meta 的策略可能是将 AI 模型商品化，另一用户指出 Meta 和 xAI 在与 OpenAI 及 Anthropic 的竞争中表现出人意料地具有竞争力。

**标签**: `#AI`, `#Meta`, `#Machine Learning`, `#Open Source`, `#Hacker News Discussion`

---

<a id="item-8"></a>
## [Meta 超级智能更新：RL 初创公司与大规模算力](https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence) ⭐️ 8.0/10

Meta 在其超级智能项目一周年进展更新中，披露了一个顶级强化学习环境初创公司的出现、前所未有的算力扩展计划，以及给 Google DeepMind 的战略建议。 这标志着 Meta 在追求超级智能方面的积极进击，凸显了强化学习环境和大规模算力基础设施在 AI 研究中日益增长的重要性。 这次算力提升被描述为前所未有地激进，规模跨度超过 2000 公里，暗示一个超大规模分布式系统。这个强化学习环境初创公司被认为是顶级水平，却似乎凭空出现。

rss · Semianalysis · 7月9日 19:16

**背景**: Meta 一直在大力投资 AI 超级智能，专注于大规模强化学习。用于游戏 AI 等领域的强化学习环境对于训练智能体至关重要。“2000 公里以上规模跨度”很可能指的是一个跨越数千公里的地理分布式计算集群。

**标签**: `#Meta`, `#superintelligence`, `#reinforcement learning`, `#AI infrastructure`, `#compute scaling`

---

<a id="item-9"></a>
## [IMGNet：使用符号模式而非余弦相似度的人脸验证模型](https://www.reddit.com/r/MachineLearning/comments/1urxvxh/i_built_imgnet_a_face_verification_model_that/) ⭐️ 8.0/10

IMGNet 是一种人脸验证模型，用滑动窗口符号模式匹配取代了余弦相似度，在 LFW 上达到 96.27%的准确率，模型仅 10.58 MB。 这种方法引入了一种新颖的人脸验证度量，关注关系符号模式而非全局角度相似性，可能提供更好的泛化能力和鲁棒性。该方法以更小的模型取得有竞争力的结果，适合资源受限的环境。 该模型使用 SW 块，在素数窗口大小下计算像素与邻居的差异，以及 IMG Sign MSE 损失，该损失纯粹基于符号模式一致性，无幅度依赖性。当应用于 ArcFace 嵌入而无需重新训练时，IMG Sign Score 在 LFW 上达到 99.58%，仅比 ArcFace+余弦低 0.24%。

reddit · r/MachineLearning · /u/img-_- · 7月9日 18:00

**背景**: 人脸验证是判断两张人脸图像是否属于同一个人的任务。传统方法使用深度学习生成嵌入向量，并通过余弦相似度（测量向量之间的角度）进行比较。LFW（野外标记人脸）是人脸验证的标准基准数据集。

**标签**: `#face verification`, `#computer vision`, `#deep learning`, `#novel approach`, `#efficient model`

---

<a id="item-10"></a>
## [蚂蚁灵波开源全球首个 MoE 具身视频基模 LingBot-Video](https://www.qbitai.com/2026/07/446458.html) ⭐️ 8.0/10

蚂蚁灵波开源了全球首个基于 MoE 架构的具身智能视频生成基础模型 LingBot-Video，总参数量 30B，推理时仅激活约 3B 参数。 此次发布大幅提升了具身视频生成的推理效率，性能约为同等规模稠密模型的 3 倍，并且是首个开源的此类模型，有望加速机器人学和世界模型的研究。 该模型采用 DiT+MoE 设计，并在包含 7 万小时具身数据的定制数据集上训练，涵盖灵巧操作、机器人移动和第一视角交互等场景。它还引入了多维强化学习奖励系统，重点关注物理合理性和任务完成度。

telegram · zaihuapd · 7月9日 04:30

**背景**: 具身智能专注于能够感知并与物理世界交互的智能体。用于具身任务的视频生成模型必须生成物理合理且与任务相关的序列。MoE（混合专家）架构使模型在保持大总容量的同时，每次推理仅激活部分参数，从而平衡性能与效率。

**标签**: `#MoE`, `#具身智能`, `#视频生成`, `#开源`, `#AI模型`

---

<a id="item-11"></a>
## [大疆 EV50 飞越珠峰至 8861 米](https://www.163.com/dy/article/L1CUCV940514R9OJ.html) ⭐️ 8.0/10

大疆尚未发布的 EV50 垂直起降运载无人机在珠峰科考中飞越 8861 米，创下同类公开测试的最高升限。 这一成就验证了 EV50 的高海拔性能，对极端环境下的物流和科研具有重要意义。 EV50 是一款复合翼无人机，可垂直起降并切换为固定翼巡航。在为期 12 天的任务中，共完成 32 架次起降，连续爬升 3730 米，返程时剩余 30%电量。

telegram · zaihuapd · 7月9日 06:00

**背景**: 无人机通常在稀薄空气中难以飞行，因此超过 8800 米的飞行是重大的工程挑战。EV50 设计用于货物运输和低空物流，此次测试证明了其在极端条件下的能力。

**标签**: `#无人机`, `#珠峰`, `#垂直起降`, `#物流`, `#测试`

---

<a id="item-12"></a>
## [国家超算互联网核心节点在郑州上线](https://36kr.com/newsflashes/3887797387344387) ⭐️ 8.0/10

2026 年 7 月 9 日，国家超算互联网核心节点在郑州上线，可提供超过 10 万卡国产人工智能算力。 这一里程碑加强了中国国产计算基础设施，减少对外国芯片的依赖，支持人工智能和超算的发展。 该节点作为全国计算资源统筹调度体系的运营管理和调度枢纽，同时整合供需对接和产业孵化等综合服务。

telegram · zaihuapd · 7月9日 07:00

**背景**: 国家超算互联网是一个连接全国超算中心以实现资源共享的项目。郑州核心节点是该网络的关键组成部分，国产 AI 算力使用本地制造的芯片以增强自给自足能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dchub.cloud/facility/5667059">国家超算互联网核心节点— , Data Center - DC Hub</a></li>

</ul>
</details>

**标签**: `#超算互联网`, `#国产算力`, `#人工智能`, `#国家基础设施`

---