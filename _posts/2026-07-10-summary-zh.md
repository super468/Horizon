---
layout: default
title: "Horizon Summary: 2026-07-10 (ZH)"
date: 2026-07-10
lang: zh
---

> From 219 items, 32 important content pieces were selected

---

1. [Dify 1.16.0-rc1 推出实验性 Linux 沙箱 Agent](#item-1) ⭐️ 8.0/10
2. [欧盟议会通过 Chat Control 1.0 法案](#item-2) ⭐️ 8.0/10
3. [OpenAI 发布 GPT-5.6，刷新 ARC-AGI-3 基准测试纪录](#item-3) ⭐️ 8.0/10
4. [Anthropic 的 J-Lens 揭示 Claude 模型中的隐藏"J 空间"](#item-4) ⭐️ 8.0/10
5. [《纽约时报》报道称 OpenAI 涉嫌伪造无法搜索训练数据](#item-5) ⭐️ 8.0/10
6. [蚂蚁灵波开源 LingBot-Video，全球首个 MoE 具身视频基模](#item-6) ⭐️ 8.0/10
7. [Colibrì：在 32GB 内存电脑上运行 7440 亿参数 GLM 5.2](#item-7) ⭐️ 7.0/10
8. [Mitchell Hashimoto 访谈：谈 Ghostty 终端与 Zig 语言选择](#item-8) ⭐️ 7.0/10
9. [Postgres 用 Rust 重写通过 100% 回归测试](#item-9) ⭐️ 7.0/10
10. [2026 年 12 月不引入闰秒](#item-10) ⭐️ 7.0/10
11. [The glass backbone: Why the Army's logistics will break in the next war](#item-11) ⭐️ 7.0/10
12. [A road to Lisp: Why Lisp](#item-12) ⭐️ 7.0/10
13. [Meta 发布 Muse Spark 1.1 首款付费 AI 智能体模型](#item-13) ⭐️ 7.0/10
14. [内部服务 TLS 证书最佳实践](#item-14) ⭐️ 7.0/10
15. [GLM 5.2 在增值税记账基准测试中达到接近人类准确率](#item-15) ⭐️ 7.0/10
16. [AI 内容泛滥 LinkedIn 和社交媒体](#item-16) ⭐️ 7.0/10
17. [ChatGPT Work](#item-17) ⭐️ 7.0/10
18. [微软 Aurora 1.5 扩展天气基础模型](#item-18) ⭐️ 7.0/10
19. [MCP 工具设计：实用方法与权衡](#item-19) ⭐️ 7.0/10
20. [A Practical Guide to GPU-Initiated Communication for Molecular Dynamics at Scale](#item-20) ⭐️ 7.0/10
21. [Meta 推出 Muse Spark 1.1 进军 AI 编程市场](#item-21) ⭐️ 7.0/10
22. [Ollama 融资 6500 万美元，用户数近 900 万](#item-22) ⭐️ 7.0/10
23. [OpenAI 关闭 ChatGPT Atlas 浏览器，上线不到一年即停运](#item-23) ⭐️ 7.0/10
24. [OpenAI 获特朗普政府批准发布 GPT-5.6，推出 ChatGPT Work](#item-24) ⭐️ 7.0/10
25. [OpenAI 发布 GPT-5.6 三档模型系列与程序化工具调用功能](#item-25) ⭐️ 7.0/10
26. [NVIDIA 发布压缩混合 MoE 大模型，实现 2.03 倍吞吐量提升](#item-26) ⭐️ 7.0/10
27. [Anthropic 为 Claude 订阅增加按量计费](#item-27) ⭐️ 7.0/10
28. [爱沙尼亚 AI"错误查找器"检测法律文本错误](#item-28) ⭐️ 7.0/10
29. [DeepSeek V4 + SGLang：百万上下文推理优化实战](#item-29) ⭐️ 7.0/10
30. [错误信息：关于 TypeScript 7.0 Go 重写的虚假报道](#item-30) ⭐️ 7.0/10
31. [大疆 EV50 飞越珠峰 8861 米创纪录](#item-31) ⭐️ 7.0/10
32. [国家超算互联网核心节点郑州上线](#item-32) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Dify 1.16.0-rc1 推出实验性 Linux 沙箱 Agent](https://github.com/langgenius/dify/releases/tag/1.16.0-rc1) ⭐️ 8.0/10

Dify 发布了 1.16.0-rc1 版本，推出实验性的 Dify Agent，该 Agent 在 Linux 沙箱中运行，并提供构建器 UI，允许用户使用技能、文件和 Dify 生态系统中的工具集成来创建 Agent。 此版本代表了 Dify 的重要新方向，紧跟新兴的基于 shell 的 LLM Agent 范式。它提供了可视化构建器和工作流集成，可能加速 AI Agent 的开发和采用。 目前所有 Dify Agent 共享同一个沙箱，这意味着一个 Agent 可能会读取或干扰另一个 Agent 的环境和数据。严格的隔离将在未来版本中添加。此版本需要数据库迁移和环境变量更改。

github · QuantumGhost · Jul 9, 14:06

**背景**: Dify 是一个用于构建 LLM 应用的开源平台，结合了可视化工作流构建器、RAG 管道和 Agent 功能。Linux 沙箱环境为 AI Agent 提供隔离执行，允许它们运行代码和命令而不影响主机系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/langgenius/dify">GitHub - langgenius/dify: Production-ready platform for ... GitHub - loong64/dify: Production-ready platform for agentic ... Dify: The Open Source Alternative to OpenAI Assistants What Is Dify? The Open-Source AI App Platform Every Developer ... Dify - AI Wiki</a></li>
<li><a href="https://docs.dify.ai/en/quick-start">30-Minute Quick Start - Dify Docs - docs.dify.ai</a></li>
<li><a href="https://www.firecrawl.dev/blog/ai-agent-sandbox">AI Agent Sandbox: How to Safely Run Autonomous Agents in 2026</a></li>

</ul>
</details>

**标签**: `#AI Agents`, `#LLM`, `#Dify`, `#Open Source`, `#Linux Sandbox`, `#AI Development Tools`

---

<a id="item-2"></a>
## [欧盟议会通过 Chat Control 1.0 法案](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 8.0/10

欧盟议会通过了 Chat Control 1.0，允许美国科技公司在没有搜查令的情况下扫描 Instagram、Discord、Snapchat、Skype、Xbox、Gmail 和 iCloud 等平台上的私人信息。尽管 314 名欧洲议会议员投票反对（多于 276 名支持的议员），但由于程序规则，否决提案未能获得所需的 361 票绝对多数。 绝对多数门槛要求 376 票（总计 751 名议员中的多数）才能否决立法。314 票反对、276 票赞成、17 票弃权、113 票缺席，否决票差 62 票未通过。投票发生在暑假前的最后一天，许多议员已返回各自国家。扫描授权适用于直接消息和电子邮件，而公共社交媒体帖子和云存储已经可以在没有这项法律的情况下被扫描。

hackernews · rapnie · Jul 9, 11:03

**背景**: Chat Control 指的是欧盟的《防止和打击儿童性虐待法规》（CSAR），最初于 2022 年 5 月提出。该立法旨在防止儿童性虐待材料（CSAM），但批评者认为它创建的大规模监控基础设施可能会被扩展到原始目的之外。欧盟议会此前曾在 2024 年 3 月两次拒绝该措施，但执政联盟利用程序规则再次将其提交表决。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://www.patrick-breyer.de/en/posts/chat-control/">Chat Control: The EU's CSAM scanner proposal</a></li>
<li><a href="https://www.techtimes.com/articles/320010/20260709/eu-parliament-passes-chat-control-default-314-meps-couldnt-block-scanning-law.htm">EU Parliament Passes Chat Control by Default: 314 MEPs Couldn't Block Scanning Law</a></li>

</ul>
</details>

**社区讨论**: 评论者批评了议会程序技巧，称其为"被扭曲的民主"，并指出投票被安排在暑假前以减少出席人数。许多人认为这威胁到欧盟的合法性，一位评论者写道"欧盟正在成为极权政府"。其他人注意到讽刺之处——尽管多数人反对该法律，但由于绝对多数要求，它仍然通过了。

**标签**: `#privacy`, `#EU-legislation`, `#surveillance`, `#chat-control`, `#democracy`

---

<a id="item-3"></a>
## [OpenAI 发布 GPT-5.6，刷新 ARC-AGI-3 基准测试纪录](https://openai.com/index/gpt-5-6/) ⭐️ 8.0/10

OpenAI 发布了 GPT-5.6，在 ARC-AGI-3 基准测试中创下 7.8%的新纪录，成为首个在该测试中获胜的前沿模型。此次发布还强调了增强的意图理解和更高的 token 效率。 这代表了 AI 推理能力的一个重要里程碑，因为 ARC-AGI 旨在测试流体智力和新颖的问题解决能力——这些领域一直是 AI 的传统弱项。对 token 效率的关注也反映了业界对成本效益 AI 部署日益增长的重视。 GPT-5.6 可以更好地推断用户的潜在目标和预期工作层级，无需明确指定每一步骤。该模型在处理图像时保留原始图像尺寸。然而，ARC-AGI-3 上的 7.8%得分仍有很大的提升空间——100%意味着在每项任务上达到与人类相当的效率。

hackernews · OpenAI News · Jul 9, 17:04

**背景**: ARC-AGI（用于人工通用智能的抽象和推理语料库）是由 François Chollet 设计的基准测试，用于测量流体智力——即解决新颖问题的能力。ARC-AGI-3 是第三个版本，引入了交互式环境，AI 代理必须在其中探索、即时获取目标并构建适应性世界模型。该基准被认为是评估真正通用 AI 推理能力最具挑战性的测试之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arcprize.org/arc-agi/2">ARC-AGI-2</a></li>

</ul>
</details>

**社区讨论**: 社区反馈显示出复杂的情绪。许多人对 ARC-AGI-3 的成就和对 token 效率的关注表示赞赏，一位用户指出欣赏"兼顾智能与 token 效率"的做法，并希望看到"每 token 最智能"指标成为行业趋势。另一些人批评了基准测试的选择做法，指出 Fable 5 被排除在比较之外，因为它"拒绝回答大部分问题"。一些用户还就 Codex 与 Claude Code 等不同编码助手的优劣展开了辩论。

**标签**: `#openai`, `#gpt-5`, `#llm`, `#artificial-intelligence`, `#machine-learning`

---

<a id="item-4"></a>
## [Anthropic 的 J-Lens 揭示 Claude 模型中的隐藏"J 空间"](https://www.technologyreview.com/2026/07/09/1140293/anthropic-found-a-hidden-space-where-claude-puzzles-over-concepts/) ⭐️ 8.0/10

这一突破解决了关于大型语言模型如何在内部处理概念的关键问题，为 AI 安全研究人员提供了前所未有的模型认知洞察力，超越了仅关注行为的评估方法——后者会忽略模型静默的内部状态。 J-Lens 不会向 Claude API 客户开放。Anthropic 使用这一工具验证了"反事实反思训练"——即基于如果 Claude 被中断并被要求反思时会说什么进行训练，而非基于任务行为本身进行训练。

rss · MIT Technology Review · Jul 9, 20:22

**背景**: 可解释性研究旨在通过检查神经网络的内部表征来理解其决策过程。雅可比矩阵是一个数学概念，描述输入变化如何影响输出，提供了一个追踪概念如何流经模型各层的透镜。这对 AI 安全至关重要，因为理解模型认知有助于在部署前识别潜在风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://explainx.ai/blog/what-is-j-lens-jacobian-lens-claude-interpretability-2026">What Is the J-Lens? Anthropic Jacobian Lens Guide</a></li>
<li><a href="https://venturebeat.com/technology/anthropics-new-j-lens-reveals-a-silent-workspace-inside-claude-that-mirrors-a-leading-theory-of-consciousness">Anthropic's new "J-lens" reveals a silent workspace inside Claude that mirrors a leading theory of consciousness | VentureBeat</a></li>
<li><a href="https://the-decoder.com/claudes-hidden-inner-monologue-is-now-readable-thanks-to-anthropics-new-jacobian-lens/">Claude's hidden inner monologue is now readable thanks to Anthropic's new Jacobian Lens</a></li>

</ul>
</details>

**标签**: `#AI interpretability`, `#Anthropic`, `#Claude`, `#LLM research`, `#AI safety`, `#machine learning`

---

<a id="item-5"></a>
## [《纽约时报》报道称 OpenAI 涉嫌伪造无法搜索训练数据](https://arstechnica.com/tech-policy/2026/07/openai-faked-inability-to-search-training-data-hid-billions-of-logs-nyt-says/) ⭐️ 8.0/10

《纽约时报》报道称，OpenAI 涉嫌伪造其无法搜索训练数据的能力，并隐藏了数十亿条日志，这在 AI 行业引发了严重的透明度和问责制担忧。 这一指控直指 AI 行业问责的核心，因为训练数据透明度对于版权合规、隐私保护和公众对 AI 系统的信任至关重要。如果指控属实，可能会引发监管审查并重塑 AI 公司处理数据治理的方式。 据称被隐藏的内容包括数十亿条系统日志，这些日志可能揭示用于训练 AI 模型的数据。学术研究已记录了训练数据提取攻击作为一种真实的安全威胁，攻击者可以从模型输出中恢复敏感信息。

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Jul 9, 19:01

**背景**: 训练数据提取攻击是机器学习中一个被充分记录的安全问题，攻击者可以通过探测 AI 模型来恢复记忆的训练数据。这种漏洞源于模型偶尔会过度拟合训练数据。AI 行业在数据来源实践方面面临越来越多的审查，多起诉讼涉及用于训练的受版权保护材料。《纽约时报》的报道加剧了人们对 AI 领域透明度日益增长的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nightfall.ai/ai-security-101/training-data-extraction-attacks">Training Data Extraction Attacks: The Essential Guide ...</a></li>
<li><a href="https://arxiv.org/abs/2012.07805">Extracting Training Data from Large Language Models Extracting Training Data from Large Language Models Data Extraction | RAND Model Inversion Attacks: Risks and Defenses Explained Model Theft and Extraction in 2026: Risks and Defense What is Training Data Extraction (AI)? - blogs.jsmon.sh</a></li>
<li><a href="https://privacy.openai.com/">OpenAI Privacy Center</a></li>

</ul>
</details>

**社区讨论**: 讨论有限，因为 Hacker News 帖子仅包含 5 条评论。没有实质性社区反馈的情况下，关于这一指控的整体情绪和更广泛观点尚不清楚。

**标签**: `#OpenAI`, `#AI regulation`, `#tech policy`, `#transparency`, `#machine learning`

---

<a id="item-6"></a>
## [蚂蚁灵波开源 LingBot-Video，全球首个 MoE 具身视频基模](https://www.qbitai.com/2026/07/446458.html) ⭐️ 8.0/10

蚂蚁灵波开源了全球首个基于 MoE 架构的具身智能视频生成基础模型 LingBot-Video。该模型总参数 30B，生成时仅激活约 3B，推理效率约为同等规模 Dense 架构的 3 倍。 这代表了具身智能视频生成领域的重大突破，将大模型容量与计算效率相结合。在面向机器人操作视频的评测基准 RBench 上，LingBot-Video 总分 0.620，超越 Wan2.6、Seedance1.5 Pro 和 Cosmos3 Super，显示出在机器人研究和应用方面的强大潜力。 该模型从架构（采用 DiT+MoE 设计平衡容量与成本）、数据（构建包含 7 万小时具身数据的画像引擎，覆盖灵巧操作、机器人移动和第一视角交互等场景）和训练（引入多维强化学习奖励系统，除美学和运动一致性外，重点关注物理合理性和任务完成度）三方面进行创新。目前已在 GitHub 上以 Apache 2.0 许可证开源。

telegram · zaihuapd · Jul 9, 04:30

**背景**: MoE（混合专家模型）是一种机器学习技术，通过门控模型将单一任务空间划分为多个子任务，由多个专家网络分别处理特定的子任务。具身智能是人工智能与机器人学交叉的前沿领域，强调智能体通过身体与环境的动态交互实现自主学习和进化。DiT（扩散 Transformer）结合了扩散模型和 Transformer 架构，用于生成高质量的图像和视频内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/混合专家模型">混合专家模型 - 维基百科，自由的百科全书</a></li>
<li><a href="https://baike.baidu.com/item/具身智能/63286570">具身智能</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/714593709">一文搞懂DiT （Diffusion Transformer） - 知乎</a></li>

</ul>
</details>

**标签**: `#MoE`, `#具身智能`, `#视频生成`, `#机器人`, `#开源模型`

---

<a id="item-7"></a>
## [Colibrì：在 32GB 内存电脑上运行 7440 亿参数 GLM 5.2](https://github.com/JustVugg/colibri) ⭐️ 7.0/10

开发者创建了 Colibrì项目，通过 int4 量化技术，在一台只有 32GB 内存的普通笔记本电脑上成功运行了 7440 亿参数的 GLM 5.2 大模型，按需从磁盘流式传输 21504 个 MoE 专家模块，引擎为单个约 1300 行的 C 文件。 这证明了庞大的混合专家模型可以在没有 GPU 的消费级硬件上运行，可能让没有昂贵设备的用户也能使用前沿的大语言模型。 密集部分（约 170 亿参数）以 int4 格式驻留在内存中（约 9.9GB），而 21504 个路由专家（约 370GB）存储在磁盘上，通过每层 LRU 缓存按需流式传输。性能达到约 0.1token/秒。

hackernews · vforno · Jul 9, 08:05

**背景**: GLM 5.2 是智谱 AI（现 Z.AI）发布的 7440 亿参数混合专家模型，被评为最强大的开源大语言模型之一。混合专家模型每 token 只激活部分参数——本例中 7440 亿参数中只激活约 400 亿。MTP（多 token 预测）是一种预测多个未来 token 以加速推理的架构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.cloudflare.com/workers-ai/models/glm-5.2/">glm-5.2 (Zhipu AI) · Cloudflare AI docs · Cloudflare Workers AI docs</a></li>
<li><a href="https://www.trendingtopics.eu/glm-5-2-chinas-zhipu-ai-beats-even-googles-top-models-with-its-new-open-llm/">GLM-5.2: China's Zhipu AI Beats Even Google's Top Models With Its New Open LLM</a></li>
<li><a href="https://www.spheron.network/blog/multi-token-prediction-mtp-gpu-cloud-deployment-guide/">Multi-Token Prediction on GPU Cloud: Deploy MTP LLMs for 2-3x Faster Inference (2026) | Spheron Blog</a></li>

</ul>
</details>

**社区讨论**: 评论对实用性表达了热情和怀疑——一些人质疑 0.1token/秒是否可用（指出 1token/秒通宵运行也有用），而其他人分享了针对苹果芯片或高端硬件（96GB 内存+RTX 5090，期望 5token/秒）的类似项目。

**标签**: `#llm`, `#local-llm`, `#glm`, `#model-quantization`, `#hardware-optimization`

---

<a id="item-8"></a>
## [Mitchell Hashimoto 访谈：谈 Ghostty 终端与 Zig 语言选择](https://alexalejandre.com/programming/interview-with-mitchell-hashimoto/) ⭐️ 7.0/10

一次访谈中，HashiCorp 创始人 Mitchell Hashimoto 透露了他选择使用 Zig 而非 Rust 构建 Ghostty 终端模拟器的原因，探讨了他的实用主义开发理念和语言选择考量。 这次访谈之所以重要，是因为 Hashimoto 是开发者工具领域的知名人物（Terraform、Vault 的创造者），他选择 Zig 表明业界对 Rust 之外的系统编程语言越来越感兴趣，引发了关于语言文化和实用主义开发的讨论。 Ghostty 是一款快速、功能丰富、跨平台的终端模拟器，采用平台原生 UI 和 GPU 加速技术。Zig 是一种系统编程语言，旨在作为 C 语言的通用改进版本，由 Andrew Kelley 于 2016 年创建，需要手动内存管理。

hackernews · veqq · Jul 9, 17:17

**背景**: Mitchell Hashimoto 是 HashiCorp 的创始人，该公司开发了 Terraform、Vault 和 Consul 等热门基础设施工具。Ghostty 是他的新终端模拟器项目。访谈探讨了他为何选择 Zig 而非 Rust 等更成熟的语言，包括对语言文化和开发理念的实际考量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ghostty.org/">Ghostty</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://ziglang.org/">Home ⚡ Zig Programming Language</a></li>

</ul>
</details>

**社区讨论**: 评论显示了对 Rust 与 Zig 文化的不同看法——一些人赞赏 Hashimoto 的实用主义和深入思考，而另一些人批评两个社区的语言争论都很狭隘。一个关键话题是维护分支的负担，人们普遍认为更多被维护的分支将使生态系统受益。

**标签**: `#Ghostty`, `#Zig`, `#Terminal Emulator`, `#Mitchell Hashimoto`, `#Programming Languages`

---

<a id="item-9"></a>
## [Postgres 用 Rust 重写通过 100% 回归测试](https://github.com/malisper/pgrust) ⭐️ 7.0/10

开发者 malisper 使用 LLM 将 Postgres 用 Rust 重建，创建了名为 pgrust 的项目，目前通过了 100% 的 Postgres 回归测试，超过 46000 个回归查询与 Postgres 的预期输出匹配。 这代表了利用 AI 辅助开发进行数据库现代化的雄心勃勃的实验，展示了 LLM 可以帮助转换传统数据库代码库。它提出了关于代码可审查性、测试方法论以及 AI 生成代码时代许可证的重要问题。 pgrust 瞄准与 Postgres 18.3 的兼容性，包含约 25 万行 Rust 代码，与 Postgres 磁盘兼容，可以从现有的 Postgres 18.3 数据目录启动。该项目在不到一个月内使用 LLM 辅助生成了 7101 个提交。

hackernews · SweetSoftPillow · Jul 9, 06:18

**背景**: PostgreSQL 是一个有 30 年历史的关系型数据库，以其可靠性和可扩展性著称。回归测试是验证数据库功能在更改后保持正确的标准化测试套件。用 Rust 这样的内存安全语言重写像 Postgres 这样的成熟数据库是一项重大工程，理论上可以提高性能和安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/malisper/pgrust">GitHub - malisper/pgrust: Postgres rewritten in Rust, now ...</a></li>
<li><a href="https://malisper.me/pgrust-rebuilding-postgres-in-rust-with-ai/">pgrust: Rebuilding Postgres in Rust with AI - malisper.me</a></li>

</ul>
</details>

**社区讨论**: 评论强调了几个关键问题：审阅者难以在一个月内审核 7101 个 LLM 生成的提交；一些人建议使用查询代理在生产负载下比较 Rust 版本和传统 Postgres 的输出；其他人担心许可证从 PostgreSQL 许可证改为 AGPL，以及原始许可证是否仍应适用于重写的代码。

**标签**: `#postgres`, `#rust`, `#llms`, `#databases`, `#rewrites`

---

<a id="item-10"></a>
## [2026 年 12 月不引入闰秒](https://datacenter.iers.org/data/latestVersion/bulletinC.txt) ⭐️ 7.0/10

国际地球自转和参考系统服务(IERS)宣布 2026 年 12 月底不会引入闰秒，这意味着 UTC-TAI 偏移量将保持在-37 秒。 这一公告影响了全球的时间计量系统，特别是那些依赖精确 UTC-GPS 和 UTC-TAI 偏移量计算的卫星导航、电信和金融交易系统。处于维护模式的系统需要这个提前通知来进行精确的时间计算。 TAI（国际原子时）和 GPS 相互之间保持恒定的 19 秒偏移量，因此如果 UTC-TAI 保持在-37 秒，那么 UTC-GPS 偏移量也保持在-18 秒。IERS 公告 C 提前发布这一通知，以便时间系统运营商做好准备。

hackernews · ChrisArchitect · Jul 9, 14:16

**背景**: 闰秒被添加到协调世界时（UTC）中当地球自转（通过 UT1 测量）与国际原子时（TAI）不同步时。IERS 负责监测地球自转并宣布插入闰秒。TAI 是一种基于原子钟的极高精度时间标准，大约每 1 亿年才会丢失一秒，而地球自转受到各种不可预测因素的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/International_Atomic_Time">International Atomic Time - Wikipedia</a></li>
<li><a href="https://www.iers.org/">IERS - International Earth Rotation and Reference Systems Service</a></li>
<li><a href="https://en.wikipedia.org/wiki/International_Earth_Rotation_and_Reference_Systems_Service">International Earth Rotation and Reference Systems Service</a></li>

</ul>
</details>

**社区讨论**: 社区成员讨论了由地质活动、天气和其他因素引起的地球自转不可预测性。有些人还开着关于在赤道安装喷气发动机的玩笑。用户还讨论了对 UNIX 时间戳和遗留系统的影响，其中一人解释了 TAI-GPS 偏移关系：由于 UTC-TAI 保持在-37 秒，UTC-GPS 也保持在-18 秒，而 TAI 和 GPS 之间存在恒定的 19 秒差值。

**标签**: `#timekeeping`, `#leap-seconds`, `#iers`, `#utc`, `#systems`

---

<a id="item-11"></a>
## [The glass backbone: Why the Army's logistics will break in the next war](https://mwi.westpoint.edu/the-glass-backbone-why-the-armys-logistics-will-break-in-the-next-war/) ⭐️ 7.0/10

An analysis of U.S. Army logistics vulnerabilities in future conflicts, highlighting the gap between professional acknowledgment of logistics importance and actual budget prioritization.

hackernews · baud147258 · Jul 9, 13:24

**标签**: `#military`, `#logistics`, `#defense`, `#strategic-analysis`, `#infrastructure`

---

<a id="item-12"></a>
## [A road to Lisp: Why Lisp](https://scotto.me/blog/2026-07-09-why-lisp/) ⭐️ 7.0/10

A blog post advocating for Lisp with an active Hacker News discussion featuring both supporters and skeptics debating Lisp's merits, practical drawbacks, and the nature of language advocacy.

hackernews · silcoon · Jul 9, 13:06

**标签**: `#lisp`, `#programming-languages`, `#hacker-news`, `#language-philosophy`, `#programming-advocacy`

---

<a id="item-13"></a>
## [Meta 发布 Muse Spark 1.1 首款付费 AI 智能体模型](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 7.0/10

Meta 发布了 Muse Spark 1.1，这是他们首款可通过 API 访问的商业 AI 智能体模型，标志着其从开源权重研究模型向付费商业产品的转变，定价为每百万 token 1.25/4.5 美元。 这代表 Meta 首款付费 AI 产品，预示着其向商业化盈利的战略转变，同时通过开源权重模型将编程助手可能商品化，直接挑战 OpenAI 和 Anthropic 等竞争对手。 该模型使用 Terminal-Bench 2.1 进行评估，资源限制为 6 个 CPU 核心和 8GB 内存，但一些评论者指出这违反了基准测试的官方规则，因为超出 CPU 或内存限制构成违规。缓存输入 token 的定价为 0.15 美元。

hackernews · ot · Jul 9, 14:10

**背景**: AI 智能体是具有目标导向行为、使用外部工具并自主执行多步骤任务的 AI 系统。开源权重模型公开分享训练好的模型参数，允许开发者在本地运行和自定义 AI 模型。Meta 此前已发布 Llama 等开源权重模型，通过免费提供强大模型来颠覆 AI 市场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is Agentic AI? | IBM</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**社区讨论**: 评论者对 Terminal-Bench 评估方法提出担忧，有人指出资源限制根据官方规则会使结果失效。另一些人则称赞其具有竞争力的价格和实用性能，其中一人展示了可用的 SVG 生成示例。战略分析认为 Meta 可以通过开源权重将编程模型商品化，发挥"搅局者"的作用。

**标签**: `#meta-ai`, `#ai-models`, `#api-services`, `#open-weights`, `#ai-business-strategy`

---

<a id="item-14"></a>
## [内部服务 TLS 证书最佳实践](https://tuxnet.dev/posts/tls-for-internal-services/) ⭐️ 7.0/10

这很重要，因为不当的 TLS 证书管理是一个常见的运维痛点，可能导致服务中断、安全漏洞，并给 DevOps 团队带来大量的管理负担。 讨论中的关键建议包括：对内部服务使用 DNS-01 挑战而非 HTTP-01，利用 Let's Encrypt 的通配符证书以避免名称泄露到证书透明度日志，并使用集中式反向代理进行 TLS 终止。

hackernews · mrl5 · Jul 9, 14:57

**背景**: 分裂视界 DNS 是一种根据查询来源（网络内部或外部）提供不同 DNS 响应的技术。DNS-01 是 Let's Encrypt 的一种验证类型，通过在 DNS 中放置特定的 TXT 记录来验证域名所有权。ACME（自动证书管理环境）是 Let's Encrypt 用于自动化证书颁发和更新的协议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://letsencrypt.org/docs/challenge-types/">Challenge Types - Let's Encrypt The Significance of Proper DNS Configuration for SSL/TLS DNS CNAME Validation for SSL Certificates - Mister PKI TXT method — Domain Control Validation — SSL/TLS · Cloudflare ... Pre-Validated DNS: Eliminate Certificate Delays from ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Split-horizon_DNS">Split-horizon DNS</a></li>

</ul>
</details>

**社区讨论**: The community shows strong preference for DNS-01 validation over split-horizon DNS, with EvanAnderson calling split-horizon DNS 'tedious make-work'. Others emphasize avoiding internal CAs entirely and using Let's Encrypt, while boscillator criticizes the inconsistent way different programming languages handle certificate trust stores.

**标签**: `#tls`, `#certificates`, `#devops`, `#security`, `#networking`

---

<a id="item-15"></a>
## [GLM 5.2 在增值税记账基准测试中达到接近人类准确率](https://toot-books.pages.dev/blog/glm-5-2-vat-benchmark) ⭐️ 7.0/10

这代表了大语言模型在专业财务任务应用方面的重大进步，有望实现复杂记账工作流程的自动化。然而，讨论揭示了 AI 造成税务错误时的法律责任以及基准测试背后公司透明度方面的关键担忧。 基准测试显示，人类执行的任务比模型更广泛，包括查找相关发票以及推理银行流水和发票/收据无法推断的情况——这些以"用户备注"的形式提供给模型。批评者还指出，Vineyard Finance LTD 公司是去年成立的，没有公开可识别的创始人。

hackernews · adamkurkiewicz · Jul 9, 18:29

**背景**: 增值税（VAT）是一种在生产和分销每个阶段征收的间接税，需要准确记录进项税和销项税以确保合规。记账涉及记录财务交易、分类费用并确保正确计算税务义务。GLM-5.2 是智谱 AI 于 2026 年 6 月发布的旗舰模型，具有 100 万 token 的上下文窗口，在多个基准测试中排名顶尖开源模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://z.ai/blog/glm-5.2">GLM-5.2: Built for Long-Horizon Tasks - z.ai</a></li>
<li><a href="https://github.com/zai-org/GLM-5">GitHub - zai-org/GLM-5: GLM-5: From Vibe Coding to Agentic ...</a></li>
<li><a href="https://auditingaccounting.com/accounting-for-value-added-tax-vat">Accounting for Value Added Tax (VAT) – Auditing Accounting</a></li>

</ul>
</details>

**社区讨论**: 评论强调了几个重要的方法论问题：基准测试中的人类需要查找发票并推理复杂情况，而模型收到的是预先处理好的用户备注。讨论者强调了一个严重的法律责任问题——如果 AI 税务欺诈，谁去坐牢？他们还警告了关于这家未知公司（Vineyard Finance LTD，去年成立，没有 LinkedIn 信息）的担忧，敦促在委托敏感财务数据之前保持谨慎。

**标签**: `#LLM`, `#AI benchmark`, `#accounting`, `#VAT`, `#machine learning`

---

<a id="item-16"></a>
## [AI 内容泛滥 LinkedIn 和社交媒体](https://www.pangram.com/blog/ai-in-your-feed) ⭐️ 7.0/10

一篇博客文章观察到 AI 生成内容在 LinkedIn 和社交媒体平台上已经无处不在，引发了关于真实性和内容质量的重大讨论。 这很重要，因为它反映了在线内容创作的文化转变，挑战了传统个人风格和真实性的概念，同时推动用户寻找算法驱动平台的替代方案。 HackerNews 的讨论吸引了 188 个赞同和 165 条评论，用户讨论了 AI 对写作风格的影响，并探索 RSS 提要作为算法策展社交动态的替代方案。

hackernews · mukmuk · Jul 9, 15:50

**背景**: 像 GPT-4 这样的大型语言模型使 AI 内容生成变得极其容易，任何人都可以用最少的努力制作出精美的帖子。LinkedIn 作为最初的专业社交平台，已成为 AI 生成内容的热点，一些用户认为这破坏了真实的个人表达。与此同时，RSS 提要——曾经是消费网页内容的主流方式——随着用户对算法策展和参与度驱动的平台越来越不满，兴趣再度升温。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thenewleafjournal.com/leafbud/rss-as-a-social-media-alternative/">RSS as a social media alternative · The New Leaf Journal</a></li>
<li><a href="https://hivemoderation.com/ai-generated-content-detection">AI-Generated Content Detection | Hive</a></li>
<li><a href="https://toolradar.com/guides/best-ai-content-detection-tools">Best AI Content Detection Tools 2026 | Tested | Toolradar</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了不同的观点——一些人力主反对 AI 写作，认为它侵蚀了个人风格，而另一些人则指出 LinkedIn 长期以来一直充斥着脚本化的不真实内容。几位用户强调 RSS 提要是一个更干净的选择，尽管他们承认失去了发现新内容的便利。一些人还对 Reddit 和其他平台上机器人的泛滥表示担忧。

**标签**: `#AI-content`, `#social-media`, `#LinkedIn`, `#digital-authenticity`, `#technology-culture`

---

<a id="item-17"></a>
## [ChatGPT Work](https://openai.com/index/chatgpt-for-your-most-ambitious-work/) ⭐️ 7.0/10

OpenAI's unification of ChatGPT and Codex into 'ChatGPT Work' is drawing heavy user criticism on HackerNews for confusing UI changes and removing casual chat functionality.

hackernews · OpenAI News · Jul 9, 17:03

**标签**: `#OpenAI`, `#Product-Launch`, `#AI-Assistant`, `#User-Feedback`, `#Product-Strategy`

---

<a id="item-18"></a>
## [微软 Aurora 1.5 扩展天气基础模型](https://www.microsoft.com/en-us/research/blog/aurora-1-5-extending-open-foundation-models-for-weather-and-earth-system-applications/) ⭐️ 7.0/10

这一扩展通过提供更全面的大气数据和不确定性估计，使 Aurora 更加适用于实际应用，对能源电网管理、气候适应规划和极端天气预报至关重要。 Aurora 1.5 现在支持小时级分辨率预报，并包含概率集合预报，提供多个具有相关概率的预报情景，而不仅仅是单一的确定性预测，从而实现更好的风险评估。

rss · Microsoft Research · Jul 9, 16:46

**背景**: 天气预测中的基础模型利用深度学习分析海量历史天气数据并进行预测。传统天气模型依赖基于物理的模拟，而 AI 基础模型直接从数据中学习模式。Aurora 是微软的开源方法，旨在为研究社区带来先进的天气预报能力。美国国家海洋和大气管理局（NOAA）最近已开始运营部署 AI 驱动的全球天气预报模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.noaa.gov/news-release/noaa-deploys-new-generation-of-ai-driven-global-weather-models">NOAA deploys new generation of AI-driven global weather models</a></li>
<li><a href="https://rmets.onlinelibrary.wiley.com/doi/10.1002/wea.70015">Probability forecasts – Part 1: ensembles and probabilistic ...</a></li>

</ul>
</details>

**标签**: `#foundation models`, `#weather prediction`, `#climate AI`, `#Microsoft Research`, `#Earth system modeling`

---

<a id="item-19"></a>
## [MCP 工具设计：实用方法与权衡](https://aws.amazon.com/blogs/machine-learning/mcp-tool-design-practical-approaches-and-tradeoffs/) ⭐️ 7.0/10

AWS 发布了一篇技术博客文章，展示了 Model Context Protocol（MCP）工具设计中的常见错误，并提供了实用的上下文工程方法来修复这些问题。 随着 MCP 成为 AI 系统连接外部工具和数据源的标准，正确的工具设计对于 AI 应用的性能至关重要，这篇博客为开发者提供了解决实际工程问题的指导。 文章重点介绍了上下文工程（context engineering）技术，这是一种超越简单提示工程的系统性方法，用于优化大型语言模型推理时的输入。

rss · AWS Machine Learning Blog · Jul 9, 16:40

**背景**: Model Context Protocol (MCP)是由 Anthropic 于 2024 年 11 月推出的开放标准和开源框架，旨在标准化 AI 系统（如大语言模型）与外部工具、数据源的集成方式。上下文工程是人工智能中的一个系统性学科，专注于设计、组装和优化大语言模型推理时的上下文输入，涵盖结构化指令、工具定义和系统提示等多个方面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://modelcontextprotocol.io/docs/getting-started/intro">What is the Model Context Protocol (MCP)?</a></li>

</ul>
</details>

**标签**: `#Model Context Protocol`, `#AI Tool Design`, `#Machine Learning Engineering`, `#Context Engineering`, `#AWS`

---

<a id="item-20"></a>
## [A Practical Guide to GPU-Initiated Communication for Molecular Dynamics at Scale](https://developer.nvidia.com/blog/a-practical-guide-to-gpu-initiated-communication-for-molecular-dynamics-at-scale/) ⭐️ 7.0/10

A practical guide explaining GPU-initiated communication techniques for optimizing molecular dynamics simulations at scale on NVIDIA GPUs.

rss · NVIDIA Developer Blog · Jul 9, 17:15

**标签**: `#GPU computing`, `#molecular dynamics`, `#HPC`, `#performance optimization`, `#computational science`

---

<a id="item-21"></a>
## [Meta 推出 Muse Spark 1.1 进军 AI 编程市场](https://techcrunch.com/2026/07/09/meta-enters-the-crowded-ai-coding-battle-with-muse-spark-1-1/) ⭐️ 7.0/10

Meta 于 2026 年 7 月 9 日正式推出 Muse Spark 1.1，这是一款多模态 AI 模型，专为代理式编程设计，与 OpenAI 和 Anthropic 的同类产品竞争，面向企业用例如 bug 修复和大型代码迁移。 这代表了 AI 编程助手市场竞争的加剧，该市场目前由 GitHub Copilot、OpenAI 和 Anthropic 主导。企业对代理式工作负载和大规模代码迁移的关注表明市场正在成熟，可能会迫使现有参与者改进他们的产品。 Meta 的人工智能负责人 Alexandr Wang 将定价描述为"非常有竞争力且吸引人"，暗示价格战可能正在酝酿。Spark 为 WhatsApp、Instagram、Facebook、Messenger 和 AI 眼镜上的 Meta AI 助手提供支持。

rss · TechCrunch AI · Jul 9, 19:40

**背景**: AI 编程助手已成为生成式 AI 领域的主要战场。这些工具使用大型语言模型帮助开发者编写、调试和重构代码。代理式 AI 指的是能够自主做出决策、采取行动并协调复杂多步骤工作流程的人工智能系统，只需最少的人工干预，这对于处理大规模自动化任务的企业特别有价值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/09/meta-enters-the-crowded-ai-coding-battle-with-muse-spark-1-1/">Meta enters the crowded AI coding battle with Muse Spark 1 ...</a></li>
<li><a href="https://www.cnbc.com/2026/07/09/meta-jumps-into-ai-coding-market-to-chase-anthropic-and-openai.html">Meta jumps into AI coding market to chase Anthropic and OpenAI</a></li>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/agentic-ai-explained">Agentic AI, explained - MIT Sloan</a></li>

</ul>
</details>

**标签**: `#AI coding assistants`, `#Meta`, `#Enterprise AI`, `#Software development tools`, `#AI competition`

---

<a id="item-22"></a>
## [Ollama 融资 6500 万美元，用户数近 900 万](https://techcrunch.com/2026/07/09/popular-open-source-ai-developer-tool-ollama-raises-65m-grows-to-nearly-9m-users/) ⭐️ 7.0/10

此轮融资表明业界对本地 AI 推理日益增长的商业兴趣，因为开发者越来越追求保护隐私且具成本效益的云端 AI 服务替代方案。庞大的用户群体证明了开发者社区对易于使用的本地 AI 开发工具的需求。 Ollama 提供下载、运行、导入和管理大型语言模型的工具。用户可以通过命令行与模型交互，也可以使用本地 HTTP API 或 Python、JavaScript 等编程语言的客户端库。

rss · TechCrunch AI · Jul 9, 13:00

**背景**: Ollama 是一款开源工具，使开发者能够在个人电脑上本地运行大型语言模型，将数据保留在本地而非发送到云服务。这种方式解决了隐私问题并降低了云基础设施的成本依赖。该工具已成为 GitHub 上最受欢迎的 AI 开发者工具之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/09/popular-open-source-ai-developer-tool-ollama-raises-65m-grows-to-nearly-9m-users/">Popular open source AI developer tool Ollama raises $65M ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ollama">Ollama - Wikipedia</a></li>
<li><a href="https://ollama.com/">Ollama</a></li>

</ul>
</details>

**标签**: `#open source`, `#AI developer tools`, `#funding`, `#Ollama`, `#machine learning`

---

<a id="item-23"></a>
## [OpenAI 关闭 ChatGPT Atlas 浏览器，上线不到一年即停运](https://www.theverge.com/ai-artificial-intelligence/963654/openai-chatgpt-atlas-ai-browser-shut-down-sunset) ⭐️ 7.0/10

OpenAI 正在关闭 ChatGPT Atlas，这是一款可以代表用户执行任务的 AI 浏览器，距离去年 10 月推出还不到一年。公司确认将“关停”Atlas，并计划将 ChatGPT Atlas、ChatGPT 应用和 OpenAI Codex 整合为一个统一的桌面应用程序。 这一关闭表明构建可行的 AI 代理产品面临实际挑战。即使拥有 OpenAI 的巨大资源创建一个能够可靠代表用户执行任务的可持续 AI 浏览器已被证明困难重重，这凸显了 AI 代理雄心与当前技术能力之间的差距。 ChatGPT Atlas 基于 Chromium 开发，仅在 macOS 上可用。它采用免费增值模式，提供付费计划的“代理模式”可在网站上执行任务。该浏览器因对开放网页链接的影响及其内存功能的安全漏洞报告而受到批评。

rss · The Verge AI · Jul 9, 20:34

**背景**: AI 代理是一类智能软件，可以代表用户追求目标、使用工具并以不同程度的自主权采取行动。与被动 AI 助手不同，它们可以通过推理和规划主动完成任务。ChatGPT Atlas 是 OpenAI 打造原生 AI 浏览器的尝试，将 AI 助手功能直接嵌入浏览体验，旨在与传统浏览器竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChatGPT_Atlas">ChatGPT Atlas</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent</a></li>
<li><a href="https://cloud.google.com/discover/what-are-ai-agents">What are AI agents? Definition, examples, and types</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI Agents`, `#Product Shutdown`, `#ChatGPT`, `#AI Industry`

---

<a id="item-24"></a>
## [OpenAI 获特朗普政府批准发布 GPT-5.6，推出 ChatGPT Work](https://www.theverge.com/ai-artificial-intelligence/963464/openai-gpt-5-6-codex-chatgpt-work) ⭐️ 7.0/10

OpenAI 已获得特朗普政府的批准，公开发布 GPT-5.6。此前该模型在“有限预览”期间仅限政府批准的组织使用。首席执行官 Sam Altman 称其为“我们迄今为止最好的模型”，该公司还宣布推出名为“ChatGPT Work”的新企业功能。 此次发布标志着美国 AI 监管的重要时刻，代表着首批通过新政府审批流程的主要 AI 模型之一。公开发布使 GPT-5.6 可供数百万用户使用，而 ChatGPT Work 使 OpenAI 在企业 AI 市场中与微软 Copilot 和谷歌 Gemini 等竞争对手的竞争更具优势。 在有限预览期间，GPT-5.6 仅对政府批准的组织开放了约两周时间。ChatGPT Work 被描述为一个可以跨应用和文件执行操作的代理，可以根据需要持续处理项目数小时，并将目标转化为完成的工作——其功能与其他企业 AI 助手类似。

rss · The Verge AI · Jul 9, 17:00

**背景**: 这一新闻发生在美国政府努力建立前沿 AI 模型监督机制的背景下。根据最近的行政命令，存在一个自愿的“早期访问”框架，AI 开发者可以允许联邦政府提前访问某些受覆盖的 AI 模型，并合作选择“可信合作伙伴”进行早期访问。GPT-5.6 的有限预览期似乎是这一监管流程的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nortonrosefulbright.com/en-us/knowledge/publications/900af3cf/executive-order-establishes-voluntary-early-access-framework-to-frontier-ai-models">EO sets voluntary ‘early access’ framework for AI models</a></li>
<li><a href="https://openai.com/index/chatgpt-for-your-most-ambitious-work/">ChatGPT is now a partner for your most ambitious work</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-5`, `#AI regulation`, `#ChatGPT Work`, `#AI industry news`

---

<a id="item-25"></a>
## [OpenAI 发布 GPT-5.6 三档模型系列与程序化工具调用功能](https://www.marktechpost.com/2026/07/09/openai-releases-gpt-5-6-a-three-tier-model-family-with-programmatic-tool-calling/) ⭐️ 7.0/10

OpenAI 于 2026 年 7 月 9 日发布了 GPT-5.6，作为三档模型系列（Sol、Terra、Luna）推出，同时带来程序化工具调用功能，该功能允许模型在隔离的 V8 运行时中编写和执行 JavaScript 来编排工具，无需返回每个中间结果。 此次发布标志着 OpenAI 从单一模型向三档定价模式的转变，直接与 Claude 的分层产品竞争。程序化工具调用是一项面向开发者的重大创新，可在实现更复杂工具编排的同时将令牌成本降低 38%至 63%。 Sol 在人工分析编码代理指数上达到 80 分（比 Claude Fable 5 高 2.8 分），在 OSWorld 2.0 上达到 62.6%，同时减少 85%的输出令牌。然而，Claude Fable 5 仍在人工分析智能指数、GDPval-AA v2、Toolathlon 和 SWE-Bench Pro 上领先。定价：Sol 为 5 美元/30 美元，Terra 为 2.5 美元/15 美元，Luna 为 1 美元/6 美元（每百万输入/输出令牌）。

rss · MarkTechPost · Jul 9, 20:45

**背景**: 程序化工具调用是一项允许大型语言模型生成 JavaScript 代码来协调单次请求中多个工具调用的功能，在隔离的 V8 沙箱环境中运行。这与传统的模型进行顺序 API 调用的工具调用方式不同。V8 是 Google 在 Chrome 和 Node.js 中使用的开源 JavaScript 引擎。三档定价直接与 Anthropic 的 Claude 分层产品（Opus 为 5 美元/25 美元，Fable 5 为 10 美元/50 美元）竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.openai.com/api/docs/guides/tools-programmatic-tool-calling">Programmatic Tool Calling | OpenAI API</a></li>
<li><a href="https://v8.dev/">V8 JavaScript engine</a></li>

</ul>
</details>

**标签**: `#openai`, `#gpt-5`, `#llm-release`, `#programmatic-tool-calling`, `#ai-benchmarks`

---

<a id="item-26"></a>
## [NVIDIA 发布压缩混合 MoE 大模型，实现 2.03 倍吞吐量提升](https://www.marktechpost.com/2026/07/09/meet-nemotron-labs-3-puzzle-75b-a9b/) ⭐️ 7.0/10

NVIDIA 发布了 Nemotron-Labs-3-Puzzle-75B-A9B，这是 Nemotron-3-Super 的压缩版本，采用迭代 Puzzle 技术，将硬件感知结构压缩与知识蒸馏恢复阶段相结合。该模型从 120.7B 总参数/12.8B 活跃参数减少到 75.3B 总参数/9.3B 活跃参数，在 8xB200 节点上实现了 2.03 倍的吞吐量提升。 这一进展意义重大，因为它展示了大规模的实际推理优化——模型体积减少 37%的同时吞吐量几乎翻倍，这对部署成本和延迟有直接影响。H100 GPU 上 8 倍的并发提升意味着服务器运营商可以为每个硬件单元服务更多用户，从而可能降低部署大型 MoE 模型的门槛。 迭代 Puzzle 技术交替进行硬件感知结构压缩（剪枝/架构搜索）和短期知识蒸馏阶段，以恢复压缩过程中损失的准确性。在单块 H100 上，1M 令牌并发从 1 个请求提升到 8 个。该模型实现每用户每秒 100 令牌的吞吐量。

rss · MarkTechPost · Jul 9, 19:31

**背景**: 混合专家（MoE）模型使用稀疏架构，每个推理仅使用部分参数（活跃参数），而总参数包括所有可用的专家。这允许构建大参数规模但计算成本适中的模型。Puzzle 是 NVIDIA 的硬件感知模型压缩框架，结合神经架构搜索（NAS）和知识蒸馏来优化特定目标硬件的模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2411.19146v1">Puzzle: Distillation-Based NAS for Inference-Optimized LLMs</a></li>
<li><a href="https://arxiv.org/abs/2411.19146">[2411.19146] Puzzle: Distillation-Based NAS for Inference ...</a></li>
<li><a href="https://medium.com/@csburakkilic/understanding-moe-architectures-the-difference-between-total-and-active-parameters-ad1d161fccaa">Understanding MoE Architectures: The Difference Between Total ...</a></li>

</ul>
</details>

**标签**: `#LLM compression`, `#Mixture of Experts`, `#NVIDIA`, `#Inference optimization`, `#Knowledge distillation`

---

<a id="item-27"></a>
## [Anthropic 为 Claude 订阅增加按量计费](https://www.wired.com/story/model-behavior-anthropic-will-charge-consumers-extra-to-use-claude-fable-5/) ⭐️ 7.0/10

Anthropic 正在为 Claude 订阅引入按量计费模式，要求用户根据使用其最佳消费级 AI 模型 Claude Fable 5 的使用量额外付费，这标志着无限固定费率访问的终结。 这预示着 AI 消费定价模式可能在整个行业发生转变，可能影响已习惯固定费率 AI 订阅的数百万用户。它可能重塑整个行业对 AI 订阅服务的预期。 这一变化专门适用于 Claude Fable 5，即 Anthropic 的顶级消费级模型。这种与传统订阅模式的告别反映了运行先进 AI 模型的高计算成本。

rss · WIRED AI · Jul 9, 18:30

**背景**: 随着技术成熟，AI 公司一直在尝试各种定价模式。订阅模式因能为消费者提供可预测的月度成本而变得流行。然而，运行像 Claude 这样的先进 AI 模型所需的重大计算资源一直在推动公司重新考虑其定价策略以保持盈利。

**标签**: `#AI pricing`, `#Anthropic`, `#Claude`, `#subscription model`, `#business strategy`

---

<a id="item-28"></a>
## [爱沙尼亚 AI"错误查找器"检测法律文本错误](https://www.wired.com/story/the-28-million-dollar-mistake-that-inspired-estonias-ai-fuckup-finder/) ⭐️ 7.0/10

爱沙尼亚部署了一款名为"Fuckup Finder"的人工智能系统来扫描法律草案中的错误。此前，一处措辞错误导致政府损失 2800 万美元。该工具在法案提交议会前扫描整个法律数据库，标记人类审查员遗漏的矛盾和歧义性语言。 这展示了人工智能在法律和政策工作流程中的实际价值，可能为政府节省数百万美元的法律错误成本。它为其他希望将人工智能纳入公共治理并实现常规任务自动化的政府提供了范例。 该系统由爱沙尼亚总理开发，目前处于测试阶段。它是爱沙尼亚更广泛数字治理举措的扩展，建立在该国作为最先进数字国家之一的声誉之上。

rss · WIRED AI · Jul 9, 10:01

**背景**: 爱沙尼亚被公认为世界上最先进的数字国家之一，被称为"电子爱沙尼亚"。政府一直在积极将人工智能技术融入公共服务和国家运作。激发该系统的 2800 万美元错误涉及一处造成重大财务后果的措辞错误，凸显了彻底法律审查的重要性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wired.com/story/the-28-million-dollar-mistake-that-inspired-estonias-ai-fuckup-finder/">The $28 Million Mistake That Inspired Estonia’s AI ‘Fuckup ...</a></li>
<li><a href="https://completeaitraining.com/news/estonia-deploys-artificial-intelligence-to-catch-legal/">Estonia deploys artificial intelligence to catch legal errors ...</a></li>

</ul>
</details>

**标签**: `#AI applications`, `#government technology`, `#Estonia`, `#legal technology`, `#automation`

---

<a id="item-29"></a>
## [DeepSeek V4 + SGLang：百万上下文推理优化实战](https://www.infoq.cn/article/qALuq71AxiG5VLmWqSzU?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

深圳 AICon 大会上的一场技术演讲，介绍了使用 SGLang 推理框架对支持百万上下文长度的 DeepSeek V4 模型进行推理优化的实战方法。 这一优化具有重要意义，因为处理百万级 token 上下文是生产环境 LLM 部署中最具挑战性的问题之一，SGLang 为需要长文档处理能力的 AI 应用开发者提供了实用的解决方案。 DeepSeek V4 是一种混合专家(MoE)模型，V4-Pro 版本拥有 1.6T 总参数(49B 激活参数)，支持 100 万 token 的上下文长度。SGLang 是一个高性能的服务框架，通过协同设计前端语言和运行时系统来优化 LLM 推理性能。

rss · InfoQ 中文站 · Jul 9, 16:15

**背景**: 长上下文 LLM 推理因注意力机制的二次复杂度而计算成本高昂。SGLang 是一个开源服务框架，设计用于在从单 GPU 到分布式集群的各种配置下提供低延迟、高吞吐量的推理性能。本次演讲旨在帮助开发者高效地在生产环境中部署 DeepSeek V4。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sglang.io/">Welcome to SGLang - SGLang Homepage</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/DeepSeek-V4-Pro · Hugging Face</a></li>
<li><a href="https://docs.sglang.io/">Welcome to SGLang - SGLang Documentation</a></li>

</ul>
</details>

**标签**: `#LLM Inference`, `#DeepSeek`, `#SGLang`, `#Long Context`, `#AI Infrastructure`

---

<a id="item-30"></a>
## [错误信息：关于 TypeScript 7.0 Go 重写的虚假报道](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 7.0/10

据称新功能包括用于并行控制的 --checkers 和 --builders 参数、用于与 TypeScript 6 并存的兼容包，以及编辑器中的 LSP 支持。然而，这则公告似乎是虚假信息——实际上并不存在这样的 TypeScript 7.0。

telegram · zaihuapd · Jul 9, 04:01

**背景**: TypeScript 是微软开发的强类型 JavaScript 超集，目前版本为 5.x 系列（而非 7.0）。它使用 TypeScript/JavaScript 编写，而非 Go。语言服务器协议（LSP）是编辑器和语言服务器之间的标准协议。当前 TypeScript 架构并未如所述那样使用 Go 或原生多线程。这似乎是虚假信息或捏造的故事。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Language_Server_Protocol">Language Server Protocol - Wikipedia</a></li>
<li><a href="https://microsoft.github.io/language-server-protocol/">Official page for Language Server Protocol</a></li>

</ul>
</details>

**标签**: `#TypeScript`, `#Go`, `#programming-languages`, `#performance`, `#misinformation`

---

<a id="item-31"></a>
## [大疆 EV50 飞越珠峰 8861 米创纪录](https://www.163.com/dy/article/L1CUCV940514R9OJ.html) ⭐️ 7.0/10

大疆尚未发布的 EV50 垂直起降运载无人机参与“巅峰使命”珠峰科考，在珠峰北坡飞越 8861 米，创下全球同类公开测试中的最高飞行升限，并获取了 8000 米以上海拔的真实大气剖面数据。 这款复合翼无人机可原地垂直起降，起飞后切换固定翼巡航。此次为期 12 天的任务中，EV50 累计完成 32 架次起降，连续爬升 3730 米，返程时仍剩 30%电量。大疆称其研发目标还包括百公里级货物运输等低空物流场景。

telegram · zaihuapd · Jul 9, 06:00

**背景**: “巅峰使命”珠峰科考是自 2017 年第二次青藏科考启动以来学科覆盖面最广、参加科考队员最多的综合性科考。此次科考是我国珠峰科考首次突破 8000 米以上海拔高度，实现了从“登山科考”向“科考登山”的战略转变。复合翼无人机融合了固定翼无人机速度快、航时长的优势与多旋翼垂直起降、空中悬停的灵活性。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://step.ac.cn/info/15113">巅峰使命珠峰科考专题</a></li>
<li><a href="https://baike.baidu.com/item/复合翼无人机/67152229">复合翼无人机_百度百科</a></li>

</ul>
</details>

**标签**: `#drone-technology`, `#aviation`, `#DJI`, `#high-altitude-flight`, `#robotics`

---

<a id="item-32"></a>
## [国家超算互联网核心节点郑州上线](https://36kr.com/newsflashes/3887797387344387) ⭐️ 7.0/10

2026 年 7 月 9 日，2026 河南省人工智能大会在郑州举行，国家超算互联网核心节点于当日正式上线运行，可对外提供超过 10 万卡国产人工智能算力，是国家超算互联网平台上线以来接入的最大规模单体国产 AI 算力资源池。 该节点的上线标志着我国在超算资源整合与调度领域迈出关键一步，构建了国家级人工智能基础设施，支撑大模型全量训练和科学计算。同时有助于降低对进口计算硬件的依赖，打造全国一体化算力网络体系。 该节点支持多品牌国产加速卡混合部署，具备灵活扩展至百万卡规模的能力。目前已连接全国 30 余家超算与智算中心，通过智能调度将全网资源利用率提升至满载水平。

telegram · zaihuapd · Jul 9, 07:00

**背景**: 国家超算互联网平台是一体化的超算算力网络和服务平台，可实现算力资源统筹调度，支撑数字中国建设。AI 加速卡是专门用于加速人工智能计算的硬件设备，相当于给电脑装上"超级外挂"，让 AI 模型训练更快、推理更高效。该平台目标是构建覆盖全国的计算资源统筹调度体系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ithome.com/0/974/370.htm">全国最大单体国产 AI 算力池落地郑州，国家超算互联网核心节点正式上...</a></li>
<li><a href="https://www.scnet.cn/home/subject/hxjd/index.html">国家超算互联网核心节点 - 超算互联网</a></li>
<li><a href="https://www.gov.cn/yaowen/liebiao/202404/content_6946204.htm">国家超算互联网平台上线__中国政府网</a></li>

</ul>
</details>

**标签**: `#国家超算互联网`, `#人工智能算力`, `#郑州`, `#基础设施`, `#国产芯片`

---