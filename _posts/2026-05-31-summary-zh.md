---
layout: default
title: "Horizon Summary: 2026-05-31 (ZH)"
date: 2026-05-31
lang: zh
---

> From 115 items, 10 important content pieces were selected

---

1. [微软将降低 Office 2019/2021 永久许可证功能](#item-1) ⭐️ 8.0/10
2. [OpenRouter 完成 1.13 亿美元 B 轮融资](#item-2) ⭐️ 8.0/10
3. [Thaw：为运行中的 LLM 提供类似 Git 的分支功能并保留 KV 缓存](#item-3) ⭐️ 8.0/10
4. [领域专业知识才是 AI 产品的真正竞争优势](#item-4) ⭐️ 7.0/10
5. [Zig ELF 链接器改进开发日志](#item-5) ⭐️ 7.0/10
6. [深入理解 Comanche 体素空间地形渲染技术](#item-6) ⭐️ 7.0/10
7. [OpenBSD 团队发布 Openrsync 实现](#item-7) ⭐️ 7.0/10
8. [Anthropic 发布跨产品 Claude 沙盒技术文档](#item-8) ⭐️ 7.0/10
9. [通过 Pyodide + Service Worker 在浏览器中运行 Python ASGI 应用](#item-9) ⭐️ 7.0/10
10. [外卖大战后遗症：行业仅需 400 万骑手，实际涌进 2000 万人](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [微软将降低 Office 2019/2021 永久许可证功能](https://consumerrights.wiki/w/Microsoft_Office_2019_and_2021_for_Mac_view-only_conversion_(2026)) ⭐️ 8.0/10

微软宣布计划从 2026 年起削减或取消 Mac 版 Office 2019 和 Office 2021 的核心功能，将这些永久许可的产品转换为仅查看模式，实际上会使其无法用于创建或编辑文档。 这一决定直接影响那些在期望软件可以无限期使用且无需订阅费用的情况下购买永久许可证的消费者，引发了对消费者权益侵犯的严重担忧，以及在向订阅模式转型时代永久软件所有权的价值问题。 根据社区推测，微软可能正在加速这一弃用以推动用户转向 Microsoft 365 订阅，这可能是受到 AI 代理工作流程需要每个实例单独许可的动机启发。该转换专门适用于 Office 2019 和 2021 永久许可证的 Mac 版本。

hackernews · antipurist · May 30, 23:26

**背景**: 永久软件许可证允许用户一次性购买软件并无限期使用，无需持续的订阅费用，这与 SaaS 订阅模式形成对比。微软 Office 传统上同时提供永久许可证版本（如 Office 2019/2021）和基于订阅的 Microsoft 365。永久模式被宣传为“经典固定版本”，类似于过去的 CD 版软件发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.paddle.com/resources/subscription-vs-license">Subscriptions vs licences : The end of the perpetual license model</a></li>
<li><a href="https://en.wikipedia.org/wiki/Microsoft_Office">Microsoft Office - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Comments express strong criticism and legal concerns, with users noting this would violate Australian consumer law guaranteeing the right to undisturbed product possession and fitness for advertised purpose. One hypothesis suggests Microsoft's urgency stems from AI labs using offline Office licenses in agent workflows, where each agent requires a separate license—potentially accelerating the deprecation timeline to force conversions to Microsoft 365.

**标签**: `#consumer-rights`, `#software-licensing`, `#microsoft-office`, `#perpetual-license`, `#tech-industry`

---

<a id="item-2"></a>
## [OpenRouter 完成 1.13 亿美元 B 轮融资](https://openrouter.ai/announcements/series-b) ⭐️ 8.0/10

OpenRouter 已完成 1.13 亿美元的 B 轮融资，保持创始人领导和管理结构，同时扩展其统一 API 网关平台，该平台通过单一的标准化接口提供对来自多个提供商的 400 多个大型语言模型的访问。 这一大额融资表明投资者对人工智能基础设施层充满信心，特别是对聚合商/中间件模型充满信心，该模型为开发者简化了多提供商访问。融资使 OpenRouter 能够继续为全球的人工智能开发者构建产品，同时保持独立性。 OpenRouter 作为统一的 API 网关，通过一个 API 聚合了 400 多个 LLM，包括来自 OpenAI、Anthropic、Google 等提供商提供的模型。用户重视账单上限等功能来限制支出，以及低摩擦的模型测试，尽管与直接提供商访问相比会有 5% 的附加费。

hackernews · freeCandy · May 30, 17:27

**背景**: OpenRouter 作为应用程序与各种 LLM 提供商之间的 API 网关/中间件运行，类似于代理层。这解决了每个提供商具有不同的 API、认证方法和功能集的问题。统一的方法允许开发者在模型和提供商之间切换，而无需更改代码，同时提供集中的账单和使用追踪。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aiwiki.ai/wiki/openrouter">OpenRouter - AI Wiki</a></li>
<li><a href="https://www.codecademy.com/article/what-is-openrouter">What is OpenRouter? A Guide with Practical Examples</a></li>
<li><a href="https://medium.com/@jawherkl/unified-llm-api-gateway-one-api-to-rule-them-all-f9c585d20923">Unified LLM API Gateway: One API to Rule Them All - Medium</a></li>

</ul>
</details>

**社区讨论**: 讨论显示人们对账单上限作为生产环境安全的重要性以及尝试新模型的便利性表示赞赏。联合创始人澄清他们保持创始人控制以进行长期建设。一些用户质疑对 Claude Opus 等昂贵模型的 5% 附加费是否值得，以及如果 LLM 市场整合为少数主导模型，OpenRouter 的价值是否能持续。

**标签**: `#openrouter`, `#funding`, `#ai-infrastructure`, `#llm-api`, `#series-b`

---

<a id="item-3"></a>
## [Thaw：为运行中的 LLM 提供类似 Git 的分支功能并保留 KV 缓存](https://github.com/thaw-ai/thaw) ⭐️ 8.0/10

Thaw 是一个能够对运行中的 LLM 推理会话进行快照的工具，它保存了模型权重、KV 缓存、调度器状态和前缀哈希表，允许 N 个子进程从分叉点 divergence 而无需重新进行预填充——本质上是给正在运行的模型提供类似「git branch」的功能。 这非常重要，因为当前分叉 LLM 代理会浪费大量计算资源——每个分支都需在相同上下文上重新运行预填充，为同一提示支付 N 倍成本。Thaw 实现了约 400 倍的加速（每次分叉轮次 0.88 秒对比约 340 秒），使得并行代理场景如强化学习 rollout、最佳 N 采样和并行编码能够大规模实现。 在 H100 80GB 上使用 Llama-3.1-8B 的基准测试显示：预热池一次性启动需 22.3 秒，之后每轮分叉（4 个分支×64 个令牌）中位时间为 0.88 秒。冷启动等效操作约需 340 秒/轮——约 400 倍的分摊成本。所有轮次在分叉边界处完全一致。支持 vLLM 和 SGLang，采用 Apache-2.0 许可证。

rss · Hacker News - Show HN · May 30, 22:07

**背景**: 在 LLM 推理中，预填充阶段处理输入提示并建立 KV 缓存（键值缓存），而解码阶段使用该缓存自回归地生成输出令牌。当前，在分叉代理时，每个分支都会重新计算预填充阶段，因为 KV 缓存没有被保留——这浪费了计算资源，因为所有分支共享相同的初始上下文。NVIDIA 的 Dynamo Snapshot 采取了相反的方法——在检查点之前释放 KV 缓存，而 Thaw 则保留 KV 缓存以使分叉几乎免费。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/not-lain/kv-caching">KV Caching Explained: Optimizing Transformer Inference Efficiency</a></li>
<li><a href="https://naddod.medium.com/understanding-the-prefill-decode-disaggregation-in-llm-inference-optimization-5c11223a5360">Understanding the Prefill-decode Disaggregation in LLM Inference Optimization | by NADDOD | Medium</a></li>
<li><a href="https://developer.nvidia.com/blog/introducing-nvidia-dynamo-a-low-latency-distributed-inference-framework-for-scaling-reasoning-ai-models/">NVIDIA Dynamo, A Low-Latency Distributed Inference Framework ...</a></li>

</ul>
</details>

**标签**: `#LLM-inference`, `#KV-cache`, `#systems-optimization`, `#AI-agents`, `#performance-engineering`

---

<a id="item-4"></a>
## [领域专业知识才是 AI 产品的真正竞争优势](https://www.brethorsting.com/blog/2026/05/domain-expertise-has-always-been-the-real-moat/) ⭐️ 7.0/10

多位评论者分享了具体的例子：一人描述了一个凭感觉编码（vibe coding）的应用，数据库设计不良导致无法正常上线；另一人描述了一个海洋数据应用（oceanconnect.ca），由于缺乏领域知识，被渔民关于数据使用的具体问题所淹没。

hackernews · aaronbrethorst · May 30, 20:40

**背景**: "护城河"一词来自沃伦·巴菲特的投资理论，指的是可持续的竞争优势。"凭感觉编码"是最近的一种趋势，使用 Cursor 等人工智能工具以最少的编程知识构建应用程序。这场讨论呼应了更广泛的关于人工智能产品开发中什么真正重要的辩论——技术能力、架构设计、品味或领域专业知识。

**社区讨论**: 评论显示出复杂的情绪。一些怀疑论者认为，随着人工智能的发展，这些"什么最重要"的观点不断变化，因此毫无意义。然而，几位评论者提供了支持这一论点的真实案例：一人强调了因数据库问题导致的 vibe coding 应用失败，另一人通过海上导航应用的反馈展示了领域专业知识的价值，表明用户存在复杂的未满足需求。

**标签**: `#AI`, `#software-development`, `#domain-expertise`, `#moat`, `#startups`

---

<a id="item-5"></a>
## [Zig ELF 链接器改进开发日志](https://ziglang.org/devlog/2026/#2026-05-30) ⭐️ 7.0/10

开发日志重点关注 ELF 目标的链接改进。快速增量链接主要是为提高开发效率而设计的，而非发布版本，这就解释了关于与发布构建时的链接时优化兼容性的问题。

hackernews · kristoff_it · May 30, 17:29

**背景**: Zig 是一种设计用于替代 C 的系统编程语言，强调零成本抽象和精确的内存控制。ELF（可执行和可链接格式）是 Linux 和许多类 Unix 系统的标准二进制格式。增量链接允许只重新链接程序的修改部分，而不是整个二进制文件，从而大大加快编辑-编译-测试循环。

**社区讨论**: 整体情绪非常积极——社区成员认为这是一个改变游戏规则的进步，使 Zig 更接近成为'THE C replacements'（终极 C 替代品）。开发者对于使用 Zig 创建 DAW 和构建可转译到 Zig 的内存安全语言表示兴奋。有人提出了关于增量链接是否与发布版本的链接时优化冲突的技术问题，并得到了澄清。

**标签**: `#zig`, `#compilers`, `#linker`, `#systems-programming`, `#open-source`

---

<a id="item-6"></a>
## [深入理解 Comanche 体素空间地形渲染技术](https://s-macke.github.io/VoxelSpace/) ⭐️ 7.0/10

这展示了 1992 年的一项开创性地形渲染技术，在当时有限的硬件上实现了逼真的飞行模拟，影响了数十年的游戏图形开发，至今仍具有学习历史渲染方法的价值。 这展示了 1992 年的一项开创性地形渲染技术，在当时有限的硬件上实现了逼真的飞行模拟，影响了数十年的游戏图形开发，至今仍具有学习历史渲染方法的价值。 该算法使用高度图方法，其中每个列表示网格位置的地形高度，渲染通过从相机向屏幕列发射射线并通过垂直线绘制计算可见性来执行。社区成员指出，该技术在严格意义上是高度图而非真正的体素，因为每个棱柱具有固定大小的正方形底面，而不是在三个轴上均匀分割空间。

hackernews · davikr · May 30, 14:25

**背景**: 《Comanche：Maximum Overkill》由 NovaLogic 开发并于 1992 年发布，其革命性的地形图形引擎采用 386/486 汇编编程驱动。体素空间算法通过透视投影将高度数据投射到二维屏幕上，并根据距离进行细节缩放。该技术可能在某些国家仍受专利保护，代码采用 MIT 许可证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/s-macke/VoxelSpace">GitHub - s-macke/VoxelSpace: Terrain rendering algorithm in less than 20 lines of code · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Comanche:_Maximum_Overkill">Comanche: Maximum Overkill - Wikipedia</a></li>
<li><a href="https://s-macke.github.io/VoxelSpace/">Voxel Space | VoxelSpace</a></li>

</ul>
</details>

**社区讨论**: 社区成员提供了宝贵的技术说明和实现方案：有人指出这实际上是基于高度图而非真正的体素技术；有人分享了移植到 AGS 引擎的经验，需要各种技巧来优化性能；还有人提供了使用原始地图数据的 C++版本；有人回忆起曾在 Visual Basic 中尝试复现但收效甚微。整体对这项经典技术充满怀念与认可。

**标签**: `#graphics-programming`, `#voxel-rendering`, `#retro-gaming`, `#comanche`, `#game-development`

---

<a id="item-7"></a>
## [OpenBSD 团队发布 Openrsync 实现](https://github.com/kristapsdz/openrsync) ⭐️ 7.0/10

rsync 是一种广泛使用的文件同步工具，用于在系统之间高效传输和同步文件。OpenBSD 的 pledge(2)系统调用将程序可以进行的系统调用限制为一组定义的"承诺"，而 unveil(2)则将文件系统可见性限制到特定路径。它们共同构成了 OpenBSD 的纵深防御方法，以保护处理不可信网络输入的应用程序。

hackernews · sph · May 30, 10:51

**背景**: rsync is a widely-used file synchronization utility for efficiently transferring and synchronizing files between systems. OpenBSD's pledge(2) system call restricts the system calls a program can make to a defined set of "promises," while unveil(2) restricts filesystem visibility to specific paths. Together, they form OpenBSD's defense-in-depth approach to securing applications that handle untrusted network input.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://man.openbsd.org/pledge.2">pledge(2) - OpenBSD manual pages</a></li>
<li><a href="https://man.openbsd.org/unveil.2">unveil(2) - OpenBSD manual pages</a></li>

</ul>
</details>

**社区讨论**: 用户报告称 openrsync 随时间推移有所改进，但在某些场景下（如远程传输期间的目录处理）仍与 Samba rsync 存在差距。讨论还提到了来自 gokrazy 团队的 Go 实现替代方案，以及关于 pledge 功能是否可以移植到 Linux 的问题。部分用户注意到，考虑到主 rsync 代码库最近的质量问题，这个发布的时机尤为重要。

**标签**: `#openrsync`, `#openbsd`, `#rsync`, `#synchronization-tools`, `#security`

---

<a id="item-8"></a>
## [Anthropic 发布跨产品 Claude 沙盒技术文档](https://simonwillison.net/2026/May/30/how-we-contain-claude/#atom-everything) ⭐️ 7.0/10

Anthropic 发布了全面的工程技术文档，详细说明了他们如何在不同产品线（Claude.ai、Claude Code 和 Claude Cowork）中对 Claude 进行沙盒化，包括使用进程隔离、虚拟机、文件系统边界和出口控制措施。 这份文档解决了关键的 AI 安全问题——防止凭证泄露——通过在 AI 代理可以访问的内容上设置硬边界。像 Anthropic 这样的大型 AI 公司如此详细地公开其安全架构，这种罕见的透明度为整个行业树立了新的标准。 Claude.ai 使用 gVisor（Google 的容器沙盒），Claude Code 在 macOS 上使用 Seatbelt，在 Linux 上使用 Bubblewrap，而 Claude Cowork 则使用完整的虚拟机（在 macOS 上使用 Apple 的虚拟化框架，在 Windows 上使用 HCS）。该文档还揭示了此前遗漏的风险，如 api.anthropic.com/v1/files 的上传漏洞向量。

rss · Simon Willison · May 30, 21:36

**背景**: 沙盒是一种关键的安全技术，用于隔离应用程序，防止恶意代码或被攻破的 AI 系统访问敏感资源。gVisor 是 Google 的容器沙盒，在用户空间中实现了约 200 个 Linux 系统调用。Seatbelt 是 macOS 的原生强制访问控制框架，被 App Store 应用和 Safari 使用。Bubblewrap 是一个无特权的 Linux 命名空间沙盒工具，被 Flatpak 等项目使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GVisor">gVisor - Wikipedia</a></li>
<li><a href="https://wiki.archlinux.org/title/Bubblewrap">Bubblewrap - ArchWiki</a></li>
<li><a href="https://hacktricks.wiki/en/macos-hardening/macos-security-and-privilege-escalation/macos-security-protections/macos-sandbox/index.html">macOS Sandbox - HackTricks</a></li>

</ul>
</details>

**社区讨论**: Simon Willison 称赞这份文档非常详尽且在 AI 安全领域实属罕见，他指出详细的安全文档并不常见。他提到现在是时候重新审视 Anthropic 的开源 srt（沙盒运行时）工具了，该工具已经成熟到可以投入生产使用。

**标签**: `#AI_safety`, `#sandboxing`, `#Anthropic`, `#Claude`, `#security`

---

<a id="item-9"></a>
## [通过 Pyodide + Service Worker 在浏览器中运行 Python ASGI 应用](https://simonwillison.net/2026/May/30/pyodide-asgi-browser/#atom-everything) ⭐️ 7.0/10

这一突破使得基于浏览器的 Python 应用程序能够完整执行 JavaScript，这意味着依赖客户端 JavaScript 的 Datasette 插件和功能现在可以在 Datasette Lite 中正常运作，大大扩展了其功能和兼容性。

rss · Simon Willison · May 30, 21:02

**背景**: Pyodide 是专门为浏览器设计的 Python 发行版，通过 WebAssembly 运行 Python 代码，实现完全无需服务器的客户端 Python 执行。ASGI（异步服务器网关接口）是定义 Python Web 服务器如何与异步应用程序通信的规范。Service Worker 是在 Web 浏览器后台运行的脚本，可以拦截网络请求并实现离线支持和高效缓存等功能。Datasette Lite 是基于浏览器的 Datasette 版本，完全使用 Pyodide 运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/pyodide/pyodide">pyodide / pyodide : Pyodide is a Python distribution for the browser ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Asynchronous_Server_Gateway_Interface">Asynchronous Server Gateway Interface - Wikipedia</a></li>
<li><a href="https://pyodide.com/">Home - Pyodide</a></li>

</ul>
</details>

**标签**: `#Pyodide`, `#WebAssembly`, `#Python-in-browser`, `#Service Workers`, `#ASGI`

---

<a id="item-10"></a>
## [外卖大战后遗症：行业仅需 400 万骑手，实际涌进 2000 万人](https://m.sohu.com/a/1029514455_122135404) ⭐️ 7.0/10

中国外卖市场由美团、京东（京东秒送）和淘宝闪购（阿里即时零售）三大平台主导。2025 年，这些公司合计投入千亿补贴进行市场份额争夺，导致大规模骑手招募，最终造成当前的运力过剩局面。

telegram · zaihuapd · May 30, 09:52

**背景**: China's food delivery market is dominated by three major platforms: Meituan, JD (JD.com's flash delivery service), and Taoxian (Alibaba's instant retail). The 2025 subsidy war saw these companies collectively invest over 100 billion yuan in rider incentives and customer discounts to capture market share, leading to massive recruitment drives that resulted in the current oversupply situation.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.163.com/dy/article/KU6JGDUE0556N7I6.html">外卖大战退潮后，2000万骑手挤在路上，1600万是“冗余运力”</a></li>
<li><a href="https://news.qq.com/rain/a/20260530V0A1PR00">外卖骑手“过剩”了？补贴退潮后，全平台日单仅1点1亿单，仅需 400 万骑...</a></li>
<li><a href="https://news.sina.cn/gn/2026-05-30/detail-inhzswyi6709564.d.html?vt=4">外卖大战后1600万骑手过剩：行业仅需400万骑手，实际涌进2000万人，超...</a></li>

</ul>
</details>

**社区讨论**: Commenters expressed sympathy for the affected riders while criticizing the platform companies for creating this situation through reckless expansion. Some noted that these 16 million redundant workers represent real families whose livelihoods were disrupted by corporate competition.

**标签**: `#gig-economy`, `#platform-labor`, `#china-tech`, `#meituan`, `#instant-commerce`

---