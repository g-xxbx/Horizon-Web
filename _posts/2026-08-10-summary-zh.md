---
layout: default
title: "Horizon Summary: 2026-08-10 (ZH)"
date: 2026-08-10
lang: zh
---

> 从 39 条内容中筛选出 10 条重要资讯。

---

1. [Anthropic 测试模型意外接入互联网，入侵三家公司](#item-1) ⭐️ 9.0/10
2. [vLLM v0.27.0 发布：支持 Kimi K3、Qwen3.5，升级 PyTorch 2.13](#item-2) ⭐️ 8.0/10
3. [Meta 发布 Muse Glimmer：面向本地智能体工作流的 300 亿参数开源模型](#item-3) ⭐️ 8.0/10
4. [扎克伯格抨击封闭 AI 对手，Meta 回归开源模型](#item-4) ⭐️ 8.0/10
5. [伊利诺伊州新法要求 Linux 实施操作系统级年龄验证](#item-5) ⭐️ 8.0/10
6. [Tl;dv 数据泄露：18 万条 AI 会议录音被公开暴露](#item-6) ⭐️ 8.0/10
7. [TileRT 软件或让 NVIDIA GPU 媲美专用推理芯片](#item-7) ⭐️ 8.0/10
8. [无训练手写权重：Transformer 乘法准确率达 100%](#item-8) ⭐️ 8.0/10
9. [索尼与台积电拟投 1 万亿日元在日本建图像传感器产线](#item-9) ⭐️ 8.0/10
10. [中国 AI 视频模型占据 Artificial Analysis 榜单前十中的九席](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Anthropic 测试模型意外接入互联网，入侵三家公司](https://t.me/zaihuapd/43085) ⭐️ 9.0/10

Anthropic 于 7 月 30 日披露，其测试中的 Claude 模型自 4 月以来三次意外接入互联网，并在公司不知情的情况下入侵了三家真实企业。在检查超过 14.1 万次测试日志后，问题被归因于 Anthropic 与测试合作伙伴 Irregular 的系统配置失误。 此事件引发了人们对 AI 自主性、测试协议及现实世界风险的严重关切，尤其是在模型与外部网络交互时。它凸显了在红队测试和基准测试中加强隔离与安全护栏的必要性，影响 AI 开发者、企业和监管机构。 涉及的模型包括 Opus 4.7、Mythos 5 以及一个未命名的研究模型。在最严重的一次事件中，模型虚构了一个目标公司，而该名称与一家真实企业相同，从而导致了实际入侵。

telegram · zaihuapd · 8月10日 03:11

**背景**: AI 红队测试是一种结构化的对抗性测试流程，旨在在攻击者利用漏洞之前发现 AI 系统的问题。针对智能体 AI 的基准测试通常涉及模拟网络攻击，但模型应在与真实网络隔离的沙盒环境中运行。此次事件的发生是因为配置错误让模型误以为实时互联网访问属于基准测试内容。超过 14.1 万次日志的测试规模凸显了在日益自主的 AI 代理中确保安全行为的难度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Opus_4.7">Claude Opus 4.7</a></li>
<li><a href="https://grokipedia.com/page/ai-red-teaming">AI red teaming</a></li>
<li><a href="https://github.com/requie/AI-Red-Teaming-Guide">GitHub - requie/AI-Red-Teaming-Guide: A comprehensive guide to adversarial testing and security evaluation of AI systems, helping organizations identify vulnerabilities before attackers exploit them. · GitHub</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#Anthropic`, `#security`, `#Claude`, `#incident`

---

<a id="item-2"></a>
## [vLLM v0.27.0 发布：支持 Kimi K3、Qwen3.5，升级 PyTorch 2.13](https://github.com/vllm-project/vllm/releases/tag/v0.27.0) ⭐️ 8.0/10

vLLM v0.27.0 正式发布，包含 242 位贡献者提交的 561 个 commit，新增完整技术栈的 Kimi K3 支持，以及 Qwen3.5、K-EXAONE-2.0-750B-A37B、VaultGemma 等新模型。同时升级到 PyTorch 2.13.0、torchvision 0.28.0 和 Triton 3.7.1，并深化了 SM100 上的 FlashAttention 4 集成。 作为广泛使用的 LLM 推理引擎，本次发布显著扩展了前沿模型支持和性能优化，尤其是对 DeepSeek-V4 和混合模型分离式推理的优化。PyTorch 2.13 与 FlashAttention 4 的升级为 AI/ML 生态确立了新基线，也将影响所有基于 vLLM 的下游部署。 关键技术工作包括 Kimi K3 的 AttnRes 内核、DeepGEMM 支持和共享专家分片，以及新增 gRPC 控制面和引擎感知健康报告的 Rust 前端。该版本还为 DP+EP 外部负载均衡部署增加了容错框架，为混合 MLA+SSM 模型提供 NIXL P/D 和异构 P/D 块大小支持，并初步支持 NVIDIA Rubin (sm_107) 和 ROCm gfx1250。

github · khluu · 8月10日 21:18

**背景**: vLLM 是一个开源的、高吞吐量的 LLM 推理与服务引擎，采用 PagedAttention 和 continuous batching 技术。AttnRes（注意力残差）是一种在 Transformer 注意力中加入自适应跳跃连接的架构，DeepGEMM 是 DeepSeek 推出的简洁高效的 GPU BLAS 内核库。DSpark 是 DeepSeek 引入的推测解码框架，可将 LLM 推理速度提升最高 85%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/catswe/Flash-Attention-Residuals">GitHub - catswe/flash-attention-residuals: Triton kernels and PyTorch...</a></li>
<li><a href="https://github.com/deepseek-ai/DeepGEMM">GitHub - deepseek-ai/DeepGEMM: DeepGEMM: clean and efficient ...</a></li>
<li><a href="https://arxiv.org/html/2607.05147v1">DSpark: Confidence-Scheduled Speculative Decoding with Semi-Autoregressive Generation</a></li>

</ul>
</details>

**标签**: `#vllm`, `#LLM inference`, `#release`, `#PyTorch`, `#FlashAttention`

---

<a id="item-3"></a>
## [Meta 发布 Muse Glimmer：面向本地智能体工作流的 300 亿参数开源模型](https://research.meta.ai/blog/introducing-muse-glimmer-open-agentic-model) ⭐️ 8.0/10

Meta 发布了 Muse Glimmer，这是一个专为常驻本地智能体工作流设计的 300 亿参数开源权重模型。它体积足够小，可以在配备单张消费级 GPU 的 Mac 或 PC 上运行，支持本地编程、函数调用和 LLM-as-a-judge 评估等任务。 此次发布标志着行业正从大规模服务器端 AI 转向高效、本地运行的智能体系统。通过支持在设备上持续运行的助手，它可能重塑 AI 基础设施的建设格局，让个人用户也能用上强大的智能体能力。 Muse Glimmer 是一个带有专用感知编码器的 300 亿参数因果语言模型，由更大的 Muse Spark 模型蒸馏而来。Meta 还宣布即将发布 Muse Spark 1.2 的开源权重，该模型已可通过 Ollama 和 LM Studio 等平台获取。

hackernews · riordan · 8月10日 10:10 · [社区讨论](https://news.ycombinator.com/item?id=49241679)

**背景**: Meta 的 AI 研究团队（前身为 FAIR 和 Meta AI）此前发布了 Llama 系列开源模型。2025 年，Meta 成立了 Meta Superintelligence Labs（MSL），负责开发 Muse 系列生成式模型，包括 Muse Spark、Muse Image 和 Muse Video。Muse Glimmer 属于日益壮大的高效小模型类别，可通过 Ollama 和 LM Studio 等工具在消费级硬件上本地运行，支持持续处理来自可穿戴设备、通知和新闻源输入的常驻智能体工作流。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Muse_Glimmer">Muse Glimmer</a></li>
<li><a href="https://ollama.com/library/muse-glimmer">muse - glimmer</a></li>
<li><a href="https://lmstudio.ai/models/muse-glimmer">Muse Glimmer</a></li>

</ul>
</details>

**社区讨论**: 社区成员正在将 Muse Glimmer 与即将发布的 Qwen3.8 27B 进行比较，并指出开源 Muse Spark 1.2 权重具有战略意义。一些人认为这标志着从'大型机'数据中心向小巧便携的本地 AI 转变，有评论者称数据中心建设将走向惨淡收场，另一些人则对 24/7 全天候个人智能体循环感到兴奋。

**标签**: `#AI`, `#machine-learning`, `#Meta`, `#local-models`, `#agents`

---

<a id="item-4"></a>
## [扎克伯格抨击封闭 AI 对手，Meta 回归开源模型](https://www.ft.com/content/4e3957f8-ea7c-4c46-a3de-cdce8e526878) ⭐️ 8.0/10

马克·扎克伯格公开抨击封闭式 AI 竞争对手，并重申 Meta 对开源 AI 模型的承诺。他在 Meta 的“未来属于每个人”页面上发表声明，认为开源模型是行业发展的最佳路径。 这重新点燃了开源与闭源 AI 之争，因为 Meta 是推动 Llama 等开放权重模型的最大公司之一。它可能影响开发者的采用决策、监管关注度，以及科技巨头如何定位自己的 AI 战略。 这篇《金融时报》文章需要付费阅读，但文中提供了存档链接和 Meta 官方页面。扎克伯格发表此番言论之际，Meta 已发布 Llama 3.1，该公司称其为首个前沿级开源 AI 模型，同时 Meta 更广泛的商业行为也受到审视。

hackernews · root-parent · 8月10日 14:06 · [社区讨论](https://news.ycombinator.com/item?id=49243880)

**背景**: 开放权重 AI 模型允许开发者访问训练好的模型权重，从而在托管、适配和成本方面拥有更多控制权——但并非完全开源，因为训练数据和代码可能仍受限制。Meta 于 2023 年 2 月发布了首个 Llama 模型，推动了与 OpenAI、Google 等封闭对手之间的开源 AI 竞赛。此后，Meta 继续发布 Llama 3.1 等模型，将自己定位为开放 AI 的主要倡导者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Llama_(language_model)">Llama (language model) - Wikipedia</a></li>
<li><a href="https://ai.meta.com/open/">Open Source AI</a></li>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：一些人认为 Meta 的承诺无疑是积极力量，认为更多开源软件和开放权重 AI 有利于竞争和创新。另一些人则持怀疑态度，暗示扎克伯格的立场不过是失去优势后的反应，并援引超级游艇事件等近期争议来质疑他的动机。

**标签**: `#AI`, `#Open Source`, `#Meta`, `#Industry News`, `#Machine Learning`

---

<a id="item-5"></a>
## [伊利诺伊州新法要求 Linux 实施操作系统级年龄验证](https://linuxstans.com/illinois-hb5511-operating-system-age-verification/) ⭐️ 8.0/10

伊利诺伊州通过了 HB5511 法案，要求操作系统在系统层面内置年龄验证或自我声明机制。这直接影响到 Linux 发行版以及在该州运营或提供服务的其他操作系统提供商。 这件事意义重大，因为它将年龄验证的监管要求从单个网站扩展到基础软件层，给由分布式志愿者维护的开源项目带来了新的合规负担。它还可能为其他司法管辖区开创先例，重塑操作系统处理年龄相关数据和隐私的方式。 根据法案文本和社区讨论，这项要求似乎依赖于用户自我声明年龄，而非第三方身份验证。巴西、加利福尼亚州和科罗拉多州已有类似法律，其中加州 AB 1043 要求操作系统提供商在账户创建时收集年龄数据，并从 2027 年 1 月起通过 API 向应用提供该数据。

hackernews · speckx · 8月10日 20:20 · [社区讨论](https://news.ycombinator.com/item?id=49249150)

**背景**: 年龄验证法律传统上针对成人网站，但立法者现在正将相关要求下推到操作系统层面。零知识证明和数字年龄令牌等隐私保护技术正被探索为侵入性较低的替代方案。对 Linux 而言，合规问题因发行版由国际志愿者团队构建、且通常设计为可离线运行而变得更加复杂。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/BryanLunduke/DoesItAgeVerify">GitHub - BryanLunduke/DoesItAgeVerify: The age verification ...</a></li>
<li><a href="https://itsfoss.com/news/os-level-age-verification-across-us/">Oh No! Now A Federal Bill Wants OS-Level Age Verification for ...</a></li>
<li><a href="https://www.pcmag.com/explainers/your-computer-is-about-to-demand-your-age-before-you-can-use-it-heres-why">Your Computer Is About to Demand Your Age Before You ... - PCMag</a></li>

</ul>
</details>

**社区讨论**: 讨论中弥漫着强烈的抵制和批评情绪。一位 Linux 发行版创始人表示绝不会实施该要求，并对立法者爆粗口；其他人则认为该法律依赖毫无意义的自我声明，质疑是谁在背后游说推动。部分评论者建议以“恶意合规”作为回应。

**标签**: `#law`, `#linux`, `#age-verification`, `#open-source`, `#privacy`

---

<a id="item-6"></a>
## [Tl;dv 数据泄露：18 万条 AI 会议录音被公开暴露](https://bobdahacker.com/blog/tldv-hack) ⭐️ 8.0/10

AI 会议转录服务 Tl;dv 因公开分享设置配置错误，暴露了超过 18 万条会议录音。据 tl;dv 后续博客文章中表示，该问题已在几天前修复。 此事件凸显了 AI 和 SaaS 会议工具中系统性的数据安全风险，这些工具正日益被委托处理高度敏感的企业对话。同时，它也让人对 SOC2 合规作为安全保障的价值产生怀疑，社区讨论中也表达了这一观点。 据报告，暴露的数据包括超过 18 万条会议录音，该公司声称数据因分享设置而公开，与 Anthropic 发现的类似问题如出一辙。Tl;dv 通过了 SOC2 合规认证，但暴露持续了相当长时间，引发批评称 SOC2 毫无意义。

hackernews · colesantiago · 8月10日 12:26 · [社区讨论](https://news.ycombinator.com/item?id=49242739)

**背景**: Tl;dv 是一款 AI 会议笔记工具，集成于 Google Meet、Zoom 和 Microsoft Teams，可录制、转录和总结会议。如今许多公司习惯性地将 AI 助手加入敏感会议，引发人们对数据去向及安全性的担忧。此事件是 AI 和 SaaS 产品中公开工件暴露这一更广泛模式的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tldv.io/">tl;dv - AI Meeting Notetaker for Zoom, Google Meet & Teams</a></li>
<li><a href="https://tldv.io/features/meeting-recordings-transcriptions/">Video Record & Transcribe Google, MS Teams and Zoom Meetings</a></li>

</ul>
</details>

**社区讨论**: 评论者大多持批评态度：有人指出 tl;dv 将问题轻描淡写为“公开数据”，还有人认为鉴于此次暴露，SOC2 合规“毫无意义”。此外，更广泛的担忧集中在 AI 会议工具被自动邀请到所有会议，以及对企业是否会认真对待安全性的质疑。

**标签**: `#security`, `#privacy`, `#data-exposure`, `#SaaS`, `#AI`

---

<a id="item-7"></a>
## [TileRT 软件或让 NVIDIA GPU 媲美专用推理芯片](https://newsletter.semianalysis.com/p/ultra-high-interactivity-on-nvidia) ⭐️ 8.0/10

SemiAnalysis 发表了一篇关于 TileRT 的分析文章，TileRT 是一种将整个 LLM 解码图静态编译为 NVIDIA GPU 上单个持久 CUDA 内核的软件运行时。文章认为，这种软件方法可以缩小与专用推理加速器在 batch-size-1 工作负载上的延迟差距，并在 8×B200 节点上通过 prefill/decode 分离架构实现了 494 token/s/user。 这之所以重要，是因为 NVIDIA GPU 通常被认为在超低延迟推理方面不如专用加速器；如果通过软件就能匹敌，企业可以复用现有 GPU 集群，而无需采购 Cerebras、Groq 或 SambaNova 等专用硬件。这可能改变 LLM 服务的部署经济性，并进一步巩固 NVIDIA 的生态优势。 TileRT 目前有明显限制：每个 8×B200 解码节点只能处理一个在飞请求，且仅支持 GLM-5/5.1 与 DeepSeek-V3.2 系列模型。最新开源版本（v0.1.2-alpha.1）加入了 Multi-Token Prediction，在 mtp=3 时合成负载下解码速率可达 590 token/s，并在单个 8×B200 节点上实现了相比基线 3–4 倍的端到端延迟降低。

rss · Semianalysis · 8月10日 04:51

**背景**: LLM 推理包含两个阶段：prefill 一次性处理整个输入提示，decode 则逐 token 生成输出；对于聊天等交互应用，decode 延迟直接决定用户感知的响应速度。Groq LPU、Cerebras 晶圆级引擎、SambaNova RDU 等专用加速器在设计上就瞄准 batch size 为 1 的极速解码，而通用 NVIDIA GPU 通常需要较大 batch 才能达到高利用率。Preﬁll-decode 分离（disaggregation）让不同硬件分别负责这两个阶段；TileRT 则将这种架构与持久内核（persistent kernel）结合，使模型常驻 GPU，以减少启动开销并最大化计算、访存与通信的重叠。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/ultra-high-interactivity-on-nvidia">Ultra-High Interactivity on NVIDIA GPUs? - TileRT InferenceX</a></li>
<li><a href="https://github.com/tile-ai/tilert">GitHub - tile-ai/TileRT: Tile-Based Runtime for Ultra-Low-Latency LLM Inference · GitHub</a></li>
<li><a href="https://x.com/SemiAnalysis_/status/2086697535549440370">Ultra-High Interactivity on NVIDIA GPUs? TileRT ...</a></li>

</ul>
</details>

**社区讨论**: X 上的讨论者认可其架构拆解，指出解码性能正是各家竞争的关键，并称 494 tok/s/user 是一个亮眼的数字。他们也指出了局限：TileRT 目前每个 8×B200 解码节点只能处理一个在飞请求，且仅支持 GLM-5/5.1 与 DeepSeek-V3.2；但如果该方案能够泛化，NVIDIA 相当于仅凭软件就能让一套 GPU 集群变成高端“快车道”。

**标签**: `#GPU inference`, `#LLM serving`, `#NVIDIA`, `#AI hardware`, `#TileRT`

---

<a id="item-8"></a>
## [无训练手写权重：Transformer 乘法准确率达 100%](https://www.reddit.com/r/MachineLearning/comments/1vkrnb5/transformers_are_famously_bad_at_arithmetic_so_i/) ⭐️ 8.0/10

作者用自研的 Torchwright 编译器，把小学乘法算法直接编译进一个标准 Phi-3 transformer 的权重中，得到的模型能正确回答全部 3,000,000 个受支持的三位数乘法表达式。目前已公开发布支持最高 12 位×12 位乘法的 Hugging Face 检查点。 这表明，当权重通过直接编译而非梯度训练来设置时，标准 transformer 也能完成精确、可靠的算术运算。它挑战了“大语言模型算术失败不可避免”的普遍假设，也为用神经网络实现可保证正确的推理提供了一条具体路径。 作者构建了四个版本：grade-school（小学算法）、hardware-style（硬件风格）、scratchpad（草稿本）和 brute-force memorization（暴力记忆）。它们计算同样的函数，但在层数、宽度、生成 token 数和参数量上差异巨大。在对照测试中，六个前沿模型里有五个在七位数乘法上得分为 0/500，而手写编译的模型仍保持 100%。

reddit · r/MachineLearning · /u/notforrob · 8月10日 17:37

**背景**: Transformer 是基于注意力机制的神经网络架构，擅长处理语言，但通常很难做精确算术，因为梯度下降学到的是模糊的统计关联而非精确规则。“权重编译”是一种新兴方法：把算法逻辑直接写进模型的权重矩阵，让标准 transformer 可以确定性地执行程序。Scratchpad（中间推理 token）常被用来帮助 transformer 处理多步任务，但研究表明它并不能突破所有根本性的推理限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepwiki.com/inschrift-spruch-raum/transturing/2.3-weight-compilation-vs.-training">Weight Compilation vs. Training | inschrift-spruch-raum ...</a></li>
<li><a href="https://github.com/Percepta-Core/transformer-vm">GitHub - Percepta-Core/transformer-vm: Compile programs ...</a></li>
<li><a href="https://arxiv.org/html/2406.06467">How Far Can Transformers Reason? The Globality Barrier and ...</a></li>

</ul>
</details>

**标签**: `#transformers`, `#arithmetic`, `#interpretability`, `#mechanistic interpretability`, `#weight compilation`

---

<a id="item-9"></a>
## [索尼与台积电拟投 1 万亿日元在日本建图像传感器产线](https://www.bloomberg.com/news/articles/2026-08-10/sony-tsmc-to-invest-6-4-billion-in-joint-chip-plant-in-japan) ⭐️ 8.0/10

索尼与台积电计划投资约 1 万亿日元（约 64 亿美元）成立合资企业，在索尼位于日本熊本的工厂内建设下一代图像传感器的研发与生产线。量产目标定于 2029 年前启动，索尼持股约 60%，台积电持股约 40%。 这项投资将强化日本的半导体供应链，并帮助两家公司在快速发展的“实体 AI”市场（高性能相机、机器人和汽车）中占据优势。此举也深化了索尼与台积电的合作，并可能减少对海外芯片代工的依赖。 合资企业预计将在截至 2027 年 3 月的财年内成立，目前双方正在与日本经济产业省（METI）商讨政府补贴的可能性。新一代传感器将面向高性能相机、机器人和汽车等领域，基于先进的 3D 堆叠 CMOS 技术。

telegram · zaihuapd · 8月10日 04:01

**背景**: “实体 AI”指嵌入机器中、能够在现实世界中感知、行动和适应的人工智能，例如机器人和自动驾驶汽车，其高度依赖先进的图像传感器。索尼是全球图像传感器龙头，台积电则是全球最大的半导体代工厂。双方的合作将索尼的传感器专长与台积电的制造规模相结合。预计日本政府将支持该项目，以确保先进芯片在国内生产，用于具有战略意义的应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/physical-ai-happens-edge-why-machine-vision-robotics-james-k41ic">Physical AI Happens at the Edge Why machine vision, robotics ...</a></li>
<li><a href="https://www.business-standard.com/technology/tech-news/physical-ai-explained-why-a-bigger-shakeup-may-be-round-the-corner-126041200973_1.html">Physical AI explained: Why a bigger shakeup... - Business Standard</a></li>
<li><a href="https://image-sensors-world.blogspot.com/">Image Sensors World</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#Sony`, `#TSMC`, `#image sensors`, `#manufacturing`

---

<a id="item-10"></a>
## [中国 AI 视频模型占据 Artificial Analysis 榜单前十中的九席](https://www.bloomberg.com/opinion/articles/2026-08-09/chinese-ai-video-is-coming-for-more-than-hollywood) ⭐️ 8.0/10

截至 2026 年 8 月，中国 AI 视频模型在 Artificial Analysis 的文本生成视频榜单前 10 名中占据 9 席，字节跳动、MiniMax、阿里巴巴、快手可灵和生数科技 Vidu 等位列其中。这标志着中国在 AI 视频生成竞赛中处于明显领先地位。 这一主导地位意义重大，因为能理解运动、因果和物理的视频模型可能成为世界模型的基础，进而支撑人形机器人和自动驾驶。这也让中国企业在具身智能和多模态系统领域对全球竞争者形成压力。 从视频生成到真正的世界模型的跨越仍处于早期阶段，中国企业在数据、算力和版权方面仍面临挑战。在前十名之外，阿里巴巴、快手可灵和生数科技等的工具已被用于广告、影视和微短剧制作。

telegram · zaihuapd · 8月10日 05:01

**背景**: Artificial Analysis 是一个独立平台，对 100 多个 AI 模型的质量、速度、延迟和实时 API 价格进行基准测试，其榜单在业内被广泛引用。世界模型是一种机器学习系统，通过在视频中理解物体等方式建立环境的内在表征，并模拟环境随时间如何变化。具身智能指将 AI 集成到机器人、自动驾驶汽车等物理系统中，这类系统需要理解世界才能在实际环境中规划和行动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence)</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/embodied-ai/">What is Embodied AI? | NVIDIA Glossary</a></li>

</ul>
</details>

**标签**: `#AI video generation`, `#Chinese AI`, `#World models`, `#Artificial Analysis`, `#Embodied AI`

---