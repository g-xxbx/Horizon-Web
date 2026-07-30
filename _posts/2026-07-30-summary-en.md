---
layout: default
title: "Horizon Summary: 2026-07-30 (EN)"
date: 2026-07-30
lang: en
---

> From 38 items, 12 important content pieces were selected

---

1. [Kimi K3 Open-Weight Model Reaches Frontier with Novel Innovations](#item-1) ⭐️ 9.0/10
2. [Stacked Pull Requests Launch in Public Preview on GitHub](#item-2) ⭐️ 8.0/10
3. [DeepMind's Gemini Robotics 2 Enables Whole-Body Robot Intelligence](#item-3) ⭐️ 8.0/10
4. [Muon Mystery Solved, Old Results Reassessed](#item-4) ⭐️ 8.0/10
5. [OpenAI cuts GPT-5.6 Luna price by 80%](#item-5) ⭐️ 8.0/10
6. [GCC steering committee announces AI contribution policy](#item-6) ⭐️ 8.0/10
7. [Why is everyone trying to build a solid-state battery?](#item-7) ⭐️ 8.0/10
8. [Professor loses potential PhD students due to conference review process](#item-8) ⭐️ 8.0/10
9. [MLVC: Multi-Platform Learned Video Codec for Real-World Deployment](#item-9) ⭐️ 8.0/10
10. [UK Proposes Loosening Apple and Google App Payment Rules](#item-10) ⭐️ 8.0/10
11. [Russia charges Telegram founder Durov with aiding terrorism, issues arrest warrant](#item-11) ⭐️ 8.0/10
12. [EU launches AI gigafactory tender to attract €30 billion investment](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Kimi K3 Open-Weight Model Reaches Frontier with Novel Innovations](https://www.reddit.com/r/MachineLearning/comments/1vaysjf/how_kimi_k3_engineered_its_way_to_the_frontier_r/) ⭐️ 9.0/10

Moonshot AI released Kimi K3, an open-weight model that ranks fourth among 580 models on the Artificial Analysis leaderboard, introducing innovations including Delta Attention, Quantile Balancing, and AgentENV. This achievement shows that open-weight models can compete with proprietary frontier models, significantly lowering barriers for AI research and development. Delta Attention replaces the KV cache in 69 of the 93 layers with a single 128x128 matrix per head, reducing memory for a 1M-token context from 104.6 GiB to 27.2 GiB. Quantile Balancing handles 896 experts per layer without hyperparameter tuning, and AgentENV creates 51 million sandboxes with 133 ms checkpoints and 49 ms resumes for RL training.

reddit · r/MachineLearning · /u/noninertialframe96 · Jul 30, 16:37

**Background**: Open-weight models publicly release their model weights but may not disclose training data or code. Kimi K3 uses a Mixture of Experts (MoE) architecture with 896 experts per layer, which requires efficient load balancing to avoid uneven utilization. The Quantile Balancing method addresses this by computing bias directly from router score margins. AgentENV is a microVM runtime based on Firecracker that provides isolated environments for reinforcement learning.

<details><summary>References</summary>
<ul>
<li><a href="https://jianyuh.github.io/attention/2025/12/13/KDA.html">Linear Attention : Kimi Delta Attention | Jianyu Huang’s Blog</a></li>
<li><a href="https://openathena.ai/blog/quantile-balancing/">Mixture of Experts Quantile Balancing: Validated at 32B-A5B (1e22 FLOPs) Scale | Open Athena</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#open-weight models`, `#attention mechanisms`, `#reinforcement learning`, `#Moonshot AI`

---

<a id="item-2"></a>
## [Stacked Pull Requests Launch in Public Preview on GitHub](https://github.blog/changelog/2026-07-30-stacked-pull-requests-are-now-in-public-preview/) ⭐️ 8.0/10

GitHub has launched stacked pull requests in public preview, allowing developers to create an ordered series of small, reviewable pull requests that build on top of each other. This feature introduces a stacked workflow natively to one of the largest code forges, potentially improving code review efficiency and enabling faster, safer integration of large changes. The feature includes a GitHub CLI extension (`gh stack`) for creating and managing stacks, though the initial release has known issues such as broken merging of entire stacks and re-approval requirements when using squash and merge.

hackernews · tomzorz · Jul 30, 16:26 · [Discussion](https://news.ycombinator.com/item?id=49112232)

**Background**: Stacked pull requests, also known as stacked diffs, are a workflow where a large change is split into a chain of smaller, dependent pull requests. This approach allows each PR to be reviewed and CI-checked independently, reducing merge conflicts and speeding up the development cycle.

<details><summary>References</summary>
<ul>
<li><a href="https://github.blog/changelog/2026-07-30-stacked-pull-requests-are-now-in-public-preview/">Stacked pull requests are now in public preview - GitHub Changelog</a></li>
<li><a href="https://github.github.com/gh-stack/">GitHub Stacked PRs | GitHub Stacked PRs</a></li>
<li><a href="https://docs.github.com/en/pull-requests/how-tos/stacked-pull-requests">Stacked pull requests 🥞 - GitHub Docs</a></li>

</ul>
</details>

**Discussion**: The community has shown great interest, with many praising the workflow improvement. However, some users reported bugs, particularly with merging entire stacks and the need for re-approval on squash merges. The GitHub team responded, acknowledging the issues and promising further updates.

**Tags**: `#github`, `#pull-requests`, `#developer-tools`, `#version-control`, `#workflow`

---

<a id="item-3"></a>
## [DeepMind's Gemini Robotics 2 Enables Whole-Body Robot Intelligence](https://deepmind.google/blog/gemini-robotics-2-brings-whole-body-intelligence-to-robots/) ⭐️ 8.0/10

Google DeepMind has released Gemini Robotics 2, a new AI model integrating Gemini large language models with robots to achieve whole-body intelligence, enabling more natural and capable manipulation using the entire robot body. This marks a major advance in embodied AI, moving from separate perception and control to a unified whole-body model. It could accelerate the development of more adaptive robots for real-world tasks like household assistance and industrial automation. Gemini Robotics 2 is built on Gemini 2.0 and designed for real-time control, but access is currently limited to trusted testers such as Agile Robots and Boston Dynamics. The model still shows limitations in motion fluidity compared to human dexterity.

hackernews · ai2027 · Jul 30, 15:15 · [Discussion](https://news.ycombinator.com/item?id=49111237)

**Background**: Whole-body intelligence in robotics refers to coordinating the entire body—limbs, torso, sensors—for tasks, rather than only using specific end-effectors. Embodied intelligence is the broader concept that intelligent behavior emerges from body-environment interaction. The Gemini Robotics series from DeepMind integrates language, vision, and action capabilities to enable robots to understand natural language and perform complex tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gemini_Robotics">Gemini Robotics</a></li>
<li><a href="https://en.wikipedia.org/wiki/Embodied_intelligence">Embodied intelligence</a></li>
<li><a href="https://deepmind.google/models/gemini-robotics/">Gemini Robotics — Google DeepMind</a></li>

</ul>
</details>

**Discussion**: A DeepMind researcher praised the lab's breadth of research, while others expressed skepticism about robotic actuation and motion fluidity. Some noted that despite current limitations, progress could be rapid, similar to LLMs. A few questioned the practicality of humanoid robots in home environments.

**Tags**: `#robotics`, `#AI`, `#DeepMind`, `#Gemini`, `#embodied intelligence`

---

<a id="item-4"></a>
## [Muon Mystery Solved, Old Results Reassessed](https://www.quantamagazine.org/physicists-solve-a-muon-mystery-now-old-results-dont-add-up-20260729/) ⭐️ 8.0/10

Physicists have resolved the long-standing muon g-2 anomaly, leading to a reinterpretation of previous experimental results. This resolution eliminates a major tension with the Standard Model of particle physics and may shift the direction of future research. The mystery was solved by a new theoretical calculation that reconciled the experimental measurement with the Standard Model prediction.

hackernews · ibobev · Jul 30, 15:22 · [Discussion](https://news.ycombinator.com/item?id=49111305)

**Background**: The muon g-2 experiment measures the anomalous magnetic moment of the muon, a sensitive test of the Standard Model. For decades, there was a noticeable discrepancy between experimental values and theoretical predictions, hinting at possible new physics. The recent breakthrough resolves this discrepancy without invoking new particles.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Muon_g-2">Muon g-2 - Wikipedia</a></li>
<li><a href="https://news.fnal.gov/2025/06/muon-g-2-most-precise-measurement-of-muon-magnetic-anomaly/">Muon g-2 announces most precise measurement of the magnetic anomaly of ...</a></li>

</ul>
</details>

**Discussion**: Comments show relief that the long-standing problem is solved, with a mix of humor about Feynman diagrams and philosophical reflections on scientific paradigms.

**Tags**: `#physics`, `#muon`, `#particle physics`, `#science`, `#paradigm shift`

---

<a id="item-5"></a>
## [OpenAI cuts GPT-5.6 Luna price by 80%](https://openai.com/index/advancing-the-price-performance-frontier-with-gpt-5-6/) ⭐️ 8.0/10

OpenAI announced an 80% cost reduction for GPT-5.6 Luna, its fastest and most affordable model, driven by kernel optimizations and efficiency improvements. This dramatic price drop challenges the notion that AI model costs have plateaued, enabling broader adoption and more intensive usage of LLMs for enterprises and developers. GPT-5.6 Luna supports up to 1 million tokens of context and is one of three tiers in the GPT-5.6 family, alongside Sol and Terra. The 80% reduction comes from 20% lower serving costs and over 15% improvement in token-generation efficiency.

hackernews · tedsanders · Jul 30, 17:15 · [Discussion](https://news.ycombinator.com/item?id=49112867)

**Background**: GPT-5.6 is a model generation from OpenAI, available in three variants: Sol (most capable), Terra (balanced), and Luna (most efficient and cheapest). The price-performance frontier represents the optimal balance between model capability and cost. This announcement marks the first major price cut for the GPT-5.6 line since its launch in July 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/advancing-the-price-performance-frontier-with-gpt-5-6/">Advancing the price - performance frontier with GPT-5.6 | OpenAI</a></li>
<li><a href="https://www.vellum.ai/blog/gpt-5-6-benchmarks-explained">GPT - 5 . 6 Sol vs Terra vs Luna : Which Tier Should You Actually Use?</a></li>

</ul>
</details>

**Discussion**: Community members expressed shock and excitement at the 80% price cut, with some comparing it to the dial-up to broadband transition. Several users noted that Luna was already very cheap and this change makes it even more accessible, though some debated the difficulty of optimally selecting models for different tasks.

**Tags**: `#GPT-5.6`, `#OpenAI`, `#price-performance`, `#AI models`, `#cost reduction`

---

<a id="item-6"></a>
## [GCC steering committee announces AI contribution policy](https://lwn.net/Articles/1086041/) ⭐️ 8.0/10

The GCC steering committee has announced a policy addressing AI-generated contributions to the project, clarifying guidelines for contributors who use AI tools. This policy sets a precedent for major open-source projects dealing with AI contributions, highlighting the need for clear rules to maintain code quality and author accountability. The policy appears to emphasize human oversight and accountability for AI-generated content, with a welcoming approach to guide contributors who may not yet follow the rules.

hackernews · arto · Jul 30, 11:45 · [Discussion](https://news.ycombinator.com/item?id=49108685)

**Background**: GCC (GNU Compiler Collection) is a foundational open-source compiler project that supports multiple languages. As AI coding tools become widespread, projects like GCC must establish policies to ensure contributions remain maintainable and trustworthy.

**Discussion**: The discussion includes a notable quote about AI enabling wealth to access skill without rewarding skill, and some comments suggest that such policies may inadvertently benefit AI companies by ensuring high-quality training data.

**Tags**: `#gcc`, `#open-source`, `#ai policy`, `#community`, `#software development`

---

<a id="item-7"></a>
## [Why is everyone trying to build a solid-state battery?](https://www.construction-physics.com/p/why-is-everyone-trying-to-build-a) ⭐️ 8.0/10

This article explores the technical and practical reasons behind the global push to develop solid-state batteries, including their potential for higher energy density and improved safety over conventional lithium-ion batteries. Solid-state batteries could transform energy storage for electric vehicles, consumer electronics, and military drones by significantly enhancing performance and safety, while also potentially reducing costs in the long run. The article notes that not all solid-state battery types effectively stop dendrite growth; the 'holy grail' is a polymer single-ion conductor with low activation energy. Additionally, existing sodium-sulfur solid electrolyte batteries require operating temperatures above 300°C, limiting their applications.

hackernews · crescit_eundo · Jul 30, 12:38 · [Discussion](https://news.ycombinator.com/item?id=49109193)

**Background**: Solid-state batteries use a solid electrolyte instead of the liquid or gel electrolyte found in traditional lithium-ion batteries. This design can potentially offer higher energy density, longer cycle life, and improved safety by eliminating flammable liquid components. However, challenges such as dendrite formation and high manufacturing costs have hindered widespread commercialization. The technology has garnered significant attention from automakers, electronics companies, and defense sectors for its potential to overcome limitations of current battery technology.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Solid-state_battery">Solid-state battery - Wikipedia</a></li>
<li><a href="https://www.cas.org/resources/cas-insights/solid-state-battery-technology">How solid-state battery technology is changing energy storage | CAS</a></li>
<li><a href="https://www.quantumscape.com/battery-technology/">Solid State Battery Technology | QuantumScape</a></li>

</ul>
</details>

**Discussion**: The community comments provide valuable technical insights, including the different types of solid-state batteries and their varying effectiveness against dendrites. A commenter highlights military drones as a 'killer app' due to the critical importance of energy density for airborne applications. There is also a call for more research and a mention of existing high-temperature sodium-sulfur solid electrolyte batteries.

**Tags**: `#battery technology`, `#energy storage`, `#solid-state`, `#materials science`, `#technology trends`

---

<a id="item-8"></a>
## [Professor loses potential PhD students due to conference review process](https://www.reddit.com/r/MachineLearning/comments/1vawwb8/i_have_lost_three_and_a_half_potential_phd/) ⭐️ 8.0/10

An early-career assistant professor reports that the stressful peer review process at top machine learning conferences has caused three talented undergraduate students to decline PhD opportunities, and a fourth almost did the same. This highlights a systemic flaw in ML academia where the review process not only frustrates researchers but also discourages the next generation of talent. It underscores the urgent need for reform in conference review practices to sustain the field's growth. The professor states that the students' papers were parts of ongoing research well above the acceptance bar, yet they faced rejection after multiple resubmissions, with one paper receiving four unanimous weak accepts being rejected.

reddit · r/MachineLearning · /u/AffectionateLife5693 · Jul 30, 15:30

**Background**: The 'big three' machine learning conferences—NeurIPS, ICML, and ICLR—are the most prestigious venues for publishing ML research. However, due to explosive growth in submissions, the review process has become increasingly strained, leading to randomness and frustration. Studies have analyzed the declining review quality and its impact on the community.

<details><summary>References</summary>
<ul>
<li><a href="https://towardsdatascience.com/some-issues-in-the-review-process-of-machine-learning-conferences-2c19c1eef42f/">Some Issues in the Review Process of Machine Learning Conferences | Towards Data Science</a></li>
<li><a href="https://arxiv.org/abs/2011.12919">[2011.12919] Analyzing the Machine Learning Conference Review Process</a></li>
<li><a href="https://dev.to/valesys/declining-review-quality-at-top-ml-conferences-comparing-icmlneuripsiclr-with-journal-style-iom">Declining Review Quality at Top ML Conferences: Comparing ICML/NeurIPS/ICLR with Journal-Style Venues like TMLR - DEV Community</a></li>

</ul>
</details>

**Tags**: `#academia`, `#peer review`, `#machine learning`, `#conference`, `#PhD students`

---

<a id="item-9"></a>
## [MLVC: Multi-Platform Learned Video Codec for Real-World Deployment](https://www.reddit.com/r/MachineLearning/comments/1vb3xwd/mlvc_multiplatform_learned_video_codec_for/) ⭐️ 8.0/10

MLVC is a learned video codec that achieves cross-platform compatibility by transmitting entropy-model scale parameters through the hyperprior, avoiding the need for bit-exact execution on different NPUs, and runs at ~100 FPS for 360p/540p video on consumer NPUs. This work addresses the critical cross-platform compatibility barrier that has prevented neural video codecs from replacing traditional codecs like H.264 and AV1, potentially enabling practical deployment of AI-based codecs with higher compression efficiency. MLVC transmits entropy-model scale parameters explicitly through the hyperprior, so the neural network itself does not need to run bit-exactly across NPUs. The codec achieves ~100 FPS on consumer NPUs like the Apple M3 Neural Engine, where INT8 operations are simulated using FP16.

reddit · r/MachineLearning · /u/tanelai · Jul 30, 19:40

**Background**: Learned video codecs use neural networks to compress video more efficiently than hand-engineered codecs like H.264 and AV1. However, they require high computational power and face cross-platform incompatibility: small numerical differences between NPUs can cause entropy decoding failures. MLVC overcomes this by making the entropy model robust to such differences without requiring bit-exact execution.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2606.28027">MLVC: A Multi-platform Learned Video Codec for Real-World...</a></li>

</ul>
</details>

**Tags**: `#learned video codec`, `#cross-platform compatibility`, `#neural networks`, `#video encoding`, `#AI codec`

---

<a id="item-10"></a>
## [UK Proposes Loosening Apple and Google App Payment Rules](https://t.me/zaihuapd/42855) ⭐️ 8.0/10

The UK Competition and Markets Authority (CMA) proposed on June 30, 2025, to allow app developers to direct users to payment options outside the Apple App Store and Google Play Store, aiming to reduce fees and foster competition. This could significantly lower costs for developers and consumers, potentially reshaping the mobile app ecosystem by reducing the dominance of Apple and Google's in-app payment systems, which typically charge 15-30% commissions. The CMA also considers requiring Apple to open its NFC technology for contactless payments on iOS. The proposals are under consultation as part of the UK's new digital markets regime, and Apple and Google were already designated as having strategic market status in mobile ecosystems last year.

telegram · zaihuapd · Jul 30, 02:10

**Background**: App stores like Apple's App Store and Google Play typically require developers to use their in-app payment systems, charging commissions of 15-30%. This has been a focus of antitrust scrutiny globally. The UK's Digital Markets, Competition and Consumers Act (DMCC) gives the CMA new powers to regulate firms with "strategic market status". The current proposals are based on that act.

<details><summary>References</summary>
<ul>
<li><a href="https://juejin.cn/pin/7108519404467388423">英 国 竞 争 和 市 场 管 理 局 （ CMA ）上周五表示，针对苹果公司和Al...</a></li>
<li><a href="https://wap.cj.sina.cn/pc/7x24/4962062">英 国 竞 争 与 市 场 管 理 局 ._7x24快讯_新浪财经</a></li>
<li><a href="https://m.zhaochengzang.com/news/58248.html">nfc ...</a></li>

</ul>
</details>

**Tags**: `#应用商店`, `#反垄断`, `#支付规则`, `#苹果`, `#Google`

---

<a id="item-11"></a>
## [Russia charges Telegram founder Durov with aiding terrorism, issues arrest warrant](https://t.me/zaihuapd/42859) ⭐️ 8.0/10

On July 29, the Russian Federal Security Service (FSB) filed criminal charges against Telegram founder Pavel Durov for aiding terrorism under Article 205.1.1.1 of the Criminal Code and placed him on an international wanted list. This unprecedented move directly targets a major tech founder for platform liability, raising questions about legal accountability for content moderation. It could set a dangerous precedent for international tech law and impact Telegram's operations. The FSB specifically alleges that Telegram management refused to delete channels, groups, and bots used by Ukrainian intelligence and terrorist organizations to coordinate attacks in Russia, resulting in casualties and billions of rubles in losses.

telegram · zaihuapd · Jul 30, 03:45

**Background**: Telegram is a popular messaging app that offers public channels and group functionalities. The FSB claims that the platform's management failure to remove content used by terrorist groups constitutes aiding terrorism under Russian criminal law.

**Tags**: `#Telegram`, `#Pavel Durov`, `#terrorism`, `#Russia`, `#encryption`

---

<a id="item-12"></a>
## [EU launches AI gigafactory tender to attract €30 billion investment](https://www.wsj.com/world/europe/eu-opens-call-for-creation-of-local-ai-gigafactories-c286213d) ⭐️ 8.0/10

The European Commission has opened a tender for up to seven AI 'gigafactories', aiming to mobilize approximately €30 billion in total investment, with €10 billion coming from EU and member state funds. This initiative marks a major policy push to boost Europe's competitiveness in AI, helping close the gap with the US and China. It will provide massive computing power for training complex AI models, benefiting European startups, researchers, and industry. The tender covers two phases: site selection and expansion. Bids are due November 12, winners announced by July 2027, and facilities must be operational within 18 months of contract signing. The gigafactories are expected to be equipped with around 100,000 advanced AI chips.

telegram · zaihuapd · Jul 30, 11:50

**Background**: AI gigafactories are large-scale computing facilities dedicated to training the most complex AI models. They require massive numbers of advanced AI chips (e.g., GPUs) and provide computing power, data access, and storage services for AI companies and researchers. The EU is investing to catch up with the US and China in AI infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://www.esmchina.com/news/12780.html">豪掷2000亿欧元！欧盟AI超级工厂计划曝光-国际电子商情</a></li>
<li><a href="https://m.thepaper.cn/newsDetail_forward_30139469">10万颗先进AI芯片，撬动1.5万亿，欧盟官宣AI超级工厂计划</a></li>
<li><a href="https://www.industrysourcing.cn/article/465106">10万颗AI芯片撬动1.5万亿！欧盟官宣AI超级工厂计划_荣格工业资源网</a></li>

</ul>
</details>

**Tags**: `#EU`, `#AI`, `#investment`, `#technology-policy`, `#infrastructure`

---