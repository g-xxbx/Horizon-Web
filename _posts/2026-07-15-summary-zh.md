---
layout: default
title: "Horizon Summary: 2026-07-15 (ZH)"
date: 2026-07-15
lang: zh
---

> 从 31 条内容中筛选出 6 条重要资讯。

---

1. [Stripe 与 Advent 联合出价 530 亿美元收购 PayPal](#item-1) ⭐️ 9.0/10
2. [马斯克：X 将无条件开源全部代码](#item-2) ⭐️ 9.0/10
3. [无 GPU 跑 Gemma 4 26B: 13 岁 Xeon 达 5t/s](#item-3) ⭐️ 8.0/10
4. [Claude web_fetch 漏洞导致用户记忆数据泄露](#item-4) ⭐️ 8.0/10
5. [PyTorch 模型在 T4 上比 A100 慢 170 倍：寻找瓶颈原因](#item-5) ⭐️ 8.0/10
6. [DeepSeek 完成逾 500 亿元首轮融资，特殊架构维持创始人控制](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Stripe 与 Advent 联合出价 530 亿美元收购 PayPal](https://www.reuters.com/business/finance/stripe-advent-offer-buy-paypal-more-than-53-billion-sources-say-2026-07-15/) ⭐️ 9.0/10

据消息人士透露，支付公司 Stripe 与私募股权公司 Advent International 联合出价超过 530 亿美元收购 PayPal。 此次收购将使 Stripe、PayPal、Venmo 和 Braintree 等主要支付平台整合在一起，可能重塑在线支付格局，并引发重大的反垄断担忧。 该交易涵盖 PayPal 旗下包括 Venmo 和 Braintree 在内的整个生态系统。PayPal 拥有 Stripe 所缺少的银行牌照，这可能为放贷和监管灵活性提供战略优势。

hackernews · rvz · 7月15日 03:32 · [社区讨论](https://news.ycombinator.com/item?id=48915953)

**背景**: PayPal 是一种广泛使用的在线支付系统，还拥有 Venmo、Braintree 和 Xoom。Stripe 是面向在线企业的主要支付处理商。Advent International 是一家全球私募股权公司，截至 2025 年 11 月管理资产约 1000 亿美元。合并后的市场份额可能面临监管机构严格的反垄断审查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Advent_International">Advent International</a></li>
<li><a href="https://www.adventinternational.com/">Advent International - A leading global private equity investor</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了对竞争减少和潜在费用增加的担忧，一些人指出 Stripe 对成人行业和大麻等行业的限制政策。其他人强调了反垄断影响并建议剥离部分品牌。PayPal 银行牌照的战略价值也被探讨。

**标签**: `#stripe`, `#paypal`, `#acquisition`, `#fintech`, `#antitrust`

---

<a id="item-2"></a>
## [马斯克：X 将无条件开源全部代码](https://x.com/elonmusk/status/2077361679034118271) ⭐️ 9.0/10

埃隆·马斯克宣布，在完成安全审查后，X 平台将无条件开源全部代码，并邀请第三方审查者检查运行中的系统，以确保公开的代码与实际运行的代码一致。 此举可能为社交媒体平台的透明度设定新标准，有望增进用户和开发者社区的信任，并促使其他平台效仿。 开源的前提是完成安全漏洞审查。第三方审查者将被允许检查生产系统，以确认运行中的代码与已发布的源代码一致，从而确保代码的真实性。

telegram · zaihuapd · 7月15日 13:32

**背景**: 开源代码公开可见，任何人都可以审查，从而促进透明度和安全性。目前大多数社交媒体平台运行专有闭源代码，用户难以验证平台行为。马斯克的声明旨在解决长期以来对算法不透明和信任问题的担忧。

**标签**: `#open source`, `#social media`, `#transparency`, `#Elon Musk`, `#code review`

---

<a id="item-3"></a>
## [无 GPU 跑 Gemma 4 26B: 13 岁 Xeon 达 5t/s](https://www.neomindlabs.com/2026/06/08/running-gemma-4-26b-at-5-tokens-sec-on-a-13-year-old-xeon-with-no-gpu/) ⭐️ 8.0/10

一位开发者展示了在 13 年历史的 Xeon CPU 上（无 GPU）运行 26B 参数的 Gemma 4 混合专家模型，达到约 5 tokens/秒的速度。 这表明现代大语言模型甚至可以在非常旧的硬件上本地运行，有望无需昂贵 GPU 就能普及 AI 访问，同时也引发了本地推理与云服务成本效益的讨论。 Gemma 4 26B 模型采用混合专家架构，每个 token 仅激活 40 亿参数，使其在 CPU 上推理高效。文章声称仅使用 CPU 计算就达到了 5 tokens/秒。

hackernews · neomindryan · 7月15日 15:34 · [社区讨论](https://news.ycombinator.com/item?id=48922434)

**背景**: Gemma 4 是 Google DeepMind 推出的模型系列，有密集和混合专家（MoE）变体。26B A4B 模型采用混合专家架构，每个 token 只使用部分参数，减少计算量，从而以更低推理成本实现更大有效模型尺寸。在无 GPU 的旧消费硬件上运行此类模型得益于量化技术和高效推理框架的进步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ollama.com/library/gemma4">gemma 4</a></li>
<li><a href="https://gemma4.com/">Gemma 4 — Google DeepMind</a></li>
<li><a href="https://lmstudio.ai/models/gemma-4">Gemma 4</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了成本效益，指出在某些地区使用推理提供商的费用比本地推理的电费更便宜。另一位分享了在双 Xeon 256GB DDR4 上运行多个模型的基准测试。还有预测到 2027 年中，大于 200B 的 MoE 模型将能在基础消费硬件上运行。

**标签**: `#LLM`, `#local inference`, `#Gemma 4`, `#old hardware`, `#cost analysis`

---

<a id="item-4"></a>
## [Claude web_fetch 漏洞导致用户记忆数据泄露](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

研究人员 Ayush Paul 发现 Anthropic 的 Claude web_fetch 工具存在一个绕过漏洞，可通过恶意网站的嵌套链接诱导模型泄露用户记忆中的姓名、所在城市和雇主等信息。 该漏洞揭示了同时拥有私有数据访问和网页浏览能力的 AI 代理存在严重安全缺陷，可能导致用户敏感信息泄露。它凸显了在基于大语言模型的系统中防止数据外泄的持续挑战。 攻击之所以成功，是因为 web_fetch 可以访问已获取页面中嵌入的链接，从而形成重定向链。Anthropic 表示已内部发现该问题并关闭了漏洞（移除了该能力），因此未支付漏洞赏金。

rss · Simon Willison · 7月15日 14:21

**背景**: Claude 的 web_fetch 工具旨在从用户提供的 URL 获取网页内容，并设有限制以防止数据外泄。然而，当 AI 代理拥有私有数据访问、处理不可信输入并能与外界通信时，就会面临‘致命三重威胁’（lethal trifecta）。提示注入攻击可利用这些条件诱导模型泄露信息。web_fetch 工具最初的设计允许跟随已获取页面内的链接，这为攻击者创造了漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted content, and external communication</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection</a></li>
<li><a href="https://simonwillison.net/2025/Sep/10/claude-web-fetch-tool/">Claude API: Web fetch tool</a></li>

</ul>
</details>

**标签**: `#AI security`, `#prompt injection`, `#data exfiltration`, `#Claude`, `#vulnerability`

---

<a id="item-5"></a>
## [PyTorch 模型在 T4 上比 A100 慢 170 倍：寻找瓶颈原因](https://www.reddit.com/r/MachineLearning/comments/1ux6a9x/pytorch_model_running_170x_slower_on_t4_vs_a100/) ⭐️ 8.0/10

一位机器学习从业者报告称，其使用 4D 相关体积和 transformer 层、运行在 FP32 精度的 PyTorch 点跟踪模型，在 NVIDIA T4 GPU 上比在 A100 GPU 上慢了约 170 倍，尽管 GPU 利用率达 99% 且启用了常见优化。 这种极端的速度差异突显了 GPU 代际间的架构差异可能对模型性能产生巨大影响，而找出瓶颈原因可以为在成本较低的 GPU（如 T4）上部署模型提供关键的优化策略。 该模型构建 4D 相关体积以实现密集帧匹配，随后进行 transformer 处理，使用纯 FP32 精度、批大小为 1，输入为 256×256 的视频帧；这种缓慢在两台独立的 T4 机器上一致出现，且 GPU 利用率达到 99%。

reddit · r/MachineLearning · /u/Future-Structure-296 · 7月15日 13:44

**背景**: NVIDIA T4 和 A100 采用不同的架构：T4 基于 Turing（2018 年），而 A100 基于 Ampere（2020 年）。A100 的 CUDA 核心数量约为 T4 的两倍，内存带宽高约 1.6 倍，并拥有更大的缓存，这对像 4D 相关体积构建这样的内存密集型操作极为有利。4D 相关体积是一种用于密集匹配任务（如光流）的数据结构，它计算两张图像中所有特征向量对之间的点积，需要大量的内存访问。在纯 FP32 模式下，T4 无法利用张量核心，因此性能完全依赖 CUDA 核心和内存带宽。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ruojincai.github.io/ExtremeRotation/">Extreme Rotation Estimation using Dense Correlation Volumes</a></li>
<li><a href="https://arxiv.org/html/2505.16942">Efficient Correlation Volume Sampling for Ultra-High-Resolution Optical Flow Estimation</a></li>

</ul>
</details>

**标签**: `#pytorch`, `#gpu-performance`, `#nvidia-t4`, `#nvidia-a100`, `#ml-engineering`

---

<a id="item-6"></a>
## [DeepSeek 完成逾 500 亿元首轮融资，特殊架构维持创始人控制](https://t.me/zaihuapd/42589) ⭐️ 8.0/10

DeepSeek 完成首轮融资，募资逾 500 亿元人民币（约合 74 亿美元），估值超过 500 亿美元。该公司采用非常规架构，投资者需将资金注入由 CEO 梁文锋管理的有限合伙企业，并接受五年锁定期且不享有表决权。 此次融资表明投资者对 DeepSeek 的 AI 能力充满信心，其特殊架构使创始人在大规模融资后仍能保持控制权。这可能影响其他高增长初创公司如何在融资需求与创始人控制之间取得平衡。 创始人梁文锋个人投资 200 亿元。腾讯和宁德时代分别考虑或计划投资 100 亿元和 50 亿元，成为最大的外部投资者。五年锁定期和无表决权是核心条款。

telegram · zaihuapd · 7月15日 12:56

**背景**: 在有限合伙架构中，创始人作为普通合伙人（GP）享有完全表决权，而投资者作为有限合伙人（LP）享有经济收益但无控制权。这种结构常用于集中控制权。锁定期（此处为五年）限制投资者在一定期限内转让股份，确保长期承诺。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/30995033225">初创公司创始人及股东股权架构如何设置 - 知乎</a></li>
<li><a href="https://www.qidufanyi.com/news/526.html">lock-up period及其相关内容 | 旗渡法律翻译中心</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#AI`, `#financing`, `#unicorn`, `#startup`

---