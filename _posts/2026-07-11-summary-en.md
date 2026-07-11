---
layout: default
title: "Horizon Summary: 2026-07-11 (EN)"
date: 2026-07-11
lang: en
---

> From 30 items, 9 important content pieces were selected

---

1. [vLLM v0.25.0 makes Model Runner V2 default, drops PagedAttention](#item-1) ⭐️ 9.0/10
2. [Humanoid robot performs first live pig gallbladder surgery remotely](#item-2) ⭐️ 9.0/10
3. [SGLang v0.5.15: GLM-5.2 Tuning, Spec V2, IndexShare MTP](#item-3) ⭐️ 8.0/10
4. [ClickHouse scales PgBouncer 4x with SO_REUSEPORT and peering](#item-4) ⭐️ 8.0/10
5. [George Hotz Warns Against 'Cult of Intelligence' in AI Development](#item-5) ⭐️ 8.0/10
6. [VultronRetriever models top MTEB, released on HuggingFace](#item-6) ⭐️ 8.0/10
7. [Apple Sues OpenAI Over Trade Secret Theft](#item-7) ⭐️ 8.0/10
8. [Six U-Boot Bootloader Vulnerabilities Allow Arbitrary Code Execution at Boot](#item-8) ⭐️ 8.0/10
9. [OpenAI Releases GPT-5.6 Series with Sol, Terra, Luna Tiers](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0 makes Model Runner V2 default, drops PagedAttention](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 sets Model Runner V2 as the default execution path for all dense models, removes the legacy PagedAttention algorithm, and achieves performance parity between the Transformers modeling backend and native vLLM. This release represents a major architectural shift, simplifying the codebase and improving performance. The Transformers backend parity allows users to define custom models without speed loss, broadening vLLM's usability. Model Runner V2, a redesigned execution core, brings support for EVS, realtime embeddings, and prefix caching for Mamba hybrids. The Transformers backend adds FP8 MoE support and fixes for CUDA graphs and embedding scaling.

github · khluu · Jul 11, 20:06

**Background**: PagedAttention, introduced with vLLM in 2023, optimized memory management by storing key-value cache in fixed-size blocks. Model Runner V2 is a ground-up reimplementation aiming for modularity and efficiency. This release consolidates on MRV2 and removes the older V1/PagedAttention path.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PagedAttention">PagedAttention</a></li>
<li><a href="https://vllm.ai/blog/2026-03-24-mrv2">Model Runner V2: A Modular and Faster Core for vLLM</a></li>
<li><a href="https://github.com/vllm-project/vllm/blob/main/docs/design/model_runner_v2.md">vllm/docs/design/model_runner_v2.md at main · vllm-project ...</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#LLM inference`, `#release`, `#open source`, `#machine learning`

---

<a id="item-2"></a>
## [Humanoid robot performs first live pig gallbladder surgery remotely](https://arstechnica.com/ai/2026/07/humanoid-robots-controlled-by-surgeons-did-world-first-operation-on-live-pigs/) ⭐️ 9.0/10

Surgeons remotely controlled a Unitree G1 humanoid robot to perform the world's first laparoscopic gallbladder surgery on live pigs. The results were published in Nature. This breakthrough demonstrates that low-cost, general-purpose humanoid robots can be used for telesurgery, potentially expanding access to surgical care in remote, rural, battlefield, or space settings. It challenges the dominance of expensive specialized surgical robots like the da Vinci system. The Unitree G1 base model costs $13,500, or about $67,000 with dexterous hands, a fraction of the cost of da Vinci systems which range from $500,000 to millions. The robot is compact, standing 1.5 meters tall and weighing 27 kg.

telegram · zaihuapd · Jul 11, 02:29

**Background**: Humanoid robots are designed to mimic human form and movement, and dexterous hands are robotic end-effectors that can manipulate tools with fine motor skills. The da Vinci surgical system is a specialized robotic platform for minimally invasive surgery, but it is very expensive and not general-purpose. This study, led by researchers at UC San Diego, marks the first time a general-purpose humanoid robot has been used for live surgery.

<details><summary>References</summary>
<ul>
<li><a href="https://www.jinantimes.com.cn/news-243-5048472.html">jinantimes.com.cn/news-243-5048472.html</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/717179760">一文看懂灵巧手 - 知乎</a></li>
<li><a href="https://zh.wikipedia.org/wiki/达芬奇手术系统">达芬奇手术系统 - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**Tags**: `#humanoid robot`, `#telesurgery`, `#medical robotics`, `#Nature publication`

---

<a id="item-3"></a>
## [SGLang v0.5.15: GLM-5.2 Tuning, Spec V2, IndexShare MTP](https://github.com/sgl-project/sglang/releases/tag/v0.5.15) ⭐️ 8.0/10

SGLang v0.5.15 has been released, featuring production tuning for GLM-5.2 on Blackwell GPUs with NVFP4 format, enabling 500+ tokens/s/user on 8x B300. It also makes Spec V2 the default scheduling for zero-overhead speculative decoding and introduces IndexShare MTP to reduce draft-step costs by up to 1.9x. This release significantly improves LLM serving efficiency, particularly for long-context models like GLM-5.2, with higher throughput and lower latency. The optimizations advance the state of the art in speculative decoding and attention mechanisms, benefiting the broader AI inference ecosystem. Spec V2 achieves +11% end-to-end throughput by eliminating host-device syncs and fusing metadata operations. IndexShare MTP reuses the indexer top-k across draft steps, lowering compute cost for long contexts, and the release also includes shape-specialized GEMM kernels and breakable CUDA Graph by default.

github · Fridge003 · Jul 10, 22:58

**Background**: GLM-5.2 is a 744B MoE language model developed by Zhipu AI, optimized for long-context tasks with an IndexShare architecture that reuses the indexer across sparse attention layers. NVFP4 is a 4-bit floating-point format introduced with NVIDIA Blackwell GPUs, enabling efficient low-precision inference. Multi-Token Prediction (MTP) speeds up speculative decoding by predicting multiple tokens simultaneously, and IndexShare MTP reduces draft-step costs by reusing top-k indices across steps.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/zai-org/GLM-5.2">zai-org/GLM-5.2 · Hugging Face</a></li>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision Inference | NVIDIA Technical Blog</a></li>
<li><a href="https://news.smol.ai/issues/26-06-16-glm-52">GLM 5.2: the top Frontend Coding model in the world, IndexShare ...</a></li>

</ul>
</details>

**Tags**: `#sglang`, `#LLM serving`, `#performance optimization`, `#inference`, `#release`

---

<a id="item-4"></a>
## [ClickHouse scales PgBouncer 4x with SO_REUSEPORT and peering](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

ClickHouse's blog details how they increased PgBouncer throughput by 4x by enabling SO_REUSEPORT and peering, allowing multiple PgBouncer processes to share the same port and coordinate query cancellation. This optimization is critical for PostgreSQL connection pooling performance, especially in high-traffic environments. It demonstrates a practical technique that can be adopted by other PgBouncer users to scale their database access layer without additional hardware. SO_REUSEPORT enables multiple PgBouncer processes to listen on the same TCP port, while peering allows processes to forward cancel requests to the correct owner session. The setup requires a peer_id in configuration and binding to the same port.

hackernews · saisrirampur · Jul 11, 15:28 · [Discussion](https://news.ycombinator.com/item?id=48872874)

**Background**: PgBouncer is a lightweight connection pooler for PostgreSQL that manages client connections to reduce the overhead of database connections. By default, PgBouncer runs as a single process, which can become a bottleneck. SO_REUSEPORT is a Linux socket option that allows multiple sockets to bind to the same port, enabling kernel-level load distribution. Peering in PgBouncer allows multiple processes to share session state and forward cancel requests.

<details><summary>References</summary>
<ul>
<li><a href="http://www.pgbouncer.org/usage.html">PgBouncer command-line usage</a></li>
<li><a href="https://www.pgbouncer.org/config.html">PgBouncer config</a></li>
<li><a href="https://lwn.net/Articles/542629/">The SO_REUSEPORT socket option [LWN.net]</a></li>

</ul>
</details>

**Discussion**: Community comments include suggestions of alternative tools like Odyssey and pgdog. Some users expressed interest in the practical details of peering and SO_REUSEPORT, while others shared their experiences using PgBouncer in Kubernetes. Overall, the discussion was positive and the blog post was seen as a valuable technical deep-dive.

**Tags**: `#PgBouncer`, `#PostgreSQL`, `#performance`, `#connection pooling`, `#ClickHouse`

---

<a id="item-5"></a>
## [George Hotz Warns Against 'Cult of Intelligence' in AI Development](https://geohot.github.io//blog/jekyll/update/2026/07/11/ai-2040.html) ⭐️ 8.0/10

George Hotz published a blog post titled 'AI 2040 and the cult of intelligence,' criticizing ideological control and censorship in AI development and advocating for freedom. This post highlights the growing tension between AI safety and freedom of speech/development, sparking debate on how AI should be regulated. The high engagement indicates strong community interest in these issues. The blog argues that freedom is binary and worth fighting for, and warns against an AI 'cult of intelligence' that would enforce ideological conformity. Community comments discuss implications for thoughtcrime, censorship, and physical-world actions.

hackernews · rvz · Jul 11, 18:04 · [Discussion](https://news.ycombinator.com/item?id=48874200)

**Background**: George Hotz, also known as geohot, is a prominent hacker and entrepreneur who founded comma.ai, an open-source self-driving car company. He frequently comments on AI and technology policy. The 'cult of intelligence' phrase criticizes the tendency to treat AI as an infallible oracle or to impose strict ideological controls on its outputs.

**Discussion**: The comments show a split: some agree with Hotz about the dangers of AI censorship and ideological bias, while others argue that freedom is not absolute and that AI agents acting in the real world need regulation. One user warns about invisible logging of 'thoughtcrime' and biased responses.

**Tags**: `#AI`, `#freedom`, `#ethics`, `#technology policy`

---

<a id="item-6"></a>
## [VultronRetriever models top MTEB, released on HuggingFace](https://www.reddit.com/r/MachineLearning/comments/1utmxq8/vultronretriever_family_of_models_released_on/) ⭐️ 8.0/10

VultronRetrieverPrime-8B became the global #1 on the MTEB leaderboard, with the whole family released on HuggingFace, demonstrating offline edge deployment on iPhone. This release sets a new state-of-the-art in retrieval with significant efficiency gains (16x smaller index, 12x higher throughput) while enabling fully offline operation on edge devices, making advanced retrieval accessible for mobile and embedded applications. The VultronRetriever family includes three models: Prime-8B, Core-4.5B, and Flash-0.8B, all designed with the Hydra Architecture for late interaction retrieval. They were trained on datasets with 0% cross-dataset duplication and 0% evaluation contamination.

reddit · r/MachineLearning · /u/madkimchi · Jul 11, 15:22

**Background**: MTEB (Massive Text Embedding Benchmark) is a standardized benchmark for evaluating text embedding models across diverse tasks. Late interaction retrieval processes queries and documents separately until final stages, enabling efficient and precise retrieval. Edge deployment allows models to run locally on devices like smartphones without cloud connectivity.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/spaces/mteb/leaderboard">MTEB Leaderboard - a Hugging Face Space by mteb</a></li>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/mteb-leaderboard/">MTEB Leaderboard - GeeksforGeeks</a></li>
<li><a href="https://weaviate.io/blog/late-interaction-overview">An Overview of Late Interaction Retrieval Models... | Weaviate</a></li>

</ul>
</details>

**Tags**: `#information retrieval`, `#MTEB leaderboard`, `#embeddings`, `#edge deployment`, `#HuggingFace`

---

<a id="item-7"></a>
## [Apple Sues OpenAI Over Trade Secret Theft](https://www.cnbc.com/2026/07/10/apple-openai-lawsuit-trade-secrets.html) ⭐️ 8.0/10

On July 10, 2026, Apple filed a lawsuit in the U.S. District Court for Northern California against OpenAI, two former employees, and io Products, alleging systematic theft of trade secrets related to hardware design and manufacturing to accelerate OpenAI's consumer hardware efforts. This legal action intensifies the rivalry between two tech titans over AI hardware and talent, potentially setting precedents for protection of trade secrets in the fast-moving AI industry. Apple specifically alleges that former employee Chang Liu downloaded dozens of hardware files after his departure, and that OpenAI hardware head Tang Yew Tan sent supplier information to his personal email and instructed job candidates to bring Apple components to interviews. Apple also claims over 400 of its former employees are now working at OpenAI.

telegram · zaihuapd · Jul 11, 03:14

**Background**: Apple has long treated its hardware design and manufacturing processes as closely guarded trade secrets, while OpenAI, known primarily for AI software like ChatGPT, has been expanding into consumer hardware, including potential AI-powered devices. The lawsuit reflects growing tensions as companies compete for talent and proprietary knowledge in the AI hardware space.

**Tags**: `#Apple`, `#OpenAI`, `#lawsuit`, `#trade secrets`, `#hardware`

---

<a id="item-8"></a>
## [Six U-Boot Bootloader Vulnerabilities Allow Arbitrary Code Execution at Boot](https://www.bleepingcomputer.com/news/security/new-u-boot-flaws-could-enable-stealthy-firmware-attacks/) ⭐️ 8.0/10

Security firm Binarly disclosed six vulnerabilities in the U-Boot bootloader's FIT image signature verification, with two allowing arbitrary code execution and four causing device crashes. The flaws have been present since U-Boot version 2013.07. These vulnerabilities are critical because they allow attackers to execute malicious code before the operating system boots, bypassing security measures. Affecting a wide range of embedded and IoT devices, they could enable persistent firmware attacks, especially on systems with remote update capabilities like BMCs. Binarly reported the flaws to U-Boot maintainers, and patches have been accepted. However, fixes must be integrated by hardware vendors into firmware updates, leaving unsupported devices potentially vulnerable forever. The vulnerabilities are tracked as BRLY-2026-037 through BRLY-2026-042.

telegram · zaihuapd · Jul 11, 08:32

**Background**: U-Boot (Das U-Boot) is a universal boot loader commonly used in embedded systems and IoT devices. It supports a format called FIT (Flattened Image Tree) that allows bundling multiple images with cryptographic signatures to ensure authenticity and integrity. The six vulnerabilities discovered by Binarly reside in the FIT signature verification code, potentially allowing attackers to bypass validation and execute malicious code before the operating system loads.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Das_U-Boot">Das U - Boot - Wikipedia</a></li>
<li><a href="https://docs.u-boot-project.org/en/latest/usage/fit/signature.html">U-Boot FIT Signature Verification — Das U-Boot unknown version...</a></li>
<li><a href="https://cybersecuritynews.com/u-boot-fit-signature-verification/">Six U-Boot FIT Signature Verification Flaws Enable Code Execution...</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#U-Boot`, `#bootloader`, `#firmware`

---

<a id="item-9"></a>
## [OpenAI Releases GPT-5.6 Series with Sol, Terra, Luna Tiers](https://t.me/zaihuapd/42497) ⭐️ 8.0/10

OpenAI released the GPT-5.6 series on June 26, 2026, offering three model variants: Sol (flagship), Terra (balanced), and Luna (cost-efficient). The series emphasizes improved coding, knowledge work, design, research, and cybersecurity capabilities, and introduces max/ultra reasoning, multi-agent collaboration, and programmatic tool calling. This release signals a major step in OpenAI's model optimization, offering tiered options that allow users to balance cost and performance for different use cases. The cost efficiency and capability improvements make advanced AI more accessible for both high-end research and high-volume production applications. Sol with max reasoning achieves state-of-the-art results on coding benchmarks using fewer tokens and lower cost compared to rivals. Terra offers roughly GPT-5.5 quality at half the price, while Luna is latency-optimized for high-concurrency, low-cost scenarios.

telegram · zaihuapd · Jul 11, 13:34

**Background**: GPT-5.6 is OpenAI's latest model family, succeeding GPT-5.5 and GPT-5. The three tiers cater to different needs: Sol for demanding tasks, Terra for balanced performance, and Luna for high throughput. The introduction of max and ultra reasoning modes allows users to scale inference compute for complex problems, and programmatic tool calling enables agents to execute code to interact with tools.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-6/">GPT‑5.6: Frontier intelligence that scales with your ambition</a></li>
<li><a href="https://codersera.com/blog/gpt-5-6-sol-terra-luna/">GPT-5.6 Sol, Terra & Luna Explained: Tiers, Pricing ...</a></li>
<li><a href="https://andrew.ooo/answers/what-is-gpt-5-6-sol-terra-luna-openai-june-2026/">What is GPT-5.6? Sol, Terra, Luna Explained (June 2026)</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#GPT-5.6`, `#AI models`, `#machine learning`

---