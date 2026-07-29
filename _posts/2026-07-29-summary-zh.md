---
layout: default
title: "Horizon Summary: 2026-07-29 (ZH)"
date: 2026-07-29
lang: zh
---

> 从 43 条内容中筛选出 8 条重要资讯。

---

1. [AI 蠕虫通过 Copilot for Word 自我传播](#item-1) ⭐️ 9.0/10
2. [TurboFieldfare：在 M 系列 Mac 上用 2GB RAM 运行 Gemma 4 26B](#item-2) ⭐️ 8.0/10
3. [Superlogical：Mitchell Hashimoto 基于 libghostty 的新公司](#item-3) ⭐️ 8.0/10
4. [KOReader：开源电子阅读器优化墨水屏阅读体验](#item-4) ⭐️ 8.0/10
5. [长政策文档无法可靠地约束 AI 智能体。](#item-5) ⭐️ 8.0/10
6. [Claude 共享对话漏洞致大量隐私信息外泄](#item-6) ⭐️ 8.0/10
7. [报告称 Hugging Face 被广泛用于生成深度伪造裸照](#item-7) ⭐️ 8.0/10
8. [反网络暴力法草案规制 AI 网暴](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [AI 蠕虫通过 Copilot for Word 自我传播](https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/) ⭐️ 9.0/10

安全研究员 Håkon Måløy 展示了一种新型提示注入攻击，利用 Microsoft Word 中的 Copilot 传播自我复制的文档型 AI 蠕虫。 这证明集成到生产力工具中的 AI 助手可被利用来自主传播恶意软件，对企业和个人用户构成重大安全风险。 该攻击利用 Copilot 无法区分用户指令和文档内容的弱点，通过隐藏文本注入命令，使 Copilot 修改并传播有效载荷。截至发布时，尚无可靠的缓解措施。

hackernews · Canopy9560 · 7月29日 11:44 · [社区讨论](https://news.ycombinator.com/item?id=49096188)

**背景**: 提示注入是一种安全漏洞，大语言模型（LLM）会将用户提供的内容误认为指令，从而绕过安全措施。间接提示注入可将恶意指令嵌入文档或网页中，当 LLM 处理这些内容时，便会执行指令。在此案例中，攻击者将隐藏命令放入 Word 文档，Copilot 处理文档时可能执行这些命令，进而修改文档或创建包含相同有效载荷的新文档，实现蠕虫传播。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/">Context Collapse, Part 3 - AI Worming through Word</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://www.theregister.com/security/2026/07/29/word-worm-crawls-into-copilot-spreads-chaos/5280588">Word worm crawls into Copilot, spreads chaos - The Register</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为这是一类无法修复的漏洞，唯一的有效缓解措施是避免给予 AI 代理过多数据访问权限。一些用户已卸载 Copilot 来保护数据。还有人展示了隐藏文本等攻击方法仍然有效。

**标签**: `#AI security`, `#prompt injection`, `#Copilot`, `#malware`, `#cybersecurity`

---

<a id="item-2"></a>
## [TurboFieldfare：在 M 系列 Mac 上用 2GB RAM 运行 Gemma 4 26B](https://github.com/drumih/turbo-fieldfare) ⭐️ 8.0/10

一个名为 TurboFieldfare 的开源推理引擎通过在 SSD 上流式传输专家权重，在任意 M 系列 Mac 上仅用 2 GB 内存即可运行 4 位量化版 Gemma 4 26B-A4B-IT 模型。 这使得在内存有限的消费级硬件上运行大型混合专家模型成为可能，让设备端 AI 更易用、更实用。它展示了一种高效的 SSD 卸载方法，可能为其他推理引擎带来启发。 TurboFieldfare 在 8GB M2 MacBook Air 上达到 5–6 tok/s，在 M5 MacBook Pro 上达到 31–35 tok/s。它使用小型专家缓存和有界并行 pread 将 SSD 读取与 GPU 计算重叠，并包含一个实验性的 OpenAI 兼容本地服务器，支持流式输出和工具调用。

hackernews · gitpusher42 · 7月29日 15:05 · [社区讨论](https://news.ycombinator.com/item?id=49098510)

**背景**: Gemma 4 26B 是一种混合专家（MoE）模型，每个 token 仅激活部分参数（专家），因此适合从较慢的存储设备流式加载。传统推理需要将整个模型加载到内存中，但 TurboFieldfare 将共享层和 KV 缓存保留在内存中，仅在需要时从 SSD 获取所需专家。SSD 远慢于 RAM，因此引擎使用缓存和重叠 I/O 来隐藏延迟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/google/gemma-4-26B-A4B-it">google/gemma-4-26B-A4B-it · Hugging Face</a></li>
<li><a href="https://arxiv.org/html/2508.06978v1">SSD Offloading for LLM Mixture-of-Experts Weights Considered Harmful in Energy Efficiency</a></li>

</ul>
</details>

**社区讨论**: 评论将 TurboFieldfare 与 llama.cpp 的 mmap 方法进行比较，并指出通过专家流式加载可能也能实现类似效果。用户欣赏其创新性和技术细节，有人为旧版 macOS 提供了编译建议。还有人好奇如何将该引擎适配到 Nvidia Jetson 等其他硬件上。

**标签**: `#on-device-ai`, `#inference-engine`, `#gemma`, `#macos`, `#ssd-offloading`

---

<a id="item-3"></a>
## [Superlogical：Mitchell Hashimoto 基于 libghostty 的新公司](https://www.superlogical.com/) ⭐️ 8.0/10

Mitchell Hashimoto 宣布成立新公司 Superlogical，该公司将基于开源 libghostty 终端组件构建商业产品。 这意义重大，因为它为广受欢迎的 Ghostty 终端模拟器建立了可持续的商业模式，同时保持其核心组件免费可用，可能加速基于终端的应用程序开发，并激励类似的开源策略。 Superlogical 将使用与其他人相同的 MIT 许可组件，并将向上游贡献共享终端工作。Ghostty 本身已转让给一个非营利组织，以确保其独立性。

hackernews · yan · 7月29日 15:41 · [社区讨论](https://news.ycombinator.com/item?id=49098965)

**背景**: Ghostty 是一款快速、跨平台的终端模拟器，使用 GPU 加速和原生用户界面。libghostty 是其核心库，提供零依赖的 C 和 Zig API 用于终端模拟。Mitchell Hashimoto 是 Ghostty 的创建者，也以创建 Vagrant 和在 HashiCorp 参与 Terraform 工作而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ghostty.org/">Ghostty</a></li>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty-org/ghostty: Ghostty is a fast, feature ...</a></li>
<li><a href="https://mitchellh.com/writing/libghostty-is-coming">Libghostty Is Coming – Mitchell Hashimoto</a></li>

</ul>
</details>

**社区讨论**: 讨论整体积极，用户 simonw 称赞将 Ghostty 转让给非营利组织并在 libghostty 上构建 Superlogical 的开源策略。也有将其与 OLE/COM 等组件技术比较的评论，以及提到相关项目如 pi-web 和 herdr。

**标签**: `#terminal`, `#open-source`, `#software-engineering`, `#developer-tools`, `#ghostty`

---

<a id="item-4"></a>
## [KOReader：开源电子阅读器优化墨水屏阅读体验](https://koreader.rocks/) ⭐️ 8.0/10

KOReader 是一款开源电子阅读器应用，因其在墨水屏设备上广泛的格式支持和定制化而受到称赞，但用户界面复杂和偶尔卡顿也受到批评。社区讨论显示了多样化的用户体验和高参与度。 该讨论凸显了社区对开源电子阅读器软件的强烈偏好，影响了设备购买决策。它反映了墨水屏阅读应用中功能丰富性与用户友好性之间的持续权衡。 KOReader 支持多种文件格式，包括 EPUB、PDF、DjVu、MOBI 等。它可以安装在越狱的 Kindle 和 Kobo 上，但有些用户认为界面不直观，更喜欢原生阅读器。

hackernews · Cider9986 · 7月29日 11:05 · [社区讨论](https://news.ycombinator.com/item?id=49095865)

**背景**: 墨水屏设备专为阅读设计，具有低功耗和护眼屏幕，但原生软件通常限制格式支持和定制化。KOReader 是一款运行在多种墨水屏设备上的开源替代品，提供文本重排、阅读进度同步和夜间模式等高级功能。这次社区讨论揭示了用户如何在高级功能与界面复杂性之间权衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://koreader.rocks/">KOReader</a></li>
<li><a href="https://grokipedia.com/page/KOReader">KOReader</a></li>

</ul>
</details>

**社区讨论**: 社区评论呈现不同观点：部分用户认为 KOReader 具有变革性，甚至基于其兼容性购买设备，而另一些用户则认为界面不直观，更喜欢原生阅读器。批评者提到手势反应慢和同步问题，但支持者赞扬其格式支持自由度。总体而言，讨论非常活跃，获得 637 分和 203 条评论，反映出强烈兴趣。

**标签**: `#open-source`, `#e-reader`, `#e-ink`, `#kindle`, `#kobo`

---

<a id="item-5"></a>
## [长政策文档无法可靠地约束 AI 智能体。](https://arxiv.org/abs/2607.25398) ⭐️ 8.0/10

一篇名为《Handbook.md》的新研究论文表明，长政策文档无法可靠地约束 AI 智能体，因为模型在上下文处理和指令遵循方面存在困难。 这一发现至关重要，因为组织越来越多地在生产环境中部署 AI 智能体，而可靠的策略合规性对于安全性和治理至关重要。它凸显了当前长上下文模型的一个根本性局限。 该论文指出，由于工作记忆和注意力的限制，模型难以遵循冗长的指令，这与人类的表现类似。这引发了对依赖于政策文档的 AI 智能体系统可靠性的担忧。

hackernews · spIrr · 7月29日 13:01 · [社区讨论](https://news.ycombinator.com/item?id=49096969)

**背景**: AI 智能体是可以自主执行任务的系统，通常由指令或政策文档引导。大型语言模型（LLM）的最新进展使智能体能够处理长上下文，但研究表明，性能会随着长度增加而显著下降，这一问题被称为'迷失在中间'。指令遵循仍然是一个挑战，特别是在政策冲突或冗长的情况下。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/agentic-ai-has-reliability-problem-why-following-may-harder-sahu-wvg3c">Agentic AI Has a Reliability Problem: Why Following ...</a></li>
<li><a href="https://github.com/agent-sh/agentsys/blob/main/agent-docs/LLM-INSTRUCTION-FOLLOWING-RELIABILITY.md">agentsys/agent-docs/LLM-INSTRUCTION-FOLLOWING-RELIABILITY.md ...</a></li>
<li><a href="https://arxiv.org/html/2602.16666v1">Towards a Science of AI Agent Reliability - arXiv.org</a></li>

</ul>
</details>

**社区讨论**: 评论指出，长上下文模型往往宣称拥有大标记限制，但由于量化和糟糕的采样而在实践中失败。一些人将模型表现与人类局限性进行比较，指出即使是人类也难以处理冗长的政策文档。来自 Claude 用户的轶事证据表明，在实际任务中，CLAUDE.md 文件中的指令会被绕过，这表明存在实际可靠性差距。

**标签**: `#LLM`, `#AI Agents`, `#Long Context`, `#Policy Compliance`, `#Reliability`

---

<a id="item-6"></a>
## [Claude 共享对话漏洞致大量隐私信息外泄](https://t.me/zaihuapd/42830) ⭐️ 8.0/10

Anthropic 旗下的 Claude AI 助手存在隐私漏洞：用户生成的公开共享对话链接未设置禁止搜索引擎抓取的标签，导致 API 密钥、加密货币钱包、个人信息等敏感数据可通过 Google 搜索直接获取。该问题持续存在，Anthropic 尚未修复。 该漏洞对 Claude 用户构成严重隐私风险，敏感信息可通过搜索引擎被任何人获取。这暴露了 Anthropic 在安全方面的基础性疏忽，尤其是在竞争对手 ChatGPT 曾出现类似问题并迅速修复的背景下。 共享对话 URL 缺少 'noindex' 标签或 HTTP 标头，导致搜索引擎能够将其编入索引。泄露的信息包括 API 密钥、加密货币钱包详情、个人简历、律师咨询记录、内部项目文档以及社会安全号码等。

telegram · zaihuapd · 7月29日 02:40

**背景**: 'noindex' 标签是一种标准的网页机制，用于阻止搜索引擎将页面编入索引。在使用 Claude 或 ChatGPT 等 AI 助手共享对话时，用户可能认为只有拥有直接链接的人才能查看内容，但如果没有 noindex，这些页面可能会出现在搜索结果中。Anthropic 未能为共享链接应用此标签，导致了大规模的泄露。用户可以在设置中手动删除特定共享对话。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ithome.com/0/982/802.htm">数百条 Claude 聊天记录被谷歌索引，Anthropic...</a></li>
<li><a href="https://cn-sec.com/archives/5366349.html">Claude AI... | CN-SEC 中文网</a></li>
<li><a href="https://developers.google.com/search/docs/crawling-indexing/block-indexing">Block Search Indexing with noindex | Google Search Central ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一，但多数批评 Anthropic。尽管有人认为共享链接本意即为公开，但 Reddit 用户和网络安全专家普遍认为缺少 noindex 标签是基础性错误。讨论反映出用户与提供者之间隐私责任的争议。

**标签**: `#privacy`, `#security vulnerability`, `#Claude`, `#AI`, `#data leak`

---

<a id="item-7"></a>
## [报告称 Hugging Face 被广泛用于生成深度伪造裸照](https://www.theverge.com/ai-artificial-intelligence/971723/hugging-face-nudify-deepfake-undress-women-children) ⭐️ 8.0/10

AI Forensics 的报告发现，Hugging Face 的图像编辑模型被广泛用于制作非自愿的深度伪造裸照。该机构设置的蜜罐在 7 天内收到超过 1000 条请求，其中 73% 涉及性内容，近 7% 针对儿童。 这突显了严重的伦理和平台责任问题，因为 Hugging Face 是领先的开源模型中心，但防护措施不足。这种滥用影响了弱势群体，特别是女性和儿童，并强调了在 AI 平台中需要更好的内容审核。 Hugging Face 排名前九的图像编辑模型中有七个可以轻易按简单提示为女性“脱衣”，无需精心构造绕过话术。AI Forensics 建议增加提示词过滤与输出扫描机制，以阻止有害图像生成。

telegram · zaihuapd · 7月29日 08:20

**背景**: Hugging Face 是一家公司和开源社区，托管了超过 10 万个预训练机器学习模型，其中包括许多图像生成模型。深度伪造技术利用 AI 将已有的图像或视频叠加到目标图像上，常被用于制作非自愿的色情内容。蜜罐是一种网络安全工具，通过模拟系统来吸引和分析攻击者。该研究使用蜜罐收集关于哪些模型被请求的数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face - 维基百科，自由的百科全书</a></li>
<li><a href="https://zh.wikipedia.org/zh-cn/深伪技术">深伪技术 - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**标签**: `#Hugging Face`, `#deepfake`, `#AI安全`, `#内容审核`, `#伦理问题`

---

<a id="item-8"></a>
## [反网络暴力法草案规制 AI 网暴](https://mp.weixin.qq.com/s/PrzKFhbwjgFEGBPADvFD6Q) ⭐️ 8.0/10

2026 年 7 月 29 日，国家互联网信息办公室公布《反网络暴力法（征求意见稿）》，其中包含针对 AI 生成网络暴力的专门条款，要求平台建立监测识别机制。 这是中国首次在法律层面明确规制 AI 生成的网络暴力，对平台施加了严格的防范义务。此举为中国的 AI 治理和内容审核开创了重要先例。 草案要求网络服务提供者建立监测识别和防护机制，并对利用 AI 技术制作传播网络暴力信息作出专门规定。同时引入多部门协同治理和人格权侵害禁令，受害者可请求精神损害赔偿。

telegram · zaihuapd · 7月29日 10:59

**背景**: 中国一直在加强反网络暴力的法律框架。2024 年发布了《网络暴力信息治理规定》作为部门规章。新草案若通过，将把这些措施提升为全国人大通过的法律，具有更强的法律效力，并专门针对 AI 生成的内容进行规制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gov.cn/zhengce/202501/content_6997441.htm">网络暴力信息治理规定_国家互联网信息办公室_中国政府网</a></li>
<li><a href="https://www.moj.gov.cn/pub/sfbgw/flfggz/flfggzbmgz/202410/t20241009_507262.html">网络暴力信息治理规定</a></li>

</ul>
</details>

**标签**: `#cyberbullying`, `#AI regulation`, `#China internet law`, `#content moderation`, `#policy`

---