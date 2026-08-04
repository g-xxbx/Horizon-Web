---
layout: default
title: "Horizon Summary: 2026-08-04 (EN)"
date: 2026-08-04
lang: en
---

> From 41 items, 11 important content pieces were selected

---

1. [Mistral releases Shieldstral, a 3B open-weights multimodal moderation model](#item-1) ⭐️ 8.0/10
2. [Waymo's Driverless Ride-Hailing Opens to Everyone in Dallas](#item-2) ⭐️ 8.0/10
3. [Keyv and Related npm Packages Compromised in Shai-Hulud Supply Chain Attack](#item-3) ⭐️ 8.0/10
4. [Xbox Outage Blocks Disc Games, Reigniting Digital Ownership Debate](#item-4) ⭐️ 8.0/10
5. [Apple Expands Lawsuit, Says More Ex-Employees May Have Leaked Data to OpenAI](#item-5) ⭐️ 8.0/10
6. [Engineering Harnesses for Self-Improving AI Agents](#item-6) ⭐️ 8.0/10
7. [MiniMax-H3 Omni-Modal Model Ported to MLX for Apple Silicon](#item-7) ⭐️ 8.0/10
8. [Russia Mandates Third-Party App Stores Like RuStore on Apple Devices from 2025](#item-8) ⭐️ 8.0/10
9. [Cloudflare Drops Third-Party Security Tools, Uses $58/Month Claude for Bug Bounty Triage](#item-9) ⭐️ 8.0/10
10. [Google Builds $200B Wall Street Financing Machine for Anthropic's AI Chips](#item-10) ⭐️ 8.0/10
11. [China's First Mandatory L3/L4 Autonomous Driving Safety Standard Set for 2027](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Mistral releases Shieldstral, a 3B open-weights multimodal moderation model](https://mistral.ai/news/shieldstral/) ⭐️ 8.0/10

Mistral released Shieldstral, a 3B-parameter open-weights multimodal safety classifier that performs content moderation on text and image inputs. According to Mistral, it outperforms models up to 7x its size. This provides platform operators a cost-effective, customizable moderation solution that can be self-hosted and adapted to specific policies, addressing a practical bottleneck for social and image-sharing services. It also signals a trend toward smaller, fine-tuned specialist models over frontier-scale general models. Shieldstral uses natural-language policy questions and returns a yes/no classification, with the moderation policy passed in the request field rather than baked into weights. The model's roadmap includes multilingual coverage, longer-document robustness, and broader multimodal safety.

hackernews · riadsila · Aug 4, 16:36 · [Discussion](https://news.ycombinator.com/item?id=49171268)

**Background**: Open-weight models release trained weights so anyone can download and run them, but they typically omit training code and datasets, distinguishing them from fully open-source AI. Multimodal content moderation analyzes text, images, and other signals to enforce platform policies. Shieldstral is an example of a compact model that embeds policy at inference time, allowing flexible moderation without retraining.

<details><summary>References</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral. | Mistral AI</a></li>
<li><a href="https://docs.mistral.ai/models/model-cards/shieldstral-1-0">Shieldstral 1.0 - docs.mistral.ai</a></li>
<li><a href="https://www.unite.ai/mistrals-shieldstral-packs-policy-adaptive-safety-screening-into-3b-parameters/">Mistral’s Shieldstral Packs Policy-Adaptive Safety Screening ...</a></li>

</ul>
</details>

**Discussion**: Community comments ask whether Shieldstral supports arbitrary rulesets or just big-tech style moderation, and compare it to OpenAI's omni-moderation. One user jokes it should be named 'Safestral' and praises Mistral's strategy of focused smaller models. Another sees it as a realistic, cost-effective solution for content moderation in user-generated-content platforms.

**Tags**: `#AI`, `#content moderation`, `#open-weights`, `#Mistral`, `#multimodal`

---

<a id="item-2"></a>
## [Waymo's Driverless Ride-Hailing Opens to Everyone in Dallas](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 8.0/10

Waymo announced that its fully driverless ride-hailing service is now open to everyone in Dallas, Texas. This marks the latest expansion of the company's autonomous vehicle operations into a major Texas metro area. Opening to the general public in Dallas gives more residents direct access to fully driverless transportation in a sprawling, car-dependent region. It also fuels broader public debate over how autonomous vehicles will shape urban policy, safety, and housing affordability. Dallas-Fort Worth is one of the largest metroplexes in the US, with low density and few public transit options, making it a demanding environment for driverless technology. Community commenters also raised unresolved legal questions about liability, insurance, and criminal responsibility when an autonomous vehicle is involved in an incident.

hackernews · xnx · Aug 4, 18:29 · [Discussion](https://news.ycombinator.com/item?id=49172836)

**Background**: Waymo is an autonomous vehicle company that operates a driverless ride-hailing service, with vehicles that have no safety driver behind the wheel. The company has been gradually expanding its service to more cities, and community comments indicate Waymo cars have already become a familiar sight in areas such as Los Angeles.

**Discussion**: Community comments highlight both enthusiasm and open questions. Some residents praise Waymo vehicles as predictable, safe road participants and note potential benefits for a sprawling region like Dallas-Fort Worth, while a commercial real estate professional argues driverless cars could serve as an effective affordable housing policy. Others raise unresolved legal questions about fines, insurance, and criminal liability when a driverless car breaks the law or causes harm.

**Tags**: `#autonomous-vehicles`, `#waymo`, `#transportation`, `#urban-policy`, `#robotics`

---

<a id="item-3"></a>
## [Keyv and Related npm Packages Compromised in Shai-Hulud Supply Chain Attack](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 8.0/10

Attackers compromised the GitHub account of the Keyv maintainer and used that access to push credential-stealing malware across the maintainer's entire npm package portfolio. This is part of the active Shai-Hulud worm campaign targeting the npm ecosystem. Keyv has roughly 127 million weekly downloads on npm, making this a highly impactful supply chain attack that can compromise many downstream projects. It highlights how a single maintainer account compromise can quickly poison the open-source ecosystem and urges developers to audit dependencies and disable install hooks. In the Keyv incident, the worm poisoned 353 versions across 79 package names while repository hooks remained present. Pre-install/post-install hooks played a key role in the infection, and the worm is self-replicating, stealing developer and CI credentials.

hackernews · cimi_ · Aug 4, 11:01 · [Discussion](https://news.ycombinator.com/item?id=49166874)

**Background**: npm packages are open-source JavaScript libraries installed via the npm registry, often with automatic install scripts. A supply chain attack occurs when attackers compromise a maintainer account or a package to inject malware that spreads to every project depending on it. Shai-Hulud is a self-replicating worm first reported in September 2025, and it has been compromising npm packages at scale by abusing install hooks to deliver credential-stealing payloads. Developers are advised to audit package integrity and consider disabling install scripts.

<details><summary>References</summary>
<ul>
<li><a href="https://cybersecuritynews.com/keyv-npm-package-compromised/">Keyv npm Package with 127M Weekly Downloads Compromised in ...</a></li>
<li><a href="https://thehackernews.com/2026/08/keyv-linked-npm-worm-poisons-hundreds.html">Keyv-Linked npm Worm Poisons Hundreds of Packages, Plants ...</a></li>
<li><a href="https://unit42.paloaltonetworks.com/npm-supply-chain-attack/">"Shai-Hulud" Worm Compromises npm Ecosystem in Supply Chain Attack (Updated November 26)</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration with npm's reliance on install hooks, with one suggesting a moratorium on new pre-install/post-install hooks. Developers shared practical mitigation tips, such as setting `min-release-age=5` in `.npmrc` and using grep to detect compromised packages in node_modules. Overall sentiment is concerned but action-focused.

**Tags**: `#security`, `#npm`, `#supply-chain`, `#open-source`, `#malware`

---

<a id="item-4"></a>
## [Xbox Outage Blocks Disc Games, Reigniting Digital Ownership Debate](https://birchtree.me/blog/xbox-goes-down-you-cant-play-games-you-own-on-disc/) ⭐️ 8.0/10

An Xbox network outage recently left users unable to launch disc-based games they own, as the console performed an online entitlement check before allowing play. The incident sparked widespread discussion about how physical media ownership can be undermined by always-online DRM. This matters because it shows that even physical game purchases can become unplayable during server outages, undermining the notion of true ownership. It affects all gamers and intensifies the ongoing debate over DRM, digital rights, and game preservation, with the community deeply divided on the issue. The outage primarily affected Xbox consoles with disc-based games installed, as the system's mandatory online check tied to account entitlements could not be completed. Notably, Microsoft had previously claimed that a 2022 update removed the online verification requirement for most installed disc games, but this incident proves that some titles or scenarios still enforce connectivity checks.

hackernews · surprisetalk · Aug 4, 12:01 · [Discussion](https://news.ycombinator.com/item?id=49167448)

**Background**: DRM (Digital Rights Management) refers to technologies used to prevent unauthorized copying and distribution of digital media, often requiring an internet connection to 'phone home' and verify ownership. In gaming, this can mean that even physical discs contain a license that must be checked online, so a server outage can block gameplay. Microsoft had required online checks for Xbox disc installations since 2013, but relaxed this in 2022 for most games; the recent outage reveals that such checks continue to exist in certain cases.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gog.com/blog/what-exactly-is-drm-in-video-games-and-why-should-you-care/">Understanding DRM in Games: Impact and Solutions</a></li>
<li><a href="https://www.flatpanelshd.com/news.php?subaction=showfull&id=1663671757">Microsoft backtracks on controversial DRM scheme for Xbox game discs - FlatpanelsHD</a></li>
<li><a href="https://www.theshortcut.com/p/microsoft-has-fixed-its-xbox-drm-problem">Microsoft has stealthily fixed its Xbox DRM problem</a></li>

</ul>
</details>

**Discussion**: The comments reflect strong criticism of current DRM practices and nostalgia for older consoles, with users arguing that ownership should mean the ability to play permanently, offline, and across devices. One user described how launching Halo on Steam forced Microsoft account creation, captcha, and login friction, while another pointed out that PS3-era online games still work today with better latency. Many commenters emphasized that the core issue is not physical versus digital media, but preserving fundamental ownership rights like resale, backup, lending, and long-term playability.

**Tags**: `#gaming`, `#DRM`, `#digital-rights`, `#ownership`, `#Xbox`

---

<a id="item-5"></a>
## [Apple Expands Lawsuit, Says More Ex-Employees May Have Leaked Data to OpenAI](https://techcrunch.com/2026/08/04/apple-says-more-ex-employees-may-have-taken-confidential-data-to-openai/) ⭐️ 8.0/10

Apple has broadened its ongoing lawsuit to allege that more former employees may have taken confidential data to OpenAI, beyond the original defendant. The expanded claim includes the downloading of highly sensitive technical documents from Apple's systems. This escalation underscores the intensifying legal friction between Apple and OpenAI, with implications for talent mobility and trade-secret protection across the AI industry. It also highlights the competitive stakes in proprietary hardware and AI development among major tech players. According to legal filings, the original employee exploited an authentication bug to access Apple's confidential third-party cloud repository and downloaded at least thirty-seven sensitive documents. Apple also did not concede that the 'residual access' left to former employees stemmed from poor security practices on its part.

hackernews · thewebguyd · Aug 4, 15:37 · [Discussion](https://news.ycombinator.com/item?id=49170479)

**Background**: Apple has a long history of aggressively defending its intellectual property, including suing former employees and competitors over alleged trade-secret theft. This lawsuit stems from allegations that an ex-employee brought confidential material to OpenAI, which is developing advanced AI and reportedly venturing into custom hardware. The case may influence how confidentiality agreements are applied when employees move to AI-focused rivals.

**Discussion**: Commenters are divided: some view the lawsuit as a typical Apple intimidation tactic, recalling Steve Jobs' threats to sue Nest over poaching, while others see OpenAI's hardware ambitions as a vanity project that litigation might unintentionally kill. Another commenter counters that the allegations involve documented screenshots, not just employees' memory, and others mock OpenAI CEO Sam Altman for criticizing Apple's security practices.

**Tags**: `#Apple`, `#OpenAI`, `#lawsuit`, `#employee confidentiality`, `#AI industry`

---

<a id="item-6"></a>
## [Engineering Harnesses for Self-Improving AI Agents](https://lilianweng.github.io/posts/2026-07-04-harness/) ⭐️ 8.0/10

On July 4, 2026, Lilian Weng published a technical post exploring how to engineer 'harnesses'—the prompts, tools, skills, and other scaffolding around an LLM—so AI agents can improve their own performance. The post focuses on fitness functions, tool optimization, and optimization loops for large codebases. This matters because improving the harness—rather than retraining model weights—is emerging as a key lever to boost agent performance, quality, and cost efficiency. Developers building production agents and coding assistants will be directly affected as the community moves toward treating prompts and code as a new training paradigm. Key details include the need for a generic, reliable, and accurate fitness function for codebases, plus letting agents read production traces, write their own tools, and use eval/test splits to avoid reward hacking. The post also positions harness optimization as more sample-efficient than weight training, since causal theories can outperform correlations.

hackernews · tosh · Aug 4, 06:17 · [Discussion](https://news.ycombinator.com/item?id=49164896)

**Background**: Harness engineering is the discipline of designing the constraints, feedback loops, tools, and verification around an AI agent to make it reliable and production-ready. Traditionally LLM progress centered on model weights, but harness engineering treats the surrounding code and prompts as an optimization target in itself, using techniques such as trace analysis and AI-generated tooling. This post reflects the broader trend of 'self-improving AI agents', where agents use RL, verifiers, and search to improve their own behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://harness-engineering.ai/">Home | Harness Engineering</a></li>
<li><a href="https://www.agent-engineering.dev/article/harness-engineering-in-2026-the-discipline-that-makes-ai-agents-production-ready">What Is Harness Engineering? Guide to Reliable AI Agents ...</a></li>

</ul>
</details>

**Discussion**: The discussion is largely positive and practical. One commenter insists that building a generic fitness function for codebases is the first step toward agent-driven harness optimization; another reports that auto-research for harnesses works surprisingly well when agents read traces, write their own tools, and use val/test splits. Others speculate about harnesses generating their own RLHF/DPO datasets to fine-tune the models they run, while one commenter jokingly calls it the 'quest for Torment Nexus'.

**Tags**: `#AI agents`, `#harness engineering`, `#LLM`, `#self-improvement`, `#software engineering`

---

<a id="item-7"></a>
## [MiniMax-H3 Omni-Modal Model Ported to MLX for Apple Silicon](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 8.0/10

MiniMax released MiniMax-H3, a general-purpose omni-modal generative system that accepts text, images, audio, and video to generate up to 15-second video clips with audio. A new Python package, PipeNetwork/minimax-h3-mlx, ports the model to MLX so it runs locally on Apple Silicon; Simon Willison demonstrated it on an M5 Max MacBook Pro. This makes a state-of-the-art omni-modal video generation model accessible to individual developers on consumer Apple hardware, without relying on cloud APIs. It demonstrates the growing ecosystem of MLX ports that bring large generative models to local, private, and offline workflows. The model requires downloading roughly 115 GB of model files, and generating a 15-second clip took just under 45 minutes on an M5 Max. The initial output had speech-like audio artifacts because no prompt guidance was provided for the audio; MiniMax publishes a video prompt writing guide that explains how to control audio and other aspects.

rss · Simon Willison · Aug 4, 19:10

**Background**: MiniMax-H3 is an open-weight, omni-modal generation model that jointly understands multimodal contexts spanning text, images, video, and audio. It generates video with native stereo audio at up to 2K resolution and supports lengths of 4 to 15 seconds. MLX is an array framework from Apple designed for efficient machine learning on Apple silicon, leveraging the unified memory architecture; it provides a NumPy-like API that makes ports like this practical.

<details><summary>References</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H3: An Open Model Breaking the Boundaries Between ...</a></li>
<li><a href="https://mlx-framework.org/">MLX</a></li>
<li><a href="https://huggingface.co/MiniMaxAI/MiniMax-H3">MiniMaxAI/ MiniMax - H 3 · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#MLX`, `#MiniMax`, `#video-generation`, `#omni-modal`, `#Apple-Silicon`

---

<a id="item-8"></a>
## [Russia Mandates Third-Party App Stores Like RuStore on Apple Devices from 2025](https://t.me/zaihuapd/42963) ⭐️ 8.0/10

The Russian State Duma passed a new law, effective September 1, 2025, requiring Apple and Google to allow installation of the Russian third-party app store RuStore on devices such as iPhone and iPad, and forbidding them from restricting its installation or updates. This law forces major platform holders like Apple and Google to open their ecosystems in the Russian market, challenging their app store monopolies and potentially setting a precedent for regulators in other countries. It directly affects app distribution, developer pricing, and payment methods, impacting both local developers and global tech policy debates. The law also prohibits vendors from blocking installation or updates of third-party software, restricting alternative software functions, forcing developer pricing, or limiting payment methods. RuStore, developed by VK with government support, had over 50 million monthly active users by late 2024, surpassing Google Play in the Russian market.

telegram · zaihuapd · Aug 4, 05:25

**Background**: RuStore is a Russian app distribution platform created by VK with support from the Russian Ministry of Digital Development, and since 2023 it has been pre-installed on all smartphones sold in Russia. The new law is part of broader Russian efforts to guarantee local users and developers access to domestic apps amid tensions with foreign tech companies, echoing similar regulatory actions like the European Union's Digital Markets Act.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RuStore">RuStore</a></li>
<li><a href="https://asmo.am/development/rustore">RuStore Publication | ASMO Armenia</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#App Store`, `#Regulation`, `#Russia`, `#Tech Policy`

---

<a id="item-9"></a>
## [Cloudflare Drops Third-Party Security Tools, Uses $58/Month Claude for Bug Bounty Triage](https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600) ⭐️ 8.0/10

Cloudflare CSO Grant Bourzikas revealed at a Sydney event that the company now uses Anthropic's Claude Sonnet to automate vulnerability bounty triage—including deduplication and value assessment—for only $58 per month. Cloudflare has also built over 200 autonomous security agents and largely replaced third-party security tools with internally developed applications. This reveals a striking cost advantage for AI-driven security operations: the same task would cost about $200,000 per month with Anthropic's specialized security model Mythos. It also signals that major cloud providers may increasingly build in-house security stacks, reshaping the vendor-customer relationship in enterprise security. Bourzikas cautioned other enterprises against copying Cloudflare's approach, arguing that not every bank should develop all its own security software. Chief Strategy Officer Stephanie Cohen linked the company's 1,100-person layoff to AI automation and said Cloudflare plans to become a micropayment intermediary between AI companies and publishers.

telegram · zaihuapd · Aug 4, 09:24

**Background**: Bug bounty programs invite external researchers to find vulnerabilities in exchange for rewards, and triage is the process of deduplicating and prioritizing those reports. Claude Sonnet is Anthropic's cost-efficient model, while Mythos is Anthropic's purpose-built security research model that, according to search results, was released in preview on April 7, 2026 and reportedly discovered vulnerabilities across major operating systems and browsers. Autonomous security agents are AI-driven systems that can independently perform offensive or defensive security tasks, though their reliability depends heavily on the quality of the data they process.

<details><summary>References</summary>
<ul>
<li><a href="https://agentconn.com/blog/claude-mythos-ai-security-agent-review/">Claude Mythos : AI Security Agent That Found 271... - AgentConn Blog</a></li>
<li><a href="https://www.bugcrowd.com/blog/setting-the-bar-high-for-bug-bounty-triage-and-validation/">Setting the Bar High for Bug Bounty Triage and Validation | @Bugcrowd</a></li>
<li><a href="https://www.okoone.com/spark/technology-innovation/autonomous-security-agents-are-only-as-good-as-the-data-behind-them/">Autonomous security agents are only as good as the data... | Okoone</a></li>

</ul>
</details>

**Tags**: `#AI`, `#security`, `#Cloudflare`, `#vulnerability management`, `#Anthropic`

---

<a id="item-10"></a>
## [Google Builds $200B Wall Street Financing Machine for Anthropic's AI Chips](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

Financial Times reported on August 4 that Google has quietly built one of the largest infrastructure financing structures in history, delivering over $150 billion in AI chips to Anthropic under contracts totaling roughly $200 billion. The first special-purpose vehicle, Compute SPV, closed its debut deals in June, acquiring about $35 billion in hardware—roughly 1 gigawatt of compute and 1 million TPUs. This move creates a new paradigm for funding AI infrastructure, keeping hundreds of billions in hardware off balance sheets and drawing in major financial institutions like Apollo, Blackstone, and Morgan Stanley. It also lets Anthropic—which has no credit rating—secure enormous compute capacity without traditional corporate debt. The structure splits risk among participants: Google guarantees data centers, Broadcom buys and helps finance chips, and Apollo and Blackstone purchase hardware and lease it back to Anthropic. About 80% of the ~$200 billion in contracts is tied directly to chips, and the model borrows from Boeing and GE's manufacturer-financing practices for aircraft and engines.

telegram · zaihuapd · Aug 4, 10:52

**Background**: TPUs are Google's custom application-specific integrated circuits (ASICs) designed to accelerate machine learning workloads. Special-purpose vehicles (SPVs) are legal entities used to isolate financial risk, often for asset securitization, so that assets held by the SPV are separated from a parent company's bankruptcy estate. Manufacturer financing, as used by Boeing and GE, involves the maker helping customers obtain funding for the equipment they sell.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/张量处理单元">张量处理单元 - 维基百科，自由的百科全书</a></li>
<li><a href="https://docs.cloud.google.com/tpu/docs/system-architecture-tpu-vm">TPU architecture | Google Cloud Documentation</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1937092244185261642">一文全解特殊目的载体(SPV)，资产证券化破产隔离的法律性质和实际问题</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#Google-Anthropic`, `#chip financing`, `#Wall Street`, `#data centers`

---

<a id="item-11"></a>
## [China's First Mandatory L3/L4 Autonomous Driving Safety Standard Set for 2027](https://t.me/zaihuapd/42972) ⭐️ 8.0/10

China's MIIT has submitted for approval the first mandatory national standard for L3/L4 autonomous driving safety, with public comment opening June 17 and a recommended implementation date of July 1, 2027. The standard introduces a Safety Case framework requiring companies to justify safety through claims, arguments, and evidence. This marks a shift in China's AV regulation from loose concept-setting to binding safety requirements, directly impacting automakers, suppliers, and the broader industry. As a major automotive market, China's mandatory standard could also shape global autonomous driving safety regulation. The standard sets distinct requirements for L3 human-machine handover and L4 system autonomous risk handling. Under the Safety Case framework, companies must build a 'claim-argument-evidence' chain covering the full lifecycle, moving regulatory logic from clause compliance to self-certification of safety.

telegram · zaihuapd · Aug 4, 13:06

**Background**: A Safety Case is a structured safety argumentation system supported by evidence, used to demonstrate that a system is acceptably safe in a specific operating environment, covering the entire lifecycle from design to regulation. Industry has seen frameworks such as the Open Autonomy Safety Case Framework and Aurora's Safety Case Framework, with experts describing 2026 as a structural inflection point where autonomous driving safety regulation enters the Safety Case era.

<details><summary>References</summary>
<ul>
<li><a href="https://baike.baidu.com/item/Safety+Case/67871945">Safety Case - 百度百科</a></li>
<li><a href="https://www.sohu.com/a/1040778204_100084983">中国工程院院士李骏：自动驾驶安全进入Safety Case时代_搜狐汽车_搜狐...</a></li>
<li><a href="https://arxiv.org/pdf/2404.05444">The Open Autonomy Safety Case Framework</a></li>

</ul>
</details>

**Tags**: `#autonomous driving`, `#regulation`, `#safety`, `#China`, `#L3/L4`

---