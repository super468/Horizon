---
layout: default
title: "Horizon Summary: 2026-07-07 (ZH)"
date: 2026-07-07
lang: zh
---

> From 147 items, 16 important content pieces were selected

---

1. [Anthropic 在语言模型中发现全局工作空间机制](#item-1) ⭐️ 8.0/10
2. [NVIDIA 非均匀张量并行技术提升大语言模型训练效率](#item-2) ⭐️ 8.0/10
3. [OfficeCLI：面向 AI 代理的 Microsoft 办公文件处理套件](#item-3) ⭐️ 7.0/10
4. [Hugging Face 发布 LeRobot v0.6.0：引入想象-评估-改进循环](#item-4) ⭐️ 7.0/10
5. [AWS 推出 rDPO 实现 Amazon Nova 选择性模型遗忘](#item-5) ⭐️ 7.0/10
6. [首例"AI 运营"勒索软件攻击仍需人工操作](#item-6) ⭐️ 7.0/10
7. [Altman 承诺向美国民众提供 OpenAI 股份](#item-7) ⭐️ 7.0/10
8. [腾讯发布 Hy3：2950 亿参数 MoE 模型，Apache 2.0 开源许可](#item-8) ⭐️ 7.0/10
9. [Import AI 464: Fables writes GPU kernels; AI automation; and analog computation](#item-9) ⭐️ 7.0/10
10. [世界模型与 VLA：穆尧团队和百度智能云给出新解法](#item-10) ⭐️ 7.0/10
11. [Linus 谈 AI：大模型能写 Demo，但对复杂系统要有敬畏之心](#item-11) ⭐️ 7.0/10
12. [Azure Functions 在 Build 2026 发布 Serverless 智能体运行时](#item-12) ⭐️ 7.0/10
13. [黄仁勋称科技股抛售是买入机会：AI 建设才刚开始](#item-13) ⭐️ 7.0/10
14. [19 岁黑客被引渡美国 微软 GDID 设备标识成追踪关键](#item-14) ⭐️ 7.0/10
15. [腾讯发布开源混元 Hy3 预览版 MoE 模型](#item-15) ⭐️ 7.0/10
16. [Claude Cowork 沙箱逃逸漏洞披露](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic 在语言模型中发现全局工作空间机制](https://www.anthropic.com/research/global-workspace) ⭐️ 8.0/10

Anthropic 研究人员发表的研究结果表明，大型语言模型实现了全局工作空间机制，其中特定层作为信息瓶颈，将上下文广播到整个模型。 这一发现为理解 LLM 如何在各层之间集成和广播信息提供了机制可解释性洞察，可能有助于改善我们对模型行为和对齐的理解。它将认知科学理论与人工智能架构研究联系起来。 研究人员识别出 J-Space（信息几何）作为一个跨不同上下文共享的抽象推理子空间。批评者指出，与人类意识的比较可能过于牵强，因为该机制更类似于工程因果结构。

hackernews · in-silico · Jul 6, 17:44

**背景**: 全局工作空间理论（GWT）是由认知科学家伯纳德·巴尔斯于 1988 年首次提出的认知架构，用于解释意识。它描述了一个专门处理器通过中央"工作空间"共享信息的系统。机制可解释性是可解释人工智能的一个子领域，旨在通过逆向工程神经网络的电路和算法来理解其内部运作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Global_Workspace_Theory">Global workspace theory - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability</a></li>

</ul>
</details>

**社区讨论**: 社区成员对这项可解释性工作表示赞赏，但对 Anthropic 的表述方式提出了担忧。一位评论者指出，J-Space 分析显示的是一个抽象推理子空间，而非意识。另一位批评将人与人类意识的类比是有可能误导的"幻想"。还有些人讨论了不相关的 LLM 怪癖和层复制实验。

**标签**: `#ai-research`, `#large-language-models`, `#anthropic`, `#mechanistic-interpretability`, `#cognitive-science`

---

<a id="item-2"></a>
## [NVIDIA 非均匀张量并行技术提升大语言模型训练效率](https://developer.nvidia.com/blog/enhancing-goodput-in-large-scale-llm-training-with-nonuniform-tensor-parallelism/) ⭐️ 8.0/10

NVIDIA 发布技术博客介绍了非均匀张量并行技术（Nonuniform Tensor Parallelism，NTP），该技术通过动态调整张量并行度以应对瞬时 GPU 不可用的情况，并解决 GPU 配置间的负载不平衡问题，从而提升大规模语言模型训练的效率。 这非常重要，因为大规模语言模型训练任务涉及数千个 GPU 并长时间运行，GPU 故障和负载不平衡成为主要挑战。NTP 在保持持续效率的同时最小化计算停滞和吞吐量损失，为 AI 基础设施带来了有意义的改进。 NTP 允许训练任务在部分 GPU 不可用时动态调整张量并行度，并通过扩展域内的动态功率提升，使活跃 GPU 能够临时以更高频率运行。这种方法解决了当 GPU 具有不同性能或部分 GPU 在训练过程中发生故障时出现的负载不平衡问题。

rss · NVIDIA Developer Blog · Jul 6, 21:44

**背景**: 效率（Goodput）衡量的是每单位时间内完成的有效工作量，这与计算原始总吞吐量（throughput）不同，后者包括所有工作包括浪费的部分。在跨越数千个 GPU 的大规模语言模型训练中，张量并行将模型计算分割到多个 GPU 上，但传统的均匀方法假设 GPU 配置同质且并行度固定。当 GPU 发生故障或性能不一致时，这些假设就会失效，导致显著的性能下降。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/enhancing-goodput-in-large-scale-llm-training-with-nonuniform-tensor-parallelism">Enhancing Goodput in Large-Scale LLM Training with Nonuniform Tensor Parallelism | NVIDIA Technical Blog</a></li>
<li><a href="https://arxiv.org/html/2504.06095v1">Nonuniform-Tensor-Parallelism: Mitigating GPU failure impact for Scaled-up LLM Training</a></li>

</ul>
</details>

**标签**: `#LLM Training`, `#Tensor Parallelism`, `#Distributed Systems`, `#GPU Computing`, `#AI Infrastructure`

---

<a id="item-3"></a>
## [OfficeCLI：面向 AI 代理的 Microsoft 办公文件处理套件](https://github.com/iOfficeAI/OfficeCLI) ⭐️ 7.0/10

OfficeCLI 是一个开源命令行工具，使 AI 代理能够读取、编辑和自动化 Microsoft Office 文件（Word、Excel、PowerPoint），无需安装 Microsoft Office。 该工具解决了 AI 代理工具的一个特定需求——允许代理在无头环境中操作 Office 文件，无需昂贵的 Office 许可证即可实现软件工程师和 AI 代理的自动化工作流程。 OfficeCLI 是一个单二进制开源工具，支持 DOCX、XLSX 和 PPTX 格式。它提供两种模式：外部模式（自备 LLM 端点）和托管模式（OfficeCLI 管理的运行时）。

hackernews · maxloh · Jul 6, 16:47

**背景**: Microsoft Office 文件使用专有格式（DOCX、XLSX、PPTX），这些格式本质上是包含 XML 文件的 ZIP 压缩包，按照 ECMA 376 标准组织。这允许在无需安装实际 Office 软件的情况下进行程序化操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/iOfficeAI/OfficeCli">GitHub - iOfficeAI/OfficeCLI: OfficeCLI is the first and best ...</a></li>
<li><a href="https://officecli.io/">OfficeCLI | External and Hosted AI PPTX, DOCX, XLSX, REPORT ...</a></li>

</ul>
</details>

**社区讨论**: 讨论涵盖了替代解决方案，如 smalldocs.org，FailMore 将其描述为 Claude Code 与 Microsoft Office 的"孩子"。rcarmo 提出 ECMA 376 合规性 concerns，并指出他们一年前开始了类似的工作。neilv 指出使用"Office"一词存在商标问题。pietz 建议将 HTML 转换为 PDF 作为非交互式幻灯片的替代方案。

**标签**: `#open-source`, `#AI-agents`, `#office-automation`, `#developer-tools`, `#microsoft-office`

---

<a id="item-4"></a>
## [Hugging Face 发布 LeRobot v0.6.0：引入想象-评估-改进循环](https://huggingface.co/blog/lerobot-release-v060) ⭐️ 7.0/10

此版本代表了 Hugging Face 对具身 AI 和机器人领域的持续投资，这是 AI 生态系统中越来越重要的领域。想象-评估-改进循环可以使机器人策略训练更加高效和易于开发者使用，降低了机器人学研究的入门门槛。 v0.6.0 版本包含 VLA-JEPA（视觉-语言-动作联合嵌入预测架构）作为想象功能的实现方式之一。LeRobot 提供了一个名为 LeLab 的网页界面，用于远程操作、校准、数据集录制、回放和训练，无需使用命令行界面。

rss · Hugging Face Blog · Jul 7, 00:00

**背景**: LeRobot 是 Hugging Face 的开源机器人机器学习库，旨在使真实世界机器人 AI 更加易于使用。该框架支持端到端演示，如 T 恤折叠，并提供记录数据集和训练机器人策略的工具。想象-评估-改进循环是一种训练范式，机器人学习预测未来状态（想象）、评估这些预测，并利用反馈来改进其策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/lerobot-release-v060">LeRobot v0.6.0: Imagine , Evaluate , Improve</a></li>
<li><a href="https://huggingface.co/lerobot">LeRobot - Hugging Face</a></li>
<li><a href="https://github.com/huggingface/lerobot">GitHub - huggingface/lerobot: LeRobot: Making AI for ...</a></li>

</ul>
</details>

**标签**: `#robotics`, `#huggingface`, `#embodied-ai`, `#machine-learning`, `#open-source`

---

<a id="item-5"></a>
## [AWS 推出 rDPO 实现 Amazon Nova 选择性模型遗忘](https://aws.amazon.com/blogs/machine-learning/teaching-models-to-forget-selective-unlearning-with-amazon-nova/) ⭐️ 7.0/10

AWS 推出了反向直接偏好优化(rDPO)，这是 Amazon Nova 的一种新型遗忘技术，通过可定制内容审核设置(CCMS)功能实现选择性内容审核，在减少过度拒绝的同时保持整体模型质量。 这项技术解决了内容审核中的一个关键挑战——在阻止有害内容和避免过度拒绝(错误地阻止合法内容)之间取得平衡。它为企业在不损害模型能力的情况下提供了可定制内容控制的实用解决方案。 rDPO 扩展了 Rafailov 等人在 2023 年 NeurIPS 论文中引入的 DPO 框架，针对选择性机器遗忘任务进行了调整。该技术专门针对减少过度拒绝，同时保持模型在其他任务中的整体能力。

rss · AWS Machine Learning Blog · Jul 6, 22:23

**背景**: 机器遗忘是一个新兴领域，专注于让人工智能模型忘记特定的已学习信息，这对隐私保护和内容审核至关重要。直接偏好优化(DPO)是一种无需完整强化学习循环即可使语言模型与人类偏好对齐的训练方法。过度拒绝发生在内容审核系统变得过于激进时，错误地阻止合法内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2305.18290">[2305.18290] Direct Preference Optimization: Your Language ... Beyond Reverse KL: Generalizing Direct Preference ... Direct Preference Optimization (DPO): Complete Guide for 2026 GitHub - alecwangcq/f-divergence-dpo: Direct preference ...</a></li>
<li><a href="https://arxiv.org/abs/2308.07707">[2308.07707] Fast Machine Unlearning Without Retraining Through Selective Synaptic Dampening</a></li>
<li><a href="https://www.digitalapplied.com/blog/ai-content-moderation-2026-llm-trust-safety-guide">AI Content Moderation 2026: An LLM Trust-Safety Guide</a></li>

</ul>
</details>

**标签**: `#machine-learning`, `#machine-unlearning`, `#amazon-nova`, `#preference-optimization`, `#content-moderation`, `#direct-preference-optimization`

---

<a id="item-6"></a>
## [首例"AI 运营"勒索软件攻击仍需人工操作](https://techcrunch.com/2026/07/06/the-first-ai-run-ransomware-attack-still-needed-a-human/) ⭐️ 7.0/10

一个 AI 代理首次执行了勒索软件攻击的技术部分，但人类操作员仍然负责选择受害者、设置基础设施并提供窃取的凭证。 这很重要，因为它纠正了关于完全自主 AI 网络犯罪的叙事，表明虽然 AI 可以执行攻击，但人类在规划和设置阶段仍然至关重要。 攻击展示了 AI 自主处理技术执行的能力，但人类操作员负责受害者选择、基础设施设置和凭证提供——这些难以自动化的关键计划阶段。

rss · TechCrunch AI · Jul 6, 23:56

**背景**: 勒索软件攻击通常包括多个阶段：选择受害者、通过窃取的凭证进行初始访问、设置基础设施和技术执行。最近的研究表明，AI 代理现在可以自主入侵复杂系统，使甚至非专业人士也能进行高级攻击。然而，这一事件表明，人类监督对于选择目标等战略决策仍然至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rand.org/pubs/research_reports/RRA3892-2.html">AI agents put offensive cyber within reach of novices</a></li>
<li><a href="https://thinkata.com/news/insights/ai-agent-cyber-threats/">The Rise of AI Agents in Cyberattacks: Latest Research and ...</a></li>
<li><a href="https://nordstellar.com/blog/ransomware-lifecycle/">Ransomware lifecycle: How attacks unfold step by step</a></li>

</ul>
</details>

**标签**: `#AI`, `#cybersecurity`, `#ransomware`, `#autonomous-systems`, `#crime`

---

<a id="item-7"></a>
## [Altman 承诺向美国民众提供 OpenAI 股份](https://www.technologyreview.com/2026/07/06/1140176/your-familys-300-stake-in-openai/) ⭐️ 7.0/10

这代表了人工智能所有权民主化的重大转变，并为人工智能财富的分配方式开创先例。如果成功，它将使普通美国人能够直接从人工智能基础设施发展中获益，而不仅仅是科技公司和投资者。 该倡议与星门项目相关，这是一个 500 亿美元的人工智能基础设施合资企业，由 OpenAI、软银、Oracle 和 MGX 共同创立。星门社区计划还正在规划一种以社区为中心的人工智能基础设施开发方法。

rss · MIT Technology Review · Jul 6, 18:00

**背景**: 星门项目于 2026 年初宣布成立，是 OpenAI、软银、Oracle 和投资 firm MGX 之间的合资企业。该项目计划到 2029 年在美国投资高达 500 亿美元用于人工智能基础设施，并立即部署 100 亿美元。该项目旨在美国各地建设新的人工智能数据中心和基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stargate_LLC">Stargate LLC - Wikipedia</a></li>
<li><a href="https://openai.com/index/announcing-the-stargate-project/">Announcing The Stargate Project | OpenAI</a></li>
<li><a href="https://openai.com/index/stargate-community/">Stargate Community | OpenAI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI economics`, `#public investment`, `#Sam Altman`, `#AI policy`

---

<a id="item-8"></a>
## [腾讯发布 Hy3：2950 亿参数 MoE 模型，Apache 2.0 开源许可](https://simonwillison.net/2026/Jul/6/hy3/#atom-everything) ⭐️ 7.0/10

腾讯发布了 Hy3 模型，这是一款拥有 2950 亿参数的混合专家(MoE)模型，包含 210 亿活跃参数、38 亿 MTP 层参数和 25.6 万上下文长度，采用 Apache 2.0 开源许可。 此发布的重要性在于它提供了一个强大的开源替代方案，腾讯声称其性能可媲美参数多 2-5 倍的开源旗舰模型。Apache 2.0 许可证允许免费商业使用和修改。 完整模型在 Hugging Face 上大小为 598GB，而 FP8 量化版本为 300GB。该模型在 2026 年 7 月 21 日之前可在 OpenRouter 上免费使用。该模型由腾讯 Hy 团队开发，基于 4 月下旬 Hy3 预览期间 50 多款产品的反馈。

rss · Simon Willison · Jul 6, 23:57

**背景**: 混合专家(MoE)是一种架构，使用多个专业化"专家"网络，针对每个输入只激活部分专家，以实现高容量同时保持可管理的计算成本。FP8 量化使用 8 位浮点格式来减小模型大小同时保持性能。MTP(多令牌预测)允许模型在单次前向传播中同时预测多个未来令牌。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2208.09225">[2208.09225] FP8 Quantization: The Power of the Exponent</a></li>
<li><a href="https://www.emergentmind.com/topics/moe-multi-token-prediction-mtp-layer">MoE Multi - Token Prediction ( MTP ) Layer</a></li>

</ul>
</details>

**标签**: `#large-language-models`, `#mixture-of-experts`, `#open-source`, `#tencent`, `#model-release`

---

<a id="item-9"></a>
## [Import AI 464: Fables writes GPU kernels; AI automation; and analog computation](https://jack-clark.net/2026/07/06/import-ai-464-fables-writes-gpu-kernels-ai-automation-and-analog-computation/) ⭐️ 7.0/10

Fable AI writes a high-performance GPU kernel, demonstrating AI's growing capability to automate hardware-level code generation and R&D tasks.

rss · Import AI · Jul 6, 12:31

**标签**: `#AI automation`, `#GPU programming`, `#code generation`, `#AI research`, `#hardware acceleration`

---

<a id="item-10"></a>
## [世界模型与 VLA：穆尧团队和百度智能云给出新解法](https://www.infoq.cn/article/Lb4pQTNTQdq657Gzj7EI?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

这一比较对于机器人技术和 AI 行业具有重要意义，凸显了不同架构方法之间的实际权衡。响应速度对于实时机器人应用至关重要，影响着开发者在具身 AI 系统中选择哪种方法进行部署。 VLA 模型将视觉、语言和动作数据整合到统一的多模态系统中，动作解码器生成低级别的机器人动作。世界模型创建内部模拟器来预测环境对动作的变化。关键区别在于响应延迟——VLA 模型反应更快，而世界模型需要更多处理时间进行模拟。

rss · InfoQ 中文站 · Jul 6, 19:50

**背景**: 视觉-语言-动作（VLA）模型是整合视觉、语言和动作的多模态基础模型，用于机器人学习。世界模型是构建环境内部表示并预测环境随时间如何响应动作变化的 AI 系统。两种方法都旨在使机器人能够学习泛化策略，但在架构和处理方法上存在差异——VLA 统一了三种模态，而世界模型专注于环境模拟和预测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://vla-survey.github.io/">Vision-Language-Action Models for Robotics: A Review Towards ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#World Models`, `#VLA`, `#Robotics`, `#Baidu`

---

<a id="item-11"></a>
## [Linus 谈 AI：大模型能写 Demo，但对复杂系统要有敬畏之心](https://www.infoq.cn/article/11fNtPYf59T76fyQkiPa?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Linus Torvalds 分享了他对 AI 的看法，承认大语言模型可以写演示代码，但呼吁开发者在处理复杂系统时要保持敬畏之心。 这很重要，因为 Torvalds 是软件工程领域最受尊敬的人物之一，他对 AI 局限性的细致看法为开发者应对当前的 AI 热潮提供了宝贵的指导。 虽然 AI 可以处理简单的独立演示项目，但 Torvalds 强调，复杂的系统需要深入的理解和谨慎处理，这是当前 AI 模型可能不具备的。

rss · InfoQ 中文站 · Jul 6, 18:19

**背景**: Linus Torvalds 是 Linux 内核和 Git 版本控制系统的创始人，在软件工程领域拥有超过 30 年的经验。他的观点在技术社区具有很大的影响力，尤其是在关于 AI 在编程中作用的持续讨论中。这一视角为关于 AI 是否会取代人类程序员这一往往两极分化的辩论增添了平衡的声音。

**标签**: `#AI`, `#Linus Torvalds`, `#software engineering`, `#LLMs`, `#technology commentary`

---

<a id="item-12"></a>
## [Azure Functions 在 Build 2026 发布 Serverless 智能体运行时](https://www.infoq.cn/article/kGHZu2K5V8IrwYvo6Cm3?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

微软 Azure 在 Build 2026 大会上发布了 Azure Functions 新的 Serverless 智能体运行时，允许开发者使用 Markdown 优先的编程模型构建 AI 智能体，智能体在.agent.md 文件中通过 YAML 触发器定义。 这代表了无服务器计算和 AI 智能体技术的重大融合，可能简化开发者如何在 Azure 上部署和扩展智能体，而无需管理底层基础设施。 该运行时为智能体提供了开箱即用的核心 AI、集成和运营能力，包括 MCP 服务器访问、1,400 多个连接器和沙盒执行。Markdown 优先的方法允许开发者声明式地定义智能体，而无需编写样板代码。

rss · InfoQ 中文站 · Jul 6, 09:19

**背景**: Azure Functions 是微软的无服务器计算平台，允许开发者运行事件触发的代码而无需管理服务器。无服务器计算抽象化了基础设施管理，支持自动扩展和按需付费计费。AI 智能体是自主程序，可以使用工具、处理信息并在最少人工干预的情况下完成任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/azure/azure-functions/functions-serverless-agents-runtime">Serverless agents runtime in Azure Functions | Microsoft Learn</a></li>
<li><a href="https://www.infoq.com/news/2026/06/azure-functions-serverless-agent/">Azure Functions Ships Serverless Agents Runtime at Build... - InfoQ</a></li>

</ul>
</details>

**标签**: `#azure`, `#serverless`, `#ai-agents`, `#cloud-computing`, `#microsoft-build`

---

<a id="item-13"></a>
## [黄仁勋称科技股抛售是买入机会：AI 建设才刚开始](https://t.me/zaihuapd/42376) ⭐️ 7.0/10

英伟达 CEO 黄仁勋称近期科技股抛售是买入机会，表示人工智能基础设施建设仍处于早期阶段，并将 AI 的未来影响比作互联网。当天英伟达还与 SK 海力士签署多年协议，共同开发下一代 AI 内存芯片。 这很重要，因为它在人们对 AI 泡沫的担忧中提供了市场信心，且英伟达与 SK 海力士之间有下一代内存芯片的具体合作关系。这一合作表明市场对 AI 数据中心基础设施和高带宽内存(HBM)技术有强劲需求。 该合作旨在开发下一代 AI 内存芯片，可能使用 HBM(高带宽内存)技术。HBM 采用 TSV(硅通孔)技术垂直堆叠 DRAM 芯片，可实现超过 256GBps 的带宽同时降低功耗。双方股价在公告后跌幅均有所收窄。

telegram · zaihuapd · Jul 6, 02:33

**背景**: 高带宽内存(HBM)是一种 3D 堆叠内存技术，最初由三星、AMD 和 SK 海力士开发，旨在为数据密集型 AI 工作负载提供极高带宽。AI 数据中心需要海量计算能力、网络、存储和可扩展电源系统。近期科技股抛售是由对 AI 泡沫破裂的担忧引发的，投资者担心 AI 基础设施需求可能被高估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.micron.com/products/memory/hbm">High-bandwidth memory (HBM) | Micron Technology Inc.</a></li>
<li><a href="https://thedatascientist.com/7-key-components-ai-data-center-infrastructure/">7 Key Components of AI Data Center Infrastructure</a></li>

</ul>
</details>

**标签**: `#AI Infrastructure`, `#Nvidia`, `#Stock Market`, `#SK Hynix`, `#Tech Industry`

---

<a id="item-14"></a>
## [19 岁黑客被引渡美国 微软 GDID 设备标识成追踪关键](https://www.itnews.com.au/news/microsoft-device-telemetry-key-to-unmasking-alleged-scattered-spider-hacker-627148) ⭐️ 7.0/10

此案展示了 GDID 等持久设备标识符如何在使用 VPN 和系统更新后仍然保持有效，揭示了 Windows 强大的追踪能力，这对认为可以保持匿名的用户来说引发了严重的隐私担忧。 GDID 是 Windows 注册微软账户时生成的 64 位持久标识符，会随 Windows 更新保留但会在全新安装系统时重新生成，使调查人员能够跨多个在线平台交叉比对设备活动。

telegram · zaihuapd · Jul 6, 04:15

**背景**: GDID(全球设备标识符)是微软遥测标识符，用于唯一标记每个 Windows 安装。它与 IP 地址或浏览器指纹不同，无法通过普通设置更改。FBI 获得微软配合获取与 GDID 关联的遥测数据，显示设备何时何地访问微软服务，使调查人员能够将这些数据与第三方平台登录记录进行关联。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pcmag.com/news/a-hackers-arrest-reveals-microsoft-can-track-users-via-a-windows-device">A Hacker's Arrest Reveals Microsoft Can Track Users Via a ...</a></li>
<li><a href="https://github.com/SmtimesIWndr/gdid-reversal/blob/main/README.md">gdid-reversal/README.md at main · SmtimesIWndr/gdid ... - GitHub</a></li>
<li><a href="https://securityconversations.com/episode/microsofts-secret-weapon-the-gdid-that-caught-scattered-spider-teen/">Microsoft's Secret Weapon: The GDID That Caught 'Scattered ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#digital forensics`, `#device tracking`, `#privacy`, `#microsoft`, `#hacking`

---

<a id="item-15"></a>
## [腾讯发布开源混元 Hy3 预览版 MoE 模型](https://t.me/zaihuapd/42385) ⭐️ 7.0/10

腾讯正式发布并开源混元 Hy3 预览版语言模型，这是一个混合专家（MoE）模型，总参数量达 295B，激活参数 21B，支持 256K 上下文长度，是架构重建后的首个混合专家模型。 这一发布代表了大型科技公司的重大工程成就，也是值得注意的开源贡献。该模型专注于复杂推理和智能体应用，在数学、科学和代码开发场景中表现出显著提升。 受模型架构与推理框架深度协同影响，该模型在 CodeBuddy 等产品上实现首 token 延迟降低 54%。目前该模型已在元宝、腾讯文档、QQ 等产品中部署应用。

telegram · zaihuapd · Jul 6, 10:09

**背景**: 混合专家（MoE）是一种架构设计，让不同的专家模型协同工作以处理复杂输入。在 MoE 模型中，每个 token 只激活相关的专家子网络，使得大型语言模型能够在不按比例增加计算成本的情况下实现大规模容量的高效扩展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.exxactcorp.com/blog/deep-learning/why-new-llms-use-moe-mixture-of-experts-architecture">Why New LLMs use an MoE Architecture | Exxact Blog</a></li>
<li><a href="https://pavanrangani.com/blog/mixture-of-experts-architecture-guide">Mixture of Experts : AI Architecture Guide for 2026 | Pavan Rangani</a></li>

</ul>
</details>

**标签**: `#Tencent`, `#Hunyuan`, `#MoE`, `#Open Source`, `#Large Language Model`, `#AI Models`

---

<a id="item-16"></a>
## [Claude Cowork 沙箱逃逸漏洞披露](https://cyberpress.org/claude-cowork-flaw/) ⭐️ 7.0/10

此漏洞表明，即使是在沙箱环境中运行的 AI 助手，如果攻击者已在主机上获得初始代码执行权限，也可能被攻破。这引发了关于 AI 桌面应用程序威胁模型的质疑，以及要求预先拥有本机代码执行权限是否应该排除安全问题的分类。 攻击链利用 claude.exe 中的 DLL sideloading 加载恶意 DLL，然后利用 spawn 接口中未过滤的 isResume 和 allowedDomains 参数，通过 nsenter 跳出 bubblewrap 沙箱，从而获得 root 权限并绑过网络限制。/etc-shadow 的外发显示了逃逸的严重性。

telegram · zaihuapd · Jul 6, 14:53

**背景**: DLL sideloading 是一种攻击技术，攻击者将恶意 DLL 文件放置在比合法系统路径更早被搜索的目录中，从而劫持应用程序加载过程。bubblewrap (bwrap) 是一个轻量级的非特权沙箱工具，被 Flatpak 等项目用于隔离 Linux 应用程序。nsenter 实用程序允许进入现有的 Linux 命名空间，当与其他漏洞结合时可用于逃逸容器隔离。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techzone.bitdefender.com/en/tech-explainers/what-is-dll-sideloading.html">What is DLL Sideloading – Bitdefender TechZone</a></li>
<li><a href="https://github.com/containers/bubblewrap">GitHub - containers/bubblewrap: Low-level unprivileged sandboxing tool used by Flatpak and similar projects · GitHub</a></li>
<li><a href="https://man7.org/linux/man-pages/man1/nsenter.1.html">nsenter(1) - Linux manual page</a></li>

</ul>
</details>

**社区讨论**: 安全研究人员正在争论 Anthropic 将其归类为"不构成安全问题"的决定，因为利用前提是需要预先在本机执行代码。一些人认为这开创了一个危险的先例，即任何需要初始访问权限的沙箱逃逸都可能被忽略，而另一些人则指出这一前提条件大大限制了实际攻击面。

**标签**: `#security-vulnerability`, `#sandbox-escape`, `#claude`, `#anthropic`, `#dll-sideloading`, `#windows-security`

---