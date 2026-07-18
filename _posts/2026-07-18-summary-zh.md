---
layout: default
title: "Horizon Summary: 2026-07-18 (ZH)"
date: 2026-07-18
lang: zh
---

> 从 38 条内容中筛选出 9 条重要资讯。

---

1. [GPT-5.6 提示关闭凸优化领域 30 年空白](#item-1) ⭐️ 9.0/10
2. [LG 显示器通过 Windows Update 未经同意强制安装软件](#item-2) ⭐️ 9.0/10
3. [月之暗面发布 Kimi K3：开源 2.8 万亿参数模型，前端编程登顶](#item-3) ⭐️ 9.0/10
4. [StackOverflow 活动下降：AI 还是平台政策？](#item-4) ⭐️ 8.0/10
5. [PHK 告别之作：回顾自行车棚效应与开源智慧](#item-5) ⭐️ 8.0/10
6. [Meta 拟向 Anthropic 出租百亿美元 AI 算力](#item-6) ⭐️ 8.0/10
7. [SpaceX 与五角大楼谈判提供 AI 算力](#item-7) ⭐️ 8.0/10
8. [特朗普政府拟设类似 FINRA 的 AI 模型审查机构](#item-8) ⭐️ 8.0/10
9. [旧金山责令苹果谷歌下架'脱衣'应用](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [GPT-5.6 提示关闭凸优化领域 30 年空白](https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/) ⭐️ 9.0/10

研究人员通过向 GPT-5.6 输入一个提示词，解决了凸优化领域一个存在 30 年的未解决问题，填补了长期空白。该成果被数学界认定为真实的学术贡献。 这一突破表明人工智能能够为高等数学研究做出实质性贡献，可能加速优化及相关领域的进展。同时也标志着数学家处理未解决问题的方式可能发生转变，人工智能现在能够处理以前被认为超出其能力范围的问题。 被解决的问题涉及在球形域上最小化凸 Lipschitz 函数的时间复杂度，而球形域限制并非本质性的，因为任何有界域都可以进行变量替换。据称该证明使用了 GPT-5.6 的 Sol Pro 版本而非 Ultra 版本，体现了模型之间的能力差异。

hackernews · mbustamanter · 7月18日 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48957779)

**背景**: 凸优化是数学优化的一个子领域，要求目标函数为凸函数且可行集为凸集，使得许多问题类别存在多项式时间的高效算法。该领域存在 30 年的空白指的是某个关于凸优化算法最优收敛率的开放问题，尽管经过大量努力仍未被解决。继 OpenAI 的 CDC 证明等类似成就之后，这一结果为 AI 辅助数学证明的列表增添了新成员。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Convex_optimization">Convex optimization</a></li>

</ul>
</details>

**社区讨论**: 社区普遍认可该成果为真实贡献，但部分人指出它比循环双覆盖证明更为小众。评论者讨论了这是否标志着 AI 能够处理中等难度问题，从而将人类研究者解放出来从事更具创造性的工作，而另一些人则担忧这对传统上通过解决此类问题来锻炼的初级研究者的影响。此外还有关于 GPT-5.6 Sol Pro 与 Ultra 版本差异的讨论，推测涉及多智能体编排。

**标签**: `#AI`, `#convex optimization`, `#mathematics`, `#breakthrough`, `#GPT`

---

<a id="item-2"></a>
## [LG 显示器通过 Windows Update 未经同意强制安装软件](https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent) ⭐️ 9.0/10

据报道，当用户通过 HDMI 连接 LG 显示器时，Windows Update 会自动静默安装 LG 扩展和 LG 显示器应用安装包，无需任何用户交互或同意。 这种行为破坏了用户控制和安全性，因为安装的软件以系统权限运行，在每次启动时持久化，并能显示第三方广告（如 McAfee），引发了严重的隐私和供应链担忧。 安装会在连接 LG 显示器时自动发生，即使之前已连接过；安装的应用具有互联网访问权限和完全的系统权限，且没有沙盒保护。

hackernews · baranul · 7月18日 10:21 · [社区讨论](https://news.ycombinator.com/item?id=48956688)

**背景**: Windows Update 会分发来自硬件制造商的驱动和软件包，而显示数据通道（DDC/CI）允许显示器与 PC 通信，可能触发自动下载。LG 正在利用这一机制推送不受欢迎的软件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent">LG monitors silently install software through Windows Update without user consent - VideoCardz.com</a></li>
<li><a href="https://cybersecuritynews.com/windows-update-installs-lg-monitor-app-pushes-mcafee-ads/">Windows Update Silently Installs LG Monitor App That Pushes McAfee Ads</a></li>
<li><a href="https://en.wikipedia.org/wiki/Display_Data_Channel">Display Data Channel - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区表达了强烈愤怒，将这种行为比作恶意软件，并指出严重的隐私和安全影响。用户分享了通过组策略或设备安装设置阻止自动下载制造商应用的解决方法。

**标签**: `#security`, `#windows`, `#privacy`, `#lg-monitors`, `#supply-chain-attack`

---

<a id="item-3"></a>
## [月之暗面发布 Kimi K3：开源 2.8 万亿参数模型，前端编程登顶](https://t.me/zaihuapd/42637) ⭐️ 9.0/10

月之暗面发布了 Kimi K3，这是全球首个开源的 2.8 万亿参数模型，采用 Kimi Delta Attention 与 Attention Residuals 架构，具备原生视觉能力和 100 万 token 上下文窗口。在 Frontend Code Arena 基准测试中以 1679 分排名第一，超越 Fable 5，从上一代 Kimi k2.6 的第 18 名跃升至榜首。 此次发布表明开源模型能够在前端编程等专业基准测试中与顶尖专有模型竞争甚至超越。它也凸显了中国 AI 实验室在全球 AI 竞赛中的快速进步，有望降低 AI 辅助软件开发的成本并加速创新。 K3 采用了结合 Kimi Delta Attention（线性注意力模块）和 Attention Residuals（标准残差连接的替代品）的新颖架构。该模型是开源的，定价为输入/输出每百万 token 3/15 美元，与 ChatGPT 5.6 和 Opus 4.8 等专有模型价格相当。

telegram · zaihuapd · 7月18日 02:29

**背景**: Kimi Delta Attention 是一种表现力强的线性注意力模块，扩展了 Gated DeltaNet，通过更细粒度的门控机制更有效地利用有限的有限状态 RNN 内存。Attention Residuals 允许每一层选择性地聚合所有先前层的信息，提高了模型深度利用效率。Frontend Code Arena 是一个评估 AI 模型前端编程能力的基准测试，Kimi K3 以 1679 分排名第一，在 7 个类别中 6 个居首。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2510.26692">[2510.26692] Kimi Linear: An Expressive, Efficient Attention Architecture</a></li>
<li><a href="https://github.com/MoonshotAI/Attention-Residuals">GitHub - MoonshotAI/ Attention - Residuals · GitHub</a></li>
<li><a href="https://digg.com/tech/we56zqdp">Chinese model Kimi-K3 tops Frontend Code Arena benchmark · Digg</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，从前沿实验室进行知识蒸馏是不可避免的，开源模型将继续挑战专有模型。有人报告使用 Kimi K3 时花费了较长时间和较高成本，而其他人则讨论了政府对开放权重模型可能施加限制的影响。还有人对 K3 与 ChatGPT 5.6、Opus 4.8 等专有模型的价格和性能进行了比较。

**标签**: `#AI`, `#Large Language Models`, `#Open Source`, `#2.8T`, `#Frontend Coding`

---

<a id="item-4"></a>
## [StackOverflow 活动下降：AI 还是平台政策？](https://data.stackexchange.com/stackoverflow/query/1953768#graph) ⭐️ 8.0/10

Stack Exchange Data Explorer 上的一个数据查询图显示了 StackOverflow 活动自 2014 年以来持续下降，引发了关于下降原因是 AI 编码助手还是平台自身政策的讨论。 这一分析很重要，因为它挑战了仅靠 AI 就摧毁了 StackOverflow 的简单叙事，突出了社区管理和平台设计在在线社区衰落中的作用。 该图显示活动在 2014 年左右达到顶峰，远在 ChatGPT 发布之前，并在 2021 年 StackOverflow 被 Prosus 收购后进一步下降。评论者认为，平台严格的审核和缺乏社区建设是主要因素。

hackernews · secretslol · 7月18日 11:12 · [社区讨论](https://news.ycombinator.com/item?id=48956949)

**背景**: StackOverflow 是一个受程序员欢迎的问答网站，以其优先考虑高质量问题和答案的严格审核而闻名。然而，这种方法被批评为对新手不友好。与此同时，像 ChatGPT 这样的 AI 编码助手提供即时答案，减少了访问该网站的需求。活动下降反映了开发者寻求帮助方式的更大转变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stack_Overflow">Stack Overflow - Wikipedia</a></li>
<li><a href="https://stackoverflow.blog/2024/05/29/developers-get-by-with-a-little-help-from-ai-stack-overflow-knows-code-assistant-pulse-survey-results/">Developers get by with a little help from AI: Stack Overflow Knows code assistant pulse survey results - Stack Overflow</a></li>
<li><a href="https://www.reddit.com/r/programming/comments/1hyz63l/coding_help_on_stackoverflow_dives_as_ai/">r/programming on Reddit: Coding help on StackOverflow dives as AI assistants rise</a></li>

</ul>
</details>

**社区讨论**: 评论者大多将下降归因于 StackOverflow 自身的政策，指出平台通过高参与门槛和抑制对话的文化排斥了新用户。一些人指出，下降在 AI 普及之前就开始了，表明内部问题是主要原因。

**标签**: `#stackoverflow`, `#AI impact`, `#community management`, `#online communities`, `#data analysis`

---

<a id="item-5"></a>
## [PHK 告别之作：回顾自行车棚效应与开源智慧](https://queue.acm.org/detail.cfm?id=3818307) ⭐️ 8.0/10

著名 BSD 开发者 Poul-Henning Kamp 在 ACM Queue 上发表告别文章，反思了“自行车棚效应”（bikeshedding）并分享了他几十年开源开发的经验。 这篇文章提供了一位开源关键人物的罕见而坦率的观点，引发了关于项目管理、社区动态以及软件开发中琐事陷阱的重要讨论。 PHK 以 1994 年创建 MD5crypt 密码哈希算法而闻名，该算法早于 bcrypt 和其他现代方案。术语“bikeshedding”由 Kamp 于 1999 年在 BSD 社区推广，源于 Parkinson 的琐事定律。

hackernews · Ygg2 · 7月18日 17:27 · [社区讨论](https://news.ycombinator.com/item?id=48960155)

**背景**: “自行车棚效应”即琐事定律，描述了人们倾向于在简单易懂的琐碎问题上花费过多时间，而忽视更重要更复杂的问题。该概念由 C. Northcote Parkinson 于 1957 年提出，后来通过 Kamp 的文章在软件开发领域流行。这一现象在开源项目中尤为常见，因为许多贡献者可能因其易理解性而关注表面问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bikeshedding">Bikeshedding</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了各种反应：有人建议可逆决策应凭直觉做出以避免自行车棚效应，另一个人强调了 PHK 对 MD5crypt 的贡献。还有一位幽默地抱怨用 JIRA 面板取代自行车棚效应反而让情况更糟，一位读者最初反应消极，但后来欣赏文章的深度。

**标签**: `#open source`, `#bikeshedding`, `#PHK`, `#project management`, `#culture`

---

<a id="item-6"></a>
## [Meta 拟向 Anthropic 出租百亿美元 AI 算力](https://www.nytimes.com/2026/07/17/technology/meta-anthropic-ai-computing-power.html) ⭐️ 8.0/10

Meta 正与 AI 初创公司 Anthropic 谈判，拟将其 AI 数据中心算力租予后者，潜在交易规模达 100 亿美元，为期两年。谈判由 Anthropic 于今年 6 月提出，尚处早期阶段，未必能最终成交。 这笔潜在交易凸显出 AI 算力的极度稀缺，促使 AI 实验室与科技巨头之间达成战略合作。对于 Meta 而言，出租闲置算力既能开辟新收入来源，也有助于缓解投资者对其巨额基础设施建设支出的担忧。 若达成协议，Anthropic 将按月付款，双方均可提前退出。Meta 今年计划投入高达 1450 亿美元，其中大量用于 AI 与数据中心建设。

telegram · zaihuapd · 7月18日 01:14

**背景**: Anthropic 是一家专注于 AI 安全的公司，于 2021 年由前 OpenAI 员工创立，旗下拥有大语言模型 Claude。截至 2026 年 5 月，其估值达 9650 亿美元，成为全球最具价值的纯 AI 公司。训练和运行前沿 AI 模型需要大量专用算力，这种资源日益稀缺且昂贵，促使 Meta 等公司投入巨资建设基础设施，并可能将闲置算力出租。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic</a></li>

</ul>
</details>

**标签**: `#AI`, `#Meta`, `#Anthropic`, `#computing infrastructure`, `#business deal`

---

<a id="item-7"></a>
## [SpaceX 与五角大楼谈判提供 AI 算力](https://www.wsj.com/tech/ai/spacex-in-talks-to-provide-computing-power-for-pentagons-ai-push-15e752e4) ⭐️ 8.0/10

SpaceX 正与美国国防部谈判，提供数据中心算力用于运行 AI 模型，交易金额可能高达数十亿美元。谈判仍在进行中，存在破裂可能。 这笔交易将加深 SpaceX 与五角大楼的关系，并凸显国安领域对 AI 算力的需求增长。它也可能加剧云服务商之间的国防合同竞争。 五角大楼近期已批准 SpaceX、亚马逊、谷歌、微软和甲骨文在机密环境中使用 AI 模型。SpaceX 近月还与 Anthropic 和谷歌签署了类似的算力供应协议，并计划扩展其云计算业务。

telegram · zaihuapd · 7月18日 01:44

**背景**: AI 算力是指训练和运行 AI 模型所需的计算能力。云计算提供按需获取计算资源的能力。五角大楼正加速采用云计算以支持国安和日常作战中的 AI 应用。SpaceX 原本是一家航天公司，如今正拓展云服务业务，可能利用自身基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.elecfans.com/d/6442715.html">AI 算 力 ：智能时代的核心驱动 力 -电子发烧友网</a></li>
<li><a href="https://f5.pm/go-200169.html">机 密 计 算 的崭露头角与未来前景</a></li>

</ul>
</details>

**标签**: `#AI`, `#云计算`, `#国防`, `#SpaceX`, `#五角大楼`

---

<a id="item-8"></a>
## [特朗普政府拟设类似 FINRA 的 AI 模型审查机构](https://www.bloomberg.com/news/articles/2026-07-17/us-considers-creating-finra-like-watchdog-to-vet-top-ai-models) ⭐️ 8.0/10

特朗普政府正考虑设立一个类似金融业监管局（FINRA）的独立机构，负责在顶尖 AI 模型发布前审查其安全性。该计划由财政部长斯科特·贝森特牵头，目前正由白宫幕僚长苏茜·威尔斯审阅。 此举旨在回应华尔街对网络安全的担忧以及硅谷对临时性政府管控的不满，让两大行业在制定安全标准方面拥有更大发言权。这标志着美国 AI 监管向制度化迈出重要一步。 该方案仍在讨论中，尚未最终确定，总统特朗普也未审阅。此前，Anthropic 和 OpenAI 曾对美国要求修改或限制其最新模型提出异议。该计划与 Google DeepMind 首席执行官德米斯·哈萨比斯提出的行业资助独立监管机构的建议方向一致。

telegram · zaihuapd · 7月18日 05:45

**背景**: FINRA 是一个受美国证券交易委员会（SEC）监督的行业自律组织（SRO），负责监管经纪公司。该提案将创建一个类似的 AI 行业自律组织，由行业资助但接受政府监督。政府内部存在分歧，一方主张建立类似食品药品监督管理局（FDA）的独立审查机构，另一方则倾向于较为柔性的行业指导框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://goodinfo.net/posts/ai-tech/white-house-considers-ai-model-vetting-may-2026/">白宫考虑在 AI 模 型 发布前进行 安 全 审 查 | 全 球 全 景日报 | goodinfo.net</a></li>

</ul>
</details>

**标签**: `#AI监管`, `#特朗普政府`, `#FINRA`, `#AI安全`, `#政策`

---

<a id="item-9"></a>
## [旧金山责令苹果谷歌下架'脱衣'应用](https://techcrunch.com/2026/07/17/apple-and-google-ordered-to-purge-nudify-apps-from-app-stores/) ⭐️ 8.0/10

旧金山市检察长邱信福已要求苹果和谷歌从其应用商店中下架数十款利用人工智能生成非自愿亲密深度伪造图像的'脱衣'应用。 这一行动凸显了人工智能生成深度伪造图像带来的法律和伦理挑战，并强调了平台在防止滥用方面的责任。它可能为监管非自愿合成媒体树立先例，影响科技公司处理有害内容的方式。 检察长信中指出，这些公司可能已从上架这些应用中获利数百万美元，并面临民事处罚。苹果已下架三款应用并终止相关开发者账号，谷歌则已暂停五款 Play 商店应用。

telegram · zaihuapd · 7月18日 08:45

**背景**: 脱衣应用利用人工智能深度伪造技术，未经同意将照片（通常为女性）修改为裸体。网络上超过 90%的深度伪造视频是非自愿的色情内容。多个国家已立法将此类深度伪造定为犯罪。科技公司面临越来越大的压力，需要主动审核平台上有害的 AI 生成内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nudify_apps">Nudify apps</a></li>
<li><a href="https://medium.com/@shreyasinha551/the-hidden-crisis-how-non-consensual-deepfakes-are-weaponizing-womens-images-63123ee61417">The Hidden Crisis: How Non - Consensual Deepfakes Are... | Medium</a></li>
<li><a href="https://dig.watch/updates/non-consensual-deepfakes-consent-and-power-in-synthetic-media">Non - consensual deepfakes , consent, and... | Digital Watch Observatory</a></li>

</ul>
</details>

**标签**: `#AI ethics`, `#deepfakes`, `#platform regulation`, `#privacy`, `#Apple`

---