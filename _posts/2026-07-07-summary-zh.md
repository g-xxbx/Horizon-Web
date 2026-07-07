---
layout: default
title: "Horizon Summary: 2026-07-07 (ZH)"
date: 2026-07-07
lang: zh
---

> 从 38 条内容中筛选出 14 条重要资讯。

---

1. [MIRA：用于多人火箭联盟的 50 亿参数世界模型](#item-1) ⭐️ 9.0/10
2. [OpenWrt One：首款官方开源硬件路由器](#item-2) ⭐️ 8.0/10
3. [GLM 5.2 与即将到来的 AI 利润崩塌](#item-3) ⭐️ 8.0/10
4. [Ternlight：7MB 嵌入模型通过 WASM 在浏览器中运行](#item-4) ⭐️ 8.0/10
5. [Anthropic 发现语言模型中的全局工作空间](#item-5) ⭐️ 8.0/10
6. [微软重组 Xbox 部门以提升利润率](#item-6) ⭐️ 8.0/10
7. [腾讯发布 Hy3：295B 参数的 MoE 模型，采用 Apache 2.0 许可](#item-7) ⭐️ 8.0/10
8. [英伟达 GPU 债务担保推动 7 万亿美元 AI 基础设施热潮](#item-8) ⭐️ 8.0/10
9. [LingBot-Vision：用于自监督学习的掩码边界建模](#item-9) ⭐️ 8.0/10
10. [TRACE：开源层级记忆系统提升 LLM 智能体性能](#item-10) ⭐️ 8.0/10
11. [SpaceX 猎鹰 9 号再入大气层产生锂羽流](#item-11) ⭐️ 8.0/10
12. [马斯克解散 xAI，更名为 SpaceXAI](#item-12) ⭐️ 8.0/10
13. [中国拟五年投入 2 万亿元建设全国算力网络](#item-13) ⭐️ 8.0/10
14. [New-API 修复计费漏洞：超大参数导致负数扣费](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [MIRA：用于多人火箭联盟的 50 亿参数世界模型](https://www.reddit.com/r/MachineLearning/comments/1upofuw/mira_multiplayer_interactive_world_models_trained/) ⭐️ 9.0/10

MIRA 是一个拥有 50 亿参数的世界模型，基于 10,000 小时的合成火箭联盟数据训练，可在单个 NVIDIA B200 GPU 上以每秒 20 帧的速度实现 4 人交互式模拟。团队发布了可玩的在线演示、技术报告以及一个包含 1,000 小时 4 人游戏数据的数据集。 这是迈向多人游戏大规模交互式世界模型的开创性一步，可能改变游戏 AI、模拟和强化学习研究。代码、数据集和模型的开源发布降低了世界建模领域进一步创新的门槛。 该模型在单个 B200 GPU 上以 20 fps 的速度运行 4 人游戏，B200 配备 180 GB HBM3e 显存，功耗 1000 瓦。合成数据集是通过火箭联盟回放文件和游戏统计 API 生成的。

reddit · r/MachineLearning · /u/MasterScrat · 7月7日 07:59

**背景**: AI 中的世界模型是一种机器学习系统，它构建环境的内部表示，并预测环境如何响应动作而变化。火箭联盟是一款流行的车辆足球视频游戏，提供丰富的连续状态-动作数据，非常适合训练此类模型。NVIDIA B200 是一款基于 Blackwell 架构的高端 GPU，专为 AI 工作负载设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/dgx-b200/">DGX B200: The Foundation for Your AI Factory | NVIDIA</a></li>
<li><a href="https://www.techpowerup.com/gpu-specs/b200.c4210">NVIDIA B200 Specs | TechPowerUp GPU Database</a></li>

</ul>
</details>

**标签**: `#world models`, `#reinforcement learning`, `#multiplayer`, `#Rocket League`, `#open-source`

---

<a id="item-2"></a>
## [OpenWrt One：首款官方开源硬件路由器](https://openwrt.org/toh/openwrt/one) ⭐️ 8.0/10

OpenWrt One 作为 OpenWrt 社区首款官方开源硬件路由器板已发布，售价 89 美元。它采用 MediaTek MT7981B SoC，支持双频 Wi-Fi 6、PoE 和 mikroBUS 扩展接口。 该设备标志着开源网络领域的一个里程碑，提供完全由社区支持、不可变砖的路由器，优先考虑用户控制和可修复性。它可能推动 OpenWrt 的更广泛采用，并激发类似的开放硬件计划。 OpenWrt One 设计为不可变砖，配有硬件开关可分别刷写 NOR 和 NAND 闪存。它包含两个以太网口、三个 USB 端口，默认运行 OpenWrt，也可运行 Debian 等其他操作系统。

hackernews · peter_d_sherman · 7月6日 18:23 · [社区讨论](https://news.ycombinator.com/item?id=48808482)

**背景**: OpenWrt 是一个面向嵌入式设备的开源 Linux 发行版，广泛用于替换路由器厂商固件以增强功能和延长寿命。OpenWrt One 是 OpenWrt 社区与 Banana Pi 及软件自由保护组织合作开发的首款官方硬件板。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openwrt.org/toh/openwrt/one">[OpenWrt Wiki] OpenWrt One</a></li>
<li><a href="https://www.tomshardware.com/networking/open-source-openwrt-one-router-released-at-usd89-hacker-friendly-device-sports-two-ethernet-ports-three-usb-ports-with-dual-band-wi-fi-6">Open-source OpenWrt One router released at $89 — 'hacker ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenWrt">OpenWrt - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体积极，用户对开放硬件方法以及即将推出的支持 Wi-Fi 7 的 OpenWrt Two 表示兴奋。一些用户指出 OpenWrt 安装可能复杂，但赞赏项目的持久性和延长路由器寿命的能力。

**标签**: `#openwrt`, `#open hardware`, `#router`, `#networking`, `#open source`

---

<a id="item-3"></a>
## [GLM 5.2 与即将到来的 AI 利润崩塌](https://martinalderson.com/posts/the-upcoming-ai-margin-collapse-part-1-glm-5-2/) ⭐️ 8.0/10

Martin Alderson 认为，像 GLM 5.2 这样的开放权重模型（其价格仅为专有模型的 15-20%）将把 AI 推理利润推向零，类似于过去云和软件领域的商品化过程。 如果利润崩塌，主要提供商当前的高成本 AI 商业模式可能变得不可持续，从而可能重塑整个 AI 生态系统并加速开源替代方案的采用。 GLM 5.2 是 Z.AI 的旗舰模型，拥有 100 万 token 的上下文，能够处理小程序开发等长周期任务，并以开放权重形式在 Hugging Face 和 Ollama 上提供。

hackernews · martinald · 7月6日 20:14 · [社区讨论](https://news.ycombinator.com/item?id=48809877)

**背景**: AI 行业目前对 GPT-4 和 Claude 等专有模型保持高利润率，但开放权重模型历史上曾压低其他技术领域的价格。GLM 5.2 代表了有能力的新一波开放模型，可能颠覆这种定价能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://martinalderson.com/posts/the-upcoming-ai-margin-collapse-part-1-glm-5-2/">GLM 5.2 and the coming AI margin collapse (part 1) - Martin Alderson</a></li>
<li><a href="https://huggingface.co/zai-org/GLM-5.2">zai-org/GLM-5.2 · Hugging Face</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM-5.2 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：有人认为原始成本并不能保证市场主导地位（以云和办公套件为例），而另一些人则认为当前 AI 成本对其用例来说已经微不足道。一些用户已经开始通过 OpenRouter 等 API 转向更便宜的开源模型。

**标签**: `#AI`, `#economics`, `#open-source`, `#commoditization`, `#GLM`

---

<a id="item-4"></a>
## [Ternlight：7MB 嵌入模型通过 WASM 在浏览器中运行](https://ternlight-demo.vercel.app/) ⭐️ 8.0/10

Ternlight 是一个从 MiniLM 蒸馏而来的 7MB 嵌入模型，采用三元量化，并通过 Rust/WASM SIMD 完全在浏览器中运行，实现高效的语义相似度计算。 这使得无需服务器调用的实用客户端语义搜索成为可能，保护用户隐私并降低延迟，对隐私敏感应用和离线可用的网络工具意义重大。 该模型输出 384 维嵌入向量，采用三元量化感知训练来缩小体积同时保持质量；推理引擎用 Rust 从头编写，并通过 SIMD 指令编译为 WebAssembly。

hackernews · soycaporal · 7月6日 23:06 · [社区讨论](https://news.ycombinator.com/item?id=48811644)

**背景**: 嵌入模型将文本转换为捕获语义含义的数值向量，从而实现相似性搜索。传统模型过大，不适合浏览器使用；Ternlight 使用三元量化（权重限制为-1、0、+1）和 WebAssembly SIMD，实现了极小的体积和快速的 CPU 推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2303.01505">[2303.01505] Ternary Quantization: A Survey</a></li>
<li><a href="https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2">sentence-transformers/all-MiniLM-L6-v2 · Hugging Face</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/WebAssembly/Reference/SIMD">WebAssembly SIMD-specific instructions - WebAssembly | MDN</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞该项目的创新性和实用价值，并建议与 DuckDB HNSW 搜索集成以及用于本地隐私保护搜索。一位用户指出演示页面突然的 CPU 飙升令人吃惊，建议添加按钮来触发演示。

**标签**: `#embedding models`, `#WASM`, `#quantization`, `#browser ML`, `#semantic search`

---

<a id="item-5"></a>
## [Anthropic 发现语言模型中的全局工作空间](https://www.anthropic.com/research/global-workspace) ⭐️ 8.0/10

Anthropic 的研究在 Claude 中识别出一小簇内部模式，称为“J 空间”，它充当全局工作空间，使模型能够在不同上下文中进行连贯推理。 这一发现提供了对语言模型如何保持连贯性并执行高阶推理的机制理解，将 AI 研究与全局工作空间理论等认知科学概念联系起来。 J 空间不参与大多数常规任务，如流利说话或事实回忆；当阻止 Claude 使用它时，模型会失去高阶认知功能，但其他行为正常。

hackernews · in-silico · 7月6日 17:44 · [社区讨论](https://news.ycombinator.com/item?id=48808002)

**背景**: 全局工作空间理论最初来自神经科学，提出意识思维将来自不同脑模块的信息整合到一个统一的工作空间中。Anthropic 的研究将这一概念应用于 AI，表明语言模型可能具有类似的内部机制，跨层整合信息以实现连贯推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/global-workspace">A global workspace in language models \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Global_workspace_theory">Global workspace theory - Wikipedia</a></li>
<li><a href="https://www.lesswrong.com/posts/3PaLrzxagpbnNtPLT/a-global-workspace-in-language-models">A global workspace in language models</a></li>

</ul>
</details>

**社区讨论**: 评论者指出与先前实验的相似之处，例如复制解决数学问题的层以提高性能，并讨论了 J 空间是否真正类似于意识。一些人认为这些发现与训练动态的预期一致，而另一些人则呼吁与人类认知进行更直接的比较。

**标签**: `#AI research`, `#language models`, `#Anthropic`, `#model internals`, `#neural networks`

---

<a id="item-6"></a>
## [微软重组 Xbox 部门以提升利润率](https://news.xbox.com/en-us/2026/07/06/resetting-xbox/) ⭐️ 8.0/10

微软宣布对 Xbox 部门进行重大重组，旨在解决尽管每季度营收达 50 亿美元但利润率偏低的问题。此举包括精简运营，并可能让工作室恢复独立以重回增长。 此次重组标志着 Xbox 战略转向，从激进的 Game Pass 扩张和收购转向追求盈利，可能重塑主机战争格局，并影响整个游戏行业对可持续商业模式的关注。 该部门每季度营收约 50 亿美元，但利润仅 1.5-1.6 亿美元，利润率微薄且无增长。据报道，CEO Asha 将过去的失误归咎于公司管理层，并计划在可能的情况下让工作室恢复独立运营。

hackernews · dijksterhuis · 7月6日 14:18 · [社区讨论](https://news.ycombinator.com/item?id=48804993)

**背景**: Xbox 一直是与索尼和任天堂并列的游戏主机市场主要参与者。近年来，微软大力投资 Game Pass 订阅服务和工作室收购（如 Bethesda、动视暴雪）以参与竞争，但这些策略并未转化为相应的利润增长。

**社区讨论**: 评论者反应不一：有人批评微软无法将游戏作为艺术形式来管理，也有人指出任天堂在简单游戏上的成功与 Xbox 专注于电影化大制作形成对比。多位用户对裁员表示同情，并将糟糕的战略决策归咎于前负责人 Phil Spencer。

**标签**: `#Xbox`, `#Microsoft`, `#gaming industry`, `#corporate strategy`, `#profitability`

---

<a id="item-7"></a>
## [腾讯发布 Hy3：295B 参数的 MoE 模型，采用 Apache 2.0 许可](https://simonwillison.net/2026/Jul/6/hy3/#atom-everything) ⭐️ 8.0/10

腾讯发布了 Hy3，这是一个 295B 参数的混合专家（MoE）语言模型，具有 21B 激活参数和 3.8B MTP 层参数，采用宽松的 Apache 2.0 许可。该模型在 OpenRouter 上免费提供，截止到 2026 年 7 月 21 日。 Hy3 的性能优于同尺寸模型，并能与参数规模大 2-5 倍的旗舰开源模型相媲美，这使其成为开源 AI 生态系统的重要补充。其 Apache 2.0 许可和免费可用性降低了开发者和研究人员的门槛。 完整模型在 Hugging Face 上为 598GB，FP8 量化版本为 300GB，支持 256K 上下文长度。该模型由腾讯混元团队开发，并在预览阶段吸收了来自 50 多个产品的反馈。

rss · Simon Willison · 7月6日 23:57

**背景**: 混合专家（MoE）是一种机器学习技术，每个输入只激活多个专门子网络（专家）中的一部分，从而以比密集模型更少的计算量实现高效扩展。Hy3 使用门控机制将 token 路由到相关专家，在 295B 总参数中仅激活 21B 参数即可实现高性能。MTP（多 token 预测）是一个辅助头，可同时预测多个未来 token，从而提升推理速度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>

</ul>
</details>

**标签**: `#AI`, `#open-source`, `#LLM`, `#MoE`, `#Tencent`

---

<a id="item-8"></a>
## [英伟达 GPU 债务担保推动 7 万亿美元 AI 基础设施热潮](https://newsletter.semianalysis.com/p/nvidia-gpu-debt-backstop-unleashes) ⭐️ 8.0/10

英伟达推出了一项为期 6 年的 GPU 担保计划，为新型云（neocloud）GPU 集群和数据中心租赁提供最低收入保障，旨在解锁预计到 2029 年将达到 7.1 万亿美元的 AI 计算建设债务融资。 这一机制将计算访问范围扩大到超大规模云服务商和大型 AI 实验室之外，使新型云得以发展并加速 AI 基础设施部署。同时，它将风险从贷款方转移至英伟达，可能重塑 AI 融资格局。 该计划要求构建“AI 项目三位一体”，即资本、承购协议和数据中心。目前，贷款方在提供债务融资前要求有承购合同或来自投资级超大规模云服务商的担保。

rss · Semianalysis · 7月6日 21:53

**背景**: 历史上，AI 建设主要由谷歌、亚马逊、Meta 和微软等超大规模云服务商通过现金流资助。过去一年，即使是这些巨头也开始转向债务融资。英伟达的担保计划旨在填补新型云的资金缺口，这些新型云缺乏独立获得贷款的信用评级。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/nvidia-gpu-debt-backstop-unleashes">Nvidia GPU Debt Backstop Unleashes the AI Project Trinity ...</a></li>
<li><a href="https://www.newsbang.com/news/article/story_id-p008-154842">Nvidia Launches 6-Year GPU Backstop Program to Unlock AI ...</a></li>
<li><a href="https://digg.com/tech/finswqcv">SemiAnalysis CEO Dylan Patel projects AI debt financing will exceed...</a></li>

</ul>
</details>

**社区讨论**: 一些批评者警告称，7 万亿美元的 AI 债务和资本支出预测可能助长不可持续的泡沫，并将其与过去的金融危机相提并论。其他人则对做出这些预测的分析师表示不信任。

**标签**: `#Nvidia`, `#AI infrastructure`, `#debt financing`, `#neocloud`, `#datacenter economics`

---

<a id="item-9"></a>
## [LingBot-Vision：用于自监督学习的掩码边界建模](https://www.reddit.com/r/MachineLearning/comments/1up4cjh/lingbotvision_masked_boundary_modeling_for/) ⭐️ 8.0/10

LingBot-Vision 提出了掩码边界建模方法，教师网络生成密集边界场并强制学生重建边界区域，在 NYUv2 线性探测深度估计任务上以 1.1B 参数模型达到 0.296 RMSE，优于 DINOv3-7B（0.309 RMSE），且参数量大幅减少。 这项工作表明，明确引导自监督学习聚焦于边界区域可以产生更高效、更有效的视觉表征，有望减少下游任务（如深度估计和分割）对大规模模型和数据的需求。 该方法使用逐像素分类分布表示边界场以避免 EMA 教师下的崩溃，并应用 a-contrario 验证测试过滤解码片段。模型在 1.61 亿张图像上训练（不到 DINOv3 数据的三分之一），在编码器初始化研究中表现出一致优势，但在 ImageNet 分类和 ADE20K 分割上仍落后于 DINOv3。

reddit · r/MachineLearning · /u/StillThese3747 · 7月6日 17:37

**背景**: 自监督学习旨在从无标签数据中学习有用的表征。掩码图像建模是一种流行的自监督学习范式，模型需要重建被掩码的图像部分。DINOv3 是一种最先进的自监督学习方法，使用自蒸馏并在多种视觉任务上表现优异。LingBot-Vision 在此基础上，通过显式掩码教师预测的边界区域来改进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2401.00897">[2401.00897] Masked Modeling for Self-supervised ... - arXiv.org</a></li>
<li><a href="https://www.catalyzex.com/s/Nyuv2">Nyuv 2</a></li>
<li><a href="https://centreborelli.ens-paris-saclay.fr/en/node/3050">CLOUD DETECTION BY INTER-BAND PARALLAX AND A-CONTRARIO VALIDATION</a></li>

</ul>
</details>

**社区讨论**: 社区讨论有限，但指出 NYUv2 上 0.013 的 RMSE 改进可能受探测超参数影响，且缺乏与 ADIOS/AttMask 等硬掩码基线的消融实验令人担忧。作者承认 DINOv3 的 Gram 锚定仍然需要，表明边界强制是补充而非替代。

**标签**: `#self-supervised learning`, `#computer vision`, `#representation learning`, `#depth estimation`, `#ViT`

---

<a id="item-10"></a>
## [TRACE：开源层级记忆系统提升 LLM 智能体性能](https://www.reddit.com/r/MachineLearning/comments/1uoz5jo/trace_opensource_hierarchical_memory_for_llm/) ⭐️ 8.0/10

TRACE 是一个面向 LLM 智能体的开源层级记忆系统，它将对话历史组织成带有分支和摘要的主题树，在使用 gpt-oss-20B 模型时，在 MemoryAgentBench 的 EventQA 任务上达到了 82.5% 的 F1 分数。 这表明层级记忆方法即使使用较小的开源权重模型，也能显著优于基于扁平 RAG 的方法（例如 Mem0 的 37.5% 和 MemGPT 的 26.2%），从而使高级记忆能力更加可及且成本更低。 基准测试在本地使用 gpt-oss-20B，并非与相同骨干模型的直接对比；作者指出 Mem0 的事实提取步骤需要严格的 JSON 输出，而 gpt-oss 无法干净解析，且 Letta 需要完整的服务器设置。

reddit · r/MachineLearning · /u/PsychologicalDot7749 · 7月6日 14:35

**背景**: LLM 智能体通常难以处理长期记忆，依赖将过去所有交互同等对待的扁平检索增强生成（RAG）。像 TRACE 这样的层级记忆系统将信息组织成主题树，从而实现更高效的检索和上下文理解。MemoryAgentBench 是一个评估 LLM 智能体记忆的基准套件，其中 EventQA 专注于时间事件推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2506.07398">[2506.07398] G-Memory: Tracing Hierarchical Memory for Multi ... H-MEM: Hierarchical Memory for High-Efficiency Long-Term ... H-MEM: Hierarchical Memory for High-Efficiency Long-Term ... H-MEM: Hierarchical Memory for High-Efciency Long-Term ... TeleAI-UAGI/Awesome-Agent-Memory - GitHub IAAR-Shanghai/Awesome-AI-Memory - GitHub G-Memory: Tracing Hierarchical Memory for Multi-Agent Systems</a></li>
<li><a href="https://github.com/HUST-AI-HYZ/MemoryAgentBench">GitHub - HUST-AI-HYZ/ MemoryAgentBench : Open source code for...</a></li>
<li><a href="https://openai.com/index/introducing-gpt-oss/">Introducing gpt-oss - OpenAI</a></li>

</ul>
</details>

**社区讨论**: Reddit 讨论称赞了这项工作的新颖方法和强劲结果，一些用户质疑与不同骨干模型上的闭源模型进行比较的公平性。作者承认了这一局限性，并提供了完整的 JSON 日志以保证透明度。

**标签**: `#LLM`, `#memory`, `#open-source`, `#benchmark`, `#agents`

---

<a id="item-11"></a>
## [SpaceX 猎鹰 9 号再入大气层产生锂羽流](https://t.me/zaihuapd/42387) ⭐️ 8.0/10

一项《自然·通讯》研究利用激光雷达在 96 公里高空直接测量到 2025 年 2 月 19 日 SpaceX 猎鹰 9 号上面级在欧洲上空失控再入产生的锂污染羽流，锂浓度飙升 10 倍。 这是首次直接探测到火箭再入产生的金属污染，凸显了随着火箭发射增加，快速发展的航天业面临的新环境问题。 羽流被观测了 27 分钟，并追溯到猎鹰 9 号上面级的失控再入路径；该研究于 2026 年 2 月 19 日发表在《通讯·地球与环境》上。

telegram · zaihuapd · 7月6日 11:17

**背景**: 火箭上面级经常失控再入大气层，燃烧并释放锂、铝、铜等金属。锂用于火箭燃料和电池合金。激光雷达（LiDAR）利用激光脉冲探测大气颗粒物。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nature.com/articles/s43247-025-03154-8">Measurement of a lithium plume from the uncontrolled re-entry of a Falcon 9 rocket | Communications Earth & Environment</a></li>
<li><a href="https://www.sciencenews.org/article/rocket-reentry-metal-pollution-detected">Metal pollution from a rocket reentry detected for the first time</a></li>
<li><a href="https://gizmodo.com/study-confirms-reentering-spacex-rockets-are-peppering-the-upper-atmosphere-with-metal-pollution-2000723932">Study Confirms: Reentering SpaceX Rockets Are Peppering the Upper...</a></li>

</ul>
</details>

**标签**: `#space pollution`, `#SpaceX`, `#atmospheric science`, `#environmental impact`, `#rocket reentry`

---

<a id="item-12"></a>
## [马斯克解散 xAI，更名为 SpaceXAI](https://x.com/i/status/2074214064746832060) ⭐️ 8.0/10

埃隆·马斯克宣布解散作为独立公司的 xAI，将其更名为 SpaceXAI 并并入 SpaceX。该公告于 2026 年 5 月 6 日发布，此前 SpaceX 已于 2026 年 2 月收购了 xAI。 此次整合标志着 AI 格局的重大转变，xAI 的技术（包括 Grok）和团队将完全融入 SpaceX 的运营。这标志着马斯克将 AI 开发集中到 SpaceX 品牌下的战略，可能加速 AI 在太空探索及其他领域的应用。 此次收购对 SpaceX 的估值为 1 万亿美元，对 xAI 的估值为 2500 亿美元。xAI 的旗舰产品包括 AI 聊天机器人 Grok 和于 2025 年 3 月收购的社交网络 X。该公司还建造了 Colossus 超级计算机并启动了数据中心业务。

telegram · zaihuapd · 7月7日 02:30

**背景**: xAI 由埃隆·马斯克于 2023 年创立，是一家独立的 AI 公司，旨在与 OpenAI 等公司竞争。它开发了对话式 AI 聊天机器人 Grok，后来收购了社交媒体平台 X。2026 年 2 月，SpaceX 以全股票交易收购了 xAI，使其成为全资子公司。更名为 SpaceXAI 标志着整合的完成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/XAI_(company)">SpaceXAI - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/SpaceXAI">SpaceXAI</a></li>
<li><a href="https://www.fifthrow.com/blog/from-x-ai-to-space-xai-how-elon-musk-s-bold-integration-is-reshaping-ai-venture-building-and-the-innovation-playbook">From xAI to SpaceXAI: How Elon Musk’s Bold Integration Is Reshaping AI, Venture Building, and the Innovation Playbook | FifthRow – Autonomous AI Apps for Research, Strategy, Consulting</a></li>

</ul>
</details>

**标签**: `#Elon Musk`, `#xAI`, `#SpaceX`, `#AI`, `#corporate restructuring`

---

<a id="item-13"></a>
## [中国拟五年投入 2 万亿元建设全国算力网络](https://t.me/zaihuapd/42399) ⭐️ 8.0/10

中国计划未来五年投入约 2 万亿元（2950 亿美元），建设全国互联数据中心网络，并优先采用华为等本土供应商的 AI 芯片，占比至少八成。 这一大规模基础设施投资旨在减少中国对英伟达、AMD 等美国芯片供应商的依赖，同时将分散的区域算力资源整合为统一网络，以提升 AI 和高性能计算能力。 中国电信、中国联通等国有电信企业将运营主要设施，并已推出 Token 套餐，将算力像移动数据一样打包销售，降低了 AI 模型的使用成本。

telegram · zaihuapd · 7月7日 04:45

**背景**: 该计划是北京“六网”基础设施计划的关键一环，旨在构建全国一体化算力体系。Token 套餐，例如中国移动低至 5.99 元的算力次包，允许用户按需付费使用算力，类似于移动数据套餐。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.21jingji.com/article/20260518/herald/9dd8ac86feed239fb9fd341ba64265ec.html">三大运营商开卖Token套餐，AI算力进入“话费账单”时代 - 21经济网</a></li>

</ul>
</details>

**标签**: `#China`, `#AI infrastructure`, `#computing network`, `#chip localization`, `#government investment`

---

<a id="item-14"></a>
## [New-API 修复计费漏洞：超大参数导致负数扣费](https://github.com/QuantumNous/new-api/commit/d0bd8aa) ⭐️ 8.0/10

QuantumNous/new-api 项目修复了一个计费漏洞：用户可控的超大参数可触发整数溢出，导致配额扣减变为负数，产生类似反向充值的效应。 此修复防止了对 API 计费系统的财务利用，保护了服务提供商和用户免受潜在损失或未经授权的信用增益。它凸显了在财务逻辑中输入验证的重要性。 修复对参数增加了上限校验，并引入饱和算术逻辑，防止配额计算结果在转为整数时回绕为负数。还补充了其他入口的边界检查，阻止通过超大数字绕过类型检查的攻击。

telegram · zaihuapd · 7月7日 07:26

**背景**: 整数溢出发生在算术运算结果超出给定整数类型可表示的最大值时，导致结果回绕为负数或很小的数。在计费系统中，这可能导致错误的扣费。饱和算术将结果限制在预定义范围内，而不是回绕，从而防止此类漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.invicti.com/learn/integer-overflow">Integer Overflow</a></li>
<li><a href="https://en.wikipedia.org/wiki/Saturation_arithmetic">Saturation arithmetic</a></li>
<li><a href="https://deepwiki.com/QuantumNous/new-api/2.6-quota-and-billing-system">Quota & Billing System | QuantumNous/new-api | DeepWiki</a></li>

</ul>
</details>

**标签**: `#security`, `#billing`, `#vulnerability`, `#open-source`, `#API`

---