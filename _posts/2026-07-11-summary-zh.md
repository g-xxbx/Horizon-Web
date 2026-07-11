---
layout: default
title: "Horizon Summary: 2026-07-11 (ZH)"
date: 2026-07-11
lang: zh
---

> 从 30 条内容中筛选出 9 条重要资讯。

---

1. [vLLM v0.25.0 默认启用 Model Runner V2，移除 PagedAttention](#item-1) ⭐️ 9.0/10
2. [人形机器人远程完成活猪胆囊切除手术](#item-2) ⭐️ 9.0/10
3. [SGLang v0.5.15 发布：GLM-5.2 调优、Spec V2 和 IndexShare MTP](#item-3) ⭐️ 8.0/10
4. [ClickHouse 使用 SO_REUSEPORT 和 peering 将 PgBouncer 吞吐量提升 4 倍](#item-4) ⭐️ 8.0/10
5. [乔治·霍兹警告 AI 发展中的“智能崇拜”](#item-5) ⭐️ 8.0/10
6. [VultronRetriever 模型登顶 MTEB 并发布在 HuggingFace 上](#item-6) ⭐️ 8.0/10
7. [苹果因商业机密窃取起诉 OpenAI](#item-7) ⭐️ 8.0/10
8. [U-Boot 引导程序 6 漏洞可绕过验证执行恶意代码](#item-8) ⭐️ 8.0/10
9. [OpenAI 发布 GPT-5.6 系列，包含 Sol、Terra、Luna 三个层级](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0 默认启用 Model Runner V2，移除 PagedAttention](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 将所有密集模型的默认执行路径切换为 Model Runner V2，移除了传统的 PagedAttention 算法，并使 Transformers 建模后端性能达到原生 vLLM 水平。 此版本代表了重大的架构转变，简化了代码库并提升了性能。Transformers 后端达到原生速度意味着用户可以定义自定义模型而不损失速度，扩展了 vLLM 的可用性。 Model Runner V2 是重新设计的执行核心，支持 EVS、实时嵌入和 Mamba 混合模型的 prefix caching。Transformers 后端新增 FP8 MoE 支持，并修复了 CUDA graph 和 embed scaling 问题。

github · khluu · 7月11日 20:06

**背景**: PagedAttention 于 2023 年随 vLLM 推出，通过将 key-value 缓存存储在固定大小的块中来优化内存管理。Model Runner V2 是完全重写的实现，旨在提高模块化和效率。此版本整合到 MRV2 并移除了旧的 V1/PagedAttention 路径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PagedAttention">PagedAttention</a></li>
<li><a href="https://vllm.ai/blog/2026-03-24-mrv2">Model Runner V2: A Modular and Faster Core for vLLM</a></li>
<li><a href="https://github.com/vllm-project/vllm/blob/main/docs/design/model_runner_v2.md">vllm/docs/design/model_runner_v2.md at main · vllm-project ...</a></li>

</ul>
</details>

**标签**: `#vllm`, `#LLM inference`, `#release`, `#open source`, `#machine learning`

---

<a id="item-2"></a>
## [人形机器人远程完成活猪胆囊切除手术](https://arstechnica.com/ai/2026/07/humanoid-robots-controlled-by-surgeons-did-world-first-operation-on-live-pigs/) ⭐️ 9.0/10

外科医生远程操控宇树 G1 人形机器人，在活猪身上完成了全球首例微创胆囊切除手术。研究成果已发表在《自然》期刊。 这一突破表明，低成本通用人形机器人可用于远程手术，有望将手术服务扩展到偏远、农村、战场甚至太空等场景。这对达芬奇等昂贵专用手术机器人的主导地位构成挑战。 宇树 G1 基础款售价 13500 美元，配备灵巧手后约 67000 美元，仅为达芬奇系统（50 万至数百万美元）的零头。该机器人高约 1.5 米、重约 27 公斤，十分紧凑。

telegram · zaihuapd · 7月11日 02:29

**背景**: 人形机器人模仿人类形态和运动，灵巧手是能够精细操作工具的机器人末端执行器。达芬奇手术系统是一种专用的微创手术机器人平台，但价格昂贵且非通用。这项由加州大学圣地亚哥分校研究人员领导的研究，标志着通用人形机器人首次被用于活体手术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.jinantimes.com.cn/news-243-5048472.html">jinantimes.com.cn/news-243-5048472.html</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/717179760">一文看懂灵巧手 - 知乎</a></li>
<li><a href="https://zh.wikipedia.org/wiki/达芬奇手术系统">达芬奇手术系统 - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**标签**: `#humanoid robot`, `#telesurgery`, `#medical robotics`, `#Nature publication`

---

<a id="item-3"></a>
## [SGLang v0.5.15 发布：GLM-5.2 调优、Spec V2 和 IndexShare MTP](https://github.com/sgl-project/sglang/releases/tag/v0.5.15) ⭐️ 8.0/10

SGLang v0.5.15 已发布，针对 Blackwell GPU 上的 GLM-5.2 模型进行了 NVFP4 格式的生产调优，在 8x B300 上实现了每用户 500+ tokens/s。它还将 Spec V2 设为默认调度以实现零开销推测解码，并引入了 IndexShare MTP 以将草稿步成本降低高达 1.9 倍。 此版本显著提高了 LLM 服务效率，特别是对于 GLM-5.2 等长上下文模型，提供了更高吞吐量和更低延迟。这些优化推进了推测解码和注意力机制的前沿，惠及更广泛的 AI 推理生态系统。 Spec V2 通过消除主机-设备同步和融合元数据操作，实现了端到端吞吐量提升 11%。IndexShare MTP 在草稿步骤间复用索引器 top-k，降低长上下文的计算成本。该版本还包括形状专用的 GEMM 内核和默认开启的可中断 CUDA Graph。

github · Fridge003 · 7月10日 22:58

**背景**: GLM-5.2 是智谱 AI 开发的 744B 参数 MoE 语言模型，采用 IndexShare 架构跨稀疏注意力层复用索引器，针对长上下文任务进行了优化。NVFP4 是 NVIDIA Blackwell GPU 引入的 4 位浮点格式，可实现高效的低精度推理。多令牌预测（MTP）通过同时预测多个令牌来加速推测解码，而 IndexShare MTP 通过在步骤间复用 top-k 索引来降低草稿步成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/zai-org/GLM-5.2">zai-org/GLM-5.2 · Hugging Face</a></li>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision Inference | NVIDIA Technical Blog</a></li>
<li><a href="https://news.smol.ai/issues/26-06-16-glm-52">GLM 5.2: the top Frontend Coding model in the world, IndexShare ...</a></li>

</ul>
</details>

**标签**: `#sglang`, `#LLM serving`, `#performance optimization`, `#inference`, `#release`

---

<a id="item-4"></a>
## [ClickHouse 使用 SO_REUSEPORT 和 peering 将 PgBouncer 吞吐量提升 4 倍](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

ClickHouse 博客详细介绍了他们通过启用 SO_REUSEPORT 和 peering，使得多个 PgBouncer 进程共享同一端口并协调查询取消，从而将吞吐量提升 4 倍的方法。 该优化对 PostgreSQL 连接池性能至关重要，特别是在高流量环境中。它展示了一种实用的技术，其他 PgBouncer 用户可以借鉴，以在不增加硬件的情况下扩展数据库访问层。 SO_REUSEPORT 允许多个 PgBouncer 进程监听同一个 TCP 端口，而 peering 允许进程将取消请求转发给正确的会话所有者。此设置需要在配置中指定 peer_id，并绑定到同一端口。

hackernews · saisrirampur · 7月11日 15:28 · [社区讨论](https://news.ycombinator.com/item?id=48872874)

**背景**: PgBouncer 是一个轻量级的 PostgreSQL 连接池管理工具，用于管理客户端连接以降低数据库连接的开销。默认情况下，PgBouncer 以单进程方式运行，这可能会成为瓶颈。SO_REUSEPORT 是一个 Linux 套接字选项，允许多个套接字绑定到同一端口，实现内核级别的负载分发。PgBouncer 的 peering 功能允许多个进程共享会话状态并转发取消请求。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://www.pgbouncer.org/usage.html">PgBouncer command-line usage</a></li>
<li><a href="https://www.pgbouncer.org/config.html">PgBouncer config</a></li>
<li><a href="https://lwn.net/Articles/542629/">The SO_REUSEPORT socket option [LWN.net]</a></li>

</ul>
</details>

**社区讨论**: 社区评论包括对 Odyssey 和 pgdog 等替代工具的建议。一些用户对 peering 和 SO_REUSEPORT 的实际细节表示兴趣，另一些则分享了在 Kubernetes 中使用 PgBouncer 的经验。总体上，讨论是积极的，博文被认为是一次有价值的技术深入探讨。

**标签**: `#PgBouncer`, `#PostgreSQL`, `#performance`, `#connection pooling`, `#ClickHouse`

---

<a id="item-5"></a>
## [乔治·霍兹警告 AI 发展中的“智能崇拜”](https://geohot.github.io//blog/jekyll/update/2026/07/11/ai-2040.html) ⭐️ 8.0/10

乔治·霍兹发表了一篇题为《AI 2040 与智能崇拜》的博客文章，批评了 AI 发展中的意识形态控制和审查，并倡导自由。 这篇文章凸显了 AI 安全与言论/发展自由之间日益加剧的紧张关系，引发了关于如何监管 AI 的辩论。高参与度表明社区对这些问题的强烈兴趣。 博客认为自由是二元且值得为之奋斗的，并警告不要形成一种强制意识形态一致的 AI“智能崇拜”。社区评论讨论了思想犯罪、审查以及物理世界行动的影响。

hackernews · rvz · 7月11日 18:04 · [社区讨论](https://news.ycombinator.com/item?id=48874200)

**背景**: 乔治·霍兹（又名 geohot）是一位著名的黑客和企业家，创立了开源自动驾驶公司 comma.ai。他经常评论 AI 和技术政策。“智能崇拜”一词批评了将 AI 视为无误的预言者或对其输出施加严格意识形态控制的倾向。

**社区讨论**: 评论呈现分歧：一些人同意霍兹关于 AI 审查和意识形态偏见的危险，而另一些人则认为自由不是绝对的，在现实世界中行动的 AI 代理需要监管。一位用户警告了隐形记录“思想犯罪”和倾向性回复的问题。

**标签**: `#AI`, `#freedom`, `#ethics`, `#technology policy`

---

<a id="item-6"></a>
## [VultronRetriever 模型登顶 MTEB 并发布在 HuggingFace 上](https://www.reddit.com/r/MachineLearning/comments/1utmxq8/vultronretriever_family_of_models_released_on/) ⭐️ 8.0/10

VultronRetrieverPrime-8B 成为 MTEB 排行榜全球第一，全系列模型在 HuggingFace 上发布，并在 iPhone 上展示了离线边缘部署。 此次发布在检索领域树立了新的标杆，实现了显著的效率提升（索引缩小 16 倍，吞吐量提高 12 倍），同时支持边缘设备完全离线运行，使先进的检索技术可用于移动和嵌入式应用。 VultronRetriever 系列包括三个模型：Prime-8B、Core-4.5B 和 Flash-0.8B，均采用 Hydra 架构以实现后期交互检索。这些模型在数据集上训练时实现了 0%跨数据集重复和 0%评估污染。

reddit · r/MachineLearning · /u/madkimchi · 7月11日 15:22

**背景**: MTEB（大规模文本嵌入基准）是一个用于跨多种任务评估文本嵌入模型的标准化基准。后期交互检索将查询和文档分别处理直到最后阶段，实现高效精确的检索。边缘部署允许模型在智能手机等设备上本地运行，无需云连接。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/spaces/mteb/leaderboard">MTEB Leaderboard - a Hugging Face Space by mteb</a></li>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/mteb-leaderboard/">MTEB Leaderboard - GeeksforGeeks</a></li>
<li><a href="https://weaviate.io/blog/late-interaction-overview">An Overview of Late Interaction Retrieval Models... | Weaviate</a></li>

</ul>
</details>

**标签**: `#information retrieval`, `#MTEB leaderboard`, `#embeddings`, `#edge deployment`, `#HuggingFace`

---

<a id="item-7"></a>
## [苹果因商业机密窃取起诉 OpenAI](https://www.cnbc.com/2026/07/10/apple-openai-lawsuit-trade-secrets.html) ⭐️ 8.0/10

2026 年 7 月 10 日，苹果在美国加州北区联邦法院起诉 OpenAI、两名前员工及 io Products，指控其通过系统性窃取与硬件设计和制造相关的商业机密，以加速 OpenAI 的消费级硬件研发。 这起诉讼加剧了两家科技巨头在 AI 硬件和人才方面的竞争，可能为快速发展的 AI 行业中商业机密保护树立先例。 苹果具体指控前员工 Chang Liu 在离职后下载了数十份硬件文件，OpenAI 硬件负责人 Tang Yew Tan 将供应商信息发送至个人邮箱，并要求求职者携带苹果零部件参加面试。苹果还称目前有超过 400 名前员工在 OpenAI 工作。

telegram · zaihuapd · 7月11日 03:14

**背景**: 苹果长期将其硬件设计和制造流程视为严格保密的商业机密，而 OpenAI 主要以其 AI 软件（如 ChatGPT）闻名，近年来正拓展至消费级硬件领域，包括可能的 AI 驱动设备。这起诉讼反映了企业在 AI 硬件领域争夺人才和专有知识时不断加剧的紧张关系。

**标签**: `#Apple`, `#OpenAI`, `#lawsuit`, `#trade secrets`, `#hardware`

---

<a id="item-8"></a>
## [U-Boot 引导程序 6 漏洞可绕过验证执行恶意代码](https://www.bleepingcomputer.com/news/security/new-u-boot-flaws-could-enable-stealthy-firmware-attacks/) ⭐️ 8.0/10

安全公司 Binarly 披露了 U-Boot 引导程序 FIT 签名验证中的 6 个漏洞，其中 2 个可导致任意代码执行，4 个可导致设备崩溃。这些漏洞自 U-Boot 2013.07 版本起存在。 这些漏洞十分关键，因为它们允许攻击者在操作系统启动前执行恶意代码，绕过安全措施。影响大量嵌入式和物联网设备，可能实现持久性固件攻击，尤其是支持远程更新的系统（如 BMC）。 Binarly 已向 U-Boot 维护者提交漏洞报告，补丁已被接受。但修复需要各硬件厂商集成到固件更新中，已停止支持的老旧设备可能永远无法修复。这些漏洞编号为 BRLY-2026-037 至 BRLY-2026-042。

telegram · zaihuapd · 7月11日 08:32

**背景**: U-Boot（Das U-Boot）是一种通用的开源引导加载程序，广泛用于嵌入式系统和物联网设备。它支持 FIT（Flattened Image Tree）格式，该格式允许将多个镜像与加密签名捆绑以确保真实性和完整性。Binarly 发现的 6 个漏洞位于 FIT 签名验证代码中，可能允许攻击者绕过验证并在操作系统加载前执行恶意代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Das_U-Boot">Das U - Boot - Wikipedia</a></li>
<li><a href="https://docs.u-boot-project.org/en/latest/usage/fit/signature.html">U-Boot FIT Signature Verification — Das U-Boot unknown version...</a></li>
<li><a href="https://cybersecuritynews.com/u-boot-fit-signature-verification/">Six U-Boot FIT Signature Verification Flaws Enable Code Execution...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#U-Boot`, `#bootloader`, `#firmware`

---

<a id="item-9"></a>
## [OpenAI 发布 GPT-5.6 系列，包含 Sol、Terra、Luna 三个层级](https://t.me/zaihuapd/42497) ⭐️ 8.0/10

OpenAI 于 2026 年 6 月 26 日发布了 GPT-5.6 系列，提供三种模型变体：旗舰版 Sol、平衡版 Terra 和低成本版 Luna。该系列重点提升了编码、知识工作、设计、研究和网络安全能力，并引入了 max/ultra 推理、多智能体协作和程序化工具调用。 此次发布标志着 OpenAI 在模型优化上的重大进展，通过分层选项让用户在不同用例中平衡成本与性能。成本效益和能力的提升使高级 AI 在高端研究和大规模生产应用中更加可及。 采用 max 推理的 Sol 在编码基准测试上以更少的 token 和更低的成本取得了领先结果。Terra 以一半的价格提供约等于 GPT-5.5 的质量，而 Luna 针对高并发、低成本场景优化了延迟。

telegram · zaihuapd · 7月11日 13:34

**背景**: GPT-5.6 是 OpenAI 最新的模型系列，是 GPT-5.5 和 GPT-5 的继任者。三个层级满足不同需求：Sol 用于高要求任务，Terra 用于平衡性能，Luna 用于高吞吐量。max 和 ultra 推理模式的引入使用户可以为复杂问题扩展推理计算，而程序化工具调用则使智能体能够执行代码以交互工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-6/">GPT‑5.6: Frontier intelligence that scales with your ambition</a></li>
<li><a href="https://codersera.com/blog/gpt-5-6-sol-terra-luna/">GPT-5.6 Sol, Terra & Luna Explained: Tiers, Pricing ...</a></li>
<li><a href="https://andrew.ooo/answers/what-is-gpt-5-6-sol-terra-luna-openai-june-2026/">What is GPT-5.6? Sol, Terra, Luna Explained (June 2026)</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-5.6`, `#AI models`, `#machine learning`

---