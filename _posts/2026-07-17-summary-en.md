---
layout: default
title: "Horizon Summary: 2026-07-17 (EN)"
date: 2026-07-17
lang: en
---

> From 32 items, 5 important content pieces were selected

---

1. [Full Firefox Browser Runs in Browser via WebAssembly](#item-1) ⭐️ 9.0/10
2. [Tesla Starts Production of Steering-Wheel-Free Cybercab](#item-2) ⭐️ 9.0/10
3. [Atmosphere detected on Earth-like exoplanet in habitable zone](#item-3) ⭐️ 8.0/10
4. [The State of Open Source AI: A Comprehensive Report](#item-4) ⭐️ 8.0/10
5. [Kimi Releases 2.8T Parameter Open-Source Model K3](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Full Firefox Browser Runs in Browser via WebAssembly](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter compiled the full Firefox browser to WebAssembly, enabling it to run entirely inside another browser over a WebSocket-based protocol (Wisp). This groundbreaking technical feat demonstrates the viability of running complex native applications within web environments. This achievement could revolutionize portable computing and sandboxing, allowing any browser to serve as a host for another full browser with end-to-end encryption. It also showcases the effectiveness of AI-assisted coding, as the project leveraged Claude Opus and Fable tokens to overcome significant engineering challenges. The demo uses the Wisp protocol to proxy all network traffic through Puter's servers because WebAssembly code cannot directly open network connections. The compiled gecko.wasm is 233MB, and the project reportedly cost an estimated $25,000 in AI model tokens, but actual expenses were much lower due to a Claude Max subscription.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (Wasm) is a low-level binary instruction format designed to run in web browsers at near-native speed, enabling high-performance applications like games and now full browsers. Gecko is Firefox's browser engine, known for its strong single-process support, which made it a good candidate for compilation to WebAssembly. The Wisp protocol is a lightweight way to proxy multiple TCP/UDP sockets over a single WebSocket connection, allowing Wasm code to communicate with the outside world.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to implement protocol for proxying multiple TCP/UDP sockets over a single websocket. · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gecko_(browser_engine)">Gecko (browser engine)</a></li>

</ul>
</details>

**Tags**: `#WebAssembly`, `#Firefox`, `#Gecko`, `#Browser-in-browser`, `#Wisp protocol`

---

<a id="item-2"></a>
## [Tesla Starts Production of Steering-Wheel-Free Cybercab](https://t.me/zaihuapd/42621) ⭐️ 9.0/10

Tesla has announced that it has begun mass production of the Cybercab, a fully autonomous electric vehicle without a steering wheel, pedals, or side mirrors, at its Giga Texas factory in February 2026. This marks a major milestone in the commercialization of autonomous driving technology, as the Cybercab is Tesla's first purpose-built vehicle for full autonomy and a key step toward its Robotaxi network, which could disrupt ride-hailing and personal transportation. The Cybercab is a two-seat battery-electric vehicle with no manual controls, relying entirely on Tesla's Full Self-Driving (FSD) system, which currently still requires human supervision and is not yet capable of unsupervised autonomous driving.

telegram · zaihuapd · Jul 17, 03:06

**Background**: The Cybercab is part of Tesla's Robotaxi initiative, aiming to deploy a fleet of autonomous vehicles for ride-hailing services. Unlike Tesla's consumer models, it is designed from the ground up for autonomy with no manual driving controls. Tesla has been developing its Full Self-Driving software for years, targeting Level 5 autonomy, but regulatory and technical challenges remain.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tesla_Cybercab">Tesla Cybercab - Wikipedia</a></li>
<li><a href="https://electrek.co/2026/07/06/tesla-cybercab-production-before-autonomy/">Tesla Cybercab: mass-producing a car it can't sell or drive itself | Electrek</a></li>
<li><a href="https://insideevs.com/news/787560/tesla-cybercab-robotaxi-giga-texas-production/">Tesla Begins Cybercab Production. Now Comes The Hard Part</a></li>

</ul>
</details>

**Tags**: `#特斯拉`, `#Cybercab`, `#自动驾驶`, `#Robotaxi`, `#电动汽车`

---

<a id="item-3"></a>
## [Atmosphere detected on Earth-like exoplanet in habitable zone](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

The James Webb Space Telescope has detected an atmosphere on LHS 1140b, a rocky planet in the habitable zone of a red dwarf star 48 light-years away, ruling out the possibility that it is a mini-Neptune. This discovery marks the first time an atmosphere has been confirmed on a rocky planet in the habitable zone of a red dwarf, a key step in the search for life beyond Earth and a demonstration of JWST's power in exoplanet characterization. The detection used JWST's emission spectroscopy during the planet's secondary eclipse. The atmosphere contains helium, suggesting a high escape velocity, and the planet, LHS 1140b, is 48 light-years away.

hackernews · neversaydie · Jul 17, 14:06 · [Discussion](https://news.ycombinator.com/item?id=48947560)

**Background**: The habitable zone is the region around a star where conditions could allow liquid water on a planet's surface. Red dwarfs are small, cool stars, making their habitable zones very close, which often subjects planets to intense stellar radiation. Mini-Neptunes are planets with thick hydrogen-helium atmospheres, unlike rocky Earth-like worlds. The James Webb Space Telescope (JWST) is capable of analyzing exoplanet atmospheres through transit spectroscopy.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mini-Neptune">Mini - Neptune - Wikipedia</a></li>
<li><a href="https://earthsky.org/space/super-earth-mini-neptune-and-sub-neptune-exoplanets-definitions/">Super-Earth, mini - Neptune or sub-Neptune?</a></li>

</ul>
</details>

**Discussion**: Community comments express initial skepticism about LHS 1140b being Earth-like, noting that red dwarfs strip atmospheres. However, the JWST data ruling out a mini-Neptune is acknowledged. Some suggest building a solar lens telescope and discuss interstellar propulsion, while others note the detection of helium indicates a high escape velocity.

**Tags**: `#exoplanet`, `#atmosphere`, `#habitable zone`, `#JWST`, `#red dwarf`

---

<a id="item-4"></a>
## [The State of Open Source AI: A Comprehensive Report](https://stateofopensource.ai/) ⭐️ 8.0/10

Mozilla released a report analyzing the current state and trends in open source artificial intelligence, sparking significant community discussion. The report highlights the growing dominance of open models over closed models in AI, which could reshape the industry and affect major players like OpenAI and Anthropic. The report contains numerous charts and data points, but some community members criticized its presentation as overly reliant on AI-generated content and lacking original analysis.

hackernews · rellem · Jul 17, 14:31 · [Discussion](https://news.ycombinator.com/item?id=48947825)

**Background**: Open source AI refers to artificial intelligence models that are publicly available for use, modification, and distribution, often with permissive licenses. This contrasts with closed, proprietary models from companies like OpenAI and Google. The debate centers on whether open or closed models will drive future innovation and accessibility.

**Discussion**: Community comments are mixed: some celebrate the rapid growth of open models and predict the decline of closed AI companies, while others criticize the report's quality, noting it appears AI-generated and lacks deep insight.

**Tags**: `#open source`, `#artificial intelligence`, `#industry analysis`, `#community discussion`

---

<a id="item-5"></a>
## [Kimi Releases 2.8T Parameter Open-Source Model K3](https://t.me/zaihuapd/42619) ⭐️ 8.0/10

Kimi announced K3, an open-source large language model with 2.8 trillion parameters and up to 1 million tokens of context. It uses a sparse mixture-of-experts architecture with 896 experts, activating 16 per token, and incorporates Kimi Delta Attention and Attention Residuals. If confirmed, K3 would be the largest open-source model ever, with performance claimed to rival top proprietary models. However, the comparisons to likely fictitious models (Claude Fable 5 and GPT-5.6 Sol) undermine credibility. K3 is based on Kimi Delta Attention and Attention Residuals, with a sparse MoE design that activates 16 out of 896 experts per token. The complete weights are promised to be released in the coming days, but the announcement comes from a Telegram channel rather than an official source.

telegram · zaihuapd · Jul 17, 00:02

**Background**: Sparse mixture of experts (MoE) is a technique where the model uses multiple specialized sub-networks (experts) but activates only a few per input, improving efficiency. Kimi Delta Attention is a linear attention variant that enables long-context processing with reduced computational cost. Attention Residuals allow each transformer layer to dynamically combine representations from earlier layers, potentially improving performance.

<details><summary>References</summary>
<ul>
<li><a href="https://jianyuh.github.io/attention/2025/12/13/KDA.html">Linear Attention : Kimi Delta Attention | Jianyu Huang’s Blog</a></li>
<li><a href="https://github.com/MoonshotAI/Attention-Residuals">GitHub - MoonshotAI/ Attention - Residuals · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sparse_mixture-of-experts">Sparse mixture-of-experts</a></li>

</ul>
</details>

**Tags**: `#AI`, `#large language model`, `#open-source`, `#sparse MoE`, `#Kimi`

---