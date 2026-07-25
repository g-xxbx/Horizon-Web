---
layout: default
title: "Horizon Summary: 2026-07-25 (EN)"
date: 2026-07-25
lang: en
---

> From 25 items, 8 important content pieces were selected

---

1. [SGLang v0.5.16: DSPark Speculative Decoding and Inkling Support](#item-1) ⭐️ 10.0/10
2. [vLLM v0.26.0 adds Inkling model family and DeepSeek-V4 optimizations](#item-2) ⭐️ 8.0/10
3. [Android May Restrict On-Device ADB Access](#item-3) ⭐️ 8.0/10
4. [Open-weight AI's 'Kubernetes moment' signals platform shift](#item-4) ⭐️ 8.0/10
5. [Claude Opus 5 Launches, Rivals Fable 5 at Half Price](#item-5) ⭐️ 8.0/10
6. [AMD's AI 2026 Strategy Aims to Break NVIDIA's CUDA Moat](#item-6) ⭐️ 8.0/10
7. [China Issues Offshore Trust Tax Rules: Annual Gains Taxed at 20%](#item-7) ⭐️ 8.0/10
8. [Shanghai Ctrip Business Company fined ¥10 million for data export violations](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [SGLang v0.5.16: DSPark Speculative Decoding and Inkling Support](https://github.com/sgl-project/sglang/releases/tag/v0.5.16) ⭐️ 10.0/10

SGLang v0.5.16 introduces DSPark confidence-driven speculative decoding and support for the 975B-parameter Inkling multimodal model. This release significantly enhances AI inference speed and scale, enabling efficient deployment of large language and multimodal models, and showcases advances in speculative decoding techniques. DSPark achieves 383.7 tok/s on DeepSeek-V4-Pro with TP8 on B300, while Inkling features a 1M-token context and mixed attention mechanisms.

github · Qiaolin-Yu · Jul 25, 00:13

**Background**: Speculative decoding accelerates LLM inference by using a draft model to propose multiple tokens that are verified in parallel by the target model. SGLang is a framework for efficient serving of large language and multimodal models. The DSPark algorithm introduced in this release uses confidence scores to dynamically adjust the verification window.

<details><summary>References</summary>
<ul>
<li><a href="https://www.alphaxiv.org/abs/2026.dspark">DSpark : Confidence -Scheduled Speculative Decoding ... | alphaXiv</a></li>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://en.wikipedia.org/wiki/Speculative_decoding">Speculative decoding</a></li>

</ul>
</details>

**Tags**: `#speculative decoding`, `#AI inference`, `#SGLang`, `#DeepSeek-V4`, `#Blackwell`

---

<a id="item-2"></a>
## [vLLM v0.26.0 adds Inkling model family and DeepSeek-V4 optimizations](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 was released with 411 commits, featuring full support for the Inkling model family (including piecewise CUDA graphs, NVFP4 quantization, LoRA, and speculative decoding), significant performance optimizations for DeepSeek-V4, and maturation of the KV offloading system. This release enhances vLLM's capability to serve cutting-edge multimodal MoE models like Inkling and DeepSeek-V4 efficiently, which is crucial for the LLM serving ecosystem as these large models require optimized inference to be practical. Notable technical details include piecewise CUDA graph support for flexible graph capture, NVFP4 quantization for reduced memory usage, fp32 lm_head via head_dtype for improved accuracy, and per-KV-cache-group attention backend selection for hybrid models.

github · khluu · Jul 25, 10:38

**Background**: vLLM is an open-source high-throughput LLM serving engine using PagedAttention and continuous batching. The Inkling model family by Thinking Machines Lab includes a large multimodal MoE model with 975B total parameters. Piecewise CUDA graphs allow parts of the model that are incompatible with full graph capture to remain eager while still benefiting from graph optimization.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling : Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://docs.vllm.ai/en/stable/design/cuda_graphs/">CUDA Graphs - vLLM Documentation</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#release`, `#model serving`, `#deepseek`, `#performance`

---

<a id="item-3"></a>
## [Android May Restrict On-Device ADB Access](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/) ⭐️ 8.0/10

A proposed Android update may restrict on-device ADB access, preventing apps from using ADB commands locally without a connected computer. This could affect tools like Shizuku and libadb that rely on this feature for rootless operations. This change could significantly impact Android developers and power users who depend on on-device ADB for debugging, automation, and device management. It underscores the ongoing trade-off between enhancing device security and preserving user flexibility. The proposal likely requires explicit user consent for each on-device ADB connection or restricts access to specific network interfaces. Similar past measures include RSA authentication and device whitelisting to mitigate malware risks.

hackernews · shscs911 · Jul 25, 06:57 · [Discussion](https://news.ycombinator.com/item?id=49045159)

**Background**: Android Debug Bridge (ADB) is a command-line tool that enables communication between a development machine and an Android device for debugging and app installation. On-device ADB allows these commands to run directly on the device without a host computer, empowering rootless apps to perform advanced tasks. While useful, this feature has been exploited by malware, prompting Google to consider further restrictions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Android_Debug_Bridge">Android Debug Bridge</a></li>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge (adb) | Android Studio | Android Developers</a></li>
<li><a href="https://news.ycombinator.com/item?id=49045159">Android May Soon Restrict On-Device ADB - Hacker News</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed. Some users argue the restriction targets an already low-risk vector (requiring developer mode and remote ADB enabled), while others see it as part of Google's broader trend to limit control. A few developers welcome network-specific restrictions, but many fear the change will break legitimate workflows.

**Tags**: `#Android`, `#ADB`, `#security`, `#developer tools`, `#privacy`

---

<a id="item-4"></a>
## [Open-weight AI's 'Kubernetes moment' signals platform shift](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

In a recent article, Tobi Knaup argues that open-weight AI models are following the same trajectory as Kubernetes, becoming an indispensable platform that no single vendor can control. This matters because it signals a shift away from closed, vendor-controlled AI models toward open ecosystems, similar to how Kubernetes democratized cloud infrastructure. This could accelerate innovation, reduce costs, and complicate regulation such as banning models by origin. Notable points include the impossibility of technically distinguishing models by origin based on weights, the role of open weights in providing a baseline for inference pricing, and the need for American labs to release competitive open-weight models under permissive licenses.

hackernews · tknaup · Jul 25, 14:49 · [Discussion](https://news.ycombinator.com/item?id=49048034)

**Background**: Open-weight AI models are those whose trained parameters (weights) are publicly available, enabling anyone to download, run, and customize them. This contrasts with closed models where only API access is provided. Kubernetes is the open-source container orchestration platform that became the industry standard for deploying applications, analogous to what open-weight AI could become for AI workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://allthings.how/what-is-an-open-weight-ai-model-and-how-to-use-one/">What is an Open Weight AI Model and How to Use One</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**Discussion**: Commenters raised key points: technical infeasibility of banning Chinese models based on weights (ozgung), praise for the idea that open platforms out-innovate single vendors (samizdis), confusion over AI token pricing and how open weights can provide sanity (firasd), and a call for American labs to release better open-weight models (drnick1). Overall sentiment is supportive of open-weight models but with concerns about regulation and competition.

**Tags**: `#open-weight AI`, `#artificial intelligence`, `#platform ecosystems`, `#AI regulation`, `#Kubernetes`

---

<a id="item-5"></a>
## [Claude Opus 5 Launches, Rivals Fable 5 at Half Price](https://simonwillison.net/2026/Jul/24/introducing-claude-opus-5/#atom-everything) ⭐️ 8.0/10

Anthropic has released Claude Opus 5, a new model that nearly matches the intelligence of their flagship Fable 5 model at half the price. It currently tops the Artificial Analysis leaderboard. This release significantly lowers the cost of accessing frontier AI capabilities, potentially accelerating adoption in budget-constrained applications. It also intensifies competition among AI labs to deliver high performance at lower prices. Claude Opus 5 is priced the same as its predecessor Opus 4.8 and offers a "fast mode" at double the base cost. It has improved at finding cybersecurity vulnerabilities but has not been trained to exploit them, keeping it behind the Mythos 5 model in exploitation.

rss · Simon Willison · Jul 24, 23:48

**Background**: Claude Opus 5 is the latest model from Anthropic, positioned below their flagship Fable 5. Fable 5, released in June 2026, is a "Mythos-class" model known for autonomous work and coding. The Artificial Analysis leaderboard ranks AI models by quality, price, and speed; Opus 5 currently leads it.

<details><summary>References</summary>
<ul>
<li><a href="https://fable5.io/">Fable 5 AI — Independent Model Guide & Prompt Workspace</a></li>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Anthropic`, `#Claude`, `#large language models`, `#models`

---

<a id="item-6"></a>
## [AMD's AI 2026 Strategy Aims to Break NVIDIA's CUDA Moat](https://newsletter.semianalysis.com/p/can-amd-break-the-cuda-moat-amd-advancing) ⭐️ 8.0/10

A detailed analysis from SemiAnalysis examines AMD's potential to challenge NVIDIA's CUDA dominance through new hardware like the Helios rack-scale system with MI455X GPUs and software innovations including agentic kernel generation and improved software quality. If AMD succeeds, it could break NVIDIA's long-standing CUDA moat, enabling broader adoption of AMD GPUs for AI workloads and intensifying competition in the AI hardware market. The Helios system connects 72 MI455X GPUs with 432GB HBM4 each and 260 TB/s scale-up bandwidth, while AMD is also investing in agentic kernel generation using LLMs to automatically optimize CUDA kernels, potentially reducing dependence on NVIDIA's ecosystem.

rss · Semianalysis · Jul 25, 00:33

**Background**: NVIDIA's CUDA software platform has been a key competitive advantage, locking developers into its ecosystem. AMD has its own ROCm software, but it has historically lagged in usability and performance. Agentic kernel generation uses AI to automatically write and optimize GPU kernels, which could lower the barrier for porting CUDA code to AMD hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/amd-touts-instinct-mi430x-mi440x-and-mi455x-ai-accelerators-and-helios-rack-scale-ai-architecture-at-ces-full-mi400-series-family-fulfills-a-broad-range-of-infrastructure-and-customer-requirements">AMD touts Instinct MI430X, MI440X, and MI455X AI accelerators ...</a></li>
<li><a href="https://cuda-agent.github.io/">CUDA Agent | Large-Scale Agentic RL for CUDA Kernel Generation</a></li>

</ul>
</details>

**Tags**: `#AMD`, `#CUDA`, `#AI hardware`, `#software ecosystem`, `#GPU competition`

---

<a id="item-7"></a>
## [China Issues Offshore Trust Tax Rules: Annual Gains Taxed at 20%](https://liaoning.chinatax.gov.cn/art/2026/7/24/art_5869_7823.html) ⭐️ 8.0/10

On July 24, 2026, China's Ministry of Finance and State Taxation Administration jointly issued a bulletin specifying that resident individuals must report and pay a 20% tax on property transferred into offshore trusts and on annual trust gains, regardless of distribution. The rules apply retroactively to property transfers from 2023 and require a 90-day period to settle any previously unpaid taxes without late fees. This regulation closes a major loophole used by wealthy individuals to defer or avoid personal income tax through offshore trusts, significantly impacting high-net-worth Chinese residents and cross-border asset management structures. It aligns with global trends of tax transparency and substance-over-form principles. The rules apply a flat 20% tax rate on gains (market value minus cost) at all stages—transfer, operation, and liquidation—and eliminate the previous practice of deferring tax on undistributed trust income. A transition period allows taxpayers to rectify outstanding liabilities for 2023–2025 within 90 days without penalties.

telegram · zaihuapd · Jul 25, 00:31

**Background**: Offshore trusts are legal arrangements established in low-tax jurisdictions (e.g., Cayman Islands) commonly used by Chinese residents for asset protection and tax planning. Prior to this bulletin, China lacked specific rules on the taxation of offshore trusts, prompting some individuals to contribute assets and accumulate income without reporting, deferring or avoiding tax liabilities. The new rules adopt a look-through principle, treating the trust as transparent for tax purposes and requiring annual taxation of all gains.

<details><summary>References</summary>
<ul>
<li><a href="https://www.news.cn/politics/20260724/206e5905c9204c62a0fdb918dfd1bc5a/c.html">两部门明确离岸信托个税事项-新华网</a></li>
<li><a href="https://guangdong.chinatax.gov.cn/gdsw/wzjd/2026-07/24/content_7e6e11cde80941b9b4d1f424fc42b59c.shtml">财政部税政司 税务总局所得税司有关负责人就离岸信托个人所得税有关事项答记者问</a></li>
<li><a href="https://finance.china.com.cn/money/20260725/6317718.shtml">finance.china.com.cn/money/20260725/6317718.shtml</a></li>

</ul>
</details>

**Tags**: `#离岸信托`, `#个人所得税`, `#税务合规`, `#中国税务`, `#信托新规`

---

<a id="item-8"></a>
## [Shanghai Ctrip Business Company fined ¥10 million for data export violations](https://t.me/zaihuapd/42758) ⭐️ 8.0/10

Shanghai Ctrip Business Company was fined 10 million yuan by the Shanghai Cyberspace Administration on June 13, 2025 for failing to comply with data export security assessment requirements and illegally exporting personal information. The company has cooperated with the rectification. This penalty demonstrates China's stringent enforcement of its data security and personal information protection laws, sending a strong signal that cross-border data transfer compliance is mandatory. It highlights the increased regulatory scrutiny on internet companies handling personal data and the severe financial consequences of non-compliance. The fine was issued under the Data Export Security Assessment Measures, which took effect on September 1, 2022. The Shanghai cyberspace authorities indicated they will continue to intensify enforcement against illegal cross-border data transfers in internet enterprises.

telegram · zaihuapd · Jul 25, 02:24

**Background**: China's Data Export Security Assessment Measures require data processors to undergo a security assessment before transferring important data or personal information abroad. The Personal Information Protection Law also imposes strict conditions on cross-border personal information transfers. Companies must conduct a self-assessment, sign standard contracts, or pass a government security assessment depending on the data volume and sensitivity. The Shanghai Ctrip case is one of the first high-profile enforcement actions under these rules.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gov.cn/zhengce/zhengceku/2022-07/08/content_5699851.htm">数据出境安全评估办法_国务院部门文件_中国政府网</a></li>
<li><a href="https://www.cac.gov.cn/2025-06/27/c_1752652339765002.htm">国家互联网信息办公室发布《数据出境安全评估申报指南（第三版）》_中...</a></li>

</ul>
</details>

**Tags**: `#data security`, `#regulation`, `#personal information`, `#cross-border data`, `#China`

---