---
layout: default
title: "Horizon Summary: 2026-07-15 (EN)"
date: 2026-07-15
lang: en
---

> From 31 items, 6 important content pieces were selected

---

1. [Stripe and Advent Jointly Offer $53 Billion to Acquire PayPal](#item-1) ⭐️ 9.0/10
2. [Musk: X to Unconditionally Open Source All Code](#item-2) ⭐️ 9.0/10
3. [Gemma 4 26B Runs at 5 Tokens/sec on 13-Year-Old Xeon Without GPU](#item-3) ⭐️ 8.0/10
4. [Claude web_fetch bypass allows data exfiltration of user memories](#item-4) ⭐️ 8.0/10
5. [PyTorch Model 170x Slower on T4 vs A100: Seeking Cause](#item-5) ⭐️ 8.0/10
6. [DeepSeek raises over $7.4B in first round with founder control structure](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Stripe and Advent Jointly Offer $53 Billion to Acquire PayPal](https://www.reuters.com/business/finance/stripe-advent-offer-buy-paypal-more-than-53-billion-sources-say-2026-07-15/) ⭐️ 9.0/10

Stripe and private equity firm Advent International have jointly made an offer of over $53 billion to acquire PayPal, according to sources. This acquisition would consolidate major payment platforms like Stripe, PayPal, Venmo, and Braintree under one roof, potentially reshaping the online payments landscape and raising significant antitrust concerns. The deal includes PayPal's entire ecosystem including Venmo and Braintree. PayPal holds a bank charter that Stripe lacks, which could provide strategic advantages in lending and regulatory flexibility.

hackernews · rvz · Jul 15, 03:32 · [Discussion](https://news.ycombinator.com/item?id=48915953)

**Background**: PayPal is a widely-used online payment system that also owns Venmo, Braintree, and Xoom. Stripe is a major payment processor for online businesses. Advent International is a global private equity firm with approximately $100 billion in assets under management as of November 2025. The combined market share could face intense antitrust scrutiny from regulators.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Advent_International">Advent International</a></li>
<li><a href="https://www.adventinternational.com/">Advent International - A leading global private equity investor</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concerns about reduced competition and potential fee increases, with some noting Stripe's restrictive policies on industries like cannabis and adult content. Others highlighted the antitrust implications and suggested unwinding brands. The strategic value of PayPal's bank charter was also discussed.

**Tags**: `#stripe`, `#paypal`, `#acquisition`, `#fintech`, `#antitrust`

---

<a id="item-2"></a>
## [Musk: X to Unconditionally Open Source All Code](https://x.com/elonmusk/status/2077361679034118271) ⭐️ 9.0/10

Elon Musk announced that X will unconditionally open source its entire codebase after a security review and invite third-party reviewers to verify that the running system matches the open source code. This move could set a new standard for transparency in social media platforms, potentially building greater trust with users and the developer community and putting pressure on other platforms to follow suit. The open-sourcing is conditional on the completion of a security review. Third-party reviewers will be allowed to inspect the production system to confirm that the running code matches the published source code, ensuring authenticity.

telegram · zaihuapd · Jul 15, 13:32

**Background**: Open source code is publicly accessible and can be audited by anyone, which promotes transparency and security. Most social media platforms today run proprietary, closed-source code, making it difficult for users to verify platform behavior. Musk's announcement aims to address long-standing concerns about algorithmic opacity and trust in X.

**Tags**: `#open source`, `#social media`, `#transparency`, `#Elon Musk`, `#code review`

---

<a id="item-3"></a>
## [Gemma 4 26B Runs at 5 Tokens/sec on 13-Year-Old Xeon Without GPU](https://www.neomindlabs.com/2026/06/08/running-gemma-4-26b-at-5-tokens-sec-on-a-13-year-old-xeon-with-no-gpu/) ⭐️ 8.0/10

A developer demonstrated running the 26B-parameter Gemma 4 Mixture-of-Experts model on a 13-year-old Xeon CPU with no GPU, achieving approximately 5 tokens per second. This shows that modern large language models can be run locally on very old hardware, potentially democratizing AI access without requiring expensive GPUs. It also sparks debate on the cost-effectiveness of local inference versus cloud services. The Gemma 4 26B model uses a Mixture-of-Experts architecture with only 4 billion active parameters per token, making it efficient for CPU inference. The article claims 5 tokens/sec was achieved with pure CPU computation.

hackernews · neomindryan · Jul 15, 15:34 · [Discussion](https://news.ycombinator.com/item?id=48922434)

**Background**: Gemma 4 is a family of models from Google DeepMind available in dense and MoE variants. The 26B A4B model uses Mixture-of-Experts, where only a subset of parameters are used per token, reducing computation. This allows larger effective model size with lower inference cost. Running such models on old consumer hardware without GPU is enabled by advances in quantization and efficient inference frameworks.

<details><summary>References</summary>
<ul>
<li><a href="https://ollama.com/library/gemma4">gemma 4</a></li>
<li><a href="https://gemma4.com/">Gemma 4 — Google DeepMind</a></li>
<li><a href="https://lmstudio.ai/models/gemma-4">Gemma 4</a></li>

</ul>
</details>

**Discussion**: Commenters discussed cost efficiency, with one noting that inference provider costs are cheaper than electricity for local inference in some regions. Another shared benchmarks running models on dual Xeon with 256GB DDR4. A prediction was made that by mid-2027, >200B MoE models will run on basic consumer hardware.

**Tags**: `#LLM`, `#local inference`, `#Gemma 4`, `#old hardware`, `#cost analysis`

---

<a id="item-4"></a>
## [Claude web_fetch bypass allows data exfiltration of user memories](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

Researcher Ayush Paul discovered a bypass in Anthropic's Claude web_fetch tool that allowed extraction of user memories, such as name, city, and employer, by tricking the model into following nested links from a malicious website. This vulnerability demonstrates a critical security gap in AI agents that combine private data access with web browsing capabilities, potentially exposing sensitive user information. It highlights the ongoing challenge of preventing data exfiltration in LLM-based systems. The attack worked because web_fetch could follow URLs embedded in previously fetched pages, allowing a chain of redirects. Anthropic reportedly already identified the issue internally and closed the hole by removing that ability, so no bug bounty was paid.

rss · Simon Willison · Jul 15, 14:21

**Background**: Claude's web_fetch tool is designed to fetch web content from user-provided URLs, with restrictions to prevent data exfiltration. However, AI agents face a 'lethal trifecta' when they have access to private data, process untrusted input, and can communicate externally. Prompt injection attacks can exploit these conditions to trick models into leaking information. The web_fetch tool's original design allowed following links within fetched pages, which created a loophole for attackers.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted content, and external communication</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection</a></li>
<li><a href="https://simonwillison.net/2025/Sep/10/claude-web-fetch-tool/">Claude API: Web fetch tool</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#prompt injection`, `#data exfiltration`, `#Claude`, `#vulnerability`

---

<a id="item-5"></a>
## [PyTorch Model 170x Slower on T4 vs A100: Seeking Cause](https://www.reddit.com/r/MachineLearning/comments/1ux6a9x/pytorch_model_running_170x_slower_on_t4_vs_a100/) ⭐️ 8.0/10

A machine learning practitioner reports that their PyTorch point-tracking model, which uses 4D correlation volumes and transformers in FP32, runs approximately 170 times slower on an NVIDIA T4 GPU than on an A100 GPU, despite full GPU utilization and typical optimizations. This extreme slowdown highlights how architectural differences between GPU generations can drastically affect model performance, and debugging it can reveal optimization strategies crucial for deploying models on lower-cost GPUs such as the T4. The model involves constructing 4D correlation volumes for dense frame matching followed by transformer processing, runs in pure FP32 with batch size 1 on 256x256 video frames, and the slowdown persists across two independent T4 machines with full GPU utilization.

reddit · r/MachineLearning · /u/Future-Structure-296 · Jul 15, 13:44

**Background**: The NVIDIA T4 and A100 are based on different architectures: T4 uses Turing (2018) while A100 uses Ampere (2020). The A100 has approximately twice as many CUDA cores, 1.6x higher memory bandwidth, and larger caches, which strongly benefit memory-bound operations such as building 4D correlation volumes. These volumes are data structures used in dense matching tasks (e.g., optical flow) that compute dot products between all pairs of feature vectors from two images, requiring heavy memory access. In pure FP32 mode, the T4 cannot leverage Tensor Cores, so performance relies entirely on CUDA cores and memory bandwidth.

<details><summary>References</summary>
<ul>
<li><a href="https://ruojincai.github.io/ExtremeRotation/">Extreme Rotation Estimation using Dense Correlation Volumes</a></li>
<li><a href="https://arxiv.org/html/2505.16942">Efficient Correlation Volume Sampling for Ultra-High-Resolution Optical Flow Estimation</a></li>

</ul>
</details>

**Tags**: `#pytorch`, `#gpu-performance`, `#nvidia-t4`, `#nvidia-a100`, `#ml-engineering`

---

<a id="item-6"></a>
## [DeepSeek raises over $7.4B in first round with founder control structure](https://t.me/zaihuapd/42589) ⭐️ 8.0/10

DeepSeek completed its first-round financing of over 500 billion RMB (approximately $74 billion), achieving a valuation exceeding $50 billion. The company used an unconventional structure where investors contribute to a limited partnership managed by CEO Liang Wenfeng, accepting a five-year lock-up period and no voting rights. This financing underscores strong investor confidence in DeepSeek's AI capabilities, and the special structure allows the founder to maintain control despite raising substantial capital. It may influence how other high-growth startups balance funding needs with founder control. Founder Liang Wenfeng personally contributed 200 billion RMB. Tencent and CATL are respectively considering or planning investments of 100 billion and 50 billion, making them the largest external investors. The five-year lock-up period and absence of voting rights are key terms.

telegram · zaihuapd · Jul 15, 12:56

**Background**: In a limited partnership structure, the founder acts as the general partner (GP) with full voting rights, while investors become limited partners (LP) with economic benefits but no control. This structure is commonly used to concentrate control. A lock-up period restricts investors from selling their shares for a specified time, ensuring long-term commitment; here it is five years.

<details><summary>References</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/30995033225">初创公司创始人及股东股权架构如何设置 - 知乎</a></li>
<li><a href="https://www.qidufanyi.com/news/526.html">lock-up period及其相关内容 | 旗渡法律翻译中心</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#AI`, `#financing`, `#unicorn`, `#startup`

---