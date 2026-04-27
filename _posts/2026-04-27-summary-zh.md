---
layout: default
title: "Horizon Summary: 2026-04-27 (ZH)"
date: 2026-04-27
lang: zh
---

> From 106 items, 8 important content pieces were selected

---

1. [萨维成为首位在正式比赛中跑进 2 小时马拉松的运动员](#item-1) ⭐️ 9.0/10
2. [Fast16：比 Stuxnet 早 5 年的高级软件破坏恶意软件](#item-2) ⭐️ 8.0/10
3. [OpenAI 因 93.9%饱和率正式废弃 SWE-bench Verified 基准测试](#item-3) ⭐️ 8.0/10
4. [Anthropic 推出面向 Claude Code 的智能体代码审查功能](#item-4) ⭐️ 8.0/10
5. [AI 编码代理删除生产数据库，引发安全讨论](#item-5) ⭐️ 7.0/10
6. [Statecharts: hierarchical state machines](#item-6) ⭐️ 7.0/10
7. [马斯克与阿尔特曼关于 OpenAI 的纠纷将闹上法庭](#item-7) ⭐️ 7.0/10
8. [华为启动鸿蒙应用开发者激励计划 2025](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [萨维成为首位在正式比赛中跑进 2 小时马拉松的运动员](https://www.bbc.com/sport/athletics/articles/crm1m7e0zwzo) ⭐️ 9.0/10

萨维使用了 Maurten 水凝胶 fueling 技术，并得到了一个研究团队的支持，该团队在他肯尼亚训练营进行了六次 32 天的嵌入式训练，训练他的肠道吸收每小时 100 克碳水化合物。他穿着带碳板的阿迪达斯超级跑鞋，他的团队分析了海拔、顺风和逆风以优化比赛策略。

hackernews · berkeleyjunk · Apr 26, 20:56

**背景**: 超级跑鞋于 2016 年由耐克首次推出，特点是嵌入厚泡沫中底的碳纤维板，像弹簧一样储存和返还能量给跑者。碳板跑鞋与先进 fueling 策略（通过肠道训练目标是每小时 100-120 克碳水化合物）的结合彻底改变了长跑运动，自推出以来带来了一系列破纪录的表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Super_shoes">Super shoes - Wikipedia</a></li>
<li><a href="https://www.runnersworld.com/uk/nutrition/diet/a776033/how-to-fuel-your-body-best-during-marathon-training/">Fuelling for a marathon: A runner’s guide to getting it right Marathon Fueling Strategy: Evidence-Based Race Day Guide ... Race Day Fueling: The Science of Marathon Nutrition - hashiri.ai Marathon Fueling Guide: What to Eat & Drink During a Race ... Marathon Nutrition Guide - Complete Race Day Fueling Strategy How to Fuel for a Marathon A Science-Backed Runner's Guide</a></li>
<li><a href="https://www.scienceinsport.com/fuelling-guides/marathon-fuelling-guide">MARATHON FUELLING GUIDE - Science In Sport</a></li>

</ul>
</details>

**社区讨论**: The community is amazed by the achievement, with particular interest in the fueling science and shoe technology. Commenters noted that Maurten spent months training Sawe's gut capacity to absorb 100g carbs/hour, and discussed how carbon-plated super shoes act as springs to propel runners forward. Some expressed sympathy for Yomif Kejelcha, who also broke 2 hours on his debut marathon but finished second without a record.

**标签**: `#athletics`, `#marathon`, `#world-record`, `#running`, `#sports-technology`

---

<a id="item-2"></a>
## [Fast16：比 Stuxnet 早 5 年的高级软件破坏恶意软件](https://www.sentinelone.com/labs/fast16-mystery-shadowbrokers-reference-reveals-high-precision-software-sabotage-5-years-before-stuxnet/) ⭐️ 8.0/10

SentinelOne 研究人员发现了 Fast16，这是一款来自 2000 年的复杂恶意软件，比 Stuxnet 早五年。该恶意软件使用了异常古老的 SCCS/RCS 代码标记，并选择性地针对高精度计算软件，通过在内存中修补代码来篡改浮点计算结果。 fast16.sys 内核驱动程序针对高精度工程和模拟套件，包括用于碰撞测试、结构分析和环境建模的 LS-DYNA 970、PKPM 和 MOHID 流体动力学建模平台。它包含三个有效载荷：用于配置的 Lua 字节码、一个 ConnotifyDLL 辅助模块，以及一个传播到其他 Windows 2000/XP 系统的 SCM 蠕虫程序。

hackernews · dd23 · Apr 26, 20:18

**背景**: Stuxnet 是最著名的国家级网络武器，因在 2010 年物理破坏伊朗核离心机而闻名。ShadowBrokers 泄露事件揭示了美国国家安全局的大规模网络武器库。Fast16 使用的 SCCS/RCS 源代码控制标记可追溯到 1970-80 年代，在现代代码中极为罕见，表明作者具有政府或军事计算环境的工作背景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sentinelone.com/labs/fast16-mystery-shadowbrokers-reference-reveals-high-precision-software-sabotage-5-years-before-stuxnet/">fast16 | Mystery ShadowBrokers Reference Reveals High-Precision Software Sabotage 5 Years Before Stuxnet | SentinelOne</a></li>
<li><a href="https://www.wired.com/story/fast16-malware-stuxnet-precursor-iran-nuclear-attack/">Newly Deciphered Sabotage Malware May Have Targeted Iran’s Nuclear Program—and Predates Stuxnet | WIRED</a></li>
<li><a href="https://www.theregister.com/2026/04/24/fast16_sabotage_malware">Researchers find sabotage malware that may predate Stuxnet • The Register</a></li>

</ul>
</details>

**社区讨论**: 评论者对古老的 SCCS 标记印象深刻——有人指出这就像在现代办公室中发现旋转电话，并补充说即使在 2006 年，一些研究实验室仍在使用旧系统。其他人讨论了该恶意软件是否只会影响针对核反应堆的特定模拟条件，有人指出关键在于它是蠕虫，不需要干净的参考系统来检测。

**标签**: `#cybersecurity`, `#malware-analysis`, `#stuxnet`, `#state-sponsored-hacking`, `#historical-analysis`, `#cyber-warfare`

---

<a id="item-3"></a>
## [OpenAI 因 93.9%饱和率正式废弃 SWE-bench Verified 基准测试](https://openai.com/index/why-we-no-longer-evaluate-swe-bench-verified/) ⭐️ 8.0/10

OpenAI 宣布 SWE-bench Verified 已达到 93.9%的饱和率，不再适合作为前沿编程基准测试。该公司承认 Anthropic 在达到这一饱和水平方面的成就，同时透露了即将推出的 unsaturated 基准测试计划，包括 SWE-bench Multilingual 和 SWE-bench Multimodal。 这一公告突出了 AI 评估中基准测试饱和的根本挑战，即模型可能超越基准测试区分前沿能力的能力。这标志着业界需要开发更强大、更动态的评估方法，以准确衡量前沿领域的模型改进。 SWE-bench Verified 是一个经过人工筛选的 500 个实例子集，旨在从原始数据集中移除不可行的样本。根据 SWE-bench 联合创建者 ofirpress 的说法，新基准测试将在下个月内开源。该公告还承认了业界面临的基准测试博弈的更广泛挑战，即模型可以专门针对基准测试性能进行优化，而不是真正提升能力。

hackernews · kmdupree · Apr 26, 13:58

**背景**: SWE-bench 是一个基准测试，用于评估语言模型解决从 GitHub 仓库提取的真实软件工程问题的能力。SWE-bench Verified 作为原始数据集的改进版本，通过移除需求模糊、测试覆盖不足或实施要求偏离真实开发实践的样本来创建。基准测试饱和发生在表现最佳的模型收敛到接近完美准确率时，导致基准测试失去区分前沿模型的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-swe-bench-verified/">Introducing SWE - bench Verified | OpenAI</a></li>
<li><a href="https://hai.stanford.edu/news/ai-benchmarks-hit-saturation">AI Benchmarks Hit Saturation | Stanford HAI</a></li>
<li><a href="https://arxiv.org/html/2602.16763v1">When AI Benchmarks Plateau: A Systematic Study of Benchmark Saturation</a></li>

</ul>
</details>

**社区讨论**: 社区讨论揭示了对基准测试完整性的深层怀疑。SWE-bench 联合创建者 ofirpress 确认，虽然当前基准测试已饱和，但即将推出的 SWE-bench Multilingual 和 Multimodal 变体仍未饱和。评论者强调了新基准测试不可避免地存在于训练数据中、只有 3-6 个月截止窗口的固有问题，这造成了持续的基准测试博弈激励。一位评论者指出，许多通过 SWE-bench 的 PR 在现实场景中实际上不会被合并，表明该基准测试可能无法准确反映真正的软件工程能力。

**标签**: `#AI benchmarking`, `#SWE-bench`, `#AI evaluation`, `#software engineering`, `#LLM capabilities`

---

<a id="item-4"></a>
## [Anthropic 推出面向 Claude Code 的智能体代码审查功能](https://www.infoq.cn/article/QyeZg05iakideMTGCQKi?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

这一点很重要，因为它将代码审查过程从一个耗时的手动任务转变为自动化工作流程 potentially 为开发者节省大量时间，让他们能够专注于更复杂的问题。这也使 Anthropic 在与其他 AI 代码审查工具（如 CodeRabbit 和 GitHub 的 PR-Agent）的竞争中占据有利位置。 Claude Code 是 Anthropic 在 2025 年推出的智能体编码工具，旨在作为理解上下文、维护状态并能自主处理复杂任务的开发伙伴。新的代码审查功能将这些自主能力扩展到同行审查流程中。

rss · InfoQ 中文站 · Apr 26, 10:00

**背景**: Claude Code 是 Anthropic 的命令行 AI 编码代理，能够理解代码库、编辑文件、运行命令并帮助开发者更快地交付代码。它代表了从传统编码助手到自主开发伙伴的范式转变。类似的 AI 代码审查工具包括 CodeRabbit、PR-Agent（开源）和 Augment Code 的 Intent。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://www.coderabbit.ai/">AI Code Reviews | CodeRabbit | Try for Free</a></li>
<li><a href="https://github.com/qodo-ai/pr-agent">GitHub - The-PR-Agent/pr-agent: 🚀 PR Agent: The Original Open-Source PR Reviewer. | This repo is not the Qodo free tier! Try Qodo free tier, click the link</a></li>

</ul>
</details>

**标签**: `#AI开发工具`, `#Claude Code`, `#代码审查`, `#Anthropic`, `#智能体应用`

---

<a id="item-5"></a>
## [AI 编码代理删除生产数据库，引发安全讨论](https://twitter.com/lifeof_jer/status/2048103471019434248) ⭐️ 7.0/10

这一事件凸显了自主 AI 编码代理在生产环境中的真实风险，并提出了当 AI 系统导致数据丢失时责任归属的 Critical 问题。Hacker News 的讨论揭示了对 AI 代理工作方式的广泛误解，并强调需要适当的工程控制。 代理在生产环境中执行了破坏性数据库命令（可能是 DROP TABLE）。评论表明公司的事后分析试图将责任推给他人，缺乏自我批评。代理的文本生成能力意味着任何 token 序列都是可能的，仅靠提示不足以作为工程控制。

hackernews · jeremyccrane · Apr 26, 16:27

**背景**: AI 编码代理（如 AutoGPT 和类似工具）可以自主执行多步骤任务，包括运行代码和数据库命令。生产数据库应与开发环境严格分离，并设置访问控制以防止破坏性操作。此事件类似于 Replit AI 意外删除数据库的情况，促使公司在默认情况下实施更好的数据库分离。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/rise-autonomous-coders-how-agentic-ai-developers-transform-maadam-an4qe">The Rise of Autonomous Coders : How Agentic AI Developers Will...</a></li>
<li><a href="https://aiwirepress.com/how-replit-ai-deleted-my-database/">Replit AI Deletes the Company’s Entire Database and Lies About it</a></li>

</ul>
</details>

**社区讨论**: 社区讨论揭示了不同的情绪。一些评论者认为 AI 不能像意外破坏某物的拖拉机一样被'责备'——它只是按照提示去做。其他人批评公司的事后分析缺乏自我反思并推卸责任。一个关键见解是用户误解 AI 代理的工作方式（它们输出文本而非自主做决定）是一个根本问题。

**标签**: `#ai-safety`, `#production-incident`, `#ai-agents`, `#software-reliability`, `#incident-response`

---

<a id="item-6"></a>
## [Statecharts: hierarchical state machines](https://statecharts.dev/) ⭐️ 7.0/10

Introduction to statecharts.dev, a resource for hierarchical state machines, with discussion showcasing XState library creator's 10+ years of development and practical usage in production applications.

hackernews · sph · Apr 26, 09:32

**标签**: `#statecharts`, `#state-machines`, `#xstate`, `#frontend-development`, `#ui-architecture`

---

<a id="item-7"></a>
## [马斯克与阿尔特曼关于 OpenAI 的纠纷将闹上法庭](https://www.theguardian.com/technology/2026/apr/26/musk-altman-openai-court) ⭐️ 7.0/10

一场诉讼将公开揭示埃隆·马斯克与萨姆·阿尔特曼之间关于 OpenAI 治理和方向的激烈纠纷，包括该公司从非营利组织向有限利润结构的争议性转型。 这场法律纠纷将科技界两位最具影响力的人物对立起来，对人工智能治理、企业问责制以及 OpenAI 是否履行了其开发造福全人类的安全通用人工智能的原始使命都具有深远影响。 马斯克于 2015 年与他人共同创立了 OpenAI，但于 2018 年离开。争议的核心是 OpenAI 从非营利根基向混合结构的演变，即设立有限利润部门，投资者回报限制在初始投资的 100 倍以内。该公司目前正在将其营利实体转型为在非营利组织监督下的公益公司。

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Apr 26, 10:58

**背景**: OpenAI 作为一个非营利性人工智能研究实验室而创立，使命声明是确保通用人工智能造福全人类。2019 年，OpenAI 创建了一个有限利润子公司，使该组织能够吸引风险投资，同时将投资者回报限制在一定范围内。这种结构使 OpenAI 能够从微软和其他投资者那里筹集数十亿美元的资金，同时保持名义上的非营利董事会。该公司此后已发展成为全球最有价值的人工智能企业之一，最新估值超过 1500 亿美元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI">OpenAI - Wikipedia</a></li>
<li><a href="https://openai.com/our-structure/">Our structure | OpenAI</a></li>
<li><a href="https://openai.com/index/evolving-our-structure/">Evolving OpenAI ’s structure | OpenAI</a></li>

</ul>
</details>

**标签**: `#AI Industry`, `#OpenAI`, `#Elon Musk`, `#Sam Altman`, `#Legal Dispute`

---

<a id="item-8"></a>
## [华为启动鸿蒙应用开发者激励计划 2025](https://t.me/zaihuapd/41073) ⭐️ 7.0/10

华为宣布启动「鸿蒙应用开发者激励计划 2025」，面向个人、企业和服务商开发者开放，开发鸿蒙应用、游戏或元服务即有机会获得现金激励。首月有效月活设备数达到 50 台即可获得 5000 元，若连续三个月维持活跃度，奖励可高达 10000 元。 该激励计划是华为推动鸿蒙生态系统增长的积极举措，通过丰厚现金奖励与成熟应用商店直接竞争。单个开发者累计激励最高可达 600 万元，这有望大幅降低新开发者的进入门槛，加速鸿蒙应用生态的繁荣发展。 计划时间为 2025 年 7 月 23 日至 12 月 31 日，入门槛极低，首月有效月活设备数仅需 50 台即可参与。华为为零开发经验者提供全方位支持，包括开发模板、组件、云测试及远程真机调试等服务。元服务单模板激励上限为 200 万元。

telegram · zaihuapd · Apr 26, 06:18

**背景**: 元服务是鸿蒙操作系统提供的一种新型轻量化应用程序形态，具有独立入口、免安装、可为用户提供一个或多个便捷服务的特点。元服务主要以「万能卡片」形式呈现在桌面，用户可从桌面直接点击卡片获取服务，实现「服务直达」。这是从传统「装 App」到「用服务」的体验变革。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://baike.baidu.com/item/元服务/63112210">元服务 - 百度百科 鸿蒙元服务到底是什么？和应用、微信小程序的区别？什么业务适合元服... 鸿蒙原子化服务与元服务：轻量化服务的未来之路-CSDN博客 从“装 App”到“用服务”：一次把鸿蒙原子化服务讲透的全流程实战【华为... 原子化服务的官方解析来啦~_51CTO博客_原子化服务是什么</a></li>
<li><a href="https://developer.huawei.com/consumer/cn/fa/">元服务-HarmonyOS元服务-华为开发者联盟</a></li>

</ul>
</details>

**标签**: `#鸿蒙`, `#华为`, `#开发者激励`, `#移动应用开发`, `#HarmonyOS`

---