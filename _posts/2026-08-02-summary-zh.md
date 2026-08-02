---
layout: default
title: "Horizon Summary: 2026-08-02 (ZH)"
date: 2026-08-02
lang: zh
---

> 从 28 条内容中筛选出 2 条重要资讯。

---

1. [Karpathy 的“骑着自行车的鹈鹕”基准测试引发 AI 评测讨论](#item-1) ⭐️ 8.0/10
2. [公开信显示 AI 行业在开放权重模型政策上存在分歧](#item-2) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Karpathy 的“骑着自行车的鹈鹕”基准测试引发 AI 评测讨论](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 8.0/10

Andrej Karpathy 在推特上谈到了“骑着自行车的鹈鹕”基准测试，引发了关于 AI 模型是否需要新的定性基准来测试物理世界理解能力（而不仅仅是简单的图像生成）的讨论。这一讨论迅速在 AI 社区扩散，Karpathy 本人也发布了后续推文，谈及该基准的局限性。 这件事很重要，因为它表明 AI 模型的评估方式正在从图像质量转向物理世界理解和推理能力。这一讨论可能影响开发者和研究人员未来设计基准的方式，以及他们优先关注前沿模型的哪些能力。 该基准由开发者 Simon Willison 于 2024 年底提出，使用简单提示词“生成一个骑着自行车的鹈鹕的 SVG”。Karpathy 的后续推文指出，SVG 鹈鹕有一个一眼就能看出的“标准答案”，而可玩游戏则是一个更难在大规模上目测评估的基准。

hackernews · delichon · 8月2日 04:05 · [社区讨论](https://news.ycombinator.com/item?id=49140998)

**背景**: “骑着自行车的鹈鹕”是大型语言模型的一种非正式基准测试，目的是检验模型能否为一个物理上不可能的场面生成有效且视觉连贯的 SVG 代码。它由 Simon Willison 在 2024 年底创建，作为传统基于文本基准的替代方案，因为这些传统基准往往无法捕捉视觉和空间推理中的定性方面。Andrej Karpathy 是著名的 AI 研究者，以深度学习方面的工作以及曾任特斯拉 AI 总监的经历而闻名，因此他的评论在社区中具有相当的分量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/karpathy/status/2083948654377996480">Andrej Karpathy on X: "More on the pelican on the bicycle test from ...</a></li>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark)</a></li>
<li><a href="https://ai.miraheze.org/wiki/Pelican_Bicycle_Benchmark">Pelican Bicycle Benchmark - Learn AI</a></li>

</ul>
</details>

**社区讨论**: 评论者的看法存在分歧：一些人担心这个基准被过早地宣布“解决”，并且长期接触 AI 内容降低了人们对质量的期望；另一些人则认为，这种粗糙的结果恰恰说明模型已经超越了图像生成，正迈向物理理解。还有评论指出，模型可能专门训练过生成 three.js 代码；也有用户开玩笑说要“再深入一层”，让 AI 生成一张“AI 正在生成一张骑着自行车的鹈鹕的 SVG”的 SVG。

**标签**: `#AI`, `#benchmarking`, `#Karpathy`, `#machine learning`, `#evaluation`

---

<a id="item-2"></a>
## [公开信显示 AI 行业在开放权重模型政策上存在分歧](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 8.0/10

Simon Willison 的文章总结了近期关于 AI 开发的公开信。微软牵头的《开放权重与美国 AI 领导力》公开信由包括 NVIDIA、亚马逊和 OpenAI 在内的 235 家公司签署，为开放权重模型和蒸馏技术辩护。 这揭示了 AI 政策上的重大行业分歧，大型科技公司反对美国可能对开放权重模型的限制。这些公开信可能影响 AI 监管、竞争和安全争论。 值得注意的是，Anthropic 拒绝签署并发布了自身立场，警告开放权重被威权政府滥用的风险，并呼吁打击工业规模的蒸馏操作。另一封《Pacing the Frontier》公开信由前沿 AI 实验室的 1,324 名员工签署，敦促美国支持国际治理工具以有节奏地推进 AI 发展。

rss · Simon Willison · 8月2日 04:16

**背景**: 开放权重模型是指其训练参数被公开发布的 AI 模型，任何人都可以下载、运行和修改。这与仅能通过 API 访问的封闭模型形成对比。微软的信件认为，完全依赖封闭模型会造成单点故障并削弱竞争，而批评者则提出安全和滥用方面的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#open weights`, `#AI development`, `#industry letters`

---