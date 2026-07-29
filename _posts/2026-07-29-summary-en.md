---
layout: default
title: "Horizon Summary: 2026-07-29 (EN)"
date: 2026-07-29
lang: en
---

> From 43 items, 8 important content pieces were selected

---

1. [Document-borne AI worms self-propagate through Copilot for Word](#item-1) ⭐️ 9.0/10
2. [TurboFieldfare: Run Gemma 4 26B in 2GB RAM on M-series Macs](#item-2) ⭐️ 8.0/10
3. [Superlogical: Mitchell Hashimoto's new company building on libghostty](#item-3) ⭐️ 8.0/10
4. [KOReader: Open-Source E-Reader Enhances E-Ink Devices](#item-4) ⭐️ 8.0/10
5. [Long policy documents fail to govern AI agents reliably.](#item-5) ⭐️ 8.0/10
6. [Claude shared links indexed by search engines, leaking private data](#item-6) ⭐️ 8.0/10
7. [Hugging Face platform exploited for deepfake nude image generation](#item-7) ⭐️ 8.0/10
8. [China's draft anti-cyberbullying law targets AI-generated abuse](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Document-borne AI worms self-propagate through Copilot for Word](https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/) ⭐️ 9.0/10

Security researcher Håkon Måløy has demonstrated a novel prompt injection attack that turns Microsoft Copilot for Word into a vector for self-propagating document-borne AI worms. This demonstrates that AI assistants integrated into productivity tools can be exploited to propagate malware autonomously, posing a significant security risk for enterprise and personal users alike. The attack exploits Copilot's inability to distinguish between user instructions and content within documents, using hidden text to inject commands that cause Copilot to alter and forward the payload. At publication, no robust mitigation existed.

hackernews · Canopy9560 · Jul 29, 11:44 · [Discussion](https://news.ycombinator.com/item?id=49096188)

**Background**: Prompt injection is a vulnerability where large language models (LLMs) interpret user-provided content as instructions, bypassing safety measures. Indirect prompt injection can be embedded in documents or web pages that the LLM processes. In this case, the attacker places hidden commands in a Word document; when Copilot processes the document, it can execute those commands, potentially modifying the document or creating new ones with the same payload, thus enabling the worm's spread.

<details><summary>References</summary>
<ul>
<li><a href="https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/">Context Collapse, Part 3 - AI Worming through Word</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://www.theregister.com/security/2026/07/29/word-worm-crawls-into-copilot-spreads-chaos/5280588">Word worm crawls into Copilot, spreads chaos - The Register</a></li>

</ul>
</details>

**Discussion**: Commenters widely view this as an unfixable vulnerability class, highlighting that the only real mitigation is to avoid giving AI agents broad access to data. Some users have already uninstalled Copilot to protect their data. Others demonstrate practical attack vectors like hidden text still working.

**Tags**: `#AI security`, `#prompt injection`, `#Copilot`, `#malware`, `#cybersecurity`

---

<a id="item-2"></a>
## [TurboFieldfare: Run Gemma 4 26B in 2GB RAM on M-series Macs](https://github.com/drumih/turbo-fieldfare) ⭐️ 8.0/10

An open-source inference engine called TurboFieldfare runs a 4-bit quantized Gemma 4 26B-A4B-IT model on any M-series Mac using only 2 GB of RAM by streaming expert weights from SSD. This enables running large Mixture-of-Experts models on memory-constrained consumer hardware, making on-device AI more accessible and practical. It demonstrates an efficient SSD offloading approach that could inspire similar techniques in other inference engines. TurboFieldfare achieves 5–6 tokens per second on an 8 GB M2 MacBook Air and 31–35 tok/s on an M5 MacBook Pro. It uses a small expert cache and bounded parallel pread to overlap SSD reads with GPU computation, and includes an experimental OpenAI-compatible local server with streaming and tool call support.

hackernews · gitpusher42 · Jul 29, 15:05 · [Discussion](https://news.ycombinator.com/item?id=49098510)

**Background**: Gemma 4 26B is a Mixture-of-Experts (MoE) model where only a subset of parameters (experts) are activated per token, making it suitable for streaming from slower storage. Traditional inference requires loading the entire model into RAM, but TurboFieldfare keeps the shared layers and KV cache in RAM while fetching only the needed experts from SSD on demand. SSD is much slower than RAM, so the engine uses caching and overlapping I/O to hide latency.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/google/gemma-4-26B-A4B-it">google/gemma-4-26B-A4B-it · Hugging Face</a></li>
<li><a href="https://arxiv.org/html/2508.06978v1">SSD Offloading for LLM Mixture-of-Experts Weights Considered Harmful in Energy Efficiency</a></li>

</ul>
</details>

**Discussion**: Comments compare TurboFieldfare to llama.cpp's mmap approach and suggest that similar results might be achievable with expert streaming. Users appreciate the innovation and technical details, with some providing compilation tips for older macOS versions. There is also curiosity about adapting the engine to other hardware like Nvidia Jetson.

**Tags**: `#on-device-ai`, `#inference-engine`, `#gemma`, `#macos`, `#ssd-offloading`

---

<a id="item-3"></a>
## [Superlogical: Mitchell Hashimoto's new company building on libghostty](https://www.superlogical.com/) ⭐️ 8.0/10

Mitchell Hashimoto announced Superlogical, a new company that will build commercial products on top of the open-source libghostty terminal components. This is significant because it creates a sustainable business model around the popular Ghostty terminal emulator while keeping its core components freely available, potentially accelerating development of terminal-based applications and inspiring similar open-source strategies. Superlogical will consume the same MIT-licensed components as everyone else and will contribute shared terminal work upstream. Ghostty itself has been transferred to a non-profit organization to ensure its independence.

hackernews · yan · Jul 29, 15:41 · [Discussion](https://news.ycombinator.com/item?id=49098965)

**Background**: Ghostty is a fast, cross-platform terminal emulator that uses GPU acceleration and platform-native UI. libghostty is its core library, providing a zero-dependency C and Zig API for terminal emulation. Mitchell Hashimoto is the creator of Ghostty, also known for creating Vagrant and working on Terraform at HashiCorp.

<details><summary>References</summary>
<ul>
<li><a href="https://ghostty.org/">Ghostty</a></li>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty-org/ghostty: Ghostty is a fast, feature ...</a></li>
<li><a href="https://mitchellh.com/writing/libghostty-is-coming">Libghostty Is Coming – Mitchell Hashimoto</a></li>

</ul>
</details>

**Discussion**: The discussion is largely positive, with users like simonw praising the open-source strategy of transferring Ghostty to a non-profit and building Superlogical on libghostty. There are also comparisons to component technologies like OLE/COM and mentions of related projects like pi-web and herdr.

**Tags**: `#terminal`, `#open-source`, `#software-engineering`, `#developer-tools`, `#ghostty`

---

<a id="item-4"></a>
## [KOReader: Open-Source E-Reader Enhances E-Ink Devices](https://koreader.rocks/) ⭐️ 8.0/10

KOReader is an open-source e-reader application praised for its extensive format support and customization on e-ink devices, though critiqued for its complex UI and occasional lag. The community discussion highlights diverse user experiences with high engagement. The discussion underscores the community's strong preference for open-source alternatives to proprietary e-reader software, influencing device purchasing decisions. It reflects the ongoing trade-off between feature richness and user-friendliness in e-ink reading apps. KOReader supports a wide range of file formats including EPUB, PDF, DjVu, MOBI, and many more. It can be installed on jailbroken Kindles and Kobos, but some users find the UI non-intuitive and prefer the default viewers.

hackernews · Cider9986 · Jul 29, 11:05 · [Discussion](https://news.ycombinator.com/item?id=49095865)

**Background**: E-ink devices are designed for reading with low power consumption and eye-friendly screens, but default software often limits format support and customization. KOReader is an open-source alternative that runs on many e-ink devices, providing advanced features like text reflow, reading progress sync, and night mode. This community discussion reveals how users weigh these advanced features against the complexity of the interface.

<details><summary>References</summary>
<ul>
<li><a href="https://koreader.rocks/">KOReader</a></li>
<li><a href="https://grokipedia.com/page/KOReader">KOReader</a></li>

</ul>
</details>

**Discussion**: Community comments show a mix of opinions: some users find KOReader transformative and base device purchases on its compatibility, while others find the UI unintuitive and prefer default viewers. Critics cite laggy gestures and syncing issues, but advocates praise its format support and freedom. Overall, the discussion is highly engaged with 637 points and 203 comments, reflecting strong interest.

**Tags**: `#open-source`, `#e-reader`, `#e-ink`, `#kindle`, `#kobo`

---

<a id="item-5"></a>
## [Long policy documents fail to govern AI agents reliably.](https://arxiv.org/abs/2607.25398) ⭐️ 8.0/10

A new research paper, Handbook.md, demonstrates that long policy documents are unreliable for governing AI agents, as models struggle with context handling and instruction following. This finding is critical as organizations increasingly deploy AI agents in production, where reliable policy compliance is essential for safety and governance. It highlights a fundamental limitation of current long-context models. The paper identifies that models fail to adhere to lengthy instructions due to limitations in working memory and attention, similar to human performance. This raises concerns about the reliability of agentic AI systems that depend on policy documents.

hackernews · spIrr · Jul 29, 13:01 · [Discussion](https://news.ycombinator.com/item?id=49096969)

**Background**: AI agents are systems that can autonomously perform tasks, often guided by instructions or policy documents. Recent advances in large language models (LLMs) have enabled agents to handle long contexts, but research shows that performance degrades significantly with length, a problem known as 'lost in the middle.' Instruction following remains a challenge, especially when policies conflict or are lengthy.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/agentic-ai-has-reliability-problem-why-following-may-harder-sahu-wvg3c">Agentic AI Has a Reliability Problem: Why Following ...</a></li>
<li><a href="https://github.com/agent-sh/agentsys/blob/main/agent-docs/LLM-INSTRUCTION-FOLLOWING-RELIABILITY.md">agentsys/agent-docs/LLM-INSTRUCTION-FOLLOWING-RELIABILITY.md ...</a></li>
<li><a href="https://arxiv.org/html/2602.16666v1">Towards a Science of AI Agent Reliability - arXiv.org</a></li>

</ul>
</details>

**Discussion**: Comments highlight that long-context models often claim large token limits but fail in practice due to quantization and poor sampling. Some compare model performance to human limitations, noting that even humans struggle with long policy documents. Anecdotal evidence from users of Claude suggests that instructions in CLAUDE.md files are bypassed during real tasks, indicating a practical reliability gap.

**Tags**: `#LLM`, `#AI Agents`, `#Long Context`, `#Policy Compliance`, `#Reliability`

---

<a id="item-6"></a>
## [Claude shared links indexed by search engines, leaking private data](https://t.me/zaihuapd/42830) ⭐️ 8.0/10

Anthropic’s Claude AI assistant has a privacy vulnerability where public shared conversation links are not blocked from search engine indexing, causing sensitive data like API keys, cryptocurrency wallets, and personal information to be exposed via Google search. The issue has been ongoing, and Anthropic has not yet addressed it. This vulnerability poses a serious privacy risk for Claude users, exposing potentially highly sensitive information to anyone via search engines. It highlights a fundamental security oversight by Anthropic, especially concerning as similar issues in competing products like ChatGPT were promptly resolved. The shared conversation URLs lack a 'noindex' meta tag or HTTP header, allowing search engines to index them. Exposed information includes API keys, cryptocurrency wallet details, personal resumes, lawyer-client communications, internal project documents, and social security numbers.

telegram · zaihuapd · Jul 29, 02:40

**Background**: The 'noindex' tag is a standard web mechanism used to prevent search engines from indexing a page. When sharing conversations in AI assistants like Claude or ChatGPT, users may expect that only people with the direct link can view the content, but without noindex, these pages can appear in search results. Anthropic's failure to apply this tag to shared links has led to a widespread leak. Users can delete individual shared conversations from the settings page.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ithome.com/0/982/802.htm">数百条 Claude 聊天记录被谷歌索引，Anthropic...</a></li>
<li><a href="https://cn-sec.com/archives/5366349.html">Claude AI... | CN-SEC 中文网</a></li>
<li><a href="https://developers.google.com/search/docs/crawling-indexing/block-indexing">Block Search Indexing with noindex | Google Search Central ...</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed but lean heavily toward criticizing Anthropic. While some argue that shared links are inherently public, Reddit users and cybersecurity experts overwhelmingly condemn the lack of noindex as a fundamental error. The discussion underscores a disagreement over user vs provider responsibility for privacy.

**Tags**: `#privacy`, `#security vulnerability`, `#Claude`, `#AI`, `#data leak`

---

<a id="item-7"></a>
## [Hugging Face platform exploited for deepfake nude image generation](https://www.theverge.com/ai-artificial-intelligence/971723/hugging-face-nudify-deepfake-undress-women-children) ⭐️ 8.0/10

A report by AI Forensics found that Hugging Face's image editing models are widely used to generate non-consensual deepfake nude images. Their honeypot received over 1,000 requests in seven days, with 73% involving sexual content and nearly 7% targeting children. This highlights serious ethical and platform responsibility issues, as Hugging Face is a leading open-source model hub with limited safeguards. The misuse affects vulnerable groups, especially women and children, and underscores the need for better content moderation in AI platforms. The top nine image editing models on Hugging Face included seven that could easily undress women with simple prompts, without needing sophisticated jailbreaks. AI Forensics recommends adding prompt filters and output scanning to prevent harmful image generation.

telegram · zaihuapd · Jul 29, 08:20

**Background**: Hugging Face is a company and open-source community that hosts over 100,000 pre-trained machine learning models, including many for image generation. Deepfake technology uses AI to superimpose existing images or videos onto target images, often used to create non-consensual pornographic content. A honeypot is a cybersecurity tool that simulates a system to attract and analyze attackers. This study used a honeypot to collect data on what models were being requested.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face - 维基百科，自由的百科全书</a></li>
<li><a href="https://zh.wikipedia.org/zh-cn/深伪技术">深伪技术 - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**Tags**: `#Hugging Face`, `#deepfake`, `#AI安全`, `#内容审核`, `#伦理问题`

---

<a id="item-8"></a>
## [China's draft anti-cyberbullying law targets AI-generated abuse](https://mp.weixin.qq.com/s/PrzKFhbwjgFEGBPADvFD6Q) ⭐️ 8.0/10

On July 29, 2026, China's Cyberspace Administration released a draft Anti-Cyberbullying Law for public comment, which includes specific provisions targeting AI-generated cyberbullying and requires platforms to establish monitoring mechanisms. This marks the first time Chinese law explicitly addresses AI-generated cyberbullying, imposing strict obligations on platforms to prevent and mitigate such content. It sets a significant precedent for AI governance and content moderation in China. The draft law requires internet service providers to build detection and protection mechanisms, with special provisions for AI-generated cyberbullying content. It also introduces multi-department coordination and allows victims to seek injunctions and mental damage compensation.

telegram · zaihuapd · Jul 29, 10:59

**Background**: China has been strengthening its legal framework against cyberbullying. In 2024, the 'Regulations on the Governance of Cyber Violence Information' were issued as departmental rules. The new draft law, if passed, would elevate these measures to a law passed by the National People's Congress, providing stronger legal force and specifically addressing AI-generated abuse.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gov.cn/zhengce/202501/content_6997441.htm">网络暴力信息治理规定_国家互联网信息办公室_中国政府网</a></li>
<li><a href="https://www.moj.gov.cn/pub/sfbgw/flfggz/flfggzbmgz/202410/t20241009_507262.html">网络暴力信息治理规定</a></li>

</ul>
</details>

**Tags**: `#cyberbullying`, `#AI regulation`, `#China internet law`, `#content moderation`, `#policy`

---