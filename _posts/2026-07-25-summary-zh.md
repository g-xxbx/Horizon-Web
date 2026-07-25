---
layout: default
title: "Horizon Summary: 2026-07-25 (ZH)"
date: 2026-07-25
lang: zh
---

> 从 25 条内容中筛选出 8 条重要资讯。

---

1. [SGLang v0.5.16 推出 DSPark 推测解码与 Inkling 模型支持](#item-1) ⭐️ 10.0/10
2. [vLLM v0.26.0 新增 Inkling 模型系列和 DeepSeek-V4 优化](#item-2) ⭐️ 8.0/10
3. [安卓可能限制设备端 ADB 访问](#item-3) ⭐️ 8.0/10
4. [开放权重 AI 迎来“Kubernetes 时刻”：平台转变信号](#item-4) ⭐️ 8.0/10
5. [Claude Opus 5 发布：性能直逼 Fable 5 价格减半](#item-5) ⭐️ 8.0/10
6. [AMD 2026 年 AI 战略旨在打破 NVIDIA 的 CUDA 护城河](#item-6) ⭐️ 8.0/10
7. [离岸信托个税新规：装入财产及收益须申报纳税](#item-7) ⭐️ 8.0/10
8. [上海携程商务因数据出境违规被罚 1000 万元](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [SGLang v0.5.16 推出 DSPark 推测解码与 Inkling 模型支持](https://github.com/sgl-project/sglang/releases/tag/v0.5.16) ⭐️ 10.0/10

SGLang v0.5.16 引入了 DSPark 置信度驱动的推测解码，并支持 9750 亿参数的 Inkling 多模态模型。 此版本显著提升了 AI 推理速度和规模，使得大型语言和多模态模型的高效部署成为可能，并展示了推测解码技术的进步。 DSPark 在 B300 上对 DeepSeek-V4-Pro（TP8）实现了每秒 383.7 个 token 的推理速度；Inkling 模型则支持 100 万 token 的上下文窗口并采用混合注意力机制。

github · Qiaolin-Yu · 7月25日 00:13

**背景**: 推测解码通过使用草稿模型并行提出多个 token 再由目标模型验证，从而加速大语言模型推理。SGLang 是一个高效服务大型语言和多模态模型的框架。本版引入的 DSPark 算法利用置信度分数动态调整验证窗口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.alphaxiv.org/abs/2026.dspark">DSpark : Confidence -Scheduled Speculative Decoding ... | alphaXiv</a></li>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://en.wikipedia.org/wiki/Speculative_decoding">Speculative decoding</a></li>

</ul>
</details>

**标签**: `#speculative decoding`, `#AI inference`, `#SGLang`, `#DeepSeek-V4`, `#Blackwell`

---

<a id="item-2"></a>
## [vLLM v0.26.0 新增 Inkling 模型系列和 DeepSeek-V4 优化](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 发布，包含 411 次提交，全面支持 Inkling 模型系列（包括分段 CUDA 图、NVFP4 量化、LoRA 和推测解码），对 DeepSeek-V4 进行了重大性能优化，并完善了 KV 卸载系统。 此版本增强了 vLLM 服务于先进多模态 MoE 模型（如 Inkling 和 DeepSeek-V4）的效率，对于需要优化推理才能实用的庞大模型来说至关重要。 值得注意的技术细节包括分段 CUDA 图支持以灵活捕获图形，NVFP4 量化以减少内存使用，通过 head_dtype 使用 fp32 lm_head 以提高准确性，以及针对混合模型的每 KV 缓存组注意力后端选择。

github · khluu · 7月25日 10:38

**背景**: vLLM 是一个开源的高吞吐量 LLM 推理引擎，采用 PagedAttention 和连续批处理。Thinking Machines Lab 的 Inkling 模型系列包含一个总参数 975B 的大型多模态 MoE 模型。分段 CUDA 图允许模型中对完整图捕获不兼容的部分保持急切执行，同时仍受益于图优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling : Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://docs.vllm.ai/en/stable/design/cuda_graphs/">CUDA Graphs - vLLM Documentation</a></li>

</ul>
</details>

**标签**: `#vllm`, `#release`, `#model serving`, `#deepseek`, `#performance`

---

<a id="item-3"></a>
## [安卓可能限制设备端 ADB 访问](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/) ⭐️ 8.0/10

一项安卓更新提案可能限制设备端 ADB 访问，阻止应用在无连接电脑的情况下本地使用 ADB 命令。这可能影响 Shizuku、libadb 等依赖此功能进行无需 root 操作的实用工具。 此变更可能严重影响依赖设备端 ADB 进行调试、自动化和设备管理的安卓开发者和高级用户。它凸显了加强设备安全性与保持用户自由度之间的持续权衡。 该提案可能要求每次设备端 ADB 连接都获得用户明确同意，或将访问限制在特定网络接口。此前类似措施包括 RSA 认证和设备白名单以降低恶意软件风险。

hackernews · shscs911 · 7月25日 06:57 · [社区讨论](https://news.ycombinator.com/item?id=49045159)

**背景**: 安卓调试桥（ADB）是一种命令行工具，用于开发机与安卓设备之间的通信，支持调试和应用安装。设备端 ADB 允许在设备上直接运行这些命令而无需主机电脑，使无需 root 的应用能够执行高级操作。尽管有用，但该功能曾被恶意软件利用，促使谷歌考虑进一步限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Android_Debug_Bridge">Android Debug Bridge</a></li>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge (adb) | Android Studio | Android Developers</a></li>
<li><a href="https://news.ycombinator.com/item?id=49045159">Android May Soon Restrict On-Device ADB - Hacker News</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一。一些用户认为该限制针对的已是低风险攻击向量（需开启开发者模式和远程 ADB），而另一些人则认为这是谷歌限制用户控制的更大趋势。少数开发者欢迎网络特定限制，但许多人担心这一变更会破坏合法的工作流。

**标签**: `#Android`, `#ADB`, `#security`, `#developer tools`, `#privacy`

---

<a id="item-4"></a>
## [开放权重 AI 迎来“Kubernetes 时刻”：平台转变信号](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

托比·克瑙普（Tobi Knaup）在近期文章中提出，开放权重 AI 模型正走与 Kubernetes 相同的发展轨迹，成为任何单一供应商都无法控制的基础性平台。 这标志着从封闭、供应商控制的 AI 模型向开放生态系统的转变，类似于 Kubernetes 如何使云基础设施民主化。这可能加速创新、降低成本，并使基于来源禁止模型等监管措施复杂化。 值得注意的要点包括：从技术上讲，无法根据权重区分模型来源；开放权重为推理定价提供了基准；美国实验室需要以宽松许可证发布有竞争力的开放权重模型。

hackernews · tknaup · 7月25日 14:49 · [社区讨论](https://news.ycombinator.com/item?id=49048034)

**背景**: 开放权重 AI 模型是指其训练参数（权重）公开可用的模型，任何人都可以下载、运行和定制。这与仅提供 API 访问的封闭模型形成对比。Kubernetes 是开源容器编排平台，已成为部署应用程序的行业标准，类比于开放权重 AI 可能成为 AI 工作负载的标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://allthings.how/what-is-an-open-weight-ai-model-and-how-to-use-one/">What is an Open Weight AI Model and How to Use One</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**社区讨论**: 评论者提出了关键观点：从技术上根椐权重禁止中国模型不可行（ozgung）；对开放平台超过单一供应商创新的观点表示赞赏（samizdis）；对 AI 代币定价的困惑以及开放权重如何提供合理性（firasd）；呼吁美国实验室发布更好的开放权重模型（drnick1）。总体情绪支持开放权重模型，但对监管和竞争存在担忧。

**标签**: `#open-weight AI`, `#artificial intelligence`, `#platform ecosystems`, `#AI regulation`, `#Kubernetes`

---

<a id="item-5"></a>
## [Claude Opus 5 发布：性能直逼 Fable 5 价格减半](https://simonwillison.net/2026/Jul/24/introducing-claude-opus-5/#atom-everything) ⭐️ 8.0/10

Anthropic 发布了 Claude Opus 5，这款新模型的智能水平几乎与旗舰模型 Fable 5 相当，但价格仅为其一半。目前它在 Artificial Analysis 排行榜上位居首位。 此次发布大幅降低了使用前沿 AI 能力的成本，可能加速在预算有限场景中的应用。同时也加剧了 AI 实验室之间以更低价格提供高性能模型的竞争。 Claude Opus 5 的定价与其前代 Opus 4.8 相同，并提供“快速模式”，成本为基础模型的两倍。它在发现网络安全漏洞方面有所提升，但未经过利用漏洞的训练，因此在漏洞利用方面仍落后于 Mythos 5 模型。

rss · Simon Willison · 7月24日 23:48

**背景**: Claude Opus 5 是 Anthropic 的最新模型，定位低于其旗舰产品 Fable 5。Fable 5 于 2026 年 6 月发布，是一款以自主工作和编程能力著称的“Mythos 级”模型。Artificial Analysis 排行榜根据质量、价格和速度对 AI 模型进行排名；Opus 5 目前位居榜首。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fable5.io/">Fable 5 AI — Independent Model Guide & Prompt Workspace</a></li>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>

</ul>
</details>

**标签**: `#AI`, `#Anthropic`, `#Claude`, `#large language models`, `#models`

---

<a id="item-6"></a>
## [AMD 2026 年 AI 战略旨在打破 NVIDIA 的 CUDA 护城河](https://newsletter.semianalysis.com/p/can-amd-break-the-cuda-moat-amd-advancing) ⭐️ 8.0/10

SemiAnalysis 的详细分析探讨了 AMD 通过新的硬件（如搭载 MI455X GPU 的 Helios 机架级系统）和软件创新（包括代理内核生成和改进的软件质量）来挑战 NVIDIA CUDA 主导地位的潜力。 如果 AMD 成功，它可能打破 NVIDIA 长期以来的 CUDA 护城河，使 AMD GPU 在 AI 工作负载中得到更广泛的应用，并加剧 AI 硬件市场的竞争。 Helios 系统连接了 72 个 MI455X GPU，每个配备 432GB HBM4，扩展带宽达 260 TB/s；同时 AMD 正在投资使用 LLM 的代理内核生成技术，自动优化 CUDA 内核，可能减少对 NVIDIA 生态系统的依赖。

rss · Semianalysis · 7月25日 00:33

**背景**: NVIDIA 的 CUDA 软件平台一直是其关键竞争优势，将开发者锁定在其生态系统中。AMD 有自己的 ROCm 软件，但历来在易用性和性能上落后。代理内核生成利用 AI 自动编写和优化 GPU 内核，这可能降低将 CUDA 代码移植到 AMD 硬件的门槛。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/amd-touts-instinct-mi430x-mi440x-and-mi455x-ai-accelerators-and-helios-rack-scale-ai-architecture-at-ces-full-mi400-series-family-fulfills-a-broad-range-of-infrastructure-and-customer-requirements">AMD touts Instinct MI430X, MI440X, and MI455X AI accelerators ...</a></li>
<li><a href="https://cuda-agent.github.io/">CUDA Agent | Large-Scale Agentic RL for CUDA Kernel Generation</a></li>

</ul>
</details>

**标签**: `#AMD`, `#CUDA`, `#AI hardware`, `#software ecosystem`, `#GPU competition`

---

<a id="item-7"></a>
## [离岸信托个税新规：装入财产及收益须申报纳税](https://liaoning.chinatax.gov.cn/art/2026/7/24/art_5869_7823.html) ⭐️ 8.0/10

2026 年 7 月 24 日，财政部与国家税务总局联合发布公告，明确居民个人将财产装入离岸信托及信托存续期间产生的收益，无论是否分配，均须按年申报缴纳 20%个人所得税。新规追溯至 2023 年，并要求在 90 天内补缴此前应缴未缴税款，不加收滞纳金。 该新规封堵了高净值个人通过离岸信托延迟或规避个人所得税的主要路径，对中国高净值人群和跨境资产管理架构产生重大影响。它与国际税收透明化和实质课税原则的趋势一致。 规则对所有环节（装入、存续、终止）的增值部分统一适用 20%固定税率，并消除了此前对未分配信托收益延迟纳税的漏洞。过渡期允许纳税人在 90 天内补缴 2023 年至 2025 年的应缴未缴税款，不加收滞纳金。

telegram · zaihuapd · 7月25日 00:31

**背景**: 离岸信托是在开曼群岛等低税率司法管辖区设立的法律安排，常被中国居民用于资产保护和税务筹划。在此公告发布前，中国对离岸信托的个税征管缺乏明确规定，导致部分居民将资产装入信托并累积收益而不申报，延迟或规避纳税义务。新规采用穿透原则，将信托视为税务透明实体，要求对所有收益按年征税。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.news.cn/politics/20260724/206e5905c9204c62a0fdb918dfd1bc5a/c.html">两部门明确离岸信托个税事项-新华网</a></li>
<li><a href="https://guangdong.chinatax.gov.cn/gdsw/wzjd/2026-07/24/content_7e6e11cde80941b9b4d1f424fc42b59c.shtml">财政部税政司 税务总局所得税司有关负责人就离岸信托个人所得税有关事项答记者问</a></li>
<li><a href="https://finance.china.com.cn/money/20260725/6317718.shtml">finance.china.com.cn/money/20260725/6317718.shtml</a></li>

</ul>
</details>

**标签**: `#离岸信托`, `#个人所得税`, `#税务合规`, `#中国税务`, `#信托新规`

---

<a id="item-8"></a>
## [上海携程商务因数据出境违规被罚 1000 万元](https://t.me/zaihuapd/42758) ⭐️ 8.0/10

2025 年 6 月 13 日，上海携程商务有限公司因未落实数据出境安全评估要求、违法出境个人信息，被上海市网信办罚款 1000 万元，并责令限期改正。企业已配合整改。 此次处罚彰显了中国对数据安全和个人信息保护法的严格执行，释放出跨境数据转移合规是强制要求的强烈信号。这突出表明监管机构对处理个人数据的互联网公司加强了审查，违规行为将面临严重的经济处罚。 罚款依据 2022 年 9 月 1 日起施行的《数据出境安全评估办法》。上海网信部门表示将持续加大对互联网企业违法跨境传输数据的执法力度。

telegram · zaihuapd · 7月25日 02:24

**背景**: 中国的《数据出境安全评估办法》要求数据处理者在向境外提供重要数据和个人信息前通过安全评估。《个人信息保护法》对跨境个人信息传输也规定了严格条件。企业需根据数据量和敏感度进行自评估、签订标准合同或通过政府安全评估。上海携程案是这些规则下首批高调执法行动之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gov.cn/zhengce/zhengceku/2022-07/08/content_5699851.htm">数据出境安全评估办法_国务院部门文件_中国政府网</a></li>
<li><a href="https://www.cac.gov.cn/2025-06/27/c_1752652339765002.htm">国家互联网信息办公室发布《数据出境安全评估申报指南（第三版）》_中...</a></li>

</ul>
</details>

**标签**: `#data security`, `#regulation`, `#personal information`, `#cross-border data`, `#China`

---