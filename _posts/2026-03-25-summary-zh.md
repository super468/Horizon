---
layout: default
title: "Horizon Summary: 2026-03-25 (ZH)"
date: 2026-03-25
lang: zh
---

> From 201 items, 38 important content pieces were selected

---

1. [供应链攻击：PyPI 上被植入恶意代码的 litellm 包](#item-1) ⭐️ 10.0/10
2. [2016 年 Ripgrep 基准测试显示超越 grep 及其他工具的卓越速度](#item-2) ⭐️ 9.0/10
3. [恶意 LiteLLM 包通过.pth 文件窃取凭据](#item-3) ⭐️ 9.0/10
4. [Pydantic AI v1.71.0 发布：新增 Capabilities、AgentSpec、Hooks](#item-4) ⭐️ 8.0/10
5. [Video.js v10 测试版：原始作者重写后体积缩小 88%](#item-5) ⭐️ 8.0/10
6. [Wine 11 重写内核同步层，Linux 运行 Windows 游戏性能大幅提升](#item-6) ⭐️ 8.0/10
7. [Hegel：新属性测试工具发布](#item-7) ⭐️ 8.0/10
8. [Show HN：Gemini Embedding 2 实现亚秒级视频搜索](#item-8) ⭐️ 8.0/10
9. [Epoch confirms GPT5.4 Pro solved a frontier math open problem](#item-9) ⭐️ 8.0/10
10. [EVA：ServiceNow 推出的语音智能体开源评估框架](#item-10) ⭐️ 8.0/10
11. [Claude Code 推出 AI 驱动的自动模式](#item-11) ⭐️ 8.0/10
12. [TurboQuant：用极端压缩重新定义 AI 效率](#item-12) ⭐️ 8.0/10
13. [DarkSword：自 2025 年 11 月起被利用的 Safari 零日漏洞链](#item-13) ⭐️ 8.0/10
14. [知名政治评论人张雪峰去世 年仅 39 岁](#item-14) ⭐️ 8.0/10
15. [OpenAI 关闭 Sora 视频生成应用](#item-15) ⭐️ 7.0/10
16. [苹果推出 Apple Business 平台 却遭社区批评现有工具问题多多](#item-16) ⭐️ 7.0/10
17. [导弹防御优化被证明为 NP 完全问题](#item-17) ⭐️ 7.0/10
18. [OpenAI 发布面向 AI 开发者的青少年安全政策](#item-18) ⭐️ 7.0/10
19. [ChatGPT 推出基于代理商务协议的新购物功能](#item-19) ⭐️ 7.0/10
20. [NVIDIA 向 Kubernetes 社区捐赠 GPU 驱动实现动态资源分配](#item-20) ⭐️ 7.0/10
21. [构建 NVIDIA Nemotron 3 智能体：推理、多模态 RAG、语音与安全](#item-21) ⭐️ 7.0/10
22. [Arm 发布 35 年来首款自研芯片](#item-22) ⭐️ 7.0/10
23. [Anthropic 的 Claude Code 和 Cowork 获得电脑控制功能](#item-23) ⭐️ 7.0/10
24. [TinyLoRA：13 参数微调方法在 Qwen2.5-7B 上实现 91.8% GSM8K 准确率](#item-24) ⭐️ 7.0/10
25. [LeWorldModel (LeWM)：端到端解决表示崩溃的 JEPA 架构](#item-25) ⭐️ 7.0/10
26. [Meta AI Hyperagents 实现实用化递归自我改进](#item-26) ⭐️ 7.0/10
27. [法官质疑五角大楼对 Anthropic 的供应链风险认定](#item-27) ⭐️ 7.0/10
28. [主流包管理器纷纷实现依赖冷却期安全功能](#item-28) ⭐️ 7.0/10
29. [流式专家技术使大型 MoE 模型可在有限 RAM 上运行](#item-29) ⭐️ 7.0/10
30. [Dreamer 在播客亮相后加入 Meta 超级智能实验室](#item-30) ⭐️ 7.0/10
31. [Plasmite：使用内存映射文件作为环形缓冲区的 Rust 轻量级 IPC 系统](#item-31) ⭐️ 7.0/10
32. [Lexplain：Linux 内核变更解释 AI 工具](#item-32) ⭐️ 7.0/10
33. [从写文案到盯数据、算 ROI，流量见顶后，AI Agent 正在杀进核心业务](#item-33) ⭐️ 7.0/10
34. [深度研究智能体工程化实践：从原型到生产级服务的关键挑战与解法](#item-34) ⭐️ 7.0/10
35. [阿里达摩院发布玄铁 C950 刷新 RISC-V 性能纪录](#item-35) ⭐️ 7.0/10
36. [欧盟年龄验证 App 排除非谷歌授权安卓系统](#item-36) ⭐️ 7.0/10
37. [微软发布 7 本综合 Rust 培训教材](#item-37) ⭐️ 7.0/10
38. [OpenAI 推出 Sora AI 视频生成器仅六个月后停止运营](#item-38) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [供应链攻击：PyPI 上被植入恶意代码的 litellm 包](https://github.com/BerriAI/litellm/issues/24512) ⭐️ 10.0/10

这是一个严重供应链攻击，影响了广泛使用的 LLM 网关库。攻击源自 CI/CD 管道中的 Trivy 扫描器漏洞，表明即使安全工具也可能成为攻击媒介。超过 468 个赞同和 368 条评论表明此事件对社区影响重大。 恶意包现已在 PyPI 上被隔离，阻止所有下载。Docker proxy 用户未受影响，因为项目在 requirements.txt 中固定了版本。根本原因已追溯到 Trivy CI/CD 被入侵（TeamPCP 活动），即安全扫描器本身在构建过程中被植入恶意代码。

hackernews · dot_treo · Mar 24, 12:06

**背景**: Litellm 是一个流行的 Python SDK 和代理服务器（AI 网关），为多个 LLM 提供商提供 OpenAI 兼容接口。Trivy 是 Aqua Security 开发的综合安全扫描器，用于在 CI/CD 管道中查找漏洞。最近的安全事件表明，Trivy 本身也可能被入侵以窃取 CI/CD 密钥，使其成为供应链攻击的潜在攻击向量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/BerriAI/litellm">GitHub - BerriAI/ litellm : Python SDK, Proxy Server (AI Gateway) to...</a></li>
<li><a href="https://accuknox.com/blog/trivy-supply-chain-attack">Trivy Security Scanner Just Became A Supply Chain Weapon</a></li>

</ul>
</details>

**社区讨论**: LiteLLM 维护者确认了攻击源自 Trivy，并表示 Docker 用户未受影响。社区成员讨论了加强沙箱化、深度防御和改进开发者隔离的必要性。有人分享了一个 macOS 金丝雀工具来检测可疑包对伪造密钥的访问。部分用户注意到该问题已被垃圾评论淹没。

**标签**: `#security`, `#supply-chain-attack`, `#python`, `#pypi`, `#vulnerability`, `#devsecops`

---

<a id="item-2"></a>
## [2016 年 Ripgrep 基准测试显示超越 grep 及其他工具的卓越速度](https://burntsushi.net/ripgrep/) ⭐️ 9.0/10

2016 年，Andrew Gallant 发布了全面的基准测试比较，显示 ripgrep 通过 SIMD 向量化和各种优化技术显著超越 grep、ag、git grep、ucg、pt 和 sift。 Ripgrep 使用 SIMD 向量化进行并行文本处理，实现"先查找最少见的字节"策略以加快匹配速度，默认尊重 gitignore 规则，并自动跳过隐藏文件/目录和二进制文件。

hackernews · jxmorris12 · Mar 24, 06:31

**背景**: ripgrep（rg）是由 Andrew Gallant 用 Rust 编写的逐行搜索工具，旨在成为 grep 的更快替代品，同时提供类似 ack 的智能默认值。2016 年的基准测试比较了七种不同的搜索工具，并解释了 ripgrep 性能优势的技术原因，包括 SIMD 向量化和字节级优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://burntsushi.net/ripgrep/">ripgrep is faster than {grep, ag, git grep, ucg, pt, sift} - Andrew Gallant's Blog</a></li>
<li><a href="https://github.com/BurntSushi/ripgrep">GitHub - BurntSushi/ripgrep: ripgrep recursively searches directories for a regex pattern while respecting your gitignore · GitHub</a></li>
<li><a href="https://stackoverflow.com/questions/1422149/what-is-vectorization">simd - What is " vectorization "? - Stack Overflow</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞这篇文章既是教程又是专家深度解读，并指出他们多年后仍在参考。一位开发者提到使用"最少见的字节"技术将自有搜索工具的运行时间缩短了三分之一。讨论还提到了尽管最初对与 grep 的兼容性存在怀疑，但 ripgrep 却被戏剧性地广泛采用。

**标签**: `#ripgrep`, `#grep`, `#performance`, `#systems-programming`, `#text-search`

---

<a id="item-3"></a>
## [恶意 LiteLLM 包通过.pth 文件窃取凭据](https://simonwillison.net/2026/Mar/24/malicious-litellm/#atom-everything) ⭐️ 9.0/10

这是一个影响使用 LiteLLM 的开发者的严重供应链攻击。.pth 文件技术意味着凭据窃取程序在安装时立即运行，使其比典型的恶意包（仅在导入时执行）更加危险。 恶意软件针对超过 30 个凭据来源，包括~/.ssh/、~/.gitconfig、~/.aws/、~/.kube/、~/.azure/、~/.docker/、~/.npmrc、~/.vault-token 以及各种加密货币钱包。1.82.7 版本中的漏洞位于 proxy/proxy_server.py 中需要导入触发，而 1.82.8 版本将其移至 litellm_init.pth 实现自动执行。

rss · Simon Willison · Mar 24, 15:07

**背景**: .pth 文件是 Python 路径配置文件，site 模块在 Python 启动时自动处理它们。与需要导入语句才能执行的常规 Python 代码不同，.pth 文件只需存在于 site-packages 中即可运行任意代码。这使它们成为供应链攻击的有力载体。该攻击可能始于最近对 Trivy（LiteLLM 在其 CI 管道中使用的安全扫描器）的入侵，导致 PyPI 发布凭据被窃取。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.python.org/3/library/site.html">site — Site-specific configuration hook</a></li>
<li><a href="https://blog.pypi.org/posts/2024-11-25-aiocpa-attack-analysis/">Malware Package Analysis: aiocpa - The Python Package Index Blog</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#python`, `#supply-chain-attack`, `#litellm`

---

<a id="item-4"></a>
## [Pydantic AI v1.71.0 发布：新增 Capabilities、AgentSpec、Hooks](https://github.com/pydantic/pydantic-ai/releases/tag/v1.71.0) ⭐️ 8.0/10

这些功能对这个广受欢迎的 Python AI 框架来说是非常重要的架构改进，使开发者能够为生产级应用创建更加模块化、可复用和可配置的 AI 代理。 其他功能包括具有自动回退功能的提供商自适应工具（WebSearch、WebFetch、MCP、ImageGeneration）、用于状态隔离的 AbstractToolset.for_run，以及对新 OpenAI 模型 gpt-5.4-mini 和 gpt-5.4-nano 的支持。

github · DouweM · Mar 24, 21:50

**背景**: Pydantic AI 是一个 Python 代理框架，旨在帮助开发者快速、可靠地构建生成式 AI 的生产级应用。该框架提供结构化输出验证，并与各种 LLM 提供商集成。该框架允许代理像 FastAPI 应用一样设计为可复用的形式，既可以全局实例化，也可以动态创建。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.pydantic.dev/">Pydantic AI - Pydantic AI</a></li>
<li><a href="https://github.com/pydantic/pydantic-ai">GitHub - pydantic/pydantic- ai : GenAI Agent Framework, the Pydantic...</a></li>

</ul>
</details>

**标签**: `#pydantic`, `#python`, `#ai-agents`, `#release-notes`, `#LLM-framework`

---

<a id="item-5"></a>
## [Video.js v10 测试版：原始作者重写后体积缩小 88%](https://videojs.org/blog/videojs-v10-beta-hello-world-again) ⭐️ 8.0/10

Video.js 原始创始人 Steve Heffernan 在时隔 16 年后重新接管了该项目，并与 Plyr、Vidstack 和 Media Chrome 的开发团队合作发布了 v10 测试版，新版本体积比之前缩小了 88%。 Video.js 每月被数十亿用户使用，涵盖 Amazon.com、LinkedIn、Dropbox 等知名网站。此次竞争对手项目之间的跨界合作标志着视频播放器生态系统的重要整合，对开源社区和 Web 开发领域都具有深远意义。 v10 测试版采用了现代化架构重建，由来自竞争项目的开发者协作完成。该版本在保持核心功能的同时大幅精简了代码体积，目前处于测试阶段，欢迎用户反馈问题。

hackernews · Heff · Mar 24, 18:03

**背景**: Video.js 是一个流行的开源 HTML5 视频播放器库，最初由 Steve Heffernan 创建，后被公司收购。在私募股权收购原公司并解雇维护人员后，Heffernan 决定收回项目并重新开发。Plyr、Vidstack 和 Media Chrome 都是市场上不同的视频播放器解决方案，此次合作体现了开源社区的协作精神。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://plyr.io/">Plyr - A simple, customizable HTML5 Video , Audio, YouTube and...</a></li>
<li><a href="https://vidstack.io/">Vidstack Player</a></li>
<li><a href="https://www.media-chrome.org/">Media Chrome Docs</a></li>

</ul>
</details>

**社区讨论**: 社区反应积极，有用户询问为何不采用 Web Components 形式发布，也有用户提到视频播放器领域正在发生的变化，包括 react-player 被 Mux 接管等事件。部分老用户表示期待尝试新版本，也有开发者希望等版本稳定后再测试。

**标签**: `#open-source`, `#video-player`, `#javascript`, `#performance-optimization`, `#web-development`

---

<a id="item-6"></a>
## [Wine 11 重写内核同步层，Linux 运行 Windows 游戏性能大幅提升](https://www.xda-developers.com/wine-11-rewrites-linux-runs-windows-games-speed-gains/) ⭐️ 8.0/10

Wine 11 引入了 NTSYNC，这是一个新的内核驱动程序，直接模拟 Windows NT 同步对象，取代了之前将 Windows 同步行为硬塞入现有 Linux 原语的方法。 这次重写在基准测试中带来了巨大的 FPS 提升（例如 Dirt 3 从 110 FPS 跃升至 860 FPS），代表了 Valve 资助的多年开发工作，旨在通过 Proton 改善 Linux 游戏体验。 这些极端的基准测试提升是相对于没有 fsync 的原生 Wine 而言的——现有 Proton 用户的实际提升通常在较低的单位数百分比范围内。NTSYNC 添加了一个新的内核驱动程序，直接实现 Windows NT 同步 API。

hackernews · felineflock · Mar 24, 18:34

**背景**: Wine 是一个开源兼容层，将 Windows API 调用翻译成 POSIX 兼容的调用，使 Windows 软件可以在 Linux 上运行。Proton 是 Valve 优化过的 Wine 游戏分支。NTSYNC 功能通过在内核级别实现 Windows 同步对象，解决了现代游戏中最敏感的性能操作之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.xda-developers.com/wine-11-rewrites-linux-runs-windows-games-speed-gains/">Wine 11 rewrites how Linux runs Windows games at the kernel level, and the speed gains are massive</a></li>
<li><a href="https://en.wikipedia.org/wiki/Proton_(software)">Proton (software) - Wikipedia</a></li>
<li><a href="https://tech.slashdot.org/story/26/03/24/1946246/wine-11-rewrites-how-linux-runs-windows-games-at-the-kernel-level">Wine 11 Rewrites How Linux Runs Windows Games At the Kernel Level - Slashdot</a></li>

</ul>
</details>

**社区讨论**: 评论者对基准测试的提升感到惊叹，并感谢 Valve 资助这项工作，同时也降低了期望——一位用户指出这些极端提升是相对于没有 fsync 的原生 Wine 相比，而非实际 Proton 使用情况。其他人反思使 Wine 成为可能的默默无闻且复杂的底层工作。

**标签**: `#wine`, `#linux`, `#gaming`, `#proton`, `#open-source`

---

<a id="item-7"></a>
## [Hegel：新属性测试工具发布](https://antithesis.com/blog/2026/hegel/) ⭐️ 8.0/10

Hegel 库的创始人 David MacIver 发布了 Hegel，这是一款具有先进基于位流收缩功能的新型属性测试工具。该工具支持通过 libFuzzer 集成进行覆盖率驱动的测试，并旨在改进现有的 PBT 框架。 此公告意义重大，因为 David MacIver 是测试社区中备受推崇的人物，Hegel 代表了属性测试领域的重大技术进步。基于位流的收缩方法可以更有效地简化失败的测试用例，这对调试至关重要。 Hegel 使用基于位流的收缩方法，这与传统的收缩方法不同。它与 Rust 中的 libFuzzer 和 Arbitrary crate 集成，用于覆盖率驱动的测试。该工具旨在解决 prop_flat_map 的痛点，并可能成为某些基于 proptest 的测试的替代品。

hackernews · alpaylan · Mar 24, 15:28

**背景**: 属性测试(PBT)是一种测试方法，通过生成随机输入来验证应该对所有有效输入都成立的理论。收缩是一个关键功能，可以将复杂的失败测试用例简化为更简单、更易理解的例子。Hegel 基于 MacIver 在 Hegel 方面的经验，提供了一个具有先进收缩功能的 Rust 实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.agilogy.com/2022-08-26-pbt-shrinking-part1.html">Property based testing: Shrinking (part 1) - Agilogy</a></li>
<li><a href="https://hackernoon.com/shrinking-for-easier-debugging-property-based-testing-part-3">Shrinking for Easier Debugging - Property-Based Testing (Part 3) Property-based Testing #5: Shrinking Choices, Shrinking Values GitHub - jlink/shrinking-challenge: Comparing shrinking ... Property-Based Testing: Finding Bugs You Never Thought to ... The Magic of Internal Shrinking for Property Based Testing Understanding Shrinking in Property-Based Testing with PropEr</a></li>

</ul>
</details>

**社区讨论**: 社区反应积极且技术性很强。sunshowers 表达了对基于位流收缩功能的兴趣，并询问了类似于 proptest Arbitrary trait 的规范生成器。ruuda 强调指出，使用 libFuzzer 进行覆盖率驱动的测试是一个游戏规则改变者，可以探索随机输入永远不会触发的代码路径。讨论还涉及了 PBT 在 AI 代理开发中的作用。

**标签**: `#property-based-testing`, `#hegel`, `#rust`, `#software-testing`, `#hypothesis`

---

<a id="item-8"></a>
## [Show HN：Gemini Embedding 2 实现亚秒级视频搜索](https://github.com/ssrajadh/sentrysearch) ⭐️ 8.0/10

一位开发者利用 Gemini Embedding 2 的原生视频嵌入功能构建了一个 CLI 工具，将数小时的视频片段索引到 ChromaDB 中，实现了亚秒级的自然语言视频搜索，无需转录或帧标注。 这是 Gemini Embedding 2 原生多模态嵌入功能的首次实际应用，使得文本查询与原始视频之间可以直接进行向量比较。这为使用自然语言搜索行车记录仪 footage、安保摄像头和视频档案开辟了新的可能性。 Gemini Embedding 2 将原始视频直接投影到与文本相同的 768 维向量空间中。索引成本约为每小时的视频 footage 约 2.50 美元。该工具包含静止帧检测功能，可以跳过空闲片段，使安保摄像头和哨兵模式 footage 的成本大大降低。

hackernews · sohamrj · Mar 24, 14:58

**背景**: Gemini Embedding 2 是 Google 于 2026 年 3 月发布的首个原生多模态嵌入模型，可以将文本、图像、视频、音频和文档映射到统一的嵌入空间中。ChromaDB 是专为 LLM 应用设计的开源向量数据库，优化用于存储和搜索高维嵌入向量。向量数据库通过比较嵌入向量而不是精确关键词匹配来实现语义相似性搜索。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-embedding-2/">Gemini Embedding 2: Our first natively multimodal embedding model</a></li>
<li><a href="https://news.ycombinator.com/item?id=47503617">Show HN: Gemini can now natively embed video, so I built sub-second ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Chroma_(vector_database)">Chroma ( vector database ) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 讨论中突出了现代社会普遍存在的摄像头带来的重大隐私问题，一位评论者指出这个用例是他们对 AI 发展轨迹最担忧的地方。其他人对行车记录仪搜索、家庭监控和视频编辑插件等实际应用表达了热情，这些插件可以从自然语言描述自动生成剪辑决策列表。

**标签**: `#video-search`, `#embeddings`, `#gemini`, `#chromadb`, `#computer-vision`, `#ai-tools`

---

<a id="item-9"></a>
## [Epoch confirms GPT5.4 Pro solved a frontier math open problem](https://epoch.ai/frontiermath/open-problems/ramsey-hypergraphs) ⭐️ 8.0/10

Epoch.ai confirms GPT-5.4 Pro solved an open problem in Ramsey hypergraph theory, marking a potential first for AI on frontier mathematics.

hackernews · in-silico · Mar 24, 01:53

**标签**: `#AI`, `#Mathematics`, `#FrontierMath`, `#LLM`, `#Breakthrough`

---

<a id="item-10"></a>
## [EVA：ServiceNow 推出的语音智能体开源评估框架](https://huggingface.co/blog/ServiceNow-AI/eva) ⭐️ 8.0/10

该框架解决了语音 AI 领域的一个关键空白，因为现有基准通常只评估智能体做了什么（任务完成）或听起来如何（语音质量），而不是两者兼顾。EVA 提供了一种全面的方法，有望在整个行业中实现语音智能体评估的标准化。 EVA 评估完整的多轮语音对话，而非孤立的组件。准确性维度评估智能体是否正确且忠实地完成了任务，而体验性维度则从用户视角评估交互质量。

rss · Hugging Face Blog · Mar 24, 02:01

**背景**: 语音智能体是设计用于与用户进行语音对话的 AI 系统，通常用于客服、虚拟助手和其他交互应用。此前，语音智能体评估依赖于专注于输出正确性或语音合成质量的基准测试，缺少评估真实世界对话功能和体验方面的综合框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/ServiceNow-AI/eva">A New Framework for Evaluation of Voice Agents (EVA)</a></li>
<li><a href="https://github.com/ServiceNow/eva">GitHub - ServiceNow/eva: A New End-to-end Framework for ...</a></li>

</ul>
</details>

**标签**: `#voice-agents`, `#evaluation-framework`, `#AI-benchmarks`, `#LLM-evaluation`, `#Hugging-Face`

---

<a id="item-11"></a>
## [Claude Code 推出 AI 驱动的自动模式](https://simonwillison.net/2026/Mar/24/auto-mode-for-claude-code/#atom-everything) ⭐️ 8.0/10

Anthropic 在 Claude Code 中推出了“自动模式”，这是一种新的权限模式，Claude 使用基于 Claude Sonnet 4.6 分类器实现的防护机制，在操作运行前进行审查，从而代表用户做出权限决策。 这解决了开发者面临的关键痛点：在使用 AI 编程助手时平衡便利性与安全性。自动模式提供了一种比 --dangerously-skip-permissions 更安全的替代方案，同时消除了重复的权限确认提示。 分类器使用 Claude Sonnet 4.6 运行，即使主会话使用其他模型也会如此。它会阻止超出任务范围的操作、针对不可信基础设施的操作，或看起来由恶意内容驱动的操作。默认过滤器包括“本地操作”、“只读操作”、“已声明依赖”（允许类别）以及“Git 破坏性操作”、“外部代码”（软拒绝类别）。用户可以使用自己的规则进行自定义。

rss · Simon Willison · Mar 24, 23:57

**背景**: Claude Code 是 Anthropic 的 AI 编程助手，此前需要用户手动批准每个操作或使用有风险的 --dangerously-skip-permissions 标志。新的自动模式使用单独的分类器模型在执行前评估操作，将便利性与安全防护相结合。这种方法不同于简单的允许/拒绝列表，而是使用 AI 驱动的上下文感知决策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reddit.com/r/ClaudeAI/comments/1s2ok85/claude_code_now_has_auto_mode/">Claude Code now has auto mode : r/ClaudeAI - Reddit</a></li>
<li><a href="https://9to5mac.com/2026/03/24/claude-code-gives-developers-auto-mode-a-safer-alternative-to-skipping-permissions/">Claude Code gives developers 'auto mode,' a safer alternative ... - 9to5Mac</a></li>
<li><a href="https://code.claude.com/docs/en/permission-modes">Choose a permission mode - Claude Code Docs</a></li>

</ul>
</details>

**社区讨论**: Reddit 上的讨论显示积极反响，用户认为自动模式消除了批准每个文件写入和 bash 命令的繁琐，同时比完全跳过权限提供了更多安全性。涵盖常见开发场景的默认过滤器被认为设计良好。

**标签**: `#AI coding assistants`, `#Claude Code`, `#Anthropic`, `#Developer tools`, `#AI safety`

---

<a id="item-12"></a>
## [TurboQuant：用极端压缩重新定义 AI 效率](https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/) ⭐️ 8.0/10

这一突破使得 AI 模型能够在资源受限的设备上更高效地运行，通过大幅减小模型体积和内存需求同时保持精度，对于在生产环境中部署大型语言模型至关重要。 TurboQuant 实现了模型大小的高 Reduction 率，同时保持零精度损失，特别适用于支持 Transformer 中的键值(KV)缓存和向量搜索引擎操作。

rss · Lobsters - AI · Mar 24, 20:14

**背景**: 量化是一种基本的模型压缩技术，通过降低 AI 模型中数字的精度（例如从 32 位浮点数压缩到 4 位整数）来使模型更小、更快、更便宜。向量搜索引擎依赖高维向量来表示和处理信息，对这些向量进行压缩对于可扩展性和效率至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/">TurboQuant: Redefining AI efficiency with extreme compression</a></li>
<li><a href="https://ainewsfuse.com/ai-news-fuse/turboquant-unveils-a-new-era-of-ai-compression-slashing-memory-footprint-while-boosting-speed/">TurboQuant Unveils a New Era of AI Compression, Slashing Memory...</a></li>

</ul>
</details>

**标签**: `#ai-efficiency`, `#model-compression`, `#quantization`, `#google-research`, `#machine-learning`

---

<a id="item-13"></a>
## [DarkSword：自 2025 年 11 月起被利用的 Safari 零日漏洞链](https://t.me/zaihuapd/40482) ⭐️ 8.0/10

这是一个关键的 iOS 安全漏洞，因为攻击者只需用户访问网页即可控制设备。该漏洞链已在针对沙特、土耳其、马来西亚和乌克兰用户的真实攻击中被使用，包括政府网站。GHOSTBLADE 载荷专门针对加密货币钱包。 该六漏洞链包括 CVE-2025-43529（在 iOS 18.7.3 和 26.2 中修补），所有漏洞现已在 iOS 26.3 中修复。该漏洞利用基于 JavaScript，可根据攻击者目标静默部署各种后期恶意软件家族。GHOSTBLADE 专门扫描 Coinbase、Binance、Kraken、Kucoin、OKX 和 MEXC 应用。

telegram · zaihuapd · Mar 24, 11:45

**背景**: DarkSword 代表了一个复杂的漏洞利用链，可与此前发现的 Coruna 等 iOS 漏洞工具包相提并论。这些漏洞可能被多个威胁组织同时发现，虽然 Apple 已在 iOS 26.3 中修补了这些漏洞，但运行 iOS 18.4-18.7 的设备如果不更新仍然存在漏洞。针对加密货币应用的攻击表明有经济动机的威胁组织正在采用这种工具包。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.google.com/blog/topics/threat-intelligence/darksword-ios-exploit-chain">The Proliferation of DarkSword: iOS Exploit Chain Adopted by ...</a></li>
<li><a href="https://tidbits.com/2026/03/23/darksword-exploit-threatens-iphones-still-running-ios-18/">DarkSword Exploit Threatens iPhones Still Running iOS 18</a></li>
<li><a href="https://www.malwarebytes.com/blog/mobile/2026/03/a-darksword-hangs-over-unpatched-iphones">A DarkSword hangs over unpatched iPhones | Malwarebytes</a></li>

</ul>
</details>

**社区讨论**: 安全研究人员强调，用户应立即更新到 iOS 26.3 以缓解此威胁。乌克兰政府网站被入侵的事实突显了该漏洞链的高价值目标能力。讨论还指出，有三个不同的恶意软件家族被部署，表明该漏洞已被多个威胁组织共享或出售。

**标签**: `#iOS security`, `#vulnerability research`, `#threat intelligence`, `#Safari`, `#zero-day`

---

<a id="item-14"></a>
## [知名政治评论人张雪峰去世 年仅 39 岁](https://weibo.com/1676679984/QxC4FDcyq) ⭐️ 8.0/10

讣告发出后，张雪峰在 B 站、小红书、微信公众号等多个平台的账号头像均变为灰色，这是中国社交媒体的纪念功能。。此前网络上曾流传关于他去世的传闻，但未获官方确认。 张雪峰仅在抖音平台就有 2600 万粉丝，是中国社交媒体领域最具影响力的政治评论人之一。他年仅 39 岁的突然离世引发了广泛哀悼，并让人们开始讨论「流量至上」时代内容创作者所面临的健康压力。

telegram · zaihuapd · Mar 24, 13:51

**背景**: 在中国社交媒体文化中，「变灰」是平台提供的纪念功能，用户去世后头像会自动添加灰色滤镜，作为数字悼念的方式。张雪峰以政治分析视频闻名，在各大平台积累了数千万粉丝，已成为国内网络政治评论领域的重要人物。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.163.com/dy/article/KOR04P1S0528DORE.html">讣告发出后，张雪峰的账号头像都灰了：互联网从此少了一张“敢说的嘴”|...</a></li>
<li><a href="https://www.sohu.com/a/1000671306_122396430">张雪峰多个社交平台头像变灰，一场关于健康、舆论与流量多重博弈_账号...</a></li>
<li><a href="https://news.qq.com/rain/a/20260324A06UIQ00">张雪峰多个社交平台头像变灰_腾讯新闻</a></li>

</ul>
</details>

**社区讨论**: 网友讨论情绪复杂，一方面哀悼这位「敢说的嘴」的离去，另一方面也反思中国社交媒体竞争激烈的环境下网红经济给内容创作者带来的健康压力。许多人对流量时代专业性与伦理底线的缺失表示担忧。

**标签**: `#obituary`, `#chinese-commentator`, `#sudden-death`, `#social-media`, `#china`

---

<a id="item-15"></a>
## [OpenAI 关闭 Sora 视频生成应用](https://twitter.com/soraofficialapp/status/2036532795984715896) ⭐️ 7.0/10

这一关闭标志着 AI 视频生成领域面临重大挑战，并引发了对 OpenAI 产品策略的质疑，尤其是在这个快速发展的市场中竞争对手持续推进的背景下。 该应用 于 2024 年 12 月推出，2025 年关闭。用户报告称初期兴奋后新鲜感迅速消退，商业模式的根本问题在于无法获取广告收入，因为用户通常将视频导出到其他社交平台而非留在应用内生态系统中。

hackernews · mikeocool · Mar 24, 20:01

**背景**: Sora 作为 OpenAI 对 AI 视频生成的答案推出，定位为从文本提示创建视频的工具。然而，该应用面临经典的「另一个产品的子集」问题——用户会在 Sora 中生成视频，但随后在 TikTok 和 YouTube 等成熟平台上分享，导致 OpenAI 无法获得广告收入。快速关闭也与 OpenAI 同时发布 Sora 安全指南形成对比，暴露出内部协调问题。

**社区讨论**: 评论显示出复杂情绪——一些用户对 Sora 最初带来的创作乐趣流露出真挚怀念，而批评者则指出其商业模式存在缺陷，产品作为更大平台的子集而存在。其他人质疑关闭时机与安全指南发布相吻合，一位评论者称这「不是个好兆头」。还有人将此与 OpenAI 在开发者心智份额上对抗 Anthropic 的更广泛竞争挑战联系起来。

**标签**: `#openai`, `#ai-video`, `#sora`, `#product-shutdown`, `#generative-ai`

---

<a id="item-16"></a>
## [苹果推出 Apple Business 平台 却遭社区批评现有工具问题多多](https://www.apple.com/newsroom/2026/03/introducing-apple-business-a-new-all-in-one-platform-for-businesses-of-all-sizes/) ⭐️ 7.0/10

苹果发布了 Apple Business，这是一个整合设备管理、生产力工具和客户拓展功能的一体化新平台，Apple Business Essentials 现免费提供。然而，社区评论显示现有的 Apple Business Manager 被描述为"漏洞百出"和"充满陷阱"。 这对于评估苹果企业生态系统的 IT 专业人员和 businesses 来说很重要。苹果精心准备的发布会与 IT 管理员糟糕的实际体验之间的差距表明，该平台可能无法解决企业管理的根本问题。 Apple Business Manager 的域名锁定/捕获流程要求用户迁移账户并删除个人数据，用户报告称此过程存在死胡同和复杂的迁移步骤。据报道，更改企业名称需要"危险的迁移步骤"，支持代表缺乏解决严重问题的工具。

hackernews · soheilpro · Mar 24, 15:29

**背景**: Apple Business Manager 是一个基于 Web 的门户，供 IT 管理员在组织中部署和管理 Apple 设备。Apple Business Essentials 之前为小型企业提供设备管理、云存储和支持。新的 Apple Business 平台整合了这些工具并使 Essentials 免费，将苹果更直接地定位为 Microsoft 365 和 Jamf 等企业 MDM 解决方案的竞争对手。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2026/03/introducing-apple-business-a-new-all-in-one-platform-for-businesses-of-all-sizes/">Introducing Apple Business — a new all-in-one platform for ...</a></li>
<li><a href="https://9to5mac.com/2026/03/24/apple-business-essentials-goes-free-as-apple-merges-enterprise-tools-into-apple-business/">Apple Business Essentials goes free as Apple merges ...</a></li>
<li><a href="https://support.apple.com/guide/apple-business-manager/intro-to-apple-business-manager-axm7909096bf/web">Intro to Apple Business Manager</a></li>

</ul>
</details>

**社区讨论**: 讨论显示强烈的批评：用户将域名锁定/捕获流程描述为"从苹果体验过的最糟糕的经历"和"充满陷阱"。一些人认为该平台对 50 人以下的小型企业积极，而另一些人质疑苹果是否有能力与 Microsoft 365 竞争。鉴于苹果扩展的 MDM 能力，Jamf 投资者表示担忧。

**标签**: `#apple`, `#enterprise-software`, `#business-tools`, `#product-launch`, `#it-management`

---

<a id="item-17"></a>
## [导弹防御优化被证明为 NP 完全问题](https://smu160.github.io/posts/missile-defense-is-np-complete/) ⭐️ 7.0/10

一篇技术论文证明，最优导弹防御分配问题是 NP 完全问题，这意味着随着来袭威胁数量超过某个阈值，该问题在计算上变得难以处理。 该证明表明，导弹防御分配问题包含已知 NP 完全问题的数学结构，使得开发求解大规模实例的高效算法不太可能。

hackernews · O3marchnative · Mar 24, 13:00

**背景**: NP 完全是计算复杂性理论中的一个分类，指那些解可以快速验证但随着输入规模增长可能需要极长时间求解的问题。导弹防御优化涉及决定如何将有限的防御拦截器分配给多个来袭威胁，这些威胁可能包括旨在耗尽防御系统的诱饵。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/NP-completeness">NP-completeness - Wikipedia</a></li>
<li><a href="https://onlinelibrary.wiley.com/doi/10.1155/2016/5915918">Performance Analysis and Optimal Allocation of Layered ...</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了现实世界防御的对抗性和成本不对称性：攻击者可以观察并适应防御体系，每枚导弹的成本约为防御者的三分之一，且武器生产速度比拦截器制造速度更快。一位评论者指出，面对核武器威胁，防御几乎不可能；而面对常规威胁，成本比例使持续防御在经济上不可承受。

**标签**: `#computational-complexity`, `#missile-defense`, `#game-theory`, `#np-complete`, `#military-strategy`, `#optimization`

---

<a id="item-18"></a>
## [OpenAI 发布面向 AI 开发者的青少年安全政策](https://openai.com/index/teen-safety-policies-gpt-oss-safeguard) ⭐️ 7.0/10

OpenAI 发布了青少年安全政策包——基于提示词的安全策略，旨在与 gpt-oss-safeguard 配合使用，帮助开发者在 AI 应用中构建适合青少年的保护措施。 这解决了 AI 安全领域的一个关键空白，为开发者提供了保护未成年人的具体工具，随着 AI 系统对青少年越来越容易获取，这个问题日益重要。 这些策略涵盖了暴力、自残和年龄限制内容——根据青少年发展差异研究专门针对青少年面临的风险进行定制。这些策略可与 gpt-oss-safeguard-120b 和 gpt-oss-safeguard-20b 配合使用，这两款开放权重的安全推理模型于 2025 年 10 月 29 日发布。

rss · OpenAI News · Mar 24, 11:00

**背景**: gpt-oss-safeguard 是 OpenAI 的开放权重安全推理模型，专为安全分类任务设计。开发者可以将自定义安全策略作为提示词提供，模型据此对文本进行分类。青少年安全政策包是该框架发布的首个主要策略集，针对青少年与 AI 系统交互时面临的独特风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-oss-safeguard/">Introducing gpt-oss-safeguard | OpenAI</a></li>
<li><a href="https://github.com/openai/teen-safety-policy-pack">GitHub - openai/teen-safety-policy-pack</a></li>
<li><a href="https://news.bloomberglaw.com/artificial-intelligence/openai-releases-prompt-based-safety-policies-for-teens">OpenAI Releases Prompt-Based Safety Policies For Teens</a></li>

</ul>
</details>

**社区讨论**: 开发者社区对此反应积极，认为这是 AI 未成年人安全领域的务实进展。开源方法允许开发者根据特定用例自定义策略，同时为青少年用户保持基本的保护水平。

**标签**: `#AI safety`, `#AI policy`, `#teen protection`, `#developer tools`, `#OpenAI`

---

<a id="item-19"></a>
## [ChatGPT 推出基于代理商务协议的新购物功能](https://openai.com/index/powering-product-discovery-in-chatgpt) ⭐️ 7.0/10

这代表了 ChatGPT 向电子商务领域的重大扩展，可能会改变用户通过 AI 助手发现和购买产品的方式。代理商务协议为 AI 代理设定了标准化的商业交易框架。 代理商务协议是 OpenAI 和 Stripe 开发的开放标准，实现买家、AI 代理和企业之间的对话。代理可以在整个购买过程中推理结构化状态、调用工具并实时更新客户信息。

rss · OpenAI News · Mar 24, 09:00

**背景**: 代理商务协议是一个开放标准，使 AI 代理能够代表买家与企业交互。它代表了一种新的电子商务方式，AI 助手可以通过自然对话帮助用户发现产品、比较选项并完成购买。该协议协调结账流程并安全地在各方之间共享支付凭证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.openai.com/commerce">Agentic Commerce | OpenAI Developers</a></li>
<li><a href="https://www.agenticcommerce.dev/">Agentic Commerce Protocol</a></li>

</ul>
</details>

**标签**: `#AI Products`, `#E-commerce`, `#ChatGPT`, `#Protocol Development`, `#OpenAI`

---

<a id="item-20"></a>
## [NVIDIA 向 Kubernetes 社区捐赠 GPU 驱动实现动态资源分配](https://blogs.nvidia.com/blog/nvidia-at-kubecon-2026/) ⭐️ 7.0/10

NVIDIA 向 Kubernetes 社区捐赠了一款用于 GPU 的动态资源分配驱动程序，使容器化平台上的高性能 AI 基础设施管理更加透明和高效。 这一捐赠解决了 Kubernetes 中 GPU 资源管理的关键需求，Kubernetes 承载着大多数企业 AI 工作负载。它实现了 GPU 动态分区和共享，显著提高了容器化基础设施上 AI 部署的利用率。 该驱动程序与 Kubernetes 的动态资源分配(DRA)框架集成，允许跨 pod 精细化请求和共享 GPU 资源。它建立在现有的 NVIDIA GPU 设备插件之上，该插件已在 Kubernetes 集群中将 GPU 广告为可调度的资源。

rss · NVIDIA Blog · Mar 24, 08:00

**背景**: Kubernetes 已成为企业 AI 工作负载的主要容器编排平台。该平台已通过设备插件支持 GPU 调度，但动态资源分配(DRA)提供了一种更灵活的 Kubernetes 原生方式，用于在工作负载之间请求、分配和共享 GPU 等硬件加速器。此次捐赠扩展了这些原生功能，以实现更好的 GPU 资源可视化和管理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kubernetes.io/docs/concepts/scheduling-eviction/dynamic-resource-allocation/">Dynamic Resource Allocation - Kubernetes</a></li>
<li><a href="https://github.com/NVIDIA/k8s-device-plugin">NVIDIA device plugin for Kubernetes - GitHub</a></li>
<li><a href="https://kubernetes.io/docs/tasks/manage-gpus/scheduling-gpus/">Schedule GPUs - Kubernetes</a></li>

</ul>
</details>

**标签**: `#AI Infrastructure`, `#Kubernetes`, `#GPU Computing`, `#Open Source`, `#NVIDIA`

---

<a id="item-21"></a>
## [构建 NVIDIA Nemotron 3 智能体：推理、多模态 RAG、语音与安全](https://developer.nvidia.com/blog/building-nvidia-nemotron-3-agents-for-reasoning-multimodal-rag-voice-and-safety/) ⭐️ 7.0/10

NVIDIA 发布了开发者博客文章，提供使用 Nemotron 3 模型系列构建智能体 AI 系统的技术指南，涵盖推理智能体、多模态检索增强生成（RAG）、语音交互和安全护栏等核心能力。 本教程展示了使用 Nemotron 3 模型系列（Nano、Super、Ultra）构建智能体 AI 系统的实际实现方法，展示了专业模型如何在规划、推理、检索和安全护栏方面协同工作，为开发者构建生产级 AI 智能体提供了宝贵指导。 本指南涵盖四个关键领域：使用思维链和工具调用的推理智能体、处理文本/图像/表格/音频的多模态 RAG、集成自动语音识别和文本转语音的语音交互，以及用于内容审核的安全护栏。

rss · NVIDIA Developer Blog · Mar 24, 16:00

**背景**: NVIDIA Nemotron 是英伟达开发的基础模型系列，主要包括大型语言模型和相关的推理模型。Nemotron 3 系列包含三个模型：Nano、Super 和 Ultra，专为智能体 AI 应用设计，具有强大的推理和对话能力。多模态 RAG 通过整合文本、图像、表格、音频和视频等不同数据类型来扩展传统 RAG。AI 护栏是建立 AI 系统行为边界的技术控制措施，确保输出安全且符合规范。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nemotron">Nemotron - Wikipedia</a></li>
<li><a href="https://research.nvidia.com/labs/nemotron/Nemotron-3/">NVIDIA Nemotron 3 Family of Models</a></li>
<li><a href="https://www.ibm.com/think/topics/multimodal-rag">What is multimodal RAG? - IBM</a></li>

</ul>
</details>

**标签**: `#agentic-ai`, `#nvidia-nemotron`, `#multimodal-rag`, `#ai-safety`, `#llm-agents`

---

<a id="item-22"></a>
## [Arm 发布 35 年来首款自研芯片](https://techcrunch.com/2026/03/24/arm-is-releasing-its-first-in-house-chip-in-its-35-year-history/) ⭐️ 7.0/10

这标志着 Arm 从纯授权模式向芯片制造的重大战略转型，可能颠覆半导体生态系统。作为一家之前只向其他公司授权芯片设计的公司，这代表了 Arm 直接进入硬件市场。 Arm AGI CPU 专门为 AI 推理设计，即运行训练好的 AI 模型的过程。首批客户包括 Meta、OpenAI、Cerebras 和 Cloudflare，显示出 AI 基础设施市场不同领域的广泛行业采用。

rss · TechCrunch AI · Mar 24, 19:48

**背景**: Arm Holdings 是一家英国公司，35 年来一直只向其他制造商授权其芯片设计，而不是自己生产芯片。这种授权模式允许 Arm 收取费用和版税（通常为芯片销售价格的 1-2%），而无需承担资本密集型的芯片制造开销。AI 推理是指使用训练好的 AI 模型生成预测或输出的过程，这需要大量计算，是 AI 生态系统的主要增长领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.arm.com/products/licensing">Licensing Arm Technology and Subscriptions</a></li>
<li><a href="https://www.strategyzer.com/library/arm-business-model">ARM Business Model - Strategyzer</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#Arm`, `#Meta`, `#CPU`, `#chips`

---

<a id="item-23"></a>
## [Anthropic 的 Claude Code 和 Cowork 获得电脑控制功能](https://www.theverge.com/ai-artificial-intelligence/899430/anthropic-claude-code-cowork-ai-control-computer) ⭐️ 7.0/10

Anthropic 更新了 Claude Code 和 Claude Cowork，使其能够自主执行电脑任务，包括打开文件、使用网页浏览器和应用程序，以及运行开发工具，无需任何设置，甚至在用户离开电脑时也能工作。 这代表了 AI 助手的重要能力扩展，使其能够自主处理复杂的多步骤工作流程。开发者和知识工作者可能会看到显著的生产力提升，因为 Claude 现在可以作为自主代理代表他们完成任务。 电脑控制功能最初由 Anthropic 在 2024 年 10 月作为 Claude 3.5 Sonnet 的一部分引入，使其成为第一个在公开测试版中提供电脑使用功能的前沿 AI 模型。该功能现在可以通过 Claude macOS 应用的 Code 和 Cowork 标签页获取，需要 Pro 或 Max 订阅。

rss · The Verge AI · Mar 24, 13:32

**背景**: Claude Code 是 Anthropic 为开发者设计的代理编码工具，能够理解代码库、编辑文件和运行命令。Claude Cowork 将这些代理能力带给桌面用户，用于非技术性知识工作，包括研究综合、文档准备和文件管理。电脑使用功能允许 Claude 像人类一样与电脑交互——查看屏幕、移动光标、点击按钮和输入文本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/3-5-models-and-computer-use">Introducing computer use, a new Claude 3.5 Sonnet, and Claude ...</a></li>
<li><a href="https://www.anthropic.com/product/claude-cowork">Claude Cowork | Anthropic’s agentic AI for knowledge work</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://www.pcmag.com/news/anthropics-claude-can-now-use-your-computer-to-complete-tasks-for-you">Anthropic's Claude Can Now Use Your Computer to Complete ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Anthropic`, `#Claude`, `#Productivity`, `#Automation`

---

<a id="item-24"></a>
## [TinyLoRA：13 参数微调方法在 Qwen2.5-7B 上实现 91.8% GSM8K 准确率](https://www.marktechpost.com/2026/03/24/this-ai-paper-introduces-tinylora-a-13-parameter-fine-tuning-method-that-reaches-91-8-percent-gsm8k-on-qwen2-5-7b/) ⭐️ 7.0/10

Meta FAIR、康奈尔大学和卡内基梅隆大学的研究人员推出了 TinyLoRA，这是一种极致的参数共享微调方法，可以将可训练参数减少到仅有 13 个（甚至 1 个），同时在 Qwen2.5-7B-Instruct 上实现 GSM8K 基准 91.8%的准确率，总计仅 26 字节（bf16 格式）。 这一突破代表了参数高效微调（PEFT）研究的重要进展，证明大型语言模型可以用极少的可训练参数学习复杂的推理任务。这可能会通过大幅降低计算需求和存储成本来推动 LLM 微调的普及。 该方法通过用微小的投影向量替换可训练矩阵来实现极致的参数效率。在极端共享设置下，TinyLoRA 可以缩减到仅一个可训练参数，同时仍保持推理能力。该方法基于 LoRA（低秩适配），但将其推向理论极限。

rss · MarkTechPost · Mar 24, 18:49

**背景**: LoRA（低秩适配）是一种参数高效微调技术，通过添加轻量级部分来使大型预训练模型适应特定任务，而不是更改整个模型。GSM8K 基准是一个包含 8,500 道小学数学应用题的数据集，需要多步推理，被广泛用于评估 LLM 的推理能力。参数高效微调（PEFT）方法旨在降低微调大型模型的计算和内存成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/03/24/this-ai-paper-introduces-tinylora-a-13-parameter-fine-tuning-method-that-reaches-91-8-percent-gsm8k-on-qwen2-5-7b/">This AI Paper Introduces TinyLoRA, A 13-Parameter Fine-Tuning ...</a></li>
<li><a href="https://github.com/RobotSail/TinyLoRA">TinyLoRA: Extreme Parameter-Efficient Fine-Tuning</a></li>
<li><a href="https://huggingface.co/datasets/openai/gsm8k">openai/gsm8k · Datasets at Hugging Face</a></li>

</ul>
</details>

**标签**: `#parameter-efficient fine-tuning`, `#LoRA`, `#LLM reasoning`, `#model compression`, `#Qwen2.5`

---

<a id="item-25"></a>
## [LeWorldModel (LeWM)：端到端解决表示崩溃的 JEPA 架构](https://www.marktechpost.com/2026/03/23/yann-lecuns-new-leworldmodel-lewm-research-targets-jepa-collapse-in-pixel-based-predictive-world-modeling/) ⭐️ 7.0/10

Yann LeCun 及其合作者推出了 LeWorldModel（LeWM），这是首个能够从原始像素稳定端到端训练的 JEPA（联合嵌入预测架构），仅使用两个损失项：下一嵌入预测损失和强制高斯分布潜嵌入的正则化器。这解决了像素预测世界模型中表示崩溃的根本问题。 这一突破具有重要意义，因为表示崩溃一直是像素数据训练世界模型的主要障碍。LeWM 提供了一种简洁的解决方案，仅用两个损失项就能实现稳定训练，使代理能够在紧凑的潜空间中更有效地进行推理和规划。 LeWM 可以在单个 GPU 上训练，推理速度比基础模型替代方案快近 50 倍。该架构无需之前方法所需的复杂多项损失、指数移动平均、预训练编码器或辅助监督来防止崩溃。

rss · MarkTechPost · Mar 24, 05:53

**背景**: 世界模型（WMs）是开发在紧凑潜空间中推理和规划的代理的核心框架。JEPA 是由 Yann LeCun 和 Meta AI 引入的自监督学习范式，通过从过去的表示预测未来的表示来学习表示。当模型产生冗余嵌入以 trivially 满足预测目标时，就会发生表示崩溃，这是像素世界建模中的基本挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2603.19312">[2603.19312] LeWorldModel: Stable End-to-End Joint-Embedding ...</a></li>
<li><a href="https://www.marktechpost.com/2026/03/23/yann-lecuns-new-leworldmodel-lewm-research-targets-jepa-collapse-in-pixel-based-predictive-world-modeling/">Yann LeCun’s New LeWorldModel (LeWM) Research Targets JEPA ...</a></li>
<li><a href="https://www.humanoidsdaily.com/news/yann-lecun-s-world-model-vision-gets-a-leaner-engine-introducing-leworldmodel">Yann LeCun’s World Model Vision Gets a Leaner Engine ...</a></li>

</ul>
</details>

**标签**: `#AI Research`, `#World Models`, `#Yann LeCun`, `#JEPA`, `#Representation Collapse`, `#Predictive Learning`

---

<a id="item-26"></a>
## [Meta AI Hyperagents 实现实用化递归自我改进](https://www.marktechpost.com/2026/03/23/meta-ais-new-hyperagents-dont-just-solve-tasks-they-rewrite-the-rules-of-how-they-learn/) ⭐️ 7.0/10

这一发展意义重大，因为递归自我改进可能使 AI 系统能够在无需人类干预的情况下持续增强自身能力，可能推动 AI 进步超越当前的线性改进轨迹，代表了从人类设计算法向自我进化系统的潜在范式转变。 Hyperagents 建立在 2025 年达尔文哥德尔机器(DGM)框架之上，该框架展示了 AI 系统可以在通过编码基准测试进行实证验证的同时迭代修改自身代码。然而，此类系统的实际部署引发了重要的安全和对齐问题。

rss · MarkTechPost · Mar 24, 01:42

**背景**: 哥德尔机器于 2003 年提出，是一种理论上的自我改进计算机程序，可以重写自身代码的任何部分来改进自身，前提是能够证明修改是有益的。达尔文哥德尔机器(DGM)于 2025 年 5 月由 Sakana AI 推出，是首个结合基础模型与开放式进化算法实现自我引用代码修改的实际实现。递归自我改进(RSI)理论上可能导致智能爆炸，使 AI 系统迅速超越人类智能水平。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2505.22954">[2505.22954] Darwin Godel Machine: Open-Ended Evolution of ...</a></li>
<li><a href="https://sakana.ai/dgm/">The Darwin Gödel Machine: AI that improves itself by ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement - Wikipedia</a></li>

</ul>
</details>

**标签**: `#meta-ai`, `#hyperagents`, `#recursive-self-improvement`, `#ai-research`, `#gödel-machine`

---

<a id="item-27"></a>
## [法官质疑五角大楼对 Anthropic 的供应链风险认定](https://www.wired.com/story/pentagons-attempt-to-cripple-anthropic-is-troublesome-judge-says/) ⭐️ 7.0/10

一位联邦地区法院法官在周二听证会上批评国防部将 Anthropic 标记为国家安全供应链风险，直接质疑政府这一史无前例认定的动机。 这是首次有法官公开质疑政府在 AI 监管领域的潜在过度干预，该裁决可能为联邦机构如何处理 AI 公司风险树立先例，并对未来 AI 行业的政府监管产生深远影响。 国防部长 Pete Hegseth 于 2026 年 3 月指示国防部将 Anthropic 列为供应链风险，这是首次有美国公司获得此类认定。该认定源于 Anthropic 试图限制五角大楼使用其 Claude AI 模型。

rss · WIRED AI · Mar 24, 22:13

**背景**: 供应链风险认定通常用于外国公司，美国公司被列为供应链风险前所未有。此类认定可阻止政府机构与相关公司签订合同，对公司的政府业务造成重大影响。AI 公司因安全顾虑限制军事使用 AI 技术引发了这场监管冲突。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.justsecurity.org/132851/anthropic-supply-chain-risk-designation/">What Hegseth’s “Supply Chain Risk” Designation of Anthropic ...</a></li>
<li><a href="https://www.mayerbrown.com/en/insights/publications/2026/03/anthropic-supply-chain-risk-designation-takes-effect--latest-developments-and-next-steps-for-government-contractors">Anthropic Supply Chain Risk Designation Takes Effect — Latest ...</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#Anthropic`, `#Department of Defense`, `#tech policy`, `#legal`

---

<a id="item-28"></a>
## [主流包管理器纷纷实现依赖冷却期安全功能](https://simonwillison.net/2026/Mar/24/package-managers-need-to-cool-down/#atom-everything) ⭐️ 7.0/10

这标志着 JavaScript 和 Python 生态系统供应链安全的重大转变。在 2026 年 3 月 LiteLLM 供应链攻击之后，依赖冷却期为开发者提供了防御恶意包的实用方法，让安全社区有时间在恶意更新进入生产系统之前将其检测出来。 这标志着 JavaScript 和 Python 生态系统供应链安全的重大转变。在 2026 年 3 月 LiteLLM 供应链攻击之后，依赖冷却期为开发者提供了防御恶意包的实用方法，让安全社区有时间在恶意更新进入生产系统之前将其检测出来。 各实现方式有所不同：pnpm 10.16 提供 minimumReleaseAge 和可信包排除功能，Yarn 4.10.0 使用分钟级的 npmMinimalAgeGate，Bun 1.3 通过 bunfig.toml 配置，Deno 2.6 有--minimum-dependency-age 标志，npm 11.10.0 引入 min-release-age，uv 0.9.17 添加了相对时长支持，pip 26.0 仅支持绝对时间戳的--uploaded-prior-to。pip 用户可以通过 cron 任务更新日期来解决此限制。

rss · Simon Willison · Mar 24, 21:11

**背景**: 依赖冷却期解决了在包版本发布后立即安装的风险。攻击者可以在包中注入恶意代码并快速发布新版本，希望开发者在任何人注意到之前就更新。通过等待几天，安全社区有机会发现可疑行为并发出警告。2026 年 3 月的 LiteLLM 攻击（版本 1.82.7-1.82.8 通过被攻破的 CI/CD 使用 Trivy 进行后门攻击）为这一讨论提供了及时的背景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=46005111">We should all be using dependency cooldowns - Hacker News</a></li>
<li><a href="https://nesbitt.io/2026/01/10/16-best-practices-for-reducing-dependabot-noise.html">16 Best Practices for Reducing Dependabot Noise | Andrew Nesbitt</a></li>
<li><a href="https://docs.litellm.ai/blog/security-update-march-2026">Security Update: Suspected Supply Chain Incident - liteLLM</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/popular-litellm-pypi-package-compromised-in-teampcp-supply-chain-attack/">Popular LiteLLM PyPI package compromised in TeamPCP supply ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的讨论显示情绪复杂——一些开发者担心如果不立即更新就会很脆弱，而另一些人指出在实践中这基本不是问题。Andrew Nesbitt 关于减少 Dependabot 噪音的早期工作建议等待几天让社区测试后再应用更新。

**标签**: `#supply-chain-security`, `#package-managers`, `#dependency-management`, `#security-best-practices`, `#npm`

---

<a id="item-29"></a>
## [流式专家技术使大型 MoE 模型可在有限 RAM 上运行](https://simonwillison.net/2026/Mar/24/streaming-experts/#atom-everything) ⭐️ 7.0/10

Dan Woods 的"流式专家"技术使得像 Qwen3.5-397B-A17B 和 Kimi K2.5（1 万亿参数，32B 活跃权重）这样的大型混合专家模型可以在 RAM 有限的设备上运行，方法是按需从 SSD 流式传输每个 token 所需的专家权重。 Qwen3.5-397B-A17B 仅需 48GB RAM 即可运行，Kimi K2.5 可在 96GB RAM 的 M2 Max MacBook Pro 上以约 1.7 tokens/秒运行，在 128GB M4 Max 上也是如此。iPhone 演示达到 0.6 tokens/秒，表明该技术可在不同硬件能力上工作。

rss · Simon Willison · Mar 24, 05:09

**背景**: 混合专家（MoE）模型由许多专门的"专家"网络组成，但每个 token 只激活一部分——这使得活跃参数数量可控，而总模型可以非常庞大。流式专家技术利用这一点，按需从 SSD 加载所需的专家，而不是将所有专家保存在 RAM 中。这建立在之前"LLM in a Flash"等探索 SSD 卸载用于 LLM 推理的工作之上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Mar/24/streaming-experts/">Streaming experts - simonwillison.net</a></li>
<li><a href="https://rexai.top/en/ai/llm/2026-03-24-apple-llm-in-flash-moe-local-inference/">Cramming a 400B Model into 48GB: The Magic Behind LLM in a ...</a></li>

</ul>
</details>

**标签**: `#streaming-experts`, `#Mixture-of-Experts`, `#LLM-optimization`, `#edge-computing`, `#model-deployment`

---

<a id="item-30"></a>
## [Dreamer 在播客亮相后加入 Meta 超级智能实验室](https://www.latent.space/p/ainews-dreamer-joins-meta-superintelligence) ⭐️ 7.0/10

这次招聘代表了竞争激烈的 AI 研究领域的一个重要人才获取，继续了知名研究人员加入主要 AI 实验室的趋势。它表明了行业领导者之间对顶尖 AI 人才的激烈竞争。 这次招聘是由 Meta 超级智能实验室的 Nat 和 Alex 在播客发布仅数天后完成的。即使按照行业标准，这种快速的招聘时间表也值得关注。

rss · Latent Space · Mar 24, 06:50

**背景**: Meta 超级智能实验室是 Meta 专门致力于开发先进 AI 系统的 AI 研究部门。Latent Space 播客是展示 AI 研究人员和从业者的热门平台。从播客嘉宾到员工的快速转变表明 Dreamer 是 AI 研究界的一个重要人物。

**社区讨论**: Latent Space 团队指出他们已经很习惯播客嘉宾取得巨大成功，这表明这次招聘符合他们展示有前途的 AI 研究人员并帮助他们职业发展的往绩。

**标签**: `#AI Industry`, `#Meta AI`, `#Hiring`, `#Research Labs`, `#Talent Movement`

---

<a id="item-31"></a>
## [Plasmite：使用内存映射文件作为环形缓冲区的 Rust 轻量级 IPC 系统](https://github.com/sandover/plasmite) ⭐️ 7.0/10

Plasmite 是一个基于 Rust 的轻量级 IPC 系统，重现了 Oblong Industries 内部名为 Plasma 的工具。它使用内存映射文件作为持久化环形缓冲区，采用 JSON 消息格式，并提供 Python、Go、Node 和 C 的绑定，以及 feed、follow、fetch 和 duplex 等 CLI 工具。 与典型的 IPC 系统不同，Plasmite 中的消息通道因为存储为文件而比所有读写者都长寿，甚至能跨越系统重启。这种方法支持无代理的本地 IPC，同时确保消息在进程重启和系统重启后仍然保持持久性。 该系统使用 lite3 进行快速的 JSON 处理，实现零拷贝序列化同时保持 JSON 兼容性。消息是人类可读的，性能良好，配置非常简单。duplex 命令可能对代理间通信很有用。

rss · Hacker News - Show HN · Mar 25, 00:10

**背景**: 内存映射文件通过将共享文件映射到两个进程的地址空间来实现高吞吐量的 IPC，直接进行内存访问。环形缓冲区是一种固定大小的缓冲区，首尾相连，提供高效的 FIFO 数据处理。Lite3 是一种与 JSON 兼容的零拷贝序列化格式，无需模式且自描述。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://goodyduru.com/posts/ipc-mmap/">IPC - Memory Mapped Files · Goodness Duru - goodyduru.com</a></li>
<li><a href="https://deepwiki.com/goldsborough/ipc-bench/3.2.2-memory-mapped-files-(mmap)">Memory-Mapped Files (MMAP) | goldsborough/ipc-bench | DeepWiki</a></li>
<li><a href="https://lite3.io/">Lite³: A JSON-Compatible Zero-Copy Serialization Format</a></li>

</ul>
</details>

**标签**: `#rust`, `#ipc`, `#systems-programming`, `#open-source`, `#json`

---

<a id="item-32"></a>
## [Lexplain：Linux 内核变更解释 AI 工具](https://lexplain.net/) ⭐️ 7.0/10

理解 Linux 内核变更传统上需要挖掘 git 仓库并用内核内部知识分析实际代码差异。提交说明很少传达对系统的实际影响，这使得非内核工程师很难在问题出现之前及时了解相关变更。

rss · Hacker News - Show HN · Mar 24, 22:24

**背景**: Understanding Linux kernel changes traditionally requires digging through git repositories and analyzing actual diffs with knowledge of kernel internals. Commit messages rarely convey the real-world impact on systems, making it difficult for non-kernel engineers to stay informed about relevant changes until issues arise.

**标签**: `#linux`, `#kernel`, `#ai`, `#developer-tools`, `#open-source`

---

<a id="item-33"></a>
## [从写文案到盯数据、算 ROI，流量见顶后，AI Agent 正在杀进核心业务](https://www.infoq.cn/article/P4c8cU7dalmhvWbAsqHL?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

AI agents are increasingly being deployed for core business functions like data monitoring and ROI calculation as companies face traffic saturation, marking a shift from auxiliary to critical business roles.

rss · InfoQ 中文站 · Mar 24, 15:18

**标签**: `#AI Agents`, `#Enterprise AI`, `#Digital Transformation`, `#Business Automation`, `#Marketing Technology`

---

<a id="item-34"></a>
## [深度研究智能体工程化实践：从原型到生产级服务的关键挑战与解法](https://www.infoq.cn/article/Xge5O9rQeOlg0gu0Diic?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

这解决了构建 LLM 应用工程师的主要痛点：弥合工作原型与生产级系统之间的差距。随着 AI 智能体日益普及，了解生产工程挑战对于可靠部署至关重要。 该演讲可能涵盖了 AI 智能体系统在可靠性、监控、测试和扩展方面的实用解决方案。它专门针对为复杂研究任务设计的「深度研究」类型智能体，与更简单的聊天机器人应用相比，这些智能体具有独特的工程挑战。

rss · InfoQ 中文站 · Mar 24, 09:46

**背景**: QCon 是著名的国际软件开发会议系列，邀请行业专家分享新兴技术和最佳实践。由大型语言模型（LLM）驱动的 AI 智能体是通过推理和执行动作来自主完成复杂任务的软件系统。从原型过渡到生产级服务面临重大工程挑战，包括可靠性、可观测性、错误处理和成本管理。

**标签**: `#AI Agents`, `#LLM Engineering`, `#Production Systems`, `#QCon`, `#Software Architecture`

---

<a id="item-35"></a>
## [阿里达摩院发布玄铁 C950 刷新 RISC-V 性能纪录](https://mp.weixin.qq.com/s/TTnqm8qm3Dxshj_0bxwtkw) ⭐️ 7.0/10

阿里达摩院于 3 月 24 日在上海举办的 2026 玄铁 RISC-V 生态大会上发布新一代旗舰 CPU 玄铁 C950，官方称其在 Specint2006 单核测试中得分超过 70 分，为目前公开 RISC-V 处理器中最高水平。 这代表了开源 RISC-V 架构的重大突破，将其定位用于云计算、生成式人工智能和边缘计算等高端计算场景，直接挑战 ARM 和 x86 在高性能计算市场的地位。 玄铁 C950 集成达摩院自研 AI 加速引擎，可原生运行 Qwen3、DeepSeek V3 等千亿参数级模型。但文中提及的 2026 年大会日期相对于当前时间背景存在一定的不确定性。

telegram · zaihuapd · Mar 24, 06:01

**背景**: RISC-V 是一种开源指令集架构，作为 ARM 和 x86 等专有架构的替代方案近年来获得显著关注。Specint2006（现为 SPEC CPU2006 的一部分）是广泛使用的整数 CPU 性能基准测试，分数越高表示处理能力越强。玄铁系列是阿里达摩院开发的自研 RISC-V 处理器产品线。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SPECint">SPECint - Wikipedia</a></li>
<li><a href="https://www.alibabacloud.com/en/solutions/generative-ai/qwen?_p_lc=1">Qwen - Alibaba Cloud</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V3">deepseek-ai/DeepSeek-V3 · Hugging Face</a></li>

</ul>
</details>

**标签**: `#RISC-V`, `#CPU`, `#Alibaba`, `#AI Hardware`, `#Processor`

---

<a id="item-36"></a>
## [欧盟年龄验证 App 排除非谷歌授权安卓系统](https://t.me/zaihuapd/40484) ⭐️ 7.0/10

欧盟正在开发一款开源年龄验证应用程序，要求设备通过谷歌 Play Integrity 验证以确认其为"正版"安卓系统，实际上排除了 GrapheneOS 等非谷歌授权安卓系统用户。 这代表了欧洲数字主权的重大退步，迫使公民依赖美国科技巨头谷歌来获得基本政府服务，并可能为美国技术主导欧洲基础设施开创先例。 该应用程序要求从谷歌 Play 商店下载并拥有谷歌账户，为年龄验证这一核心政府功能创造了对美国基础设施的依赖。开发者和隐私倡导者在 GitHub 上强烈反对此举，认为它违反了互操作性原则并增加了对美国科技巨头的依赖。

telegram · zaihuapd · Mar 24, 12:22

**背景**: GrapheneOS 是一款基于安卓开源项目开发的隐私和安全安卓系统，由非营利组织运营，默认移除谷歌应用和服务。谷歌 Play Integrity API 用于验证应用是否在具有有效谷歌 Play 服务的正版安卓设备上运行，常用于防止欺诈，但越来越多地被用作准入机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grapheneos.org/">GrapheneOS: the private and secure mobile OS</a></li>
<li><a href="https://grapheneos.org/features">Features overview - GrapheneOS</a></li>
<li><a href="https://developers.google.com/android/play-protect/client-protections">On-device protections | Play Protect | Google for Developers</a></li>

</ul>
</details>

**社区讨论**: 开发者社区表达了强烈反对，GitHub 和隐私论坛上的观点认为这种做法从根本上违背了欧盟数字主权目标，并为基本政府服务创造了不必要的对美国科技基础设施的依赖。

**标签**: `#EU Regulation`, `#Android`, `#Age Verification`, `#Digital Sovereignty`, `#Google Play`

---

<a id="item-37"></a>
## [微软发布 7 本综合 Rust 培训教材](https://github.com/microsoft/RustTraining) ⭐️ 7.0/10

微软在 GitHub 上发布了 7 本综合 Rust 培训教材，存放于 RustTraining 仓库，涵盖从 C/C++、C#、Python 开发者语言过渡，到高级异步编程、模式、类型驱动正确性和工程实践等主题。 这是微软对 Rust 生态系统的重大贡献，提供免费的高质量教育资源，有望加速 Rust 在 Windows 和云基础设施开发社区的采用。 每本教材包含 15-16 章，并配有 Mermaid 图、可编辑的 Rust Playground、练习和全文搜索。材料采用 MIT 和 CC-BY-4.0 双许可证发布，可在 GitHub 上获取 Markdown 源文件，并通过 GitHub Pages 浏览渲染版本。

telegram · zaihuapd · Mar 24, 23:57

**背景**: Rust 是一种以内存安全和高性能著称的系统编程语言，在云基础设施和 Windows 开发中的应用日益增加。微软一直在 Rust 方面进行投资，既用于内部工具也用于外部开发。这些培训材料涵盖了来自 C/C++、C#和 Python 开发者的过渡路径，以及异步编程和类型驱动开发等高级主题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/microsoft/RustTraining/blob/main/type-driven-correctness-book/src/ch00-introduction.md">RustTraining/type-driven-correctness-book/src/ch00 ... - GitHub</a></li>
<li><a href="https://mermaid.js.org/intro/">About Mermaid | Mermaid</a></li>

</ul>
</details>

**标签**: `#Rust`, `#Microsoft`, `#Programming Education`, `#Open Source`, `#Training Materials`

---

<a id="item-38"></a>
## [OpenAI 推出 Sora AI 视频生成器仅六个月后停止运营](https://www.bloomberg.com/news/articles/2026-03-24/openai-plans-to-discontinue-support-for-sora-ai-video-generator?srnd=phx-technology) ⭐️ 7.0/10

OpenAI 计划停止其 Sora AI 视频生成器，在上线仅六个月后关闭独立应用和开发者 API。与 Sora 相关的迪士尼合作也正在逐步收尾。 此次停用代表着 OpenAI 的重大战略转向，从 AI 视频生成转向 AI agents 和名为 Spud 的新模型。这表明 AI 行业即使对高调产品也能迅速放弃，转而投向更有前景的技术。 OpenAI 最近完成了名为 Spud 的新 AI 模型的开发。CEO Sam Altman 已不再直接负责安全团队，转而专注于资本筹集、供应链和大型数据中心建设，为公司潜在的 IPO 做准备。

telegram · zaihuapd · Mar 25, 00:30

**背景**: Sora 是 OpenAI 推出的 AI 视频生成产品，通过高调营销和迪士尼合作进行推广。仅上线 6 个月后就停用，反映了 AI 视频生成领域的竞争压力。OpenAI 现在正在重组安全团队，将安全工作更紧密地纳入开发流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomsguide.com/ai/openai-just-killed-sora-as-company-readies-ipo-and-new-spud-model">OpenAI just killed Sora as company readies IPO and new 'Spud ...</a></li>
<li><a href="https://www.benzinga.com/news/26/03/51443965/openai-ceo-shifts-responsibilities-preps-spud-ai-model-ceo-sam-altman-has-relinquished-direct-oversi">"OpenAI CEO Shifts Responsibilities, Preps 'Spud' AI Model ...</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Sora`, `#AI video generation`, `#product discontinuation`, `#AI industry`

---