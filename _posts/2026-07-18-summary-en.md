---
layout: default
title: "Horizon Summary: 2026-07-18 (EN)"
date: 2026-07-18
lang: en
---

> From 38 items, 9 important content pieces were selected

---

1. [GPT-5.6 Prompt Closes 30-Year Convex Optimization Gap](#item-1) ⭐️ 9.0/10
2. [LG monitors force-install software via Windows Update without consent](#item-2) ⭐️ 9.0/10
3. [Moonshot AI Releases Kimi K3: 2.8T Open-Source Model Tops Frontend Code Arena](#item-3) ⭐️ 9.0/10
4. [StackOverflow Decline: AI or Platform Policies?](#item-4) ⭐️ 8.0/10
5. [PHK's Farewell Reflects on Bikeshedding and Open Source Wisdom](#item-5) ⭐️ 8.0/10
6. [Meta in Talks to Rent $10B AI Compute to Anthropic](#item-6) ⭐️ 8.0/10
7. [SpaceX in Talks to Provide AI Computing to Pentagon](#item-7) ⭐️ 8.0/10
8. [US Considers FINRA-Like AI Model Watchdog](#item-8) ⭐️ 8.0/10
9. [San Francisco Orders Apple and Google to Remove 'Nudify' Apps](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [GPT-5.6 Prompt Closes 30-Year Convex Optimization Gap](https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/) ⭐️ 9.0/10

Researchers used a single prompt with GPT-5.6 to solve a long-standing open problem in convex optimization, closing a gap that had persisted for 30 years. The result was communicated as a real contribution to the field, validated by the mathematical community. This breakthrough demonstrates that AI can make meaningful contributions to advanced mathematical research, potentially accelerating progress in optimization and related fields. It also signals a shift in how mathematicians may approach open problems, as AI can now tackle problems that were previously considered beyond its reach. The solved problem concerns the time complexity of minimizing convex Lipschitz functions over spherical domains, a restriction that is not fundamental as any bounded domain can be transformed. The proof was reportedly obtained using GPT-5.6's Sol Pro variant rather than the Ultra version, highlighting differences in model capability.

hackernews · mbustamanter · Jul 18, 13:00 · [Discussion](https://news.ycombinator.com/item?id=48957779)

**Background**: Convex optimization is a subfield of mathematical optimization where the objective function is convex and the feasible set is convex, enabling efficient algorithms with polynomial-time solutions for many problem classes. A 30-year gap in this field referred to an open question about the optimal convergence rate for certain convex optimization algorithms, which had resisted solution despite extensive efforts. This result adds to a growing list of AI-assisted mathematical proofs following similar achievements like OpenAI's CDC proof.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Convex_optimization">Convex optimization</a></li>

</ul>
</details>

**Discussion**: The community largely recognized the result as a genuine contribution, though some noted it is more niche than the cyclic double cover proof. Commenters debated whether this marks a turning point where AI handles medium-hanging fruit, freeing human researchers for more creative work, while others expressed concerns about the impact on junior researchers who traditionally learn by tackling such problems. There was also discussion about the difference between GPT-5.6 Sol Pro and Ultra, with speculation about multi-agent orchestration.

**Tags**: `#AI`, `#convex optimization`, `#mathematics`, `#breakthrough`, `#GPT`

---

<a id="item-2"></a>
## [LG monitors force-install software via Windows Update without consent](https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent) ⭐️ 9.0/10

Reports reveal that LG monitors trigger Windows Update to silently install LG extension and LG Monitor App Installer packages as soon as the monitor is connected via HDMI, without any user interaction or consent. This behavior undermines user control and security, as the installed software runs with system privileges, persists across boots, and can display third-party ads like McAfee, raising serious privacy and supply-chain concerns. The installation occurs automatically upon connecting an LG monitor, even if previously connected, and the installed app has internet access and full system access without sandboxing.

hackernews · baranul · Jul 18, 10:21 · [Discussion](https://news.ycombinator.com/item?id=48956688)

**Background**: Windows Update distributes driver and software packages from hardware vendors, and the Display Data Channel (DDC/CI) allows monitors to communicate with the PC, which can trigger automatic downloads. LG is exploiting this mechanism to deliver unwanted software.

<details><summary>References</summary>
<ul>
<li><a href="https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent">LG monitors silently install software through Windows Update without user consent - VideoCardz.com</a></li>
<li><a href="https://cybersecuritynews.com/windows-update-installs-lg-monitor-app-pushes-mcafee-ads/">Windows Update Silently Installs LG Monitor App That Pushes McAfee Ads</a></li>
<li><a href="https://en.wikipedia.org/wiki/Display_Data_Channel">Display Data Channel - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community expressed strong outrage, comparing the behavior to malware and noting the severe privacy and security implications. Users shared workarounds via Group Policy or Device Installation Settings to block automatic downloads of manufacturer apps.

**Tags**: `#security`, `#windows`, `#privacy`, `#lg-monitors`, `#supply-chain-attack`

---

<a id="item-3"></a>
## [Moonshot AI Releases Kimi K3: 2.8T Open-Source Model Tops Frontend Code Arena](https://t.me/zaihuapd/42637) ⭐️ 9.0/10

Moonshot AI has released Kimi K3, the world's first open-source 2.8 trillion parameter model, featuring Kimi Delta Attention and Attention Residuals architecture, native vision capabilities, and a 100 million token context window. It achieved first place in the Frontend Code Arena benchmark with a score of 1679, surpassing Fable 5 and moving from 18th place with its predecessor Kimi k2.6. This release demonstrates that open-source models can compete with and surpass proprietary frontier models on specialized benchmarks like frontend coding. It also highlights the rapid advancement of Chinese AI labs in the global AI race, potentially lowering costs and accelerating innovation in AI-assisted software development. K3 uses a novel architecture combining Kimi Delta Attention (a linear attention module) and Attention Residuals (a drop-in replacement for standard residual connections). The model is open-source, with pricing at $3/$15 per 1M tokens for input/output, comparable to proprietary models like ChatGPT 5.6 and Opus 4.8.

telegram · zaihuapd · Jul 18, 02:29

**Background**: Kimi Delta Attention is an expressive linear attention module that extends Gated DeltaNet with a finer-grained gating mechanism, enabling more effective use of limited finite-state RNN memory. Attention Residuals allow each layer to selectively aggregate information from all previous layers, improving model depth efficiency. Frontend Code Arena is a benchmark evaluating AI models on frontend coding tasks, where Kimi K3 scored 1679, ranking first in 6 out of 7 categories.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2510.26692">[2510.26692] Kimi Linear: An Expressive, Efficient Attention Architecture</a></li>
<li><a href="https://github.com/MoonshotAI/Attention-Residuals">GitHub - MoonshotAI/ Attention - Residuals · GitHub</a></li>
<li><a href="https://digg.com/tech/we56zqdp">Chinese model Kimi-K3 tops Frontend Code Arena benchmark · Digg</a></li>

</ul>
</details>

**Discussion**: Commenters noted that distillation from frontier labs was inevitable and that open-source models will continue to challenge proprietary ones. Some reported high usage time and cost when using Kimi K3, while others debated the implications of potential government restrictions on open-weight models. There was also discussion comparing pricing and performance with proprietary models like ChatGPT 5.6 and Opus 4.8.

**Tags**: `#AI`, `#Large Language Models`, `#Open Source`, `#2.8T`, `#Frontend Coding`

---

<a id="item-4"></a>
## [StackOverflow Decline: AI or Platform Policies?](https://data.stackexchange.com/stackoverflow/query/1953768#graph) ⭐️ 8.0/10

A data query graph on Stack Exchange Data Explorer reveals a sustained decline in StackOverflow activity since 2014, sparking debate about whether the drop is due to AI coding assistants or the platform's own policies. This analysis matters because it challenges the simplistic narrative that AI alone is killing StackOverflow, highlighting the role of community management and platform design in the decline of online communities. The graph indicates that activity peaked around 2014, long before ChatGPT launched, and declined further after StackOverflow was acquired by Prosus in 2021. Commenters argue that the platform's strict moderation and lack of community building were major factors.

hackernews · secretslol · Jul 18, 11:12 · [Discussion](https://news.ycombinator.com/item?id=48956949)

**Background**: StackOverflow is a popular Q&A site for programmers, known for its strict moderation that prioritizes high-quality questions and answers. However, this approach has been criticized for creating a hostile environment for newcomers. Meanwhile, AI coding assistants like ChatGPT offer instant answers, reducing the need to visit the site. The decline in activity reflects a broader shift in how developers seek help.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stack_Overflow">Stack Overflow - Wikipedia</a></li>
<li><a href="https://stackoverflow.blog/2024/05/29/developers-get-by-with-a-little-help-from-ai-stack-overflow-knows-code-assistant-pulse-survey-results/">Developers get by with a little help from AI: Stack Overflow Knows code assistant pulse survey results - Stack Overflow</a></li>
<li><a href="https://www.reddit.com/r/programming/comments/1hyz63l/coding_help_on_stackoverflow_dives_as_ai/">r/programming on Reddit: Coding help on StackOverflow dives as AI assistants rise</a></li>

</ul>
</details>

**Discussion**: Commenters largely attribute the decline to StackOverflow's own policies, noting that the platform alienated new users with high barriers to participation and a culture that discourages conversation. Some point out that the decline started before AI became prevalent, suggesting that internal issues were the primary cause.

**Tags**: `#stackoverflow`, `#AI impact`, `#community management`, `#online communities`, `#data analysis`

---

<a id="item-5"></a>
## [PHK's Farewell Reflects on Bikeshedding and Open Source Wisdom](https://queue.acm.org/detail.cfm?id=3818307) ⭐️ 8.0/10

Poul-Henning Kamp, a legendary BSD developer, published a farewell article in ACM Queue that reflects on the concept of bikeshedding and offers insights from his decades of experience in open source development. The article provides rare, candid perspectives from a key figure in open source, sparking important discussions about project management, community dynamics, and the pitfalls of triviality in software development. PHK is known for creating the MD5crypt password hashing algorithm in 1994, which predates bcrypt and other modern schemes. The term 'bikeshedding' was popularized by Kamp in the BSD community in 1999, based on Parkinson's law of triviality.

hackernews · Ygg2 · Jul 18, 17:27 · [Discussion](https://news.ycombinator.com/item?id=48960155)

**Background**: Bikeshedding, or the law of triviality, describes the tendency to spend disproportionate time on trivial but easy-to-understand issues while neglecting more important complex ones. The concept was introduced by C. Northcote Parkinson in 1957 and later became popular in software development through Kamp's writings. This phenomenon is particularly relevant in open source projects where many contributors may focus on superficial aspects due to their accessibility.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bikeshedding">Bikeshedding</a></li>

</ul>
</details>

**Discussion**: Commenters shared diverse reactions: one suggested that reversible decisions should just be made instinctively to avoid bikeshedding, while another highlighted PHK's MD5crypt contribution. A third humorously complained that replacing bikeshedding with a JIRA board made things worse, and one reader initially reacted negatively but later appreciated the article's depth.

**Tags**: `#open source`, `#bikeshedding`, `#PHK`, `#project management`, `#culture`

---

<a id="item-6"></a>
## [Meta in Talks to Rent $10B AI Compute to Anthropic](https://www.nytimes.com/2026/07/17/technology/meta-anthropic-ai-computing-power.html) ⭐️ 8.0/10

Meta is negotiating to rent out its AI data center capacity to Anthropic in a potential deal worth $10 billion over two years. The talks, initiated by Anthropic in June, are still in early stages and may not lead to a final agreement. This potential deal highlights the immense scarcity of AI computing power, driving strategic partnerships between AI labs and tech giants. For Meta, renting out spare capacity could generate new revenue and ease investor concerns over its massive infrastructure spending. The deal would involve monthly payments, and either party could exit early. Meta plans to spend up to $145 billion this year, largely on AI and data centers.

telegram · zaihuapd · Jul 18, 01:14

**Background**: Anthropic is an AI safety-focused company behind the Claude large language model, founded by former OpenAI employees in 2021. As of May 2026, it was valued at $965 billion, reflecting the intense market demand for cutting-edge AI. Training and running advanced AI models require enormous compute resources, which are increasingly scarce and expensive, driving companies like Meta to invest billions in infrastructure and potentially rent out capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Meta`, `#Anthropic`, `#computing infrastructure`, `#business deal`

---

<a id="item-7"></a>
## [SpaceX in Talks to Provide AI Computing to Pentagon](https://www.wsj.com/tech/ai/spacex-in-talks-to-provide-computing-power-for-pentagons-ai-push-15e752e4) ⭐️ 8.0/10

SpaceX is in negotiations with the U.S. Department of Defense to provide data center computing power for running AI models, in a deal that could be worth tens of billions of dollars. The talks are still ongoing and could fall through. This deal would mark SpaceX's deepening relationship with the Pentagon and highlight the growing demand for AI computing in national security. It could also intensify competition among cloud providers seeking defense contracts. The Pentagon has recently approved SpaceX, Amazon, Google, Microsoft, and Oracle to use AI models in classified environments. SpaceX has also signed similar computing agreements with Anthropic and Google in recent months and plans to expand its cloud business.

telegram · zaihuapd · Jul 18, 01:44

**Background**: AI computing power (AI compute) is the computational capacity needed to train and run AI models. Cloud computing provides on-demand access to computing resources. The Pentagon is accelerating its adoption of cloud computing to support AI applications in national security and daily operations. SpaceX, traditionally a space company, is expanding into cloud services, potentially leveraging its own infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://www.elecfans.com/d/6442715.html">AI 算 力 ：智能时代的核心驱动 力 -电子发烧友网</a></li>
<li><a href="https://f5.pm/go-200169.html">机 密 计 算 的崭露头角与未来前景</a></li>

</ul>
</details>

**Tags**: `#AI`, `#云计算`, `#国防`, `#SpaceX`, `#五角大楼`

---

<a id="item-8"></a>
## [US Considers FINRA-Like AI Model Watchdog](https://www.bloomberg.com/news/articles/2026-07-17/us-considers-creating-finra-like-watchdog-to-vet-top-ai-models) ⭐️ 8.0/10

The Trump administration is considering creating an independent AI oversight body modeled after the Financial Industry Regulatory Authority (FINRA) to vet top AI models for safety before release. The plan, led by Treasury Secretary Scott Bessent, is under review by White House Chief of Staff Susie Wiles. This move would address Wall Street's cybersecurity concerns and Silicon Valley's dissatisfaction with ad hoc government controls, giving both industries more say in setting safety standards. It signals a major policy shift toward formalizing AI regulation in the U.S. The plan is still under discussion and has not been finalized; President Trump has not yet reviewed it. Previously, Anthropic and OpenAI objected to U.S. government requests to modify or delay their latest models. The proposal aligns with a suggestion from Google DeepMind CEO Demis Hassabis for an industry-funded independent regulator.

telegram · zaihuapd · Jul 18, 05:45

**Background**: FINRA is a self-regulatory organization (SRO) overseen by the U.S. Securities and Exchange Commission (SEC), responsible for regulating brokerage firms. The proposal would create a similar SRO for AI, funded by industry but with government oversight. Inside the administration, there are disagreements between those favoring an independent agency like the FDA and those preferring a lighter industry guidance framework.

<details><summary>References</summary>
<ul>
<li><a href="https://goodinfo.net/posts/ai-tech/white-house-considers-ai-model-vetting-may-2026/">白宫考虑在 AI 模 型 发布前进行 安 全 审 查 | 全 球 全 景日报 | goodinfo.net</a></li>

</ul>
</details>

**Tags**: `#AI监管`, `#特朗普政府`, `#FINRA`, `#AI安全`, `#政策`

---

<a id="item-9"></a>
## [San Francisco Orders Apple and Google to Remove 'Nudify' Apps](https://techcrunch.com/2026/07/17/apple-and-google-ordered-to-purge-nudify-apps-from-app-stores/) ⭐️ 8.0/10

San Francisco District Attorney David Chiu has ordered Apple and Google to remove dozens of AI-powered 'nudify' apps from their app stores that create non-consensual intimate deepfake images. This action highlights the growing legal and ethical challenges posed by AI-generated deepfakes and underscores platform responsibility in preventing abuse. It could set a precedent for regulating non-consensual synthetic media and impact how tech companies handle harmful content. The district attorney's letter states that the companies may have made millions of dollars from these apps and face civil penalties. Apple has removed three apps and terminated associated developer accounts, while Google has suspended five Play Store apps.

telegram · zaihuapd · Jul 18, 08:45

**Background**: Nudify apps use AI deepfake technology to alter photos of individuals, typically women, to appear nude without consent. Over 90% of deepfake videos online are non-consensual pornographic content. Several countries have enacted laws to criminalize such deepfakes. Tech companies face increasing pressure to proactively police their platforms for harmful AI-generated content.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nudify_apps">Nudify apps</a></li>
<li><a href="https://medium.com/@shreyasinha551/the-hidden-crisis-how-non-consensual-deepfakes-are-weaponizing-womens-images-63123ee61417">The Hidden Crisis: How Non - Consensual Deepfakes Are... | Medium</a></li>
<li><a href="https://dig.watch/updates/non-consensual-deepfakes-consent-and-power-in-synthetic-media">Non - consensual deepfakes , consent, and... | Digital Watch Observatory</a></li>

</ul>
</details>

**Tags**: `#AI ethics`, `#deepfakes`, `#platform regulation`, `#privacy`, `#Apple`

---