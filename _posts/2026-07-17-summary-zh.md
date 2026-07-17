---
layout: default
title: "Horizon Summary: 2026-07-17 (ZH)"
date: 2026-07-17
lang: zh
---

> 从 32 条内容中筛选出 5 条重要资讯。

---

1. [完整 Firefox 浏览器通过 WebAssembly 在浏览器内运行](#item-1) ⭐️ 9.0/10
2. [特斯拉无方向盘 Cybercab 在北美启动量产](#item-2) ⭐️ 9.0/10
3. [在宜居带类地行星上首次发现大气层](#item-3) ⭐️ 8.0/10
4. [开源人工智能现状报告](#item-4) ⭐️ 8.0/10
5. [Kimi 发布 2.8 万亿参数开源模型 K3](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [完整 Firefox 浏览器通过 WebAssembly 在浏览器内运行](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter 将完整版 Firefox 浏览器编译为 WebAssembly，使其能在另一浏览器中通过基于 WebSocket 的 Wisp 协议完整运行。这一突破性技术展示了在 Web 环境中运行复杂原生应用的可行性。 这一成就可能彻底改变便携式计算和沙箱技术——任何浏览器都能托管另一个完整的加密浏览器。该项目还展示了 AI 辅助编程的强大能力，利用 Claude Opus 和 Fable tokens 攻克了重大工程难题。 该演示使用 Wisp 协议通过 Puter 的服务器代理所有网络流量，因为 WebAssembly 代码无法直接打开网络连接。编译后的 gecko.wasm 大小为 233MB，项目估计使用了价值 25,000 美元的 AI 模型 tokens，但由于 Claude Max 订阅计划，实际成本低得多。

rss · Simon Willison · 7月16日 23:34

**背景**: WebAssembly (Wasm) 是一种低级二进制指令格式，能在 Web 浏览器中以接近原生速度运行，支持游戏等高性能应用，如今甚至能运行完整浏览器。Gecko 是 Firefox 的浏览器引擎，因其强大的单进程支持而著称，这使其成为编译到 WebAssembly 的理想候选。Wisp 协议是一种轻量级方式，可通过单个 WebSocket 连接代理多个 TCP/UDP 套接字，使 Wasm 代码能与外界通信。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to implement protocol for proxying multiple TCP/UDP sockets over a single websocket. · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gecko_(browser_engine)">Gecko (browser engine)</a></li>

</ul>
</details>

**标签**: `#WebAssembly`, `#Firefox`, `#Gecko`, `#Browser-in-browser`, `#Wisp protocol`

---

<a id="item-2"></a>
## [特斯拉无方向盘 Cybercab 在北美启动量产](https://t.me/zaihuapd/42621) ⭐️ 9.0/10

特斯拉于 2026 年 2 月在德州超级工厂开始量产其完全无人驾驶电动车 Cybercab，该车取消了方向盘、踏板和后视镜，完全由 AI 驾驶。 这标志着自动驾驶技术商业化的重要里程碑——Cybercab 是特斯拉首款完全为无人驾驶设计的车型，也是推进 Robotaxi 业务的关键一步，可能颠覆网约车和个人出行行业。 Cybercab 是一款双座电动车，完全依赖特斯拉的完全自动驾驶（FSD）系统，但该软件目前仍需人工监督，尚未实现完全无人驾驶。车辆专为 Robotaxi 服务设计，没有方向盘、踏板或后视镜。

telegram · zaihuapd · 7月17日 03:06

**背景**: Cybercab 是特斯拉 Robotaxi 计划的一部分，旨在部署全自动无人驾驶车队用于网约车服务。与特斯拉的乘用车不同，该车完全围绕自动驾驶设计，取消了人工驾驶控制。特斯拉多年来一直开发其 FSD 软件，目标是实现 L5 级完全自动驾驶，但技术和监管挑战依然存在。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tesla_Cybercab">Tesla Cybercab - Wikipedia</a></li>
<li><a href="https://electrek.co/2026/07/06/tesla-cybercab-production-before-autonomy/">Tesla Cybercab: mass-producing a car it can't sell or drive itself | Electrek</a></li>
<li><a href="https://insideevs.com/news/787560/tesla-cybercab-robotaxi-giga-texas-production/">Tesla Begins Cybercab Production. Now Comes The Hard Part</a></li>

</ul>
</details>

**标签**: `#特斯拉`, `#Cybercab`, `#自动驾驶`, `#Robotaxi`, `#电动汽车`

---

<a id="item-3"></a>
## [在宜居带类地行星上首次发现大气层](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

詹姆斯·韦伯太空望远镜在距地球 48 光年的红矮星宜居带内的岩石行星 LHS 1140b 上探测到了大气层，排除了它是一颗迷你海王星的可能性。 这一发现首次确认了红矮星宜居带内岩石行星上存在大气层，是寻找地外生命的关键一步，也展示了韦伯望远镜在系外行星特性刻画方面的强大能力。 该探测利用了韦伯望远镜在行星二次凌星期间的发射光谱。大气中含有氦气，暗示其逃逸速度很高。该行星 LHS 1140b 距离地球 48 光年。

hackernews · neversaydie · 7月17日 14:06 · [社区讨论](https://news.ycombinator.com/item?id=48947560)

**背景**: 宜居带是指恒星周围允许行星表面存在液态水的区域。红矮星是小型、温度较低的恒星，因此其宜居带非常靠近恒星，这使行星常常受到强烈的恒星辐射。迷你海王星是拥有浓厚氢氦大气层的行星，与岩石质类地行星不同。詹姆斯·韦伯太空望远镜（JWST）能够通过凌星光谱分析系外行星的大气层。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mini-Neptune">Mini - Neptune - Wikipedia</a></li>
<li><a href="https://earthsky.org/space/super-earth-mini-neptune-and-sub-neptune-exoplanets-definitions/">Super-Earth, mini - Neptune or sub-Neptune?</a></li>

</ul>
</details>

**社区讨论**: 社区评论最初对 LHS 1140b 是否类地表示怀疑，指出红矮星会剥离大气层。但韦伯数据排除了迷你海王星的可能性得到了认可。有人建议建造太阳透镜望远镜并讨论星际推进，还有人指出氦气探测表明逃逸速度很高。

**标签**: `#exoplanet`, `#atmosphere`, `#habitable zone`, `#JWST`, `#red dwarf`

---

<a id="item-4"></a>
## [开源人工智能现状报告](https://stateofopensource.ai/) ⭐️ 8.0/10

Mozilla 发布了一份报告，分析开源人工智能的当前现状和趋势，引发了社区广泛讨论。 报告强调了开放模型在人工智能领域日益占据主导地位，这可能重塑行业格局并影响 OpenAI 和 Anthropic 等主要参与者。 报告包含大量图表和数据点，但部分社区成员批评其呈现方式过度依赖 AI 生成内容，缺乏原创分析。

hackernews · rellem · 7月17日 14:31 · [社区讨论](https://news.ycombinator.com/item?id=48947825)

**背景**: 开源人工智能指那些公开提供使用、修改和分发权限的 AI 模型，通常采用宽松许可证。这与 OpenAI 和 Google 等公司的封闭、专有模型形成对比。争论焦点在于开放或封闭模型将如何推动未来的创新和可及性。

**社区讨论**: 社区评论呈现混合反应：一些人庆祝开放模型的快速增长并预测封闭 AI 公司的衰落，另一些人批评报告质量，认为其看起来是由 AI 生成且缺乏深刻见解。

**标签**: `#open source`, `#artificial intelligence`, `#industry analysis`, `#community discussion`

---

<a id="item-5"></a>
## [Kimi 发布 2.8 万亿参数开源模型 K3](https://t.me/zaihuapd/42619) ⭐️ 8.0/10

Kimi 宣布开源模型 K3，拥有 2.8 万亿参数，支持高达 1M token 的上下文。它采用稀疏混合专家架构，包含 896 个专家，每次激活 16 个，并集成了 Kimi Delta Attention 和 Attention Residuals 机制。 如果被证实，K3 将成为有史以来最大的开源模型，其性能据称可与顶级闭源模型相媲美。但与其比较的 Claude Fable 5 和 GPT-5.6 Sol 很可能是虚构的，这削弱了公信力。 K3 基于 Kimi Delta Attention 和 Attention Residuals，采用稀疏 MoE 设计，每个 token 从 896 个专家中激活 16 个。完整权重据称将在未来几天内开放，但该消息来自 Telegram 频道而非官方渠道。

telegram · zaihuapd · 7月17日 00:02

**背景**: 稀疏混合专家（MoE）是一种技术，模型使用多个专门化的子网络（专家），但每个输入只激活少数几个，从而提高效率。Kimi Delta Attention 是一种线性注意力变体，能够以较低的计算成本处理长上下文。Attention Residuals 允许每个 Transformer 层动态组合来自前几层的表示，可能提升性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jianyuh.github.io/attention/2025/12/13/KDA.html">Linear Attention : Kimi Delta Attention | Jianyu Huang’s Blog</a></li>
<li><a href="https://github.com/MoonshotAI/Attention-Residuals">GitHub - MoonshotAI/ Attention - Residuals · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sparse_mixture-of-experts">Sparse mixture-of-experts</a></li>

</ul>
</details>

**标签**: `#AI`, `#large language model`, `#open-source`, `#sparse MoE`, `#Kimi`

---