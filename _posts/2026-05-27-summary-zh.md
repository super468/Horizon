---
layout: default
title: "Horizon Summary: 2026-05-27 (ZH)"
date: 2026-05-27
lang: zh
---

> From 185 items, 25 important content pieces were selected

---

1. [Bob Nystrom 的«你的函数是什么颜色?»文章](#item-1) ⭐️ 8.0/10
2. [NVIDIA CUDA 13.3 带来 Tile 编程和编译器自动调优](#item-2) ⭐️ 8.0/10
3. [桑达尔·皮查伊在 Decoder 播客上讨论 AI 和搜索的未来](#item-3) ⭐️ 8.0/10
4. [AI 编码代理如何改变软件开发行业](#item-4) ⭐️ 8.0/10
5. [curl 维护者警告 AI 驱动的安全报告洪流](#item-5) ⭐️ 8.0/10
6. [Microsoft Copilot Cowork 安全漏洞可导致数据外泄](#item-6) ⭐️ 8.0/10
7. [Google Cloud 在 BigQuery 中引入跨引擎 Apache Iceberg 支持](#item-7) ⭐️ 8.0/10
8. [Gemma 4 多词元预测：生成速度最高提升约 3 倍](#item-8) ⭐️ 8.0/10
9. [园林市甲基丙烯酸甲酯储罐热失控事故分析](#item-9) ⭐️ 7.0/10
10. [维基百科编辑罢工抗议基金会技术团队裁员](#item-10) ⭐️ 7.0/10
11. [外包加本地 AI：新的成本效益替代方案](#item-11) ⭐️ 7.0/10
12. [荷兰阻止美国收购 DigiD 托管服务商](#item-12) ⭐️ 7.0/10
13. [亚马逊 Bedrock AgentCore 支付服务预览版发布](#item-13) ⭐️ 7.0/10
14. [使用 AWS 和 NVIDIA 集成构建多智能体 AI 系统](#item-14) ⭐️ 7.0/10
15. [NVIDIA 发布 CompileIQ 自动调优工具提升 GPU 内核性能](#item-15) ⭐️ 7.0/10
16. [初创公司利用印度零工收集机器人训练数据](#item-16) ⭐️ 7.0/10
17. [AI 战争已经到来](#item-17) ⭐️ 7.0/10
18. [优步总裁质疑 AI 投资回报：年度预算四个月耗尽](#item-18) ⭐️ 7.0/10
19. [调查：85%的企业希望采用智能体 AI，但 76%缺乏基础设施](#item-19) ⭐️ 7.0/10
20. [人工智能正在侵蚀入门级职业机会](#item-20) ⭐️ 7.0/10
21. [Stability AI 发布 Stable Audio 3 音频生成模型](#item-21) ⭐️ 7.0/10
22. [中国扩大对 DeepSeek、阿里巴巴等私企 AI 人才的出国限制](#item-22) ⭐️ 7.0/10
23. [AWS MCP 服务器正式可用，全面适配 API 并支持 IAM 权限控制](#item-23) ⭐️ 7.0/10
24. [Ray 算力调度在小红书 AI 数据生产中的实践](#item-24) ⭐️ 7.0/10
25. [中国审查 Meta 收购 AI 初创公司 Manus，联合创始人被限制离境](#item-25) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Bob Nystrom 的«你的函数是什么颜色?»文章](https://journal.stuffwithstuff.com/2015/02/01/what-color-is-your-function/) ⭐️ 8.0/10

这篇文章引发了广泛而深入的技术辩论,讨论显式异步信号与隐式并发模型之间的权衡,影响了多个语言的开发者对异步编程和语言设计选择的思考方式。 核心论点是异步函数创建了一种在整个调用栈中传播的"颜色" - 一旦一个函数变成异步,其调用者也必须变成异步,从而在整个代码库中产生连锁效应。

hackernews · tosh · May 26, 15:58

**背景**: 函数着色是指异步函数要求其调用者也必须是异步的现象,从而在代码库中造成分裂。这是 JavaScript、Python、Rust 和 C#等语言中的常见挑战。一些语言如 Go 通过运行时中的隐式异步处理来避免此问题,而代数效应(如 OCaml 5 中使用的)则提供了不同的解决方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://quuxplusone.github.io/blog/2018/03/16/async-roundup/">Async /await, and coloring schemes in general – Arthur O'Dwyer...</a></li>
<li><a href="https://kristoff.it/blog/zig-colorblind-async-await/">What is Zig's “Colorblind” Async /Await? | Loris Cro's Blog</a></li>

</ul>
</details>

**社区讨论**: 评论显示观点分歧:批评者认为文章过于简化,所有函数都有限制(不仅仅是异步),而支持者表示着色反映了重要的语言设计选择。人们讨论了 Go 的隐式模型、Haskell IO monad、Rust unsafe 和代数效应等替代方案。一些评论者将代数效应视为潜在的解决方案。

**标签**: `#async-await`, `#programming-languages`, `#function-coloring`, `#concurrency`, `#language-design`

---

<a id="item-2"></a>
## [NVIDIA CUDA 13.3 带来 Tile 编程和编译器自动调优](https://developer.nvidia.com/blog/nvidia-cuda-13-3-enhances-gpu-development-with-tile-programming-in-c-compiler-autotuning-and-python-updates/) ⭐️ 8.0/10

这一更新对从事 AI/ML 和 HPC 领域的 GPU 开发者具有重要影响。Tile 编程提供了一种新范式，用于表达基于 Tile 的计算模式，从而优化 NVIDIA 张量核心单元。编译器自动调优自动化了优化标志的选择，无需手动调整即可获得显著的性能提升。 CUDA Tile 基于使用 MLIR 基础设施的 Tile IR（中间表示）规范。Python 实现 cuTile 使开发者能够编写针对张量核心单元的自定义内核。Tile 编程专注于针对 NVIDIA 张量核心架构设计的基于 Tile 的计算模式和优化。

rss · NVIDIA Developer Blog · May 26, 21:39

**背景**: CUDA（统一计算设备架构）是 NVIDIA 的专有并行计算平台和 API，使开发者能够利用 GPU 进行通用计算。Tile 编程代表了一种新方法，它抽象了基于 Tile 的计算模式，使得针对张量核心等硬件的优化更加容易。编译器自动调优使用贝叶斯优化等技术自动找到最佳编译标志。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/cuda/tile">CUDA Tile | NVIDIA Developer</a></li>
<li><a href="https://github.com/NVIDIA/cuda-tile">GitHub - NVIDIA/cuda-tile: CUDA Tile IR is an MLIR-based intermediate ...</a></li>
<li><a href="https://www.spheron.network/blog/cuda-13-tile-programming-gpu-cloud/">CUDA 13 Tile Programming on GPU Cloud: A 2026 Developer Guide</a></li>

</ul>
</details>

**社区讨论**: 没有关于此新闻的社区讨论。

**标签**: `#CUDA`, `#GPU programming`, `#NVIDIA`, `#parallel computing`, `#tile programming`

---

<a id="item-3"></a>
## [桑达尔·皮查伊在 Decoder 播客上讨论 AI 和搜索的未来](https://www.theverge.com/podcast/936445/sundar-pichai-ai-search-google-zero-youtube-web) ⭐️ 8.0/10

这次专访是桑达尔·皮查伊连续第五年在谷歌 I/O 之后接受 The Verge 的 Decoder 播客采访，成为该节目的标志性传统之一。对话涵盖了 I/O 上宣布的人工智能进展、谷歌搜索的转型以及整个网络生态系统的更广泛变化。

rss · The Verge AI · May 26, 14:00

**背景**: Decoder 播客是 The Verge 的旗舰专访节目，展示与科技行业领军人物的深度对话。谷歌 I/O 是该公司的年度开发者大会，通常会在会上发布重要的产品和人工智能公告。作为 Alphabet 和谷歌的 CEO，桑达尔·皮查伊领导着拥有谷歌搜索、YouTube、Android 和谷歌云等主流产品的公司。

**标签**: `#AI`, `#Google`, `#Search`, `#Big Tech`, `#Sundar Pichai`

---

<a id="item-4"></a>
## [AI 编码代理如何改变软件开发行业](https://www.wired.com/story/how-ai-agents-plunged-tech-world-into-chaos/) ⭐️ 8.0/10

这代表了软件构建方式的根本转变。传统软件开发需要程序员手动编写和测试代码；这些 AI 代理可以自主执行整个开发流程，使任何具备基本技术知识的人都有可能成为”开发者”。 Claude Code 是 Anthropic 开发的具身化编程系统，能够读取代码库、在多个文件中进行编辑、运行测试并提交代码——对于没有工程背景的用户来说，这是直到最近才出现的软件入口点。OpenClaw 是一个免费开源的自主 AI 代理，通过大型语言模型执行任务，使用消息平台作为其主要用户界面。

rss · WIRED AI · May 26, 10:00

**背景**: AI 编码代理代表了一类新型 AI 工具，旨在在软件开发中采取自主行动，而不仅仅是生成代码建议。Claude Code 由 Anthropic 发布，能够上下文章理解整个代码库并执行复杂的开发任务。这遵循了过去计算范式转变的轨迹，但以极快的速度运行，可能自动化以前需要人类工程师数周才能完成的任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/product/claude-code">Claude Code | Anthropic's agentic coding system</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw - Wikipedia</a></li>
<li><a href="https://openclaw.ai/">OpenClaw — Personal AI Assistant</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#Claude Code`, `#software development`, `#Anthropic`, `#AI automation`

---

<a id="item-5"></a>
## [curl 维护者警告 AI 驱动的安全报告洪流](https://simonwillison.net/2026/May/26/the-pressure/#atom-everything) ⭐️ 8.0/10

curl 的创建者 Daniel Stenberg 报告称，与 2024 年相比，该项目收到的 AI 辅助安全漏洞报告增加了 4 到 5 倍，平均每天收到不止一份详细报告——这迫使他工作时间明显更长，并首次因工作与生活的平衡问题受到妻子的担忧。 这代表了开源可持续性的新兴危机：人工智能工具现在以前所未有的规模发现漏洞，但大量报告威胁到维护者的身心健康和项目生存能力——即使是 Stenberg 这样的顶尖维护者也在精疲力竭，表明许多关键的开源项目面临生存风险。 尽管报告数量激增，但有一个积极的现象：发现的几乎所有漏洞都是低危或中危级别——上一个高危级别的 curl CVE 是 2023 年 10 月发布的。然而，尽管这些漏洞普遍严重程度较低，审查和响应所有报告的"心理负担"仍然令人难以承受。

rss · Simon Willison · May 26, 23:48

**背景**: curl 是互联网上最基础的开源工具之一，几乎被所有操作系统和设备用于通过 URL 传输数据。人工智能模糊测试和漏洞扫描工具（如 AFL-Fuzz 和 AI 驱动漏洞扫描器）的最新进展大大加速了自动化安全研究，使人工智能代理能够大规模生成详细、可信的安全漏洞报告。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cset.georgetown.edu/article/ai-and-the-software-vulnerability-lifecycle/">AI and the Software Vulnerability Lifecycle | Center for Security and Emerging Technology</a></li>
<li><a href="https://en.wikipedia.org/wiki/Fuzzing">Fuzzing - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 讨论强调了对在人工智能加速漏洞发现下开源基础设施可持续性的广泛担忧。许多评论者对 Stenberg 表示同情，同时警告这种模式将蔓延到其他主要项目。一些人建议使用自动分类工具或为专职维护者提供资金作为潜在的解决方案。

**标签**: `#open-source`, `#security`, `#curl`, `#AI-assisted-discovery`, `#maintainer-burnout`

---

<a id="item-6"></a>
## [Microsoft Copilot Cowork 安全漏洞可导致数据外泄](https://simonwillison.net/2026/May/26/copilot-cowork-exfiltrates-files/#atom-everything) ⭐️ 8.0/10

提示注入是一种网络安全攻击手段，攻击者通过精心设计的欺骗性输入来操纵大型语言模型（LLM）执行非预期操作或泄露机密信息。像 Microsoft Copilot Cowork 这样的代理型 AI 系统旨在代表用户自主执行发送邮件和访问云存储等任务，使其成为此类攻击的目标。邮件客户端通常会加载外部图片以显示富媒体内容，这种行为可能被武器化以通过网络请求泄露数据。 攻击原理是诱导 Copilot Cowork 代理在邮件中嵌入外部图片 URL。当收件人打开邮件时，其邮件客户端自动加载图片，发起出站网络请求，这些请求的参数中可以编码被盗数据。结合系统生成的预认证 OneDrive 链接，攻击者可以在无需额外认证的情况下下载文件。

rss · Simon Willison · May 26, 15:36

**背景**: Prompt injection is a cybersecurity exploit where attackers craft deceptive inputs to manipulate large language models (LLMs) into performing unintended actions or revealing confidential information. Agentic AI systems like Microsoft Copilot Cowork are designed to autonomously execute tasks such as sending emails and accessing cloud storage on behalf of users, making them attractive targets for such attacks. Email clients routinely load external images to display rich content, a behavior that can be weaponized to leak data through network requests.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection | OWASP Foundation</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论强调了将提示注入、数据泄露和自主代理能力相结合的"致命三要素 "的担忧。评论者强调，根本挑战在于防止 AI 系统执行可能导致数据泄露的操作，特别是当系统的可信状态被用来绕过安全控制时。

**标签**: `#security-vulnerability`, `#prompt-injection`, `#microsoft-copilot`, `#data-exfiltration`, `#AI-safety`

---

<a id="item-7"></a>
## [Google Cloud 在 BigQuery 中引入跨引擎 Apache Iceberg 支持](https://www.infoq.cn/article/kadDStA9JWuOGHujwdoz?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

Google Cloud 宣布在 BigQuery 中支持跨引擎 Apache Iceberg，允许在不同处理引擎（包括 Spark、Trino、Flink 和 Hive）之间无缝共享数据。 这代表了数据 lakehouse 生态系统的一个重要里程碑，促进了开放表格式的采用并提高了不同查询引擎之间的互操作性。数据平台架构师和工程师将受益于更灵活的数据访问模式，而无需担心供应商锁定。 BigQuery 现在可以直接查询和写入 Apache Iceberg 表，使用提供 ACID 事务、时间旅行和模式演进能力的开放表格式。这使组织能够避免在多个处理引擎之间重复数据，同时维护单一数据源。

rss · InfoQ 中文站 · May 27, 09:07

**背景**: Apache Iceberg 是一个开源的高性能表格式，专为存储在数据湖（如 AWS S3、Azure Data Lake 和 Google Cloud Storage）中的大型分析数据集设计。数据 lakehouse 架构将数据湖的开放性和可扩展性与数据仓库的可靠性和治理结合在单一平台上。Databricks 和 Snowflake 等主要云提供商也已采用开放表格式来提高数据可移植性并减少供应商锁定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apache_Iceberg">Apache Iceberg - Wikipedia</a></li>
<li><a href="https://www.databricks.com/blog/what-is-data-lakehouse">What is a Data Lakehouse? - Databricks</a></li>
<li><a href="https://aws.amazon.com/what-is/data-lakehouse/">What is a Data Lakehouse? - Data Lakehouse Explained - AWS</a></li>

</ul>
</details>

**标签**: `#Google Cloud`, `#BigQuery`, `#Apache Iceberg`, `#Data Lakehouse`, `#Cloud Data Platform`

---

<a id="item-8"></a>
## [Gemma 4 多词元预测：生成速度最高提升约 3 倍](https://www.infoq.cn/article/vduuUvpVw0FiIcplFtGd?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

谷歌发布了 Gemma 4，引入多词元预测这一新型推理优化技术，可将生成速度提升至约 3 倍，相比之前版本有显著提升。 这一进展意义重大，因为其为开源大语言模型带来了实质性的推理速度提升，使 Gemma 4 更适用于实时应用场景，并降低了开发者构建 AI 产品的计算成本。 多词元预测的工作原理是将每个完整的 Gemma 4 目标模型与一个小型紧密耦合的"起草模型"配对，通过投机解码提前预测多个词元，允许主模型并行验证和接受预测，而非逐个进行。

rss · InfoQ 中文站 · May 26, 16:24

**背景**: 多词元预测(MTP)是大语言模型推理优化中的一项新兴技术。传统语言模型按顺序逐个生成词元，这限制了推理速度。MTP 通过同时预测多个未来词元并使用验证机制来接受正确预测来解决这一瓶颈，从而有效实现了生成过程的并行化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/gemma/gemma-4/">Gemma 4 — Google DeepMind</a></li>
<li><a href="https://kalinga.ai/gemma-4-multi-token-prediction-3x-inference/">Gemma 4 Multi - Token Prediction : Ultimate 3x AI Boost 2026</a></li>
<li><a href="https://ai.google.dev/gemma/docs/core/model_card_4">Gemma 4 model card | Google AI for Developers</a></li>

</ul>
</details>

**标签**: `#Google Gemma`, `#LLM`, `#Multi-token Prediction`, `#AI Performance`, `#Open Source`

---

<a id="item-9"></a>
## [园林市甲基丙烯酸甲酯储罐热失控事故分析](https://www.science.org/content/blog-post/methyl-methacrylate-tank) ⭐️ 7.0/10

Science.org 博客发布了一份详细的技术分析,解析了加州园林市一起甲基丙烯酸甲酯(MMA)储罐事故的化学和工程原理,探讨了导致热失控聚合反应的危险机理及其可能引发的 BLEVE(沸腾液体膨胀蒸汽爆炸)风险。 这起事故凸显了化工行业对活性单体的安全管理挑战。MMA 具有一旦受热即可自加速聚合的特性,形成热失控反应,这在化工储运中极难控制,可能引发灾难性后果。 MMA 单体需添加阻聚剂以防止意外聚合,但阻聚剂生效需要蒸气空间中至少 5%的氧气浓度。储罐材质应为不锈钢、碳钢、玻璃或铝材,以确保安全存放。

hackernews · nooks · May 26, 19:25

**背景**: 甲基丙烯酸甲酯(CH2=C(CH3)COOCH3)是一种无色液体,主要用于生产聚甲基丙烯酸甲酯(PMMA/有机玻璃)。当 MMA 受热时会触发聚合反应,而聚合反应产生的热量又会加速进一步聚合,形成热失控链式反应。BLEVE 是此类事故的最危险场景,火焰包围储罐导致内部压力急剧上升,最终造成容器破裂爆炸。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Methyl_methacrylate">Methyl methacrylate - Wikipedia</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC9920456/">Inhibition of Free Radical Polymerization : A Review - PMC</a></li>
<li><a href="https://www.yahoo.com/news/us/articles/why-orange-county-chemical-tank-100000472.html">Why is Orange County chemical tank crisis so hard to fix?</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了多起类似事故,包括苯乙烯和丁基丙烯酸酯的事后分析、金曼市 BLEVE 事件以及 2011 年东日本大地震对核电站安全的影响。有人提出了设置被动保护系统的问题,也有人从消防员视角分享了如何通过泄压防止热失控的经验。另有提及华盛顿州造纸厂同一天发生的'白液'爆炸事故。

**标签**: `#chemistry`, `#industrial safety`, `#chemical engineering`, `#incident analysis`, `#hazard prevention`

---

<a id="item-10"></a>
## [维基百科编辑罢工抗议基金会技术团队裁员](https://medium.com/@jakeorlowitz/wikipedia-is-doing-the-capitalist-thing-56a393232943) ⭐️ 7.0/10

被解雇的开发者布鲁克曾被认为是 MediaWiki 的“仁慈独裁者”（BDFL）的候选人。社区技术团队根据编辑者的众包需求进行开发，他们的被裁撤意味着非技术背景的编辑者现在必须自行维护自己的“影子 IT”基础设施。据报道，基金会约有 17 个月的运营费用储备。

hackernews · cdrnsf · May 26, 20:33

**背景**: MediaWiki 是支撑维基百科及其他维基媒体项目的开源软件平台。开源治理通常涉及社区贡献和集体决策，维护者通常担任类似“仁慈独裁者”（BDFL）的角色。社区愿望清单是志愿编辑者提交功能请求以获得专业开发工作的主要渠道。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Open-source_governance">Open-source governance</a></li>
<li><a href="https://en.wikipedia.org/wiki/Open_source">Open source - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区成员对布鲁克的解雇表示震惊，强调她对 MediaWiki 发展的历史重要性。编辑者们围绕基金会的 17 个月储备是“富有”还是财务脆弱展开辩论，一些人认为这不足以维持长期稳定。长期编辑者强调，除了简单的文字编辑之外，还有多少看不见的劳动投入到维护维基百科中。

**标签**: `#wikipedia`, `#open-source`, `#labor-relations`, `#wikimedia-foundation`, `#tech-industry`

---

<a id="item-11"></a>
## [外包加本地 AI：新的成本效益替代方案](https://www.signalbloom.ai/posts/outsourcing-plus-localai-will-soon-become-more-economical-vs-frontier-labs/) ⭐️ 7.0/10

社区强调了细微的视角：评论者指出操作员技能水平显著影响结果——具有良好提示词技巧的高级开发者表现优于缺乏积极性的团队。另一些人观察到，无论外包还是 AI 都需要详细的规格说明，质疑如果写得这么详细的提示，为什么还要外包。一些人报告说，公司已经在用美国程序员+AI 取代东欧团队。

hackernews · GodelNumbering · May 26, 12:08

**背景**: Frontier AI labs refer to leading companies like OpenAI (GPT-4), Anthropic (Claude), and Google Gemini that train large language models with massive compute resources. Local AI runs models on personal hardware rather than calling external APIs. Traditional outsourcing involves hiring external development teams, often in lower-cost regions, to handle software tasks.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apidog.com/blog/local-vs-api-ai-models/">Running AI models locally vs . via API : which should you choose?</a></li>
<li><a href="https://localaimaster.com/blog/local-ai-vs-chatgpt-cost">Local AI vs ChatGPT Cost : AI Cost Calculator... | Local AI Master</a></li>

</ul>
</details>

**社区讨论**: The community highlights nuanced perspectives: commentators note that operator skill level significantly impacts outcomes—senior devs with good prompting skills outperform less motivated teams. Others observe detailed specifications are needed for both outsourcing and AI, questioning why outsource if you're writing such detailed prompts anyway. Some report companies are already replacing Eastern European teams with US programmers + AI.

**标签**: `#AI_economics`, `#LLM_pricing`, `#outsourcing`, `#software_development`, `#AI_replacement`

---

<a id="item-12"></a>
## [荷兰阻止美国收购 DigiD 托管服务商](https://www.politico.eu/article/netherlands-blocks-us-takeover-vital-digital-supplier/) ⭐️ 7.0/10

荷兰政府阻止了美国对 Solvinity 公司的收购要约。Solvinity 是托管荷兰电子身份证系统 DigiD 的承包商，该系统为数百万公民提供服务。荷兰政府此举援引了美国《云法案》(CLOUD Act)可强制要求访问数据（无论数据存储何处）的规定，导致公民数据隐私面临风险。 这一决定代表了欧洲数字主权的重要宣示，荷兰优先保护公民数据免受外国拥有的关键基础设施带来的美国法律管辖权影响。这一先例为其他欧盟国家在处理接受敏感技术领域的外国投资与维护数据主权之间的权衡提供了参考。 此次收购方据报道为 Kyndryl 公司，这是 2021 年从 IBM 基础设施服务部门剥离成立的公司，在 63 个国家开展业务。荷兰议会此前曾通过动议要求终止与 Solvinity 的合同，但政府予以延长，因此阻止收购成为解决数据主权问题的最后政策工具。

hackernews · vrganj · May 26, 11:46

**背景**: 美国《云法案》（2018 年）使美国执法机构能够强制科技公司提供所要求的数据，无论数据存储在美国境内还是境外。DigiD 是荷兰政府的电子身份认证平台，每天处理数百万次公共服务认证请求，涵盖税收、医疗等领域。数字主权指的是国家对关键数字基础设施和数据在本国法律管辖范围内而非外国法律下进行控制的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://spotler.com/en-de/blog/what-is-the-us-cloud-act">What is the US CLOUD Act ? GDPR impact explained | Spotler</a></li>
<li><a href="https://www.hivenet.com/post/what-digital-sovereignty-really-means-in-cloud-computing">Digital Sovereignty in Cloud Computing Explained | Hivenet</a></li>

</ul>
</details>

**社区讨论**: 评论表达了终于阻止收购的欣慰之情，数周来公众持续施压，有用户指出议会在政府延长合同之前几乎一致投票赞成终止与 Solvinity 的合同。其他人认为，通过架构设计实现的隐私（加密主权，使承包商在数学上无法访问数据）优于政策承诺式的隐私，还有人质疑为什么荷兰不能为 2000 万用户自建开源身份解决方案。

**标签**: `#digital-sovereignty`, `#privacy`, `#geopolitics`, `#critical-infrastructure`, `#identity-systems`

---

<a id="item-13"></a>
## [亚马逊 Bedrock AgentCore 支付服务预览版发布](https://aws.amazon.com/blogs/machine-learning/technical-deep-dive-agentcore-payments-and-innovation-in-agentic-commerce/) ⭐️ 7.0/10

亚马逊 Bedrock AgentCore 支付服务现已在预览版中可用，可向外部服务提供即时支付，支持稳定币进行低成本微交易，并配备可配置的支出安全限制。 这使得 AI 代理能够在无需手动设置计费的情况下自主向外部服务支付，通过稳定币支持使亚美分级别的交易具有经济可行性。这对构建需要自动商务能力的代理式应用开发者来说具有重要意义。 AgentCore 支付通过 API 向外部服务提供即时支付，无需为每个提供商手动配置计费设置。稳定币支持使得原本不经济的亚美分微交易变得可行，而可配置的支出安全限制允许对代理预算和交易限额进行精细控制。

rss · AWS Machine Learning Blog · May 26, 17:57

**背景**: 亚马逊 Bedrock 是 AWS 用于构建生成式 AI 应用的完全托管服务。AgentCore 扩展了 Bedrock 的功能，使 AI 代理能够与外部服务和 API 交互。稳定币是一种设计为保持稳定价值的加密货币，通常与美元等储备资产挂钩，使其适用于传统支付手续费过于昂贵的小额交易。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.investopedia.com/terms/s/stablecoin.asp">investopedia.com/terms/s/ stablecoin .asp</a></li>

</ul>
</details>

**标签**: `#AWS`, `#AI Agents`, `#Payments`, `#Amazon Bedrock`, `#Agentic Commerce`

---

<a id="item-14"></a>
## [使用 AWS 和 NVIDIA 集成构建多智能体 AI 系统](https://aws.amazon.com/blogs/machine-learning/build-high-performance-generative-ai-systems-with-strands-agents-nvidia-nim-and-amazon-bedrock-agentcore/) ⭐️ 7.0/10

这种集成展示了生产级 AI 系统的实际架构，具备并行推理、上下文持久化和可追踪的执行路径——这些是企业级生成式 AI 部署的关键能力。 该教程使用基于 CUDA、TensorRT、TensorRT-LLM 和 Triton Inference Server 构建的 NVIDIA NIM 容器进行优化的 GPU 推理。Amazon Bedrock AgentCore 提供共享内存和内置可观测性，而 Strands Agents 是一个模型驱动的开源 SDK，只需少量代码即可实现自主智能体推理。

rss · AWS Machine Learning Blog · May 26, 17:39

**背景**: NVIDIA NIM（NVIDIA 推理微服务）是预构建的容器化 AI 服务，可在任何支持 NVIDIA GPU 的环境中部署模型——云端、数据中心或本地设备。Amazon Bedrock AgentCore 是 AWS 用于构建和运行智能体的托管服务，具有内置的可观测性。Strands Agents 是 AWS 的开源 SDK，采用模型驱动的方法，只需少量代码即可构建 AI 智能体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/nim">NIM for Developers | NVIDIA Developer</a></li>
<li><a href="https://aws.amazon.com/blogs/opensource/introducing-strands-agents-an-open-source-ai-agents-sdk/">Introducing Strands Agents , an Open Source AI Agents SDK</a></li>

</ul>
</details>

**标签**: `#multi-agent-systems`, `#generative-ai`, `#amazon-bedrock`, `#nvidia-nim`, `#ai-infrastructure`

---

<a id="item-15"></a>
## [NVIDIA 发布 CompileIQ 自动调优工具提升 GPU 内核性能](https://developer.nvidia.com/blog/extract-more-kernel-performance-with-nvidia-compileiq-auto-tuning/) ⭐️ 7.0/10

NVIDIA 发布了 CompileIQ，这是一款自動调优工具，能夠自動搜尋最優的編譯器標誌以最大化 GPU 內核性能，無需用戶具備專業的手動調優知識。 CompileIQ 可自動在不同編譯器選項之間進行搜尋，在特定硬體上評估性能以找到每個內核的最佳配置。該工具旨在解決將編譯器設置與工作負載特性相匹配的困難問題。

rss · NVIDIA Developer Blog · May 26, 22:08

**背景**: 編譯器優化是實現 GPU 內核高性能的關鍵因素。傳統的編譯器標誌（如-O3）提供一般性優化，但通常無法為特定工作負載提取最大性能。自動調優研究已表明，機器學習和系統性探索可以發現優於標準優化級別的編譯器配置，這在關於編譯器自動調優的學術調查中已有證明。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/1801.04405">A Survey on Compiler Autotuning using Machine Learning</a></li>
<li><a href="https://www.cs.umd.edu/~hollings/papers/ipdps09.pdf">Scalable Auto - tuning Framework for Compiler Optimization</a></li>

</ul>
</details>

**标签**: `#GPU optimization`, `#compiler tuning`, `#NVIDIA`, `#performance engineering`, `#CUDA`

---

<a id="item-16"></a>
## [初创公司利用印度零工收集机器人训练数据](https://techcrunch.com/2026/05/26/human-archive-taps-into-indias-services-startups-to-collect-data-for-physical-ai/) ⭐️ 7.0/10

Human Archive 由加州大学伯克利分校和斯坦福大学的研究人员创立，该公司雇佣印度的零工工人佩戴配备摄像头的帽子和传感器设备，为人工智能和机器人实验室收集真实世界的物理训练数据。 这解决了物理人工智能和机器人开发中的一个关键瓶颈——获取多样化、高质量的真实世界训练数据。它还提出了人工智能开发中全球劳动力动态的重要问题，以及从发展中经济体采购数据的伦理问题。 该公司招募印度零工工人，让他们佩戴摄像头帽子和身体传感器执行任务，采集机器人学习所需的运动数据、互动和环境响应。这些数据随后被出售给人工智能和机器人实验室用于训练。

rss · TechCrunch AI · May 26, 16:00

**背景**: 物理人工智能是指与物理世界互动的 AI 系统，如机器人、无人机和自动驾驶汽车。这些系统需要大量真实世界的互动数据来学习如何应对复杂环境——这是一个重大挑战，因为收集此类数据既昂贵又耗力。

**社区讨论**: 该倡议引发了关于利用印度零工经济进行人工智能数据收集公平性的讨论，人们担心工人是否获得足够的报酬，以及是否充分了解他们收集的数据将如何使用。一些观察者认为这可能是一种剥削模式，而其他人则认为这是在科技工作机会有限的地区提供就业机会的合法方式。

**标签**: `#physical-ai`, `#robotics`, `#data-collection`, `#india-tech`, `#startup`

---

<a id="item-17"></a>
## [AI 战争已经到来](https://www.theverge.com/ai-artificial-intelligence/937028/military-ai-warfare-red-lines) ⭐️ 7.0/10

《特定常规武器公约》（CCW）是联合国在日内瓦每年举行两次的会议，专注于致命性自主武器系统。当与会者布兰卡·马里扬（Branka Marijan）观察 2017 年 11 月的会议时，主要是在处理关于杀手机器人世界的假设性问题，而非解决已经在使用的武器问题。

rss · The Verge AI · May 26, 12:00

**背景**: 《特定常规武器公约》（CCW）是一个国际论坛，成立目的是限制或禁止被认为造成不必要痛苦或具有无区别效果的特定类型武器。自 2017 年以来，它一直在专门协商关于致命性自主武器系统的问题，通常被称为"杀手机器人"。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Convention_on_Certain_Conventional_Weapons">Convention on Certain Conventional Weapons - Wikipedia</a></li>
<li><a href="https://www.armscontrol.org/factsheets/CCW">Convention on Certain Conventional Weapons ( CCW ) At a Glance</a></li>

</ul>
</details>

**标签**: `#AI warfare`, `#autonomous weapons`, `#military AI`, `#lethal autonomous robots`, `#international law`

---

<a id="item-18"></a>
## [优步总裁质疑 AI 投资回报：年度预算四个月耗尽](https://www.theverge.com/transportation/937116/uber-ai-investment-hard-to-justify) ⭐️ 7.0/10

优步总裁安德鲁·麦克唐纳表示，公司在 2026 年仅用四个月就烧完了全年 AI 预算，但至今未看到 AI 投资的实质性回报，开始质疑 token 消耗量增加是否真的能转化为业务价值。 这是企业 AI 支出大辩论中的一个重要数据点。作为全球最大的科技公司之一，优步公开质疑 AI 投资回报，其立场可能影响企业如何评估 AI 投资，并促使各行业对 AI 价值主张进行更严格的评估。 优步主要使用 Anthropic 的 Claude Code 作为其 AI 解决方案。Token 消耗是指语言模型在交互过程中处理的输入和输出 token——这是 LLM 部署中计费的主要依据，也是衡量计算成本的关键指标。

rss · The Verge AI · May 26, 09:55

**背景**: Token 消耗是大型语言模型（LLM）性能和计费的基本单位。当用户与 Claude 或 GPT 等 AI 系统交互时，每个单词、部分单词、空格和标点符号都会计入 token 数量，直接决定计算成本。随着企业在内部运营中扩大 AI 的采用，token 消耗——因此支出的费用——可能会大幅增长，而生产率或收入却没有相应的明确提升。随着更多企业报告难以量化 AI 的实际业务影响，关于 AI 支出是否带来相应价值的争论愈演愈烈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jumpcloud.com/it-index/what-is-token-consumption-in-llms">What Is Token Consumption in LLMs? - JumpCloud</a></li>
<li><a href="https://blogs.nvidia.com/blog/ai-tokens-explained/">What Are AI Tokens ? The Language and Currency... | NVIDIA Blog</a></li>

</ul>
</details>

**标签**: `#AI business ROI`, `#corporate AI spending`, `#tech industry trends`, `#Anthropic Claude`, `#enterprise AI adoption`

---

<a id="item-19"></a>
## [调查：85%的企业希望采用智能体 AI，但 76%缺乏基础设施](https://www.technologyreview.com/2026/05/26/1137584/rethinking-organizational-design-in-the-age-of-agentic-ai/) ⭐️ 7.0/10

这一发现揭示了一个关键的企业 AI 采用差距，可能会显著延缓数字化转型计划。那些拥有雄心勃勃的 AI 战略但基础设施不足的企业，可能在成功跨越这一执行鸿沟的竞争对手面前落后。 调查显示，准备不足跨越三个维度：人员缺乏 AI 技能、流程未针对智能体工作流设计、以及传统基础设施无法支持自主 AI 智能体。这是一个具体的组织设计挑战，而非技术问题。

rss · MIT Technology Review · May 26, 14:54

**背景**: 智能体 AI 是指能够自主规划和执行多步骤任务、无需持续人工干预的 AI 系统，与传统 AI 助手不同。企业采用这类智能体不仅需要技术投资，还需要从根本上改变组织的 工作流程设计、员工培训和 AI 与人类协作方式。

**标签**: `#enterprise AI`, `#AI agents`, `#digital transformation`, `#organizational design`, `#AI adoption`

---

<a id="item-20"></a>
## [人工智能正在侵蚀入门级职业机会](https://www.technologyreview.com/2026/05/26/1137865/its-time-to-address-the-looming-crisis-in-entry-level-work/) ⭐️ 7.0/10

MIT《技术评论》的分析显示，虽然人工智能尚未在总体层面导致大规模失业，但它可能正在悄然消除传统的职业晋升培训岗位——入门级职位。 这一点很重要，因为入门级工作历来是新员工积累经验攀登职业阶梯的途径。它们的消失可能在劳动力市场中造成结构性空白，使未来一代失去前几代工人曾经拥有的机会。 分析指出，发达国家的总体就业保持稳定，最近的评估也未发现人工智能改变了总体数据的明显证据，因此这是一场隐蔽而非显而易见的危机。

rss · MIT Technology Review · May 26, 09:00

**背景**: 入门级职位历来是许多职业的第一步，提供在职培训和发展专业技能的机会。正是在这些岗位上，工人们在学习实践中积累了各行业相关知识，然后才晋升到更高级的职位。人们担心的是，人工智能自动化消除这些入门级角色的速度可能比新工人找到进入劳动力的替代途径更快。

**标签**: `#AI and employment`, `#labor market trends`, `#entry-level jobs`, `#automation economics`, `#career development`

---

<a id="item-21"></a>
## [Stability AI 发布 Stable Audio 3 音频生成模型](https://www.marktechpost.com/2026/05/26/stability-ai-releases-stable-audio-3-a-family-of-fast-latent-diffusion-models-for-audio-generation-and-editing/) ⭐️ 7.0/10

这一发布的重要性在于，SA3 Medium 在 BBC 音效基准测试的 5 秒片段上取得了 0.369 的 FAD 分数，击败了论文中评估的所有开源权重基线。这表明高质量音频生成现在可以在普通消费级硬件上运行。 该模型采用三阶段训练流程：流匹配、蒸馏预热和对抗后训练。FAD（弗里切特音频距离）用于衡量生成音频与真实音频分布之间的距离——分数越低表示输出越逼真。

rss · MarkTechPost · May 26, 22:31

**背景**: 潜空间扩散模型在压缩的潜空间而非原始音频空间中运行，从而实现更快的生成和更高的计算效率。BBC 音效基准测试是音频生成模型的标准评估数据集。FAD 是一个广泛使用的指标，与人类对音频质量的感知相关。

**标签**: `#AI`, `#audio_generation`, `#latent_diffusion`, `#Stability_AI`, `#machine_learning`

---

<a id="item-22"></a>
## [中国扩大对 DeepSeek、阿里巴巴等私企 AI 人才的出国限制](https://www.bloomberg.com/news/articles/2026-05-26/china-expands-travel-curbs-to-top-ai-talent-at-private-firms) ⭐️ 7.0/10

这些 restriction 明确针对私营企业的研究人员，与此前主要影响国有机构的管控措施有所不同。 Specifically named 的公司包括 DeepSeek 和阿里巴巴。 这一政策严重影响中国领先私营科技公司顶尖 AI 人才的国际出行能力，可能影响竞争激烈的 AI 领域的协作、知识交流和人才招聘。 这些限制明确针对私营企业的研究人员，与此前主要影响国有机构的管控措施有所不同。被点名的公司包括 DeepSeek 和阿里巴巴。

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · May 26, 15:30

**背景**: 近年来，中国逐步加强对技术人才流动的管控，旨在防止尖端 AI 研究成果泄露。旅行限制是更广泛政策框架的一部分，其中还包括对半导体和软件的出口管制，反映出中国与其他国家在人工智能领域日益增长的战略竞争。

**标签**: `#AI政策`, `#中国科技`, `#人才流动`, `#国际关系`, `#AI产业`

---

<a id="item-23"></a>
## [AWS MCP 服务器正式可用，全面适配 API 并支持 IAM 权限控制](https://www.infoq.cn/article/4gwXqyRPs4RTUIMpRte7?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

此次发布代表了云 AI 集成的重要进展，通过 IAM 权限控制提供了企业级安全保障。企业现在可以构建安全可控的 AI 助手，在适当的访问管理下利用 AWS 云资源。 AWS MCP 服务器直接与 AWS API 集成，并对所有工具交互执行 IAM 策略，确保 AI 助手在与传统 AWS 服务相同的安全边界内运行。这使得可以对 AI 应用程序可以访问的云资源进行细粒度的访问控制。

rss · InfoQ 中文站 · May 26, 10:56

**背景**: MCP（模型上下文协议）是一种新兴的协议，旨在将 AI 助手与外部工具、数据源和服务连接起来。与传统的 API 集成不同，MCP 为 AI 模型提供了与各种工具交互同时保持上下文的标准化方式。AWS IAM 是亚马逊的身份与访问管理服务，可以对 AWS 资源进行细粒度的权限控制。

**标签**: `#AWS`, `#MCP`, `#Model Context Protocol`, `#IAM`, `#云计算`

---

<a id="item-24"></a>
## [Ray 算力调度在小红书 AI 数据生产中的实践](https://www.infoq.cn/article/YHD4cguvebWJled2FK96?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

AICon 上海的一场演讲详细介绍了小红书如何在 AI 模型的整个生命周期中使用 Ray 进行算力调度，从模型诞生到上线部署。 演讲重点关注 Ray 在 AI 数据生产的分布式系统中实现高效算力资源分配的作用，涵盖数据处理、模型训练和推理服务等方面。

rss · InfoQ 中文站 · May 26, 10:00

**背景**: Ray 是一个开源的统一分布式计算框架，最初于 2016 年在加州大学伯克利分校 RISELab 开发，专门为扩展 Python 应用程序的 AI 和 ML 工作负载而设计。小红书是中国最大的社交电商平台之一，拥有数亿用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Ray_distributed_computing_framework">Ray (distributed computing framework)</a></li>

</ul>
</details>

**标签**: `#Ray`, `#ML Infrastructure`, `#Compute Scheduling`, `#Production ML`, `#Distributed Systems`

---

<a id="item-25"></a>
## [中国审查 Meta 收购 AI 初创公司 Manus，联合创始人被限制离境](https://t.me/zaihuapd/41577) ⭐️ 7.0/10

国家发展和改革委员会是中国最高经济规划机构，也负责监督外国投资法规。中国一直在加强对敏感技术领域（特别是人工智能）跨境投资的审查。Manus 因开发能够自主完成复杂多步骤任务的 AI 智能体而受到关注。

telegram · zaihuapd · May 26, 09:56

**背景**: The National Development and Reform Commission (NDRC) is China's top economic planning agency that also oversees foreign investment regulations. China has been increasingly scrutinizing cross-border investments in sensitive technology sectors, particularly artificial intelligence. Manus gained attention for developing an AI agent that can complete complex multi-step tasks autonomously.

**标签**: `#China tech regulation`, `#Meta acquisition`, `#AI startup`, `#cross-border investment`, `#US-China tech tensions`

---