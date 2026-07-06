---
layout: default
title: "Horizon Summary: 2026-07-06 (EN)"
date: 2026-07-06
lang: en
---

> From 96 items, 10 important content pieces were selected

---

1. [It's not about physical vs. digital games, it's about ownership](#item-1) ⭐️ 7.0/10
2. [Free Online Book: Introduction to Compilers and Language Design](#item-2) ⭐️ 7.0/10
3. [Amazon Mechanical Turk Stops New Customers](#item-3) ⭐️ 7.0/10
4. [Meituan Releases LongCat-2.0: 1.6T MoE Model with 1M Context](#item-4) ⭐️ 7.0/10
5. [Qwen's Former Lead Critiques Hybrid Thinking, Backs Agents](#item-5) ⭐️ 7.0/10
6. [TerminAI: Transparent AI Terminal Wrapper with MCP Support](#item-6) ⭐️ 7.0/10
7. [Bedside Camera Detects REM Sleep with Clinical EEG Validation](#item-7) ⭐️ 7.0/10
8. [Azure Functions Launches Serverless Agent Runtime at Build 2026](#item-8) ⭐️ 7.0/10
9. [Hong Kong Handles Over Half of China's Chip Imports, Record High](#item-9) ⭐️ 7.0/10
10. [China Debates Cutting SCI Publication Incentives Over Security](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [It's not about physical vs. digital games, it's about ownership](https://popcar.bearblog.dev/its-about-ownership/) ⭐️ 7.0/10

A thoughtful essay arguing that the real issue with digital games isn't physical vs. digital format, but rather the fundamental lack of true ownership - no ability to resell, transfer, or guarantee perpetual access - with Hacker News commenters adding perspectives on potential regulation, gaming industry monetization evolution, and DRM workarounds.

hackernews · popcar2 · Jul 5, 14:56

**Tags**: `#digital-rights`, `#gaming`, `#ownership`, `#drm`, `#licensing`

---

<a id="item-2"></a>
## [Free Online Book: Introduction to Compilers and Language Design](https://dthain.github.io/books/compiler/) ⭐️ 7.0/10

Dr. Douglas Thain released a free online book 'Introduction to Compilers and Language Design' in 2021, offering a hands-on approach to building a C-style compiler from scratch. This book fills a crucial gap in compiler education by providing a accessible, practical textbook that has been validated in classroom settings since 2019, earning repeated recommendations from the developer community. The book takes a practical, step-by-step approach where readers build a working C-style compiler. Community feedback notes the content focuses closely on C and its idiosyncrasies, which may be a limitation for those seeking broader language design perspectives.

hackernews · AlexeyBrin · Jul 5, 11:54

**Background**: Compilers are programs that translate source code written in one programming language into another. The 'dragon book' (Compilers: Principles, Techniques, and Tools by Aho, Sethi, and Ullman) is a classic but advanced textbook often used in graduate-level compiler courses. Dr. Thain's book offers a more accessible entry point for undergraduates and self-learners interested in compiler construction.

**Discussion**: Overall sentiment is highly positive, with one commenter personally endorsing Dr. Thain's teaching after taking his compilers class. Others suggest complementary resources like C4 (a self-compiling C-subset compiler) for extended study. Some constructive criticism notes the C-centric focus may limit exposure to broader language design concepts.

**Tags**: `#compilers`, `#education`, `#programming-languages`, `#free-resources`, `#computer-science`

---

<a id="item-3"></a>
## [Amazon Mechanical Turk Stops New Customers](https://techcrunch.com/2026/07/05/amazon-will-stop-accepting-new-customers-for-mechanical-turk/) ⭐️ 7.0/10

Amazon has announced it will stop accepting new customers for Mechanical Turk, signaling the potential end of one of the earliest and most influential crowdsourcing platforms that has operated for over two decades. This is significant because Mechanical Turk has been a foundational tool for micro-task work, data labeling, and AI training data collection since 2005. Its potential closure affects researchers, machine learning practitioners, and gig economy workers who have relied on the platform for human intelligence tasks at scale. While Amazon has not provided specific timelines or exact dates for the shutdown, the announcement marks a pivotal moment for the crowdsourcing industry. Existing users will likely continue to have access for now, but no new customers can sign up for the service.

rss · TechCrunch AI · Jul 5, 17:43

**Background**: Amazon Mechanical Turk (MTurk) was launched in 2005 and became one of the first platforms to enable businesses and researchers to crowdsource simple tasks that require human intelligence, such as data verification, survey responses, and content moderation. The platform pioneered the concept of 'Human Intelligence Tasks' (HITs) and became integral to the machine learning ecosystem for obtaining labeled training data. For nearly 20 years, MTurk has shaped the gig economy and established many practices still used in data annotation and crowdsourcing today.

**Discussion**: The news has generated significant discussion among researchers, ML practitioners, and gig workers who express nostalgia for the platform while also noting concerns about the future of crowdsourcing and the workers who relied on MTurk for income. Many are already exploring alternative platforms such as Prolific, Labelbox, and Scale AI.

**Tags**: `#amazon`, `#crowdsourcing`, `#gig-economy`, `#mechanical-turk`, `#tech-industry`

---

<a id="item-4"></a>
## [Meituan Releases LongCat-2.0: 1.6T MoE Model with 1M Context](https://www.marktechpost.com/2026/07/05/meituan-releases-longcat-2-0-a-1-6t-parameter-open-moe-model-with-native-1m-context-and-longcat-sparse-attention/) ⭐️ 7.0/10

Meituan has released LongCat-2.0, a 1.6 trillion-parameter Mixture-of-Experts model that activates approximately 48 billion parameters per token, featuring native 1-million-token context built on LongCat Sparse Attention and running end-to-end on domestic AI ASIC superpods. This release represents a significant advancement in China's AI capabilities, offering one of the longest context windows (1M tokens) available in open models while demonstrating the ability to train and serve large-scale MoE models on domestic hardware despite export restrictions on advanced chips. The model uses LongCat Sparse Attention (LSA) for efficient long-context processing with linear complexity, and implements Zero-computation experts with ScMoE for token-level dynamic compute allocation where simple tokens require no computation and complex tokens receive more resources.

rss · MarkTechPost · Jul 5, 21:25

**Background**: Mixture of Experts (MoE) is a neural network architecture that uses sparse activation, where only a subset of the model's parameters are activated for each input token, enabling larger model capacities without proportional computational cost. LongCat Sparse Attention is a sparse attention mechanism designed to handle extremely long contexts efficiently. Domestic AI ASIC refers to AI accelerators designed and manufactured in China.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://www.ai-all.info/en/ai-models/longcat-2-0">LongCat -2.0 – Meituan's Open-Source Next-Generation...</a></li>
<li><a href="https://arxiv.org/html/2512.23966v1">Efficient Context Scaling with LongCat ZigZag Attention</a></li>

</ul>
</details>

**Tags**: `#mixture-of-experts`, `#large-language-models`, `#long-context`, `#sparse-attention`, `#AI-infrastructure`

---

<a id="item-5"></a>
## [Qwen's Former Lead Critiques Hybrid Thinking, Backs Agents](https://www.marktechpost.com/2026/07/04/qwens-former-lead-on-what-hybrid-thinking-got-wrong-and-why-he-now-backs-agents/) ⭐️ 7.0/10

Junyang Lin, former technical lead of Alibaba's Qwen, explains in a talk and essay what went wrong with Qwen3's hybrid thinking modes (thinking mode for step-by-step reasoning vs. non-thinking mode for instant responses) and why he now advocates for agentic approaches over reasoning-based systems. This represents a significant architectural pivot for one of China's leading LLM families, offering rare insider perspective on what hybrid thinking failed to deliver and why the industry is shifting toward agentic AI—affecting how developers build next-generation AI systems. Qwen3 introduced hybrid thinking modes allowing models to switch between deep reasoning and quick responses, plus dynamic thinking budgets letting callers cap reasoning tokens. Lin highlights that reward hacking remains a major challenge in reinforcement learning infrastructure for agentic systems.

rss · MarkTechPost · Jul 5, 02:31

**Background**: Qwen3 was released in April 2025 with hybrid thinking modes supporting both step-by-step reasoning (Thinking Mode) and near-instant responses (non-thinking mode). The models expanded multilingual support from 29 to 119 languages. Hybrid thinking was designed to dynamically allocate reasoning resources based on query complexity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/07/04/qwens-former-lead-on-what-hybrid-thinking-got-wrong-and-why-he-now-backs-agents/">Qwen's Former Lead on What Hybrid Thinking Got... - MarkTechPost</a></li>
<li><a href="https://qwenlm.github.io/blog/qwen3/">Qwen3: Think Deeper, Act Faster | Qwen</a></li>
<li><a href="https://qwen3.app/">Qwen3: Think Deeper, Act Faster | Hybrid Thinking AI Model</a></li>

</ul>
</details>

**Tags**: `#AI Agents`, `#Large Language Models`, `#Qwen`, `#Reinforcement Learning`, `#Machine Learning Research`

---

<a id="item-6"></a>
## [TerminAI: Transparent AI Terminal Wrapper with MCP Support](https://terminai.app/) ⭐️ 7.0/10

An open-source terminal wrapper called TerminAI provides on-demand AI assistance via the Model Context Protocol (MCP), supporting Claude and Codex with automatic access to terminal scrollback and the ability to suggest shell commands that users can approve. This transparent wrapper approach addresses a key pain point in AI-assisted development tools by staying completely out of the way until needed, potentially improving developer productivity without disrupting existing workflows. The hardest technical challenges were implementing transparent scrollback integration and full-frame TUI overlay functionality, which required manual implementation as Claude couldn't handle those parts correctly. Currently alpha quality, it works on macOS (iTerm2, Terminal.app) and Linux (Yakuake/Konsole), with Windows not yet supported.

rss · Hacker News - Show HN · Jul 5, 23:46

**Background**: MCP (Model Context Protocol) is an open standard introduced by Anthropic in November 2024 that standardizes how AI assistants connect to external systems where data lives. Similar tools like Warp and Fig also offer AI-integrated terminals, but TerminAI distinguishes itself through its 'invisible until needed' transparent wrapper approach.

<details><summary>References</summary>
<ul>
<li><a href="https://modelcontextprotocol.io/docs/getting-started/intro">What is the Model Context Protocol (MCP)? - Model Context Protocol</a></li>
<li><a href="https://www.anthropic.com/news/model-context-protocol">Introducing the Model Context Protocol \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#terminal`, `#AI`, `#open-source`, `#developer-tools`, `#MCP`

---

<a id="item-7"></a>
## [Bedside Camera Detects REM Sleep with Clinical EEG Validation](https://lucidcode.com/2026/06/20/inspec-with-cgx-patch-clinical-eeg-sleep-stage-classification/) ⭐️ 7.0/10

A developer built an infrared camera device called INSPEC that detects REM sleep by measuring frame-to-frame pixel variance in the eye region. The device was validated against clinical EEG using three independent sleep stage classifiers (ez6, ez6moe, and DreamentoScorer), and all three showed matching REM periods at hours 3, 5, and 7 of the night. This represents a contactless alternative to traditional EEG-based sleep monitoring, potentially making sleep tracking more accessible and comfortable. The method could enable easier sleep studies without electrodes, benefiting both clinical research and personal health monitoring for sleep disorders. The camera uses IR light to monitor the face, measuring pixel variance in the eye region to detect eye movements under eyelids during REM sleep. Toss detection, whole-frame motion rejection, and face tracking filter out body movement and out-of-frame periods. The three classifiers were trained on ZMax data and showed some variability when applied to the CGX Patch EEG data.

rss · Hacker News - Show HN · Jul 5, 20:27

**Background**: REM (Rapid Eye Movement) sleep is traditionally detected using EEG electrodes attached to the scalp, which can be uncomfortable for subjects. Computer vision approaches offer contactless monitoring by detecting subtle facial movements under infrared light. Sleep labs use clinical-grade EEG devices to classify sleep stages into categories including wake, N1-N3 (non-REM stages), and REM. Automated classifiers like ezscore and DreamentoScorer use AI to analyze sleep data and identify these stages.

<details><summary>References</summary>
<ul>
<li><a href="https://lucidcode.com/2026/06/20/inspec-with-cgx-patch-clinical-eeg-sleep-stage-classification/">INSPEC with CGX Patch Clinical EEG Sleep Stage... | lucidcode</a></li>
<li><a href="https://arxiv.org/pdf/1811.04662">Detection of REM Sleep Behaviour Disorder by</a></li>
<li><a href="https://stumejournals.com/journals/mm/2024/2/71.full.pdf">Keywords : SLEEP MONITORING, OCULOGRAPH, EYE ...</a></li>

</ul>
</details>

**Tags**: `#sleep-monitoring`, `#REM-detection`, `#computer-vision`, `#biomedical-engineering`, `#hardware`

---

<a id="item-8"></a>
## [Azure Functions Launches Serverless Agent Runtime at Build 2026](https://www.infoq.cn/article/kGHZu2K5V8IrwYvo6Cm3?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Microsoft released the Azure Functions Serverless Agent Runtime in public preview at Build 2026, enabling developers to deploy AI agents on serverless infrastructure using .agent.md markdown files with YAML triggers. This combines two major cloud computing trends—serverless computing and AI agents—allowing developers to build agentic applications without managing infrastructure. It could significantly impact how enterprise applications are developed and deployed on Azure. Agents are defined in .agent.md files with YAML triggers, MCP server access, and 1,400+ connectors, running in sandboxed execution for security. The runtime handles triggers, model clients, tools, session storage, identity, and observability automatically.

rss · InfoQ 中文站 · Jul 6, 09:19

**Background**: Azure Functions is Microsoft's serverless compute service that automatically scales based on demand. AI agents are autonomous software programs that can reason, plan, and execute tasks using AI models. Serverless computing eliminates server management while agentic AI represents a shift toward more autonomous AI systems.

<details><summary>References</summary>
<ul>
<li><a href="https://techcommunity.microsoft.com/blog/appsonazureblog/introducing-the-azure-functions-serverless-agents-runtime-preview/4523804">Introducing the Azure Functions serverless agents runtime (preview) | Microsoft Community Hub</a></li>
<li><a href="https://www.infoq.com/news/2026/06/azure-functions-serverless-agent/">Azure Functions Ships Serverless Agents Runtime at Build 2026 - InfoQ</a></li>
<li><a href="https://learn.microsoft.com/en-us//azure/Azure-functions/functions-serverless-agents-runtime">Serverless agents runtime in Azure Functions | Microsoft Learn</a></li>

</ul>
</details>

**Tags**: `#Azure Functions`, `#Serverless`, `#AI Agents`, `#Microsoft Azure`, `#Build 2026`

---

<a id="item-9"></a>
## [Hong Kong Handles Over Half of China's Chip Imports, Record High](https://thenextweb.com/news/hong-kong-china-ai-chip-trade-hub) ⭐️ 7.0/10

In the first five months of 2026, Hong Kong processed $124 billion worth of chips destined for mainland China, accounting for 52% of China's total chip purchases - a historical high, up from just one-third a decade ago. This positions Hong Kong as a critical AI trade hub in Asia, with AI-related electronics now comprising 57-70% of its exports. However, this intermediary role also exposes Hong Kong to significant geopolitical risks from US-China tensions over semiconductor technology. Hong Kong's advantages include its free port status, zero tariffs, no capital controls, and a well-developed air cargo network - particularly suited for high-value, low-weight, time-sensitive semiconductor products. The HKTDC has raised its 2026 export growth forecast to over 20%.

telegram · zaihuapd · Jul 5, 02:45

**Background**: Hong Kong has long served as a strategic gateway between mainland China and global markets, leveraging its free port status and business-friendly policies. The dramatic increase in chip transit reflects the intensifying US-China tech competition, as both nations impose increasingly restrictive export controls on advanced semiconductors. Hong Kong's intermediary position allows it to facilitate trade while potentially exposing it to secondary sanctions risk from Washington.

<details><summary>References</summary>
<ul>
<li><a href="https://www.amz123.com/t/Z7sCjYhY">amz123.com/t/Z7sCjYhY</a></li>
<li><a href="https://www.yearbook.gov.hk/2002/shtml/c03-01.htm">第 三 章 ： 经济 ： 经 济 结 构 与 发 展</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#Hong Kong`, `#trade`, `#AI`, `#geopolitics`, `#supply chain`

---

<a id="item-10"></a>
## [China Debates Cutting SCI Publication Incentives Over Security](https://www.ft.com/content/64a811f1-b132-4211-8a8c-2252cf964039?syn-25a6b1a6=1) ⭐️ 7.0/10

China's policymakers are discussing reducing incentives for researchers to publish in international journals, considering lowering the weight of SCI papers in academic promotions and tenure decisions. The move is driven by national security concerns that academic papers may serve as channels for industrial and technological innovation leakage. This represents a significant shift in China's approach to international academic collaboration and could reshape global research partnerships. The policy could impact millions of Chinese researchers and fundamentally alter the flow of scientific knowledge between China and the international academic community. China's Ministry of National Security accused a researcher last month of leaking core equipment structure and key experimental data in pursuit of international journal publication. Since August last year, authorities have strengthened regulation of foreign academic publishing, with the National Natural Science Foundation of China requiring funded projects to publish at least 20% of representative papers in Chinese journals.

telegram · zaihuapd · Jul 6, 01:03

**Background**: SCI (Science Citation Index) is a citation indexing service maintained by Clarivate that tracks publications in science journals worldwide and is widely used to evaluate research quality. The National Natural Science Foundation of China (NSFC) is a major funding body for basic research in China. Chinese universities and research institutions have traditionally heavily weighted SCI publications in faculty promotions and tenure decisions, creating strong incentives for researchers to publish in international journals.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Web_of_Science">Web of Science - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/National_Natural_Science_Foundation_of_China">National Natural Science Foundation of China - Wikipedia</a></li>
<li><a href="https://zh.wikipedia.org/wiki/国家自然科学基金委员会">国家自然科学基金委员会 - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**Discussion**: One community comment suggested the policy could help combat academic fraud, noting that the real motivation might be addressing issues of academic integrity rather than just security concerns.

**Tags**: `#academic-publishing`, `#national-security`, `#china-policy`, `#research-regulation`, `#technology-transfer`

---