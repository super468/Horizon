---
layout: default
title: "Horizon Summary: 2026-07-19 (EN)"
date: 2026-07-19
lang: en
---

> From 103 items, 16 important content pieces were selected

---

1. [GPT-5.6 Sol Pro Solves 30-Year Convex Optimization Problem](#item-1) ⭐️ 8.0/10
2. [LG Monitors Silent Software Install via Windows Update](#item-2) ⭐️ 8.0/10
3. [Fable 5 vs GPT-5.6 Benchmark Tests /goal Feature on NP-Hard Problem](#item-3) ⭐️ 7.0/10
4. [Spare Mac Setup for Claude Code Control Tutorial](#item-4) ⭐️ 7.0/10
5. [Kimi K3: Chinese AI Model Challenges Frontier Models](#item-5) ⭐️ 7.0/10
6. [Period Tracker Apps Privacy Risks Exposed](#item-6) ⭐️ 7.0/10
7. ["Context Bombing" Defenses Stop Malicious AI Hacking Agents](#item-7) ⭐️ 7.0/10
8. [Controlling Reasoning Effort in LLMs](#item-8) ⭐️ 7.0/10
9. [Tencent Releases Three Embodied AI Foundation Models with 95%+ Success](#item-9) ⭐️ 7.0/10
10. [Why AI Agents Struggle with Reasoning Despite Data Access](#item-10) ⭐️ 7.0/10
11. [Volcano Engine Rebuilds Multimodal Transmission for Doubao Video Calls](#item-11) ⭐️ 7.0/10
12. [SpaceX in Talks to Provide AI Computing Power to Pentagon](#item-12) ⭐️ 7.0/10
13. [Kimi K3 Released: World's First Open-Source 2.8T Parameter Model](#item-13) ⭐️ 7.0/10
14. [TSMC Announces A14 1.4nm Process for 2028 Production](#item-14) ⭐️ 7.0/10
15. [US Considers FINRA-Like AI Watchdog for Model Review](#item-15) ⭐️ 7.0/10
16. [SF Orders Apple and Google to Remove Nudify Apps](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [GPT-5.6 Sol Pro Solves 30-Year Convex Optimization Problem](https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/) ⭐️ 8.0/10

OpenAI's GPT-5.6 with Sol Pro solved a 30-year-old convex optimization problem regarding upper bounds on time complexity for optimizing convex Lipschitz functions over spherical domains. This represents a genuine contribution to mathematical research in convex optimization, demonstrating AI's growing capability to solve non-trivial mathematical problems that have stumped researchers for decades. The claimed '148 minutes' actually represents 'a year plus 148 minutes' - the problem author had been working on this problem for a year with GPT 5.4 and 5.5 before the successful run with Sol Pro. Additionally, the prompt appears to have included the technique used to solve the problem. The problem concerned upper bounds on time complexity in derivative-free convex optimization.

hackernews · mbustamanter · Jul 18, 13:00

**Background**: Convex optimization is a branch of mathematical optimization that deals with minimizing convex functions over convex sets. The time complexity of such problems measures how the computational cost grows with problem size. The problem specifically concerned convex Lipschitz functions on spherical domains, which are common in theoretical computer science and applied mathematics.

<details><summary>References</summary>
<ul>
<li><a href="https://llm24.net/model/gpt-5-6-sol-pro">OpenAI : GPT-5.6 Sol Pro - OpenAI - Model Price & Provider... - LLM24</a></li>
<li><a href="https://arxiv.org/pdf/2607.13335">Closing the Oracle-Complexity Gap in Derivative-Free Convex ...</a></li>

</ul>
</details>

**Discussion**: The community discussion provided important context: some commenters noted this represents a real contribution but is more niche than the cyclic double cover conjecture. There was debate about whether mathematicians will be made obsolete, with one view being that researchers will shift to problems requiring genuinely novel approaches rather than low-hanging fruit. The distinction between Sol Pro and Ultra was also discussed, with Sol Pro being described as potentially a multi-agent system.

**Tags**: `#artificial-intelligence`, `#mathematics`, `#convex-optimization`, `#research-automation`, `#openai`

---

<a id="item-2"></a>
## [LG Monitors Silent Software Install via Windows Update](https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent) ⭐️ 8.0/10

LG monitors have been discovered silently installing third-party software through Windows Update without user consent when HDMI devices are connected, with the installed software having full system and internet access. This represents a serious security and privacy vulnerability as users have no control over what software gets installed on their systems. The software runs at every system boot without sandboxing, creating potential for exploitation by malicious actors. The software being installed is LG OnScreen Control, which provides monitor management features like Screen Split and display settings. Users can disable automatic installation through Group Policy Editor (gpedit.msc) or via System Properties > Hardware > Device Installation Settings.

hackernews · baranul · Jul 18, 10:21

**Background**: Windows Update automatically downloads and installs drivers and associated software from third-party hardware manufacturers to simplify the user experience. LG OnScreen Control is an official LG application that allows users to manage monitor features including Screen Split, monitor settings, and software updates from their PC. This mechanism can be exploited to install additional software without explicit user permission.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lg.com/levant_en/support/product-help/CT40011533-20155181426844">Help Library: Help Library: How to download the LG OnScreen ...</a></li>
<li><a href="https://support.microsoft.com/en-us/topic/understanding-driver-updates-dc88b4a0-bdc5-49d8-92ba-396ca39c90b7">Understanding driver updates | Microsoft Support</a></li>

</ul>
</details>

**Discussion**: 社区成员强调这个问题比最初报道的更严重，指出当任何HDMI设备插入时都会以零用户交互的方式发生此问题。提供了多种解决方法，包括通过gpedit.msc或sysdm.cpl禁用自动应用程序下载。评论者还指出，微软对这一安全漏洞负有责任，因为该公司控制着通过Windows Update安装的软件，目前并未强制执行禁止捆绑无关软件的指南。

**Tags**: `#security`, `#privacy`, `#windows-update`, `#lg-monitors`, `#software-install`

---

<a id="item-3"></a>
## [Fable 5 vs GPT-5.6 Benchmark Tests /goal Feature on NP-Hard Problem](https://charlesazam.com/blog/fable-5-gpt-5-6-sol-goal/) ⭐️ 7.0/10

A benchmark comparison tests Anthropic's Claude Fable 5 against OpenAI's GPT-5.6 on an NP-Hard optimization problem, specifically evaluating whether the /goal prompt feature improves AI coding assistant problem-solving performance. This benchmark provides practical insights for developers choosing between Claude and OpenAI tools for coding tasks, revealing how different search strategies and prompt features impact performance on computationally hard problems. The benchmark uses an NP-Hard problem to evaluate performance, with specific attention to whether the /goal feature (which helps AI focus on specific objectives) provides meaningful improvements. One commenter noted the chart has an inverted y-axis causing visual confusion.

hackernews · couAUIA · Jul 18, 11:00

**Background**: Fable 5 (Claude Fable 5) is Anthropic's first publicly available Mythos-class AI model, released June 9, 2026, and currently the highest-scoring model on FrontierBench for coding evaluations. NP-Hard problems are a class of computational problems that are at least as hard as the hardest problems in NP, commonly used to benchmark AI reasoning capabilities. The /goal feature is a prompt engineering technique that helps AI assistants maintain focus on specific objectives during problem-solving.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://fable5.dev/">Fable5 — Claude Fable 5, Anthropic's First Public Mythos AI</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5</a></li>

</ul>
</details>

**Discussion**: Comments reveal mixed perspectives: one user found the chart visualization confusing due to the inverted y-axis; another suggested Ultra mode might outperform /goal for search strategies; a developer shared personal experience preferring Codex over Claude Code due to speed issues; one user noted Claude tends to forget important instructions in long sessions, speculating that /goal could help; and a commenter observed GPT should excel at optimization given OpenAI's recent AtCoder Heuristics competition win.

**Tags**: `#AI`, `#benchmark`, `#Claude`, `#GPT`, `#software-engineering`

---

<a id="item-4"></a>
## [Spare Mac Setup for Claude Code Control Tutorial](https://ykdojo.github.io/claude-controls-mac/) ⭐️ 7.0/10

A new tutorial provides step-by-step instructions for setting up a spare Mac to be controlled by Claude Code, Anthropic's AI coding agent, enabling users to repurpose older Apple hardware as dedicated agent environments. This matters because it enables developers to isolate AI agents on dedicated hardware, which is useful for continuous 24/7 tasks, user acceptance testing, and home automation integration without risking the primary development machine. The tutorial focuses on physical hardware isolation, but community commenters point out that virtual machines using libvirt can provide similar isolation with faster recovery times - a VM can be dumped and reinstalled in seconds if the agent makes a mess.

hackernews · ykev · Jul 18, 16:12

**Background**: Claude Code is Anthropic's agentic coding tool that lives in the terminal, understands codebases, and executes tasks through natural language commands. Isolating AI agents is important because they can make unintended changes to systems. Physical hardware isolation uses a separate machine, while VM-based isolation (using tools like Firecracker or libvirt) provides similar protection with more flexibility.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://github.com/anthropics/claude-code">GitHub - anthropics/claude-code: Claude Code is an agentic ...</a></li>
<li><a href="https://northflank.com/blog/how-to-sandbox-ai-agents">How to sandbox AI agents in 2026: MicroVMs, gVisor & isolation strategies | Blog — Northflank</a></li>

</ul>
</details>

**Discussion**: Community commenters offer alternatives: one suggests using libvirt VMs instead of physical hardware for agent isolation since VMs can be quickly reinstalled; another shares their experience using an old Mac running Home Bridge for home automation that Claude can interact with. Some express skepticism about using expensive Macs for simple API gateway tasks.

**Tags**: `#AI-Agents`, `#Claude-Code`, `#Automation`, `#DevTools`, `#Tutorial`

---

<a id="item-5"></a>
## [Kimi K3: Chinese AI Model Challenges Frontier Models](https://stephen.bochinski.dev/blog/2026/07/18/the-kimi-k3-moment/) ⭐️ 7.0/10

Moonshot AI released Kimi K3, an open-weight AI model that claims to rival leading models from OpenAI and Anthropic at a lower cost. The model represents what Moonshot calls "a new frontier of intelligence" and is reportedly the world's largest open AI model. This development signals that Chinese AI labs are closing the gap with American frontier labs, potentially reshaping the global AI competitive landscape. It also raises questions about model distillation as a technique and future regulatory implications for AI access. Kimi K3 requires at least a $79/month plan to access the 1M context model; the $15/month plan doesn't support K3 at all. One user reported the model took significantly longer and consumed almost an entire 5-hour usage limit on a coding task compared to OpenAI's model.

hackernews · sbochins · Jul 18, 17:32

**Background**: Model distillation is a technique where knowledge from a large model is transferred to a smaller, more cost-efficient model. Frontier models are the most advanced AI models at any given time, representing the leading edge of AI capability. Kimi is a series of large language models developed by Chinese company Moonshot AI, with Kimi K2 released in July 2025 as an open-weights model.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(chatbot)">Kimi (chatbot) - Wikipedia</a></li>
<li><a href="https://www.businessinsider.com/kimi-k3-ai-model-moonshot-china-open-weights-benchmarks-pricing-2026-7">Why China's Kimi K3 AI Model Has Silicon Valley Worried - Business Insider</a></li>
<li><a href="https://www.forbes.com/sites/tylerroush/2026/07/17/chinese-ai-startup-moonshot-unveils-kimi-k3-model-will-it-challenge-openai-and-anthropic/">Chinese AI Startup Moonshot Unveils Kimi K3 Model—Will It Challenge OpenAI And Anthropic?</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work | NVIDIA Glossary</a></li>

</ul>
</details>

**Discussion**: 社区成员讨论了人工智能发展中蒸馏技术的必然性，有人指出前沿实验室"蒸馏"了所有现有人类知识到他们的模型中。其他人则表达了对未来可能限制开源模型访问的法规的担忧，并将其比作Napster时代的文件共享。用户分享了定价细节，指出K3在更便宜的套餐中不可用。

**Tags**: `#AI`, `#Chinese AI`, `#model distillation`, `#Kimi K3`, `#AI policy`

---

<a id="item-6"></a>
## [Period Tracker Apps Privacy Risks Exposed](https://www.wired.com/story/security-news-this-week-your-period-tracker-is-probably-spying-on-you/) ⭐️ 7.0/10

Wired's weekly security roundup highlighted that many period tracker apps are collecting and potentially sharing sensitive personal health data with third parties. The article also covered Russian cyberspies targeting infrastructure systems, DHS repeatedly failing to detect it had been breached, and an AI music generator exposed for scraping training data without consent. 月经追踪应用从数百万用户那里收集高度敏感的健康信息，与第三方共享这些数据会带来重大隐私和安全风险。再加上基础设施黑客攻击威胁和未经授权的AI数据抓取，这凸显了日常应用中日益增长的数字隐私和数据保护问题。 The period tracker apps in question collect menstrual cycle data, symptoms, pregnancy status, and other intimate health information that could be exploited if shared with advertisers, insurance companies, or other third parties. The AI music generator incident exposed how some companies scrape copyrighted content from the web to train their models without artists' permission.

rss · WIRED AI · Jul 18, 10:30

**Background**: Period tracking apps store highly personal health data including menstrual cycles, symptoms, and sometimes pregnancy intentions, making them attractive targets for data breaches or surveillance. Infrastructure hacking refers to cyberattacks targeting critical systems such as power grids, water supplies, and transportation networks. Data scraping for AI training involves collecting large amounts of content from the internet to train machine learning models, often without the original creators' knowledge or consent.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cyberattacks_against_infrastructure">Cyberattacks against infrastructure - Wikipedia</a></li>
<li><a href="https://scrapebadger.com/blog/how-to-scrape-data-for-ai-training-datasets-2026-guide">How to Scrape Data for AI Training Datasets (2026 Guide)</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#security`, `#mobile-apps`, `#data-breach`, `#surveillance`

---

<a id="item-7"></a>
## ["Context Bombing" Defenses Stop Malicious AI Hacking Agents](https://www.wired.com/story/prompt-injection-attacks-are-thwarting-ai-hacking-agents/) ⭐️ 7.0/10

Security researchers have demonstrated that 'context bomb' prompt injection attacks can successfully defend against malicious AI hacking agents by tricking them into shutting down before they can cause harm. This represents a novel defensive application of prompt injection techniques, turning an established attack method into a protective tool against autonomous AI agents being used for hacking. As AI agents increasingly automate offensive security tasks, this defense provides a new layer of protection. The researchers created canaries containing 'context bombs' - short text designed to trigger safety guardrails in offensive AI agents. They tested these against agents powered by Anthropic's Opus 4.8 and Google's Gemini 3.1 Pro.

rss · WIRED AI · Jul 18, 09:00

**Background**: Prompt injection is an attack technique where malicious instructions are embedded in input data to manipulate AI model behavior, overriding original system prompts. Autonomous AI hacking agents are increasingly deployed for offensive security tasks - these models can scan codebases, identify misconfigurations, and execute exploit steps with machine precision. This defensive technique leverages the same vulnerability that makes prompt injection dangerous.

<details><summary>References</summary>
<ul>
<li><a href="https://www.helpnetsecurity.com/2026/07/14/context-bombs-for-defensive-prompt-injection/">"Context bombs" can frustrate AI-driven attacks, researchers found - Help Net Security</a></li>
<li><a href="https://arstechnica.com/security/2026/07/now-defenders-are-embracing-the-prompt-injection-too/">Now, defenders are embracing the prompt injection, too - Ars Technica</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#prompt injection`, `#AI agents`, `#cybersecurity`, `#defensive security`

---

<a id="item-8"></a>
## [Controlling Reasoning Effort in LLMs](https://magazine.sebastianraschka.com/p/controlling-reasoning-effort-in-llms) ⭐️ 7.0/10

Sebastian Raschka explains how large language models can be trained to operate in different reasoning effort modes—low, medium, and high—allowing them to balance computational efficiency against reasoning performance. This approach addresses a critical trade-off in LLM deployment: faster responses versus thorough answers, and lower token costs versus superior accuracy. It enables dynamic resource allocation based on task complexity, making AI systems more efficient and cost-effective. The article explores training paradigms that teach LLMs to modulate their reasoning depth, similar to the reasoning effort controls built into OpenAI's o1 and o3-mini models. This relates to test-time scaling approaches that optimize inference compute allocation.

rss · Sebastian Raschka · Jul 18, 11:16

**Background**: Recent advances in LLM training have led to breakthroughs in reasoning performance. There's a fundamental trade-off in LLM inference between computational cost (measured in tokens processed) and reasoning quality. OpenAI's o1 model marked a significant milestone as the first reasoning-focused model, while o3-mini introduced explicit reasoning effort modes for users to choose between faster/cheaper or more accurate/thorough responses.

<details><summary>References</summary>
<ul>
<li><a href="https://lifeboat.com/blog/2026/07/controlling-reasoning-effort-in-llms">Controlling Reasoning Effort in LLMs – Lifeboat News: The Blog</a></li>
<li><a href="https://arxiv.org/abs/2503.15113">Reasoning Effort and Problem Complexity: A Scaling Analysis in LLMs</a></li>
<li><a href="https://www.requesty.ai/blog/fine-tune-your-ai-on-the-fly-quick-reasoning-with-openai-o3-mini-requesty">Fine-Tune Your AI on the Fly: Quick Reasoning with... | Requesty</a></li>

</ul>
</details>

**Tags**: `#large-language-models`, `#ai-research`, `#model-optimization`, `#reasoning-systems`, `#llm-inference`

---

<a id="item-9"></a>
## [Tencent Releases Three Embodied AI Foundation Models with 95%+ Success](https://www.infoq.cn/article/uD0p2FcQE2JKSwYY1wXK?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Tencent released three embodied AI foundation models that integrate perception-action loops, achieving over 95% success rate in industrial testing. This represents a significant breakthrough in embodied AI, an important frontier field combining AI and robotics. The perception-action loop integration is a key technical challenge that, when solved, enables robots to perform complex industrial tasks autonomously with high reliability. The three foundation models are designed to work together to enable robots to perceive their environment and take appropriate actions. Achieving over 95% success rate in real industrial testing demonstrates these models are approaching practical deployment readiness for manufacturing and automation scenarios.

rss · InfoQ 中文站 · Jul 19, 07:55

**Background**: Embodied Intelligence (具身智能) is a frontier field at the intersection of AI and robotics, emphasizing intelligent agents with physical bodies that interact with their environment. The core concept is fusing perception, action, and cognition. First proposed by Turing in 1950, the field has evolved through Brooks' behavior-based robotics in the 1980s. Today, embodied AI has moved from laboratories to real-world applications in medical, industrial automation, and home service sectors.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/具身智能">具身智能 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.amazonaws.cn/what-is/embodied-intelligence/">具身智能是什么 - 亚马逊云科技</a></li>

</ul>
</details>

**Tags**: `#embodied AI`, `#Tencent`, `#foundation models`, `#robotics`, `#Chinese AI`

---

<a id="item-10"></a>
## [Why AI Agents Struggle with Reasoning Despite Data Access](https://www.infoq.cn/article/KPd6YwU0Y1iCMGMakSmE?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

At AICon Shenzhen, a technical talk addressed the core challenge of why AI Agents can access data but fail to reason effectively, presenting an observable object graph semantic layer design and its open-source implementation as a solution. This addresses a fundamental engineering bottleneck in AI Agent development—while agents can retrieve data, they lack the architectural foundation to perform complex reasoning over that data. The semantic layer approach could significantly improve agent reliability and debugging capabilities in production systems. The talk focused on combining observability (monitoring agent behavior) with semantic layer architecture (abstracting data into business-understandable objects), enabling developers to trace reasoning paths and debug failures more effectively.

rss · InfoQ 中文站 · Jul 18, 10:00

**Background**: AI Agents powered by LLMs often face a 'reasoning gap' where they can access vast amounts of data but struggle to perform multi-step reasoning. Semantic layers traditionally sit between raw data and analytical applications, translating tables and fields into business objects. Observability in AI systems is critical because agent behavior is non-deterministic, making traditional debugging methods inadequate.

<details><summary>References</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/2003761515438811109">【Agent入门到精通】13-生产级Agent架构：可靠性、安全性与可观测性 - 知乎</a></li>
<li><a href="https://aloudata.com/resources/compare/data-modeling/semantic-layer-vs-data-middle-platform">语义层 vs 数 据 中台：企业该先做哪一层？</a></li>

</ul>
</details>

**Tags**: `#AI Agents`, `#Observability`, `#Semantic Layer`, `#LLM Engineering`, `#AI Architecture`

---

<a id="item-11"></a>
## [Volcano Engine Rebuilds Multimodal Transmission for Doubao Video Calls](https://www.infoq.cn/article/GICIrEsTJwEgGsDYFvCM?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Volcano Engine unveiled a new-generation multimodal transmission infrastructure built specifically for Doubao's video calling capabilities, representing a complete rebuild of their real-time communication foundation for the AI Agent era. This infrastructure rebuild addresses the unique challenges of real-time multimodal interaction in AI agents, which require seamless integration of voice, video, and vision capabilities at scale. As AI agents become more prevalent, having purpose-built transmission infrastructure becomes critical for delivering responsive and natural user experiences. The new transmission foundation optimizes for low-latency multimodal data flow, supporting the demanding requirements of real-time AI agent interactions including video analysis, voice response, and continuous context maintenance. This represents a shift from general-purpose real-time communication to AI-native infrastructure design.

rss · InfoQ 中文站 · Jul 18, 08:54

**Background**: Volcano Engine is ByteDance's cloud computing arm that provides technical support for Doubao, ByteDance's AI assistant. AI Agent represents an emerging paradigm in artificial intelligence systems that can autonomously execute complex tasks while maintaining contextual understanding. Multimodal transmission involves real-time synchronized processing of voice, video, and text data. The rapid development of large language models has created new demands for real-time communication infrastructure to adapt to AI-native design requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://juejin.cn/post/7602205524719091746">火 山 引 擎 正式上线 102.4T 自研交换机，构建 AI 网络新 底 座 从 AI...</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/707504322">深度盘点 AI Agent 基础设施 - 知乎</a></li>

</ul>
</details>

**Tags**: `#多模态AI`, `#实时通信`, `#火山引擎`, `#AI Agent`, `#视频通话`, `#基础设施`

---

<a id="item-12"></a>
## [SpaceX in Talks to Provide AI Computing Power to Pentagon](https://www.wsj.com/tech/ai/spacex-in-talks-to-provide-computing-power-for-pentagons-ai-push-15e752e4) ⭐️ 7.0/10

SpaceX is negotiating with the US Pentagon to provide data center computing power for running AI models, in a deal that could be worth billions of dollars. The talks are ongoing and could still fall apart, according to知情人士。 This deal represents a major expansion of SpaceX's cloud services into defense AI applications. As the Pentagon accelerates its acquisition of cloud computing capabilities for national security and battlefield AI applications, this partnership could reshape how the US military leverages commercial AI infrastructure. The Pentagon has recently approved SpaceX, Amazon, Google, Microsoft, and Oracle to operate their AI models in classified environments. SpaceX has also signed similar computing power supply agreements with Anthropic and Google in recent months, signaling plans to significantly expand its cloud computing business.

telegram · zaihuapd · Jul 18, 01:44

**Background**: SpaceX, founded by Elon Musk, is primarily known as a space exploration company but has been expanding into cloud and AI infrastructure services. Anthropic is a San Francisco-based AI company founded in 2021 by former OpenAI members, focused on AI safety. Its flagship product is Claude, a series of large language models. The Pentagon has been rapidly seeking cloud computing capabilities to support AI applications in national security and military operations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(AI)">Claude (AI) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#Pentagon`, `#AI Computing`, `#Defense Contracts`, `#Cloud Infrastructure`

---

<a id="item-13"></a>
## [Kimi K3 Released: World's First Open-Source 2.8T Parameter Model](https://t.me/zaihuapd/42637) ⭐️ 7.0/10

Moonshot AI released Kimi K3, the world's first open-source 2.8 trillion parameter model, featuring Kimi Delta Attention (KDA) and Attention Residuals architecture, with native visual understanding and a 1 million token context window. Kimi K3 achieved #1 ranking in Frontend Code Arena with 1679 points, jumping from Kimi k2.6's 18th place to the top, demonstrating significant breakthrough in frontend coding capabilities and validating the new hybrid linear attention architecture. The model uses a hybrid 3:1 ratio of KDA to global attention layers, combining efficient linear attention with traditional full attention. It won 6 out of 7 evaluation domains in Frontend Code Arena, only trailing in gaming domain.

telegram · zaihuapd · Jul 18, 02:29

**Background**: Kimi Delta Attention (KDA) is a linear attention mechanism that refines Gated DeltaNet with per-channel decay control, enabling more precise memory management. Attention Residuals replaces the fixed addition mechanism with a dynamic, learnable process. The Frontend Code Arena is a third-party benchmark that evaluates AI models' frontend coding capabilities through developer voting.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MoonshotAI/Kimi-Linear">GitHub - MoonshotAI/Kimi-Linear</a></li>
<li><a href="https://codersera.com/blog/kimi-k3-benchmarks-comparison-2026/">Kimi K3 Benchmarks vs Fable 5, GPT-5.6 & Opus</a></li>
<li><a href="https://digg.com/tech/we56zqdp">Chinese model Kimi-K3 tops Frontend Code Arena benchmark · Digg</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Open Source`, `#Model Release`, `#Benchmark`, `#Kimi`

---

<a id="item-14"></a>
## [TSMC Announces A14 1.4nm Process for 2028 Production](https://t.me/zaihuapd/42643) ⭐️ 7.0/10

TSMC has announced its next-generation A14 (1.4nm) process technology scheduled for 2028 production, with the intermediate A16 node planned for late 2026. Compared to the N2 process, A14 delivers up to 15% speed improvement at same power, or 30% power reduction at same speed, with over 20% logic density gains. This announcement demonstrates TSMC's continued leadership in advanced semiconductor manufacturing, which is critical for AI accelerators and next-generation smartphone chips. The A14 node will help TSMC maintain its competitive edge over rivals like Samsung and Intel in the ultra-advanced process market. The A14 process is progressing smoothly and ahead of schedule, with risk production expected to begin in 2027 and full manufacturing in 2028. TSMC has already started construction of its 1.4nm advanced process facility in Central Taiwan Science Park ahead of schedule.

telegram · zaihuapd · Jul 18, 05:00

**Background**: Semiconductor process nodes (like 3nm, 2nm, 1.4nm) refer to the manufacturing technology node and indicate the density and performance capabilities of chips. Smaller process nodes allow more transistors in the same area, improving performance and efficiency. N2 is TSMC's 2nm process that will enter mass production later this year. The A16 serves as an intermediate node between N2 and A14.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tweaktown.com/news/107877/tsmcs-next-gen-a14-1-4nm-process-node-is-progressing-smoothly-and-is-ahead-of-schedule/index.html">TSMC 's next-gen A 14 ( 1 . 4 nm ) process node is 'progressing smoothly...</a></li>
<li><a href="https://wccftech.com/tsmc-1-4nm-process-faces-no-obstacles-as-risk-production-to-start-in-2027/">TSMC ’s Facing No Development Obstacles With Its Next-Generation...</a></li>

</ul>
</details>

**Tags**: `#TSMC`, `#semiconductors`, `#chip manufacturing`, `#A14 process`, `#technology roadmap`

---

<a id="item-15"></a>
## [US Considers FINRA-Like AI Watchdog for Model Review](https://www.bloomberg.com/news/articles/2026-07-17/us-considers-creating-finra-like-watchdog-to-vet-top-ai-models) ⭐️ 7.0/10

The Trump administration is considering establishing an independent AI regulatory agency similar to FINRA (Financial Industry Regulatory Authority) to review top AI models for safety. The agency would report to the SEC and is being led by Treasury Secretary Scott Bessent, with the proposal currently under review by White House Chief of Staff Susie Wiles. This represents a concrete step toward formalizing AI safety reviews in the US, moving beyond temporary measures to a structured regulatory framework. The proposal addresses concerns from both Wall Street about cybersecurity risks and Silicon Valley about government-imposed restrictions, potentially giving both industries greater voice in jointly developing safety standards. The proposal aligns with DeepMind CEO Demis Hassabis's suggestion for an industry-funded independent regulator. Both Anthropic and OpenAI have previously objected to government requests to modify or limit releases of their latest models. President Trump has not yet reviewed the proposal, and the framework remains subject to change.

telegram · zaihuapd · Jul 18, 05:45

**Background**: FINRA (Financial Industry Regulatory Authority) is a self-regulatory organization that oversees brokerage firms and their registered representatives in the United States. While not a government agency, it operates under SEC oversight and plays a crucial role in regulating the securities industry. The proposed AI watchdog would follow a similar model - an independent body with industry participation but operating under government supervision to review and set safety standards for advanced AI systems.

<details><summary>References</summary>
<ul>
<li><a href="https://brokercheck.finra.org/">brokercheck. finra .org</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#US government policy`, `#AI safety`, `#technology policy`, `#federal oversight`

---

<a id="item-16"></a>
## [SF Orders Apple and Google to Remove Nudify Apps](https://techcrunch.com/2026/07/17/apple-and-google-ordered-to-purge-nudify-apps-from-app-stores/) ⭐️ 7.0/10

San Francisco City Attorney David Chiu ordered Apple and Google to remove dozens of AI-powered 'nudify' apps from their app stores, which use artificial intelligence to create non-consensual intimate deepfake images by digitally removing clothing from photos. This represents the first major regulatory enforcement action directly targeting both Apple and Google for hosting non-consensual intimate deepfake apps, holding them accountable for willful negligence and potentially millions in revenue from these harmful applications. Apple stated it has removed 3 apps and terminated associated developer accounts, while Google announced it has suspended 5 named Play Store apps. The City Attorney's office sent formal letters claiming both companies were aware of these apps charging users on their platforms but failed to act promptly.

telegram · zaihuapd · Jul 18, 08:45

**Background**: Nudify apps are AI-powered applications that use deep learning algorithms to generate synthetic nude images of individuals without their consent. Research shows approximately 96-98% of deepfake videos online are non-consensual intimate imagery, with 99-100% of depicted individuals being women. These apps represent a significant form of image-based sexual abuse enabled by generative AI technology.

<details><summary>References</summary>
<ul>
<li><a href="https://indianexpress.com/article/technology/tech-news-technology/ai-nudify-apps-spark-legal-action-against-apple-google-in-us-10792608/">AI ‘nudify’ apps spark legal action against Apple, Google in US</a></li>
<li><a href="https://www.newamerica.org/insights/a-weapon-against-women-in-politics/defining-nonconsensual-synthetic-intimate-imagery/">Defining Nonconsensual Synthetic Intimate Imagery - New America</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#deepfakes`, `#non-consensual intimate imagery`, `#platform accountability`, `#Apple`, `#Google`

---