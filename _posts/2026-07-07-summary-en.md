---
layout: default
title: "Horizon Summary: 2026-07-07 (EN)"
date: 2026-07-07
lang: en
---

> From 38 items, 14 important content pieces were selected

---

1. [MIRA: 5B-Parameter World Model for Multiplayer Rocket League](#item-1) ⭐️ 9.0/10
2. [OpenWrt One: First Official Open Hardware Router](#item-2) ⭐️ 8.0/10
3. [GLM 5.2 and the Coming AI Margin Collapse](#item-3) ⭐️ 8.0/10
4. [Ternlight: 7MB Embedding Model Runs in Browser via WASM](#item-4) ⭐️ 8.0/10
5. [Anthropic Finds Global Workspace in Language Models](#item-5) ⭐️ 8.0/10
6. [Microsoft Reshapes Xbox Division to Boost Profit Margins](#item-6) ⭐️ 8.0/10
7. [Tencent Releases Hy3: 295B MoE Model Under Apache 2.0](#item-7) ⭐️ 8.0/10
8. [Nvidia GPU Debt Backstop Fuels $7T AI Infrastructure Boom](#item-8) ⭐️ 8.0/10
9. [LingBot-Vision: Masked Boundary Modeling for Self-Supervised Learning](#item-9) ⭐️ 8.0/10
10. [TRACE: Open-Source Hierarchical Memory Boosts LLM Agents](#item-10) ⭐️ 8.0/10
11. [SpaceX Falcon 9 reentry creates lithium plume in upper atmosphere](#item-11) ⭐️ 8.0/10
12. [Elon Musk Dissolves xAI, Rebrands as SpaceXAI](#item-12) ⭐️ 8.0/10
13. [China Plans $295B National Computing Network Over 5 Years](#item-13) ⭐️ 8.0/10
14. [New-API Fixes Billing Bug: Oversized Parameters Cause Negative Charges](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [MIRA: 5B-Parameter World Model for Multiplayer Rocket League](https://www.reddit.com/r/MachineLearning/comments/1upofuw/mira_multiplayer_interactive_world_models_trained/) ⭐️ 9.0/10

MIRA is a 5-billion-parameter world model trained on 10,000 hours of synthetic Rocket League data, enabling interactive 4-player simulation at 20 frames per second on a single NVIDIA B200 GPU. The team released a playable online demo, a technical report, and a 1,000-hour dataset of 4-player gameplay. This is a groundbreaking step toward large-scale interactive world models for multiplayer games, potentially transforming game AI, simulation, and reinforcement learning research. The open-source release of code, dataset, and model lowers the barrier for further innovation in world modeling. The model runs at 20 fps for 4 players on a single B200 GPU, which features 180 GB HBM3e memory and a 1000 W power draw. The synthetic dataset was generated using Rocket League replays and the game's stats API.

reddit · r/MachineLearning · /u/MasterScrat · Jul 7, 07:59

**Background**: A world model in AI is a machine learning system that builds an internal representation of an environment and predicts how it changes in response to actions. Rocket League is a popular vehicular soccer video game that provides rich, continuous state-action data ideal for training such models. The NVIDIA B200 is a high-end GPU based on the Blackwell architecture, designed for AI workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/dgx-b200/">DGX B200: The Foundation for Your AI Factory | NVIDIA</a></li>
<li><a href="https://www.techpowerup.com/gpu-specs/b200.c4210">NVIDIA B200 Specs | TechPowerUp GPU Database</a></li>

</ul>
</details>

**Tags**: `#world models`, `#reinforcement learning`, `#multiplayer`, `#Rocket League`, `#open-source`

---

<a id="item-2"></a>
## [OpenWrt One: First Official Open Hardware Router](https://openwrt.org/toh/openwrt/one) ⭐️ 8.0/10

The OpenWrt One, the first official open hardware router board from the OpenWrt community, has been released at $89. It features a MediaTek MT7981B SoC, dual-band Wi-Fi 6, PoE, and a mikroBUS expansion header. This device marks a milestone for open-source networking, providing a fully community-supported, unbrickable router that prioritizes user control and repairability. It could encourage wider adoption of OpenWrt and inspire similar open hardware initiatives. The OpenWrt One is designed to be unbrickable with a hardware switch to separately flash NOR and NAND flash memory. It includes two Ethernet ports, three USB ports, and runs OpenWrt by default, with the ability to run other OS like Debian.

hackernews · peter_d_sherman · Jul 6, 18:23 · [Discussion](https://news.ycombinator.com/item?id=48808482)

**Background**: OpenWrt is an open-source Linux distribution for embedded devices, widely used to replace manufacturer firmware on routers for enhanced features and longevity. The OpenWrt One is the first official hardware board developed by the OpenWrt community itself, in collaboration with Banana Pi and the Software Freedom Conservancy.

<details><summary>References</summary>
<ul>
<li><a href="https://openwrt.org/toh/openwrt/one">[OpenWrt Wiki] OpenWrt One</a></li>
<li><a href="https://www.tomshardware.com/networking/open-source-openwrt-one-router-released-at-usd89-hacker-friendly-device-sports-two-ethernet-ports-three-usb-ports-with-dual-band-wi-fi-6">Open-source OpenWrt One router released at $89 — 'hacker ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenWrt">OpenWrt - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments are generally positive, with users expressing excitement about the open hardware approach and the upcoming OpenWrt Two with Wi-Fi 7. Some users note that OpenWrt installation can be complex, but appreciate the project's longevity and the ability to extend router life.

**Tags**: `#openwrt`, `#open hardware`, `#router`, `#networking`, `#open source`

---

<a id="item-3"></a>
## [GLM 5.2 and the Coming AI Margin Collapse](https://martinalderson.com/posts/the-upcoming-ai-margin-collapse-part-1-glm-5-2/) ⭐️ 8.0/10

Martin Alderson argues that open-weight models like GLM 5.2, which competes with proprietary models at 15-20% of the price, will drive AI inference margins to zero, mirroring past commoditization in cloud and software. If margins collapse, the current high-cost AI business models of major providers may become unsustainable, potentially reshaping the entire AI ecosystem and accelerating adoption of open-source alternatives. GLM 5.2 is Z.AI's flagship model with a 1M-token context, capable of long-horizon tasks like mini-program development, and is available as open weights on Hugging Face and Ollama.

hackernews · martinald · Jul 6, 20:14 · [Discussion](https://news.ycombinator.com/item?id=48809877)

**Background**: The AI industry currently sees high margins for proprietary models like GPT-4 and Claude, but open-weight models have historically driven down prices in other tech sectors. GLM 5.2 represents a new wave of capable open models that could disrupt this pricing power.

<details><summary>References</summary>
<ul>
<li><a href="https://martinalderson.com/posts/the-upcoming-ai-margin-collapse-part-1-glm-5-2/">GLM 5.2 and the coming AI margin collapse (part 1) - Martin Alderson</a></li>
<li><a href="https://huggingface.co/zai-org/GLM-5.2">zai-org/GLM-5.2 · Hugging Face</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM-5.2 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some argue that raw cost doesn't guarantee market dominance (citing examples like cloud and office suites), while others find current AI costs already negligible for their use cases. Some users are already switching to cheaper open models via APIs like OpenRouter.

**Tags**: `#AI`, `#economics`, `#open-source`, `#commoditization`, `#GLM`

---

<a id="item-4"></a>
## [Ternlight: 7MB Embedding Model Runs in Browser via WASM](https://ternlight-demo.vercel.app/) ⭐️ 8.0/10

Ternlight is a 7MB embedding model distilled from MiniLM with ternary quantization, running entirely in the browser via Rust/WASM SIMD for efficient semantic similarity computation. This enables practical client-side semantic search without server calls, preserving user privacy and reducing latency, which is significant for privacy-sensitive applications and offline-capable web tools. The model outputs 384-dimensional embeddings and uses ternary quantization-aware training to shrink size while maintaining quality; the inference engine is written from scratch in Rust and compiled to WebAssembly with SIMD instructions.

hackernews · soycaporal · Jul 6, 23:06 · [Discussion](https://news.ycombinator.com/item?id=48811644)

**Background**: Embedding models convert text into numerical vectors that capture semantic meaning, enabling similarity search. Traditional models are too large for browser use; Ternlight uses ternary quantization (weights restricted to -1, 0, +1) and WebAssembly SIMD to achieve a tiny footprint and fast CPU inference.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2303.01505">[2303.01505] Ternary Quantization: A Survey</a></li>
<li><a href="https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2">sentence-transformers/all-MiniLM-L6-v2 · Hugging Face</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/WebAssembly/Reference/SIMD">WebAssembly SIMD-specific instructions - WebAssembly | MDN</a></li>

</ul>
</details>

**Discussion**: Commenters praised the project for its novelty and practical value, with suggestions for integration with DuckDB HNSW search and local privacy-preserving search. One user noted the demo page's sudden CPU spike was startling, suggesting a button to trigger the demo.

**Tags**: `#embedding models`, `#WASM`, `#quantization`, `#browser ML`, `#semantic search`

---

<a id="item-5"></a>
## [Anthropic Finds Global Workspace in Language Models](https://www.anthropic.com/research/global-workspace) ⭐️ 8.0/10

Anthropic's research identifies a small cluster of internal patterns in Claude, termed the 'J-space', that functions as a global workspace, enabling coherent reasoning across contexts. This discovery provides a mechanistic understanding of how language models maintain coherence and perform higher-order reasoning, bridging AI research with cognitive science concepts like global workspace theory. The J-space is not involved in most routine tasks like fluent speech or fact recall; when Claude is prevented from using it, it loses higher-order cognitive functions but otherwise behaves normally.

hackernews · in-silico · Jul 6, 17:44 · [Discussion](https://news.ycombinator.com/item?id=48808002)

**Background**: Global workspace theory, originally from neuroscience, proposes that conscious thought integrates information from various brain modules into a unified workspace. Anthropic's research applies this concept to AI, showing that language models may have an analogous internal mechanism that integrates information across layers for coherent reasoning.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/global-workspace">A global workspace in language models \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Global_workspace_theory">Global workspace theory - Wikipedia</a></li>
<li><a href="https://www.lesswrong.com/posts/3PaLrzxagpbnNtPLT/a-global-workspace-in-language-models">A global workspace in language models</a></li>

</ul>
</details>

**Discussion**: Commenters noted parallels to prior experiments, such as duplicating math-solving layers to improve performance, and debated whether the J-space truly resembles conscious awareness. Some suggested the findings align with expectations from training dynamics, while others called for more direct comparisons to human cognition.

**Tags**: `#AI research`, `#language models`, `#Anthropic`, `#model internals`, `#neural networks`

---

<a id="item-6"></a>
## [Microsoft Reshapes Xbox Division to Boost Profit Margins](https://news.xbox.com/en-us/2026/07/06/resetting-xbox/) ⭐️ 8.0/10

Microsoft announced a major restructuring of its Xbox division, aiming to address thin profit margins despite generating $5 billion in quarterly revenue. The move includes trimming operations and potentially spinning off studios to return to growth. This restructuring signals a strategic shift for Xbox, moving away from aggressive Game Pass expansion and acquisitions toward profitability, which could reshape the console wars and impact the broader gaming industry's focus on sustainable business models. The division generates about $5 billion in quarterly revenue but only $150-160 million in profit, indicating a thin and non-growing margin. CEO Asha reportedly blamed corporate management for past missteps and aims to let studios return to independence where possible.

hackernews · dijksterhuis · Jul 6, 14:18 · [Discussion](https://news.ycombinator.com/item?id=48804993)

**Background**: Xbox has been a major player in the gaming console market alongside Sony and Nintendo. In recent years, Microsoft invested heavily in Game Pass subscriptions and studio acquisitions (e.g., Bethesda, Activision Blizzard) to compete, but these strategies have not translated into proportional profit growth.

**Discussion**: Commenters expressed mixed reactions: some criticized Microsoft's inability to manage gaming as an art form, while others noted that Nintendo's success with simpler games contrasts with Xbox's focus on cinematic blockbusters. Several users expressed sympathy for laid-off employees and blamed former head Phil Spencer for poor strategic decisions.

**Tags**: `#Xbox`, `#Microsoft`, `#gaming industry`, `#corporate strategy`, `#profitability`

---

<a id="item-7"></a>
## [Tencent Releases Hy3: 295B MoE Model Under Apache 2.0](https://simonwillison.net/2026/Jul/6/hy3/#atom-everything) ⭐️ 8.0/10

Tencent has released Hy3, a 295B-parameter Mixture-of-Experts (MoE) language model with 21B active parameters and 3.8B MTP layer parameters, under the permissive Apache 2.0 license. It is available for free on OpenRouter until July 21st, 2026. Hy3 outperforms similar-size models and rivals flagship open-source models with 2-5x parameters, making it a significant addition to the open-source AI ecosystem. Its Apache 2.0 license and free availability lower barriers for developers and researchers. The full model is 598GB on Hugging Face, with an FP8 quantized version at 300GB, and supports a 256K context length. The model was developed by Tencent's Hy Team and incorporates feedback from over 50 products during its preview phase.

rss · Simon Willison · Jul 6, 23:57

**Background**: Mixture-of-Experts (MoE) is a machine learning technique where multiple specialized sub-networks (experts) are activated per input, enabling efficient scaling with less compute than dense models. Hy3 uses a gating mechanism to route tokens to relevant experts, achieving high performance with only 21B active parameters out of 295B total. MTP (Multi-Token Prediction) is an auxiliary head that predicts multiple future tokens simultaneously, improving inference speed.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-source`, `#LLM`, `#MoE`, `#Tencent`

---

<a id="item-8"></a>
## [Nvidia GPU Debt Backstop Fuels $7T AI Infrastructure Boom](https://newsletter.semianalysis.com/p/nvidia-gpu-debt-backstop-unleashes) ⭐️ 8.0/10

Nvidia has launched a 6-year GPU backstop program that guarantees minimum revenue for neocloud GPU clusters and datacenter leases, aiming to unlock debt financing for AI compute buildouts projected to reach $7.1 trillion by 2029. This mechanism broadens compute access beyond hyperscalers and large AI labs, enabling neoclouds to grow and accelerating AI infrastructure deployment. It also shifts the risk from lenders to Nvidia, potentially reshaping the financing landscape for AI. The program requires assembling the 'AI Project Trinity' of capital, offtake, and datacenters. Lenders currently demand an offtake contract or a backstop from an investment-grade hyperscaler before providing debt financing.

rss · Semianalysis · Jul 6, 21:53

**Background**: Historically, AI buildouts were primarily cashflow-funded by hyperscalers like Google, Amazon, Meta, and Microsoft. Over the past year, even these giants have turned to debt. Nvidia's backstop aims to fill the funding gap for neoclouds, which lack the credit ratings to secure loans independently.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/nvidia-gpu-debt-backstop-unleashes">Nvidia GPU Debt Backstop Unleashes the AI Project Trinity ...</a></li>
<li><a href="https://www.newsbang.com/news/article/story_id-p008-154842">Nvidia Launches 6-Year GPU Backstop Program to Unlock AI ...</a></li>
<li><a href="https://digg.com/tech/finswqcv">SemiAnalysis CEO Dylan Patel projects AI debt financing will exceed...</a></li>

</ul>
</details>

**Discussion**: Some critics warn that the $7 trillion AI debt and capex forecasts could fuel an unsustainable bubble, comparing it to past financial crises. Others distrust the analysts behind the projections.

**Tags**: `#Nvidia`, `#AI infrastructure`, `#debt financing`, `#neocloud`, `#datacenter economics`

---

<a id="item-9"></a>
## [LingBot-Vision: Masked Boundary Modeling for Self-Supervised Learning](https://www.reddit.com/r/MachineLearning/comments/1up4cjh/lingbotvision_masked_boundary_modeling_for/) ⭐️ 8.0/10

LingBot-Vision introduces masked boundary modeling, where a teacher network generates a dense boundary field and forces the student to reconstruct boundary regions, achieving 0.296 RMSE on NYUv2 linear-probe depth estimation with a 1.1B parameter model, outperforming DINOv3-7B (0.309 RMSE) at a fraction of the parameters. This work demonstrates that explicitly guiding self-supervised learning to focus on boundary regions can yield more efficient and effective visual representations, potentially reducing the need for massive models and data in downstream tasks like depth estimation and segmentation. The method uses per-pixel categorical distributions for boundary fields to avoid collapse under EMA teacher, and applies an a-contrario validation test to filter decoded segments. The model was trained on 161M images (less than one-third of DINOv3's data) and shows consistent gains in encoder initialization studies, though ImageNet classification and ADE20K segmentation still trail DINOv3.

reddit · r/MachineLearning · /u/StillThese3747 · Jul 6, 17:37

**Background**: Self-supervised learning (SSL) aims to learn useful representations from unlabeled data. Masked image modeling (MIM) is a popular SSL paradigm where parts of an image are masked and the model must reconstruct them. DINOv3 is a state-of-the-art SSL method that uses self-distillation and has shown strong performance on various vision tasks. LingBot-Vision builds on these ideas by explicitly masking boundary regions predicted by the teacher.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2401.00897">[2401.00897] Masked Modeling for Self-supervised ... - arXiv.org</a></li>
<li><a href="https://www.catalyzex.com/s/Nyuv2">Nyuv 2</a></li>
<li><a href="https://centreborelli.ens-paris-saclay.fr/en/node/3050">CLOUD DETECTION BY INTER-BAND PARALLAX AND A-CONTRARIO VALIDATION</a></li>

</ul>
</details>

**Discussion**: The community discussion is limited but notes that the NYUv2 RMSE improvement of 0.013 is within the range that could be affected by probe hyperparameters, and the lack of ablation against hard-masking baselines like ADIOS/AttMask is a concern. The author acknowledges that DINOv3's Gram anchoring is still needed, suggesting boundary forcing is complementary rather than a replacement.

**Tags**: `#self-supervised learning`, `#computer vision`, `#representation learning`, `#depth estimation`, `#ViT`

---

<a id="item-10"></a>
## [TRACE: Open-Source Hierarchical Memory Boosts LLM Agents](https://www.reddit.com/r/MachineLearning/comments/1uoz5jo/trace_opensource_hierarchical_memory_for_llm/) ⭐️ 8.0/10

TRACE is an open-source hierarchical memory system for LLM agents that organizes conversation history into a topic tree with branches and summaries, achieving 82.5% F1 on MemoryAgentBench's EventQA task using the gpt-oss-20B model. This demonstrates that a hierarchical memory approach can significantly outperform flat RAG-based methods (e.g., Mem0 at 37.5% and MemGPT at 26.2%) even with a smaller open-weight model, making advanced memory capabilities more accessible and cost-effective. The benchmark used gpt-oss-20B locally, not an apples-to-apples comparison with the same backbone; the author noted that Mem0's fact-extraction step requires strict JSON output which gpt-oss couldn't parse cleanly, and Letta requires a full server setup.

reddit · r/MachineLearning · /u/PsychologicalDot7749 · Jul 6, 14:35

**Background**: LLM agents often struggle with long-term memory, relying on flat retrieval-augmented generation (RAG) that treats all past interactions equally. Hierarchical memory systems like TRACE organize information into a topic tree, enabling more efficient retrieval and context understanding. MemoryAgentBench is a benchmark suite for evaluating LLM agent memory, with EventQA focusing on temporal event reasoning.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2506.07398">[2506.07398] G-Memory: Tracing Hierarchical Memory for Multi ... H-MEM: Hierarchical Memory for High-Efficiency Long-Term ... H-MEM: Hierarchical Memory for High-Efficiency Long-Term ... H-MEM: Hierarchical Memory for High-Efciency Long-Term ... TeleAI-UAGI/Awesome-Agent-Memory - GitHub IAAR-Shanghai/Awesome-AI-Memory - GitHub G-Memory: Tracing Hierarchical Memory for Multi-Agent Systems</a></li>
<li><a href="https://github.com/HUST-AI-HYZ/MemoryAgentBench">GitHub - HUST-AI-HYZ/ MemoryAgentBench : Open source code for...</a></li>
<li><a href="https://openai.com/index/introducing-gpt-oss/">Introducing gpt-oss - OpenAI</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion praised the work for its novel approach and strong results, with some users questioning the fairness of comparing against closed-source models on different backbones. The author acknowledged the limitation and provided full JSON logs for transparency.

**Tags**: `#LLM`, `#memory`, `#open-source`, `#benchmark`, `#agents`

---

<a id="item-11"></a>
## [SpaceX Falcon 9 reentry creates lithium plume in upper atmosphere](https://t.me/zaihuapd/42387) ⭐️ 8.0/10

A Nature Communications study directly measured a lithium pollution plume from the uncontrolled reentry of a SpaceX Falcon 9 upper stage over Europe on February 19, 2025, using lidar at 96 km altitude, where lithium levels spiked 10-fold. This is the first direct detection of metal pollution from rocket reentry, highlighting a new environmental concern for the rapidly growing space industry as rocket launches increase. The plume was observed for 27 minutes and traced back to the Falcon 9 upper stage's uncontrolled reentry path; the study was published in Communications Earth & Environment on February 19, 2026.

telegram · zaihuapd · Jul 6, 11:17

**Background**: Rocket upper stages often reenter the atmosphere uncontrolled, burning up and releasing metals like lithium, aluminum, and copper. Lithium is used in rocket fuel and battery alloys. Lidar (light detection and ranging) uses laser pulses to detect atmospheric particles.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nature.com/articles/s43247-025-03154-8">Measurement of a lithium plume from the uncontrolled re-entry of a Falcon 9 rocket | Communications Earth & Environment</a></li>
<li><a href="https://www.sciencenews.org/article/rocket-reentry-metal-pollution-detected">Metal pollution from a rocket reentry detected for the first time</a></li>
<li><a href="https://gizmodo.com/study-confirms-reentering-spacex-rockets-are-peppering-the-upper-atmosphere-with-metal-pollution-2000723932">Study Confirms: Reentering SpaceX Rockets Are Peppering the Upper...</a></li>

</ul>
</details>

**Tags**: `#space pollution`, `#SpaceX`, `#atmospheric science`, `#environmental impact`, `#rocket reentry`

---

<a id="item-12"></a>
## [Elon Musk Dissolves xAI, Rebrands as SpaceXAI](https://x.com/i/status/2074214064746832060) ⭐️ 8.0/10

Elon Musk announced the dissolution of xAI as an independent company, rebranding it as SpaceXAI and merging it into SpaceX. The announcement was made on May 6, 2026, following SpaceX's acquisition of xAI in February 2026. This consolidation marks a significant shift in the AI landscape, as xAI's technology (including Grok) and team become fully integrated into SpaceX's operations. It signals Musk's strategy to centralize AI development under the SpaceX brand, potentially accelerating AI applications in space exploration and other ventures. The acquisition valued SpaceX at $1 trillion and xAI at $250 billion. xAI's flagship products include the AI chatbot Grok and the social network X, which was acquired in March 2025. The company also built the Colossus supercomputer and launched a data center business.

telegram · zaihuapd · Jul 7, 02:30

**Background**: xAI was founded by Elon Musk in 2023 as an independent AI company to compete with OpenAI and others. It developed Grok, a conversational AI chatbot, and later acquired the social media platform X. In February 2026, SpaceX acquired xAI in an all-stock transaction, making it a wholly owned subsidiary. The rebranding to SpaceXAI completes the integration.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/XAI_(company)">SpaceXAI - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/SpaceXAI">SpaceXAI</a></li>
<li><a href="https://www.fifthrow.com/blog/from-x-ai-to-space-xai-how-elon-musk-s-bold-integration-is-reshaping-ai-venture-building-and-the-innovation-playbook">From xAI to SpaceXAI: How Elon Musk’s Bold Integration Is Reshaping AI, Venture Building, and the Innovation Playbook | FifthRow – Autonomous AI Apps for Research, Strategy, Consulting</a></li>

</ul>
</details>

**Tags**: `#Elon Musk`, `#xAI`, `#SpaceX`, `#AI`, `#corporate restructuring`

---

<a id="item-13"></a>
## [China Plans $295B National Computing Network Over 5 Years](https://t.me/zaihuapd/42399) ⭐️ 8.0/10

China plans to invest approximately 2 trillion yuan ($295 billion) over five years to build a nationwide interconnected data center network, prioritizing domestic AI chips from Huawei and other local suppliers for at least 80% of the infrastructure. This massive infrastructure investment aims to reduce China's reliance on US chip suppliers like Nvidia and AMD, while integrating scattered regional computing resources into a unified national network to boost AI and high-performance computing capabilities. State-owned telecom operators like China Telecom and China Unicom will operate major facilities, and they have already launched token-based computing packages that sell computing power like mobile data, lowering the cost of AI model usage.

telegram · zaihuapd · Jul 7, 04:45

**Background**: The plan is a key part of Beijing's 'Six Networks' infrastructure initiative, which aims to build a unified national computing power system. Token packages, such as those offered by China Mobile for as low as 5.99 yuan, allow users to pay for computing power on demand, similar to mobile data plans.

<details><summary>References</summary>
<ul>
<li><a href="https://www.21jingji.com/article/20260518/herald/9dd8ac86feed239fb9fd341ba64265ec.html">三大运营商开卖Token套餐，AI算力进入“话费账单”时代 - 21经济网</a></li>

</ul>
</details>

**Tags**: `#China`, `#AI infrastructure`, `#computing network`, `#chip localization`, `#government investment`

---

<a id="item-14"></a>
## [New-API Fixes Billing Bug: Oversized Parameters Cause Negative Charges](https://github.com/QuantumNous/new-api/commit/d0bd8aa) ⭐️ 8.0/10

The QuantumNous/new-api project has fixed a billing vulnerability where oversized user-controlled parameters could trigger integer overflow, causing quota deductions to become negative and effectively reverse-charge the user. This fix prevents financial exploitation of the API billing system, protecting both service providers and users from potential losses or unauthorized credit gains. It highlights the importance of input validation in financial logic. The fix adds upper-bound checks on parameters and introduces saturation arithmetic to prevent quota calculation results from wrapping to negative when converted to integers. Additional boundary checks were applied to other entry points to block attacks via oversized numbers.

telegram · zaihuapd · Jul 7, 07:26

**Background**: Integer overflow occurs when an arithmetic operation produces a value larger than the maximum representable value for a given integer type, causing it to wrap around to a negative or small number. In billing systems, this can lead to incorrect charges. Saturation arithmetic clamps results to a predefined range instead of wrapping, preventing such vulnerabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.invicti.com/learn/integer-overflow">Integer Overflow</a></li>
<li><a href="https://en.wikipedia.org/wiki/Saturation_arithmetic">Saturation arithmetic</a></li>
<li><a href="https://deepwiki.com/QuantumNous/new-api/2.6-quota-and-billing-system">Quota & Billing System | QuantumNous/new-api | DeepWiki</a></li>

</ul>
</details>

**Tags**: `#security`, `#billing`, `#vulnerability`, `#open-source`, `#API`

---