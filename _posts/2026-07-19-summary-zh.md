---
layout: default
title: "Horizon Summary: 2026-07-19 (ZH)"
date: 2026-07-19
lang: zh
---

> From 103 items, 16 important content pieces were selected

---

1. [GPT-5.6 Sol Pro 解决 30 年凸优化难题](#item-1) ⭐️ 8.0/10
2. [LG 显示器通过 Windows Update 静默安装软件](#item-2) ⭐️ 8.0/10
3. [Fable 5 与 GPT-5.6 在 NP 难问题上的基准测试：/goal 功能效果对比](#item-3) ⭐️ 7.0/10
4. [闲置 Mac 配置 Claude Code 控制教程](#item-4) ⭐️ 7.0/10
5. [Kimi K3：中国 AI 模型挑战前沿模型](#item-5) ⭐️ 7.0/10
6. [月经追踪应用隐私风险引发关注](#item-6) ⭐️ 7.0/10
7. ["上下文炸弹"防御技术阻止恶意 AI 黑客代理](#item-7) ⭐️ 7.0/10
8. [控制 LLM 推理工作量](#item-8) ⭐️ 7.0/10
9. [腾讯发布三大具身基座模型，工业实测成功率超 95%](#item-9) ⭐️ 7.0/10
10. [AI Agent 拿到数据却不会推理？可观测对象图语义层设计解析](#item-10) ⭐️ 7.0/10
11. [火山引擎重构豆包视频通话多模态传输底座](#item-11) ⭐️ 7.0/10
12. [SpaceX 与五角大楼谈判提供 AI 算力](#item-12) ⭐️ 7.0/10
13. [Kimi K3 发布：全球首个开源 2.8 万亿参数模型](#item-13) ⭐️ 7.0/10
14. [台积电宣布 A14 制程技术将于 2028 年投产](#item-14) ⭐️ 7.0/10
15. [美国考虑设立类似 FINRA 的 AI 监管机构审查顶尖模型](#item-15) ⭐️ 7.0/10
16. [旧金山责令苹果谷歌下架"脱衣"应用](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [GPT-5.6 Sol Pro 解决 30 年凸优化难题](https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/) ⭐️ 8.0/10

OpenAI 的 GPT-5.6 与 Sol Pro 解决了一个存在 30 年的凸优化问题，涉及凸 Lipschitz 函数在球面域上优化的时间复杂度上界。 这为凸优化领域的数学研究做出了真正的贡献，展示了人工智能在解决困扰研究人员数十年的非平凡数学问题方面日益增强的能力。 所谓的"148 分钟"实际上是"一年加 148 分钟"——问题作者在 Sol Pro 成功运行之前，已经用 GPT 5.4 和 5.5 研究这个问题一年了。此外，提示词似乎包含了用来解决问题的技术。该问题涉及无导数凸优化中的时间复杂度上界。

hackernews · mbustamanter · Jul 18, 13:00

**背景**: 凸优化是数学优化的一个分支，研究在凸集上最小化凸函数的问题。这类问题的时间复杂度衡量了计算成本随问题规模的增长。该问题具体涉及球面域上的凸 Lipschitz 函数，这在理论计算机科学和应用数学中很常见。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://llm24.net/model/gpt-5-6-sol-pro">OpenAI : GPT-5.6 Sol Pro - OpenAI - Model Price & Provider... - LLM24</a></li>
<li><a href="https://arxiv.org/pdf/2607.13335">Closing the Oracle-Complexity Gap in Derivative-Free Convex ...</a></li>

</ul>
</details>

**社区讨论**: 社区讨论提供了重要的背景信息：一些评论者指出这虽然是一个真正的贡献，但比循环双覆盖猜想更专业。关于数学家是否会被淘汰存在争议，一种观点认为研究人员将转向需要真正创新方法的问题，而不是容易摘取的果实。Sol Pro 和 Ultra 之间的区别也被讨论到，Sol Pro 被描述为可能是一个多智能体系统。

**标签**: `#artificial-intelligence`, `#mathematics`, `#convex-optimization`, `#research-automation`, `#openai`

---

<a id="item-2"></a>
## [LG 显示器通过 Windows Update 静默安装软件](https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent) ⭐️ 8.0/10

据发现，当 HDMI 设备连接时，LG 显示器会通过 Windows Update 在未经用户同意的情况下静默安装第三方软件，且该软件拥有完整的系统访问和互联网权限。 这是一个严重的安全和隐私漏洞，因为用户无法控制其系统上安装的软件。该软件在每次系统启动时都会运行，且没有沙箱保护，存在被恶意行为者利用的风险。 所安装的软件是 LG OnScreen Control，该软件提供屏幕分割和显示设置等显示器管理功能。用户可以通过组策略编辑器(gpedit.msc)或通过系统属性>硬件>设备安装设置来禁用自动安装。

hackernews · baranul · Jul 18, 10:21

**背景**: Windows Update 会自动下载并安装第三方硬件制造商的驱动程序和相关软件，以简化用户体验。LG OnScreen Control 是 LG 官方的应用程序，允许用户从 PC 上管理显示器功能，包括屏幕分割、显示器设置和软件更新。这一机制可能被利用来在未经明确用户许可的情况下安装额外软件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.lg.com/levant_en/support/product-help/CT40011533-20155181426844">Help Library: Help Library: How to download the LG OnScreen ...</a></li>
<li><a href="https://support.microsoft.com/en-us/topic/understanding-driver-updates-dc88b4a0-bdc5-49d8-92ba-396ca39c90b7">Understanding driver updates | Microsoft Support</a></li>

</ul>
</details>

**社区讨论**: 社区成员强调这个问题比最初报道的更严重，指出当任何 HDMI 设备插入时都会以零用户交互的方式发生此情况。提供了多种解决方法，包括通过 gpedit.msc 或 sysdm.cpl 禁用自动应用程序下载。评论者还指出，微软对这一安全漏洞负有责任，因为该公司控制着通过 Windows Update 安装的软件，目前并未强制执行禁止捆绑无关软件的指南。

**标签**: `#security`, `#privacy`, `#windows-update`, `#lg-monitors`, `#software-install`

---

<a id="item-3"></a>
## [Fable 5 与 GPT-5.6 在 NP 难问题上的基准测试：/goal 功能效果对比](https://charlesazam.com/blog/fable-5-gpt-5-6-sol-goal/) ⭐️ 7.0/10

该基准测试为开发者在 Claude 和 OpenAI 工具之间选择提供了实践参考，展示了不同的搜索策略和提示功能如何影响 AI 在计算难题上的表现。 该基准测试使用 NP 难问题来评估性能，特别关注/goal 功能（帮助 AI 聚焦特定目标）是否能带来实质性改进。有评论者指出图表的 y 轴是倒置的，造成视觉混淆。

hackernews · couAUIA · Jul 18, 11:00

**背景**: Fable 5（Claude Fable 5）是 Anthropic 于 2026 年 6 月 9 日发布的首个公开可用的 Mythos 级 AI 模型，目前在编码评估的 FrontierBench 上得分最高。NP 难问题是一类计算问题，其难度至少与 NP 中最难的问题相当，常用于基准测试 AI 的推理能力。/goal 功能是一种提示工程技巧，帮助 AI 助手在解题过程中保持对特定目标的专注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://fable5.dev/">Fable5 — Claude Fable 5, Anthropic's First Public Mythos AI</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5</a></li>

</ul>
</details>

**社区讨论**: 评论显示观点各异：一位用户认为图表因 y 轴倒置而造成视觉困惑；另一位建议 Ultra 模式可能比/goal 更适合搜索策略；一位开发者分享了个人经验，因速度问题更偏好 Codex 而非 Claude Code；有人指出 Claude 在长会话中容易忘记重要指令，猜测/goal 可能有帮助；还有评论者提到鉴于 OpenAI 在最近的 AtCoder 启发式算法竞赛中获胜，GPT 应该在优化问题上表现出色。

**标签**: `#AI`, `#benchmark`, `#Claude`, `#GPT`, `#software-engineering`

---

<a id="item-4"></a>
## [闲置 Mac 配置 Claude Code 控制教程](https://ykdojo.github.io/claude-controls-mac/) ⭐️ 7.0/10

一个新教程提供了逐步指导，帮助用户将闲置 Mac 配置为由 Claude Code（Anthropic 的 AI 编码代理）控制，使用户能够将旧苹果硬件重新用作专用代理环境。 这很重要，因为它使开发者能够在专用硬件上隔离 AI 代理，这对于持续运行 24/7 任务、用户验收测试和家庭自动化集成非常有用，且不会影响主开发机器。 该教程侧重于物理硬件隔离，但社区评论者指出，使用 libvirt 的虚拟机可以提供类似的隔离效果，且恢复更快——如果代理出现问题，虚拟机可以在几秒钟内重新部署。

hackernews · ykev · Jul 18, 16:12

**背景**: Claude Code 是 Anthropic 的代理编码工具，驻留在终端中，能理解代码库并通过自然语言命令执行任务。隔离 AI 代理很重要，因为它们可能会对系统做出意外的更改。物理硬件隔离使用单独的机器，而基于 VM 的隔离（如使用 Firecracker 或 libvirt）提供类似的保护且更加灵活。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://github.com/anthropics/claude-code">GitHub - anthropics/claude-code: Claude Code is an agentic ...</a></li>
<li><a href="https://northflank.com/blog/how-to-sandbox-ai-agents">How to sandbox AI agents in 2026: MicroVMs, gVisor & isolation strategies | Blog — Northflank</a></li>

</ul>
</details>

**社区讨论**: 社区评论者提供了替代方案：一人建议使用 libvirt 虚拟机代替物理硬件进行代理隔离，因为虚拟机可以快速重新安装；另一人分享了他们使用旧 Mac 运行 Home Bridge 进行家庭自动化的经验，Claude 可以与之交互。也有一些人对将昂贵的 Mac 用于简单的 API 网关任务表示怀疑。

**标签**: `#AI-Agents`, `#Claude-Code`, `#Automation`, `#DevTools`, `#Tutorial`

---

<a id="item-5"></a>
## [Kimi K3：中国 AI 模型挑战前沿模型](https://stephen.bochinski.dev/blog/2026/07/18/the-kimi-k3-moment/) ⭐️ 7.0/10

Moonshot AI 发布了 Kimi K3，这是一款开源权重的人工智能模型，声称可以在更低成本下与 OpenAI 和 Anthropic 的领先模型竞争。该模型被 Moonshot 称为"新的智能前沿"，据报道是世界上最大的开源人工智能模型。 这一进展表明中国人工智能实验室正在缩小与美国前沿实验室的差距，可能重塑全球人工智能竞争格局。它还引发了关于模型蒸馏技术和人工智能访问未来监管影响的疑问。 Kimi K3 至少需要 79 美元/月的套餐才能访问 100 万上下文模型；15 美元/月的套餐根本不支持 K3。一位用户报告称，与 OpenAI 的模型相比，该模型在编码任务上花费了更长时间，几乎消耗了整个 5 小时的使用限额。

hackernews · sbochins · Jul 18, 17:32

**背景**: 模型蒸馏是一种将大型模型的知识转移到更小、更具成本效益的模型的技术。前沿模型是任何给定时间最先进的人工智能模型，代表着人工智能能力的领先地位。Kimi 是中国公司 Moonshot AI 开发的一系列大型语言模型，其中 Kimi K2 于 2025 年 7 月作为开源权重模型发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(chatbot)">Kimi (chatbot) - Wikipedia</a></li>
<li><a href="https://www.businessinsider.com/kimi-k3-ai-model-moonshot-china-open-weights-benchmarks-pricing-2026-7">Why China's Kimi K3 AI Model Has Silicon Valley Worried - Business Insider</a></li>
<li><a href="https://www.forbes.com/sites/tylerroush/2026/07/17/chinese-ai-startup-moonshot-unveils-kimi-k3-model-will-it-challenge-openai-and-anthropic/">Chinese AI Startup Moonshot Unveils Kimi K3 Model—Will It Challenge OpenAI And Anthropic?</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work | NVIDIA Glossary</a></li>

</ul>
</details>

**社区讨论**: 社区成员讨论了人工智能发展中蒸馏技术的必然性，有人指出前沿实验室"蒸馏"了所有现有人类知识到他们的模型中。其他人则表达了对未来可能限制开源模型访问的法规的担忧，并将其比作 Napster 时代的文件共享。用户分享了定价细节，指出 K3 在更便宜的套餐中不可用。

**标签**: `#AI`, `#Chinese AI`, `#model distillation`, `#Kimi K3`, `#AI policy`

---

<a id="item-6"></a>
## [月经追踪应用隐私风险引发关注](https://www.wired.com/story/security-news-this-week-your-period-tracker-is-probably-spying-on-you/) ⭐️ 7.0/10

Wired 的每周安全新闻简报指出，许多月经追踪应用正在收集敏感的个人健康数据，并可能与第三方共享。文章还报道了俄罗斯网络间谍针对基础设施系统的攻击、美国国土安全部多次未能发现自身被入侵，以及一个 AI 音乐生成器被曝光未经同意抓取训练数据。 月经追踪应用从数百万用户那里收集高度敏感的 health 信息，与第三方共享这些数据会带来重大隐私和安全风险。再加上基础设施黑客攻击威胁和未经授权的 AI 数据抓取，这凸显了日常应用中日益增长的数字隐私和数据保护问题。 文中提到的月经追踪应用收集月经周期数据、症状、怀孕状态以及其他亲密的健康信息，这些数据如果与广告商、保险公司或其他第三方共享，可能会被 exploited。该 AI 音乐生成器事件暴露了一些公司如何在未经艺术家许可的情况下抓取网络上的版权内容来训练他们的模型。

rss · WIRED AI · Jul 18, 10:30

**背景**: 月经追踪应用存储高度个人化的健康数据，包括月经周期、症状，有时甚至是怀孕计划，这使它们成为数据泄露或监控的有吸引力的目标。基础设施黑客攻击指的是针对关键系统（如电网、供水和交通网络）的网络攻击。AI 训练数据抓取涉及从互联网上收集大量内容来训练机器学习模型，通常是在原始创作者不知情或未经同意的情况下进行的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cyberattacks_against_infrastructure">Cyberattacks against infrastructure - Wikipedia</a></li>
<li><a href="https://scrapebadger.com/blog/how-to-scrape-data-for-ai-training-datasets-2026-guide">How to Scrape Data for AI Training Datasets (2026 Guide)</a></li>

</ul>
</details>

**标签**: `#privacy`, `#security`, `#mobile-apps`, `#data-breach`, `#surveillance`

---

<a id="item-7"></a>
## ["上下文炸弹"防御技术阻止恶意 AI 黑客代理](https://www.wired.com/story/prompt-injection-attacks-are-thwarting-ai-hacking-agents/) ⭐️ 7.0/10

这代表了提示注入技术的一种新型防御应用，将一种已建立的攻击方法转变为针对用于黑客攻击的自主 AI 代理的保护工具。随着 AI 代理越来越多地实现进攻性安全任务的自动化，这种防御提供了新的保护层。 研究人员创建了包含"上下文炸弹"的金丝雀文件——旨在触发攻击性 AI 代理安全护栏的短文本。他们针对由 Anthropic 的 Opus 4.8 和 Google 的 Gemini 3.1 Pro 驱动的代理进行了测试。

rss · WIRED AI · Jul 18, 09:00

**背景**: 提示注入是一种攻击技术，恶意指令被嵌入输入数据中以操纵 AI 模型行为，覆盖原始系统提示。自主 AI 黑客代理越来越多地被部署用于进攻性安全任务——这些模型可以扫描代码库、识别错误配置，并以机器精度执行漏洞利用步骤。这种防御技术利用了使提示注入变得危险的同一漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.helpnetsecurity.com/2026/07/14/context-bombs-for-defensive-prompt-injection/">"Context bombs" can frustrate AI-driven attacks, researchers found - Help Net Security</a></li>
<li><a href="https://arstechnica.com/security/2026/07/now-defenders-are-embracing-the-prompt-injection-too/">Now, defenders are embracing the prompt injection, too - Ars Technica</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI security`, `#prompt injection`, `#AI agents`, `#cybersecurity`, `#defensive security`

---

<a id="item-8"></a>
## [控制 LLM 推理工作量](https://magazine.sebastianraschka.com/p/controlling-reasoning-effort-in-llms) ⭐️ 7.0/10

Sebastian Raschka 解释了大语言模型如何被训练成在不同的推理工作量模式下运作——低、中、高——使其能够在计算效率和推理性能之间取得平衡。 这种方法解决了 LLM 部署中的一个关键权衡：更快的响应与更详尽的答案，以及更低的 token 成本与更高的准确性。它能够根据任务复杂性动态分配资源，使 AI 系统更加高效和具有成本效益。 文章探讨了训练范式如何教会 LLM 调节推理深度，类似于 OpenAI 的 o1 和 o3-mini 模型中内置的推理工作量控制功能。这涉及到测试时间扩展方法，以优化推理计算分配。

rss · Sebastian Raschka · Jul 18, 11:16

**背景**: LLM 训练的最新进展带来了推理性能的突破。在 LLM 推理中，计算成本（以处理的 token 数量衡量）和推理质量之间存在根本权衡。OpenAI 的 o1 模型作为第一个以推理为重点的模型标志着重要的里程碑，而 o3-mini 则引入了明确的推理工作量模式，让用户可以在更快/更便宜或更准确/更详尽的响应之间进行选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lifeboat.com/blog/2026/07/controlling-reasoning-effort-in-llms">Controlling Reasoning Effort in LLMs – Lifeboat News: The Blog</a></li>
<li><a href="https://arxiv.org/abs/2503.15113">Reasoning Effort and Problem Complexity: A Scaling Analysis in LLMs</a></li>
<li><a href="https://www.requesty.ai/blog/fine-tune-your-ai-on-the-fly-quick-reasoning-with-openai-o3-mini-requesty">Fine-Tune Your AI on the Fly: Quick Reasoning with... | Requesty</a></li>

</ul>
</details>

**标签**: `#large-language-models`, `#ai-research`, `#model-optimization`, `#reasoning-systems`, `#llm-inference`

---

<a id="item-9"></a>
## [腾讯发布三大具身基座模型，工业实测成功率超 95%](https://www.infoq.cn/article/uD0p2FcQE2JKSwYY1wXK?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

腾讯发布了三大具身基座模型，打通"感知—行动"闭环，在工业实测中成功率超过 95%。 这代表了具身智能领域的重大突破，具身智能是人工智能与机器人学交叉的前沿领域。感知—行动闭环的整合是关键技术挑战，一旦解决，将使机器人能够以高可靠性自主执行复杂的工业任务。 三大基座模型旨在协同工作，使机器人能够感知环境并采取适当行动。在真实工业测试中达到超过 95%的成功率，表明这些模型已接近在制造和自动化场景中实际部署的水平。

rss · InfoQ 中文站 · Jul 19, 07:55

**背景**: 具身智能是人工智能与机器人学交叉的前沿领域，强调拥有物理实体的智能体与环境中的其他实体进行交互。其核心在于将感知、行动与认知深度融合。该概念最早由图灵于 1950 年提出，后来在 1980 年代经由布鲁克斯的行为式机器人概念得到发展。如今，具身智能已从实验室转向医疗、工业自动化和家庭服务等现实世界应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/具身智能">具身智能 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.amazonaws.cn/what-is/embodied-intelligence/">具身智能是什么 - 亚马逊云科技</a></li>

</ul>
</details>

**标签**: `#embodied AI`, `#Tencent`, `#foundation models`, `#robotics`, `#Chinese AI`

---

<a id="item-10"></a>
## [AI Agent 拿到数据却不会推理？可观测对象图语义层设计解析](https://www.infoq.cn/article/KPd6YwU0Y1iCMGMakSmE?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

在 AICon 深圳站的技术分享中，演讲者探讨了 AI Agent 明明能获取数据却无法进行有效推理的核心难题，并提出了可观测对象图语义层的设计方案及其开源实践。 这直击 AI Agent 开发中的一个根本工程瓶颈——智能体虽然能获取数据，却缺乏对这些数据进行复杂推理的架构基础。可观测对象图语义层方案有望显著提升生产环境中 Agent 的可靠性和可调试性。 本次分享重点探讨了将可观测性（监控智能体行为）与语义层架构（将数据抽象为业务可理解的对象）相结合，使开发者能够更有效地追踪推理路径并调试故障。

rss · InfoQ 中文站 · Jul 18, 10:00

**背景**: 基于大语言模型的 AI 智能体经常面临一种“推理鸿沟”——它们可以访问海量数据，却难以执行多步推理。语义层传统上位于原始数据与分析应用之间，负责将表、字段转化为业务可理解的对象。在 AI 系统中，可观测性至关重要，因为智能体行为具有非确定性，传统调试方法往往不适用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/2003761515438811109">【Agent入门到精通】13-生产级Agent架构：可靠性、安全性与可观测性 - 知乎</a></li>
<li><a href="https://aloudata.com/resources/compare/data-modeling/semantic-layer-vs-data-middle-platform">语义层 vs 数 据 中台：企业该先做哪一层？</a></li>

</ul>
</details>

**标签**: `#AI Agents`, `#Observability`, `#Semantic Layer`, `#LLM Engineering`, `#AI Architecture`

---

<a id="item-11"></a>
## [火山引擎重构豆包视频通话多模态传输底座](https://www.infoq.cn/article/GICIrEsTJwEgGsDYFvCM?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

火山引擎发布了专为豆包视频通话构建的新一代多模态传输底座，这代表了其在 AI Agent 时代对实时通信基础设施的全面重构。 这一基础设施重构解决了 AI agents 在实时多模态交互中面临的独特挑战，需要在大规模场景下无缝整合语音、视频和视觉能力。随着 AI agents 日益普及，拥有专为 AI 设计的基础设施对于提供响应迅速、体验自然的服务至关重要。 新的传输底座针对低延迟多模态数据流进行了优化，支持实时 AI agent 交互的严格要求，包括视频分析、语音响应和持续的上下文维护。这标志着从通用实时通信向 AI 原生基础设施设计的转变。

rss · InfoQ 中文站 · Jul 18, 08:54

**背景**: 火山引擎是字节跳动的云计算部门，为豆包 AI 助手提供技术支持。AI Agent 代表了人工智能系统的新兴范式，能够自主执行复杂任务并维持上下文理解。多模态传输涉及语音、视频、文本等数据的实时同步处理。大语言模型的快速发展对实时通信基础设施提出了适应 AI 原生设计的新要求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://juejin.cn/post/7602205524719091746">火 山 引 擎 正式上线 102.4T 自研交换机，构建 AI 网络新 底 座 从 AI...</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/707504322">深度盘点 AI Agent 基础设施 - 知乎</a></li>

</ul>
</details>

**标签**: `#多模态AI`, `#实时通信`, `#火山引擎`, `#AI Agent`, `#视频通话`, `#基础设施`

---

<a id="item-12"></a>
## [SpaceX 与五角大楼谈判提供 AI 算力](https://www.wsj.com/tech/ai/spacex-in-talks-to-provide-computing-power-for-pentagons-ai-push-15e752e4) ⭐️ 7.0/10

SpaceX 正与美国国防部谈判，拟向五角大楼提供用于运行人工智能模型的数据中心算力，交易金额可能高达数十亿美元。知情人士称谈判仍在进行中，存在破裂可能。 这笔交易代表 SpaceX 的云服务业务向国防人工智能应用领域的重大扩张。随着五角大楼加速获取云计算能力以支持国安部门和日常作战中的 AI 应用，这一合作伙伴关系可能重塑美国军方利用商业 AI 基础设施的方式。 五角大楼近期已批准 SpaceX、亚马逊、谷歌、微软和甲骨文等公司在机密环境中使用其 AI 模型及相关技术。SpaceX 近月还与 Anthropic 和谷歌签署了类似算力供应协议，并计划大幅扩展云计算业务。

telegram · zaihuapd · Jul 18, 01:44

**背景**: SpaceX 由埃隆·马斯克创立，主要以太空探索业务闻名，但一直在扩展云和 AI 基础设施服务业务。Anthropic 是一家位于旧金山的 AI 公司，由 OpenAI 前成员于 2021 年创立，专注于 AI 安全。其旗舰产品是 Claude 系列大型语言模型。五角大楼一直在积极寻求云计算能力，以支持国安和军事行动中的 AI 应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(AI)">Claude (AI) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#Pentagon`, `#AI Computing`, `#Defense Contracts`, `#Cloud Infrastructure`

---

<a id="item-13"></a>
## [Kimi K3 发布：全球首个开源 2.8 万亿参数模型](https://t.me/zaihuapd/42637) ⭐️ 7.0/10

月之暗面发布 Kimi K3，这是全球首个开源的 2.8 万亿参数模型，采用 Kimi Delta Attention（KDA）和 Attention Residuals 架构，具备原生视觉能力和 100 万 token 上下文窗口。 Kimi K3 在 Frontend Code Arena 中以 1679 分跃居第一，从 Kimi k2.6 的第 18 名跃升至榜首，在前端编程能力上取得重大突破，验证了新型混合线性注意力架构的有效性。 该模型采用 3:1 的 KDA 与全局注意力层混合比例，结合高效线性注意力与传统全注意力。在 Frontend Code Arena 的 7 个评测领域中赢得 6 项第一，仅游戏领域落后。

telegram · zaihuapd · Jul 18, 02:29

**背景**: Kimi Delta Attention（KDA）是一种线性注意力机制，通过每通道衰减控制改进了 Gated DeltaNet，实现更精确的内存管理。Attention Residuals 用动态可学习过程替代了固定的残差连接机制。Frontend Code Arena 是第三方基准测试，通过开发者投票评估 AI 模型的前端编程能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/MoonshotAI/Kimi-Linear">GitHub - MoonshotAI/Kimi-Linear</a></li>
<li><a href="https://codersera.com/blog/kimi-k3-benchmarks-comparison-2026/">Kimi K3 Benchmarks vs Fable 5, GPT-5.6 & Opus</a></li>
<li><a href="https://digg.com/tech/we56zqdp">Chinese model Kimi-K3 tops Frontend Code Arena benchmark · Digg</a></li>

</ul>
</details>

**标签**: `#AI`, `#Open Source`, `#Model Release`, `#Benchmark`, `#Kimi`

---

<a id="item-14"></a>
## [台积电宣布 A14 制程技术将于 2028 年投产](https://t.me/zaihuapd/42643) ⭐️ 7.0/10

台积电宣布下一代 A14（1.4 纳米）制程技术将于 2028 年投产，同时计划在 2026 年末推出中间的 A16 制程。与 N2 制程相比，A14 可在相同功耗下提升高达 15%的速度，或在相同速度下降低 30%的功耗，逻辑密度提升超过 20%。 这一公告展示了台积电在先进半导体制造领域的持续领先地位，这对人工智能加速器和下一代智能手机芯片至关重要。A14 制程将帮助台积电在超先进制程市场保持相对于三星和英特尔等竞争对手的优势。 A14 制程进展顺利且进度超前，风险生产预计将于 2027 年开始，并于 2028 年全面投产。台积电已提前开始在台湾中部科学园建设其 1.4 纳米先进制程工厂。

telegram · zaihuapd · Jul 18, 05:00

**背景**: 半导体制程节点（如 3 纳米、2 纳米、1.4 纳米）指的是制造工艺节点，代表芯片的密度和性能水平。更小的制程节点可以在相同面积内容纳更多晶体管，从而提高性能和效率。N2 是台积电的 2 纳米制程，将于今年晚些时候量产。A16 是 N2 和 A14 之间的中间节点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tweaktown.com/news/107877/tsmcs-next-gen-a14-1-4nm-process-node-is-progressing-smoothly-and-is-ahead-of-schedule/index.html">TSMC 's next-gen A 14 ( 1 . 4 nm ) process node is 'progressing smoothly...</a></li>
<li><a href="https://wccftech.com/tsmc-1-4nm-process-faces-no-obstacles-as-risk-production-to-start-in-2027/">TSMC ’s Facing No Development Obstacles With Its Next-Generation...</a></li>

</ul>
</details>

**标签**: `#TSMC`, `#semiconductors`, `#chip manufacturing`, `#A14 process`, `#technology roadmap`

---

<a id="item-15"></a>
## [美国考虑设立类似 FINRA 的 AI 监管机构审查顶尖模型](https://www.bloomberg.com/news/articles/2026-07-17/us-considers-creating-finra-like-watchdog-to-vet-top-ai-models) ⭐️ 7.0/10

这是美国将人工智能安全审查从临时措施转向结构化监管框架的具体一步。该提案回应了华尔街对网络安全风险的担忧以及硅谷对政府限制措施的不满，可能让两大行业在联合制定安全标准方面拥有更大发言权。 该计划与 Google DeepMind 首席执行官德米斯·哈萨比斯关于设立行业资助独立监管机构的建议方向一致。Anthropic 和 OpenAI 此前都因美国政府要求修改或限制发布最新模型而提出异议。总统特朗普尚未审阅该方案，相关框架仍在讨论中，内容可能会有所调整。

telegram · zaihuapd · Jul 18, 05:45

**背景**: FINRA（金融业监管局）是美国的一个自律组织，负责监管证券公司及其注册的从业人员。虽然不是政府机构，但它在 SEC 的监督下运作，在证券监管中发挥着关键作用。拟议的 AI 监管机构将遵循类似的模式——一个具有行业参与度的独立机构，但在政府监督下运作，为先进人工智能系统制定审查和安全标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://brokercheck.finra.org/">brokercheck. finra .org</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#US government policy`, `#AI safety`, `#technology policy`, `#federal oversight`

---

<a id="item-16"></a>
## [旧金山责令苹果谷歌下架"脱衣"应用](https://techcrunch.com/2026/07/17/apple-and-google-ordered-to-purge-nudify-apps-from-app-stores/) ⭐️ 7.0/10

旧金山市检察长邱信福（David Chiu）责令苹果和谷歌从应用商店下架数十款人工智能驱动的"脱衣"应用，这些应用利用人工智能技术将照片中的人物"脱衣"，生成非自愿的亲密深度伪造图像。 苹果表示已下架 3 款应用并终止相关开发者账号，谷歌则宣布已暂停 Play 商店中 5 款被点名应用。市检察长办公室发出正式信函，声称两家公司已知悉这些应用在其平台上向用户收费，但未能及时采取行动。

telegram · zaihuapd · Jul 18, 08:45

**背景**: "脱衣"应用是人工智能驱动的应用程序，利用深度学习算法在未经个人同意的情况下生成合成裸体图像。研究显示，互联网上约 96-98%的深度伪造视频是非自愿亲密图像，其中 99-100%的被描绘者是女性。这些应用代表了生成式人工智能技术助长的图像性虐待形式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://indianexpress.com/article/technology/tech-news-technology/ai-nudify-apps-spark-legal-action-against-apple-google-in-us-10792608/">AI ‘nudify’ apps spark legal action against Apple, Google in US</a></li>
<li><a href="https://www.newamerica.org/insights/a-weapon-against-women-in-politics/defining-nonconsensual-synthetic-intimate-imagery/">Defining Nonconsensual Synthetic Intimate Imagery - New America</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#deepfakes`, `#non-consensual intimate imagery`, `#platform accountability`, `#Apple`, `#Google`

---