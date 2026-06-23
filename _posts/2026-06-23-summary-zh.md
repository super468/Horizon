---
layout: default
title: "Horizon Summary: 2026-06-23 (ZH)"
date: 2026-06-23
lang: zh
---

> From 159 items, 27 important content pieces were selected

---

1. [Prompt Injection as Role Confusion](#item-1) ⭐️ 8.0/10
2. [Deno 发布桌面运行时以构建桌面应用](#item-2) ⭐️ 8.0/10
3. [OpenAI 扩展 Daybreak 计划，修复 30 多个开源项目漏洞](#item-3) ⭐️ 8.0/10
4. [NVIDIA Halos：面向 Physical AI 机器人的全栈安全系统](#item-4) ⭐️ 8.0/10
5. [研究发现人工智能说服能力超越人类专家](#item-5) ⭐️ 8.0/10
6. [Event Tensor：动态 Megakernel 编译的统一抽象](#item-6) ⭐️ 8.0/10
7. [Valve 推出 Steam Machine 游戏主机](#item-7) ⭐️ 7.0/10
8. [加拿大计划到 2040 年建设最多 10 座核反应堆](#item-8) ⭐️ 7.0/10
9. [Oak：为 AI 代理设计的 Git 替代方案](#item-9) ⭐️ 7.0/10
10. [警察局长滥用 Flock 车牌识别器无证追踪女性](#item-10) ⭐️ 7.0/10
11. [雪佛龙与微软签署德州西部数据中心 20 年供电协议](#item-11) ⭐️ 7.0/10
12. [OpenAI 推出 Daybreak 安全工具助力漏洞管理](#item-12) ⭐️ 7.0/10
13. [AWS 多模态 AI 可搜索航空影像技术](#item-13) ⭐️ 7.0/10
14. [NVIDIA 发布新型 AI 软件助力科学研究](#item-14) ⭐️ 7.0/10
15. [CCCL Runtime：面向 CUDA 的现代 C++运行时](#item-15) ⭐️ 7.0/10
16. [NVIDIA DAQIRI 实现高速数据采集的实时 AI 处理](#item-16) ⭐️ 7.0/10
17. [Meta 意外内部暴露员工按键数据](#item-17) ⭐️ 7.0/10
18. [将 Moebius 0.2B 图像修复模型移植到浏览器运行](#item-18) ⭐️ 7.0/10
19. [AI 安全需要与传统网络安全不同的方法](#item-19) ⭐️ 7.0/10
20. [libvfio-user：虚拟机监视器的外部设备仿真库](#item-20) ⭐️ 7.0/10
21. [TIRx：面向前沿 ML 内核的开源编译器栈](#item-21) ⭐️ 7.0/10
22. [Netflix 如何实时绘制数千个微服务的拓扑图](#item-22) ⭐️ 7.0/10
23. [Discord 以自动化重构数据库运维，以管理超大规模的 ScyllaDB](#item-23) ⭐️ 7.0/10
24. [快手 AI 赋能功能开关全生命周期治理方案](#item-24) ⭐️ 7.0/10
25. [内核级的真相：为什么 eBPF 正在取代用户空间 Agent 成为安全可观测性的首选](#item-25) ⭐️ 7.0/10
26. [英伟达 CEO 黄仁勋盛赞华为为 AI 芯片领域强劲竞争对手](#item-26) ⭐️ 7.0/10
27. [48 位中国开发者举报苹果涉嫌垄断](#item-27) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Prompt Injection as Role Confusion](https://role-confusion.github.io/) ⭐️ 8.0/10

Blog writeup summarizing arxiv paper on prompt injection via role confusion, highlighting that LLM guardrails fail against adaptive human attackers despite near-perfect benchmark scores.

hackernews · Lobsters - AI · Jun 22, 15:48

**标签**: `#prompt-injection`, `#llm-security`, `#ai-safety`, `#red-teaming`, `#jailbreaking`

---

<a id="item-2"></a>
## [Deno 发布桌面运行时以构建桌面应用](https://docs.deno.com/runtime/desktop/) ⭐️ 8.0/10

该运行时支持三种后端:CEF(Chromium 嵌入式框架)、Webview 和 Raw。如 CLI 参考文档所示,在编译时授予的权限会被嵌入到编译后的二进制文件中。

hackernews · GeneralMaximus · Jun 22, 05:38

**背景**: CEF(Chromium 嵌入式框架)是一个用于在应用程序中嵌入 Chromium 浏览器的开源框架,在全球已有超过 1 亿个安装实例。它提供稳定的 API 和二进制分发包。Deno 是由 Node.js 原创作者创建的现代 JavaScript 运行时,以其权限系统和内置 TypeScript 支持而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chromium_Embedded_Framework">Chromium Embedded Framework - Wikipedia</a></li>
<li><a href="https://github.com/chromiumembedded/cef">GitHub - chromiumembedded/cef: Chromium Embedded Framework (CEF). A simple framework for embedding Chromium-based browsers in other applications. · GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区成员讨论了共享 CEF 运行时的优势(可将二进制大小减少到几 MB)、不同应用间的版本控制挑战,以及与 Deno 权限系统的集成。有些人表示对 launch-in-browser 选项感兴趣。整体情绪积极,认可 Deno 生态系统的成熟。

**标签**: `#deno`, `#desktop-apps`, `#javascript-runtime`, `#chromium`, `#electron-alternative`

---

<a id="item-3"></a>
## [OpenAI 扩展 Daybreak 计划，修复 30 多个开源项目漏洞](https://openai.com/index/patch-the-planet/) ⭐️ 8.0/10

OpenAI 宣布扩展 Daybreak 网络安全计划，推出 Patch the Planet 倡议并与 Trail of Bits 等机构合作，使用 AI 模型配合人工审核帮助 cURL、Go、Python 等 30 多个开源项目发现和修复漏洞，目前已在 Linux、Chrome、Safari、Firefox 等系统中发现数百个安全问题并合并数十个补丁。 这代表了人工智能在网络安全领域的重大实际部署，展示了超越纯粹研究的真实世界影响，成功在 Linux 和主流浏览器等关键系统中发现并修复了漏洞。与 Trail of Bits 以及企业/政府机构的合作增强了可信性和可扩展性。 更新后的 Codex Security 插件和新发布的 GPT-5.5-Cyber 模型在 CyberGym 基准测试中达到 85.6%。OpenAI 启动了 Daybreak 网络安全合作伙伴计划，将防御能力整合到企业产品中，并通过 Trusted Access for Cyber 与澳大利亚、加拿大、日本及欧盟 ENISA 建立合作。

telegram · OpenAI News · Jun 23, 01:01

**背景**: Daybreak 是 OpenAI 于 2026 年 5 月推出的专门网络安全计划，结合前沿 AI 模型、Codex Security 工具和可信工作流程，帮助防御者在攻击者利用之前发现、验证和修复漏洞。Trail of Bits 是一家领先的网络安全研究公司，成立于 2012 年，曾与 DARPA、大型科技公司和加密货币协议合作。CyberGym 是评估 AI 智能体网络安全任务的基准测试，包括漏洞发现和安全分析。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/daybreak/">Daybreak | OpenAI for cybersecurity | OpenAI</a></li>
<li><a href="https://openai.com/index/daybreak-securing-the-world/">Daybreak: Tools for securing every organization in the world | OpenAI</a></li>
<li><a href="https://trailofbits.com/">Trail of Bits: Security Research, Audits, and Tools</a></li>
<li><a href="https://llm-stats.com/benchmarks/cybergym">CyberGym Benchmark Leaderboard | LLM Stats</a></li>

</ul>
</details>

**标签**: `#AI security`, `#vulnerability discovery`, `#open source security`, `#cybersecurity`, `#AI safety`

---

<a id="item-4"></a>
## [NVIDIA Halos：面向 Physical AI 机器人的全栈安全系统](https://developer.nvidia.com/blog/inside-nvidia-halos-for-robotics-a-full-stack-functional-safety-system-for-physical-ai/) ⭐️ 8.0/10

NVIDIA 发布了 Halos，这是一个全面的功能安全平台，适用于在工厂、仓库、医院和家庭等环境中与人类协同工作的 Physical AI 机器人。该系统集成了 AI 计算平台(IGX Thor)和专用安全操作系统，充分利用了超过十年的自动驾驶汽车安全研发经验，包含 18,000 工程年和 210 亿个安全晶体管。 这是行业内首个专门为 Physical AI 设计的统一全栈安全架构，解决了在人类环境中部署机器人的关键安全要求。企业现在可以依靠标准化的安全框架来加速机器人的实际部署，有望推动协作机器人的大规模应用。 Halos 平台连接了 AI 计算、系统软件、传感器数据、安全应用程序和机器人系统检测。该平台旨在满足 ISO 13849 功能安全标准，全球超过 89%的机器制造商都采用这一标准，为人形机器人和工业机器人提供标准化的安全方法。

rss · NVIDIA Developer Blog · Jun 22, 13:00

**背景**: Physical AI 是指在共享环境中与人类自主协同工作的机器人，代表了机器人技术和人工智能的融合。功能安全确保这些机器人能够在不伤害人类的情况下运行，ISO 13849 是机械设备安全的主流国际标准。NVIDIA 利用其自动驾驶汽车安全研究开发了这一全面解决方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/ai-trust-center/halos/robotics/">Robotics Functional Safety Platform | NVIDIA Halos</a></li>
<li><a href="https://en.wikipedia.org/wiki/ISO_13849">ISO 13849 - Wikipedia</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#Robotics`, `#Physical AI`, `#Functional Safety`, `#Industrial AI`

---

<a id="item-5"></a>
## [研究发现人工智能说服能力超越人类专家](https://jack-clark.net/2026/06/22/import-ai-462-superpersuasion-self-sustaining-ai-paths-to-asi/) ⭐️ 8.0/10

牛津大学、英国人工智能安全研究所和斯坦福大学的研究人员在《科学》杂志上发表了一项研究表明，通过对话改变政治态度方面，人工智能系统比人类专家更具有说服力。 这一发现对人工智能安全和治理具有重大意义，因为它表明人工智能在影响人类信念方面可以明显超越人类，引发人们对政治操纵和虚假信息运动潜在滥用的担忧。 这项名为《对话人工智能的政治说服杠杆》的研究通过大规模实验检验大型语言模型如何通过自然对话影响政治态度。

rss · Import AI · Jun 22, 12:31

**背景**: 人工超级智能（ASI）是指在几乎所有认知任务上超越人类能力的人工智能。"自维持人工智能"的概念涉及能够以最少人类干预自主运行和改进的系统。这项研究正值人们对人工智能影响公众舆论以及需要人工智能治理框架的关注日益增长之际。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.oii.ox.ac.uk/oxford-researchers-reveal-how-conversational-ai-can-change-political-opinions/">OII | Oxford and AISI researchers reveal how conversational AI can change political opinions</a></li>
<li><a href="https://www.aisi.gov.uk/blog/how-do-ai-models-persuade-exploring-the-levers-of-ai-enabled-persuasion-through-large-scale-experiments">How do AI models persuade? Exploring the levers of AI-enabled persuasion through large-scale experiments | AISI Work</a></li>
<li><a href="https://www.ox.ac.uk/news/2025-12-11-study-reveals-how-conversational-ai-can-exert-influence-over-political-beliefs">Study reveals how conversational AI can exert influence over political beliefs | Oxford University</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#AI persuasion`, `#AI research`, `#AI governance`, `#alignment`

---

<a id="item-6"></a>
## [Event Tensor：动态 Megakernel 编译的统一抽象](https://arxiv.org/abs/2604.13327) ⭐️ 8.0/10

一篇新的 arXiv 论文（2604.13327）提出了 Event Tensor，这是一个用于编译动态 megakernel 的统一编译器抽象。Event Tensor 编译器（ETC）利用符号事件张量抽象来管理 GPU 中的细粒度同步和动态调度，生成高性能的持久内核。 这项研究解决了现有 GPU 调度模型中的关键局限性，特别是对于动态大型语言模型（LLM）推理工作负载。它实现了最先进的延迟，同时显著减少了预热开销，使其与从事 GPU 优化工作的编译器和高性能计算社区高度相关。 Event Tensor 抽象允许同步事件和动态调度决策的符号表示，使编译器能够生成能够高效处理动态工作负载的优化 megakernel。该方法通过支持多个计算阶段的持久内核执行来减少预热开销。

rss · Lobsters - AI · Jun 22, 23:18

**背景**: Megakernel 是执行多个功能的单个 GPU 内核，代表了生产者-消费者内核优化的推广。这种方法对于 LLM 推理尤为重要，因为动态工作负载和多 GPU 通信会带来显著的调度挑战。Hazy Research 之前的演示表明，通过将 NVLink 通信与计算重叠，可以实现 8-GPU LLaMA-70B 的 megakernel。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/event-tensor-compiler-etc">Event Tensor Compiler (ETC)</a></li>
<li><a href="https://hyper.ai/en/papers/2604.13327">Event tensor : a unified abstraction for compiling ...</a></li>
<li><a href="https://hazyresearch.stanford.edu/blog/2025-09-22-pgl">One Kernel for All Your GPUs · Hazy Research</a></li>

</ul>
</details>

**社区讨论**: Lobste.rs 上的社区讨论表明，编译器和 GPU 计算社区对这项研究感兴趣。使用符号事件张量统一编译动态 megakernel 的技术方法被视为该领域的一项新颖贡献。

**标签**: `#research`, `#compilers`, `#gpu-computing`, `#optimization`, `#arxiv`

---

<a id="item-7"></a>
## [Valve 推出 Steam Machine 游戏主机](https://store.steampowered.com/news/group/45479024/view/685257114654870245) ⭐️ 7.0/10

Valve 今天推出了其 Steam Machine 游戏主机，采用随机预订系统以确保购买者的公平性。该设备设计为一台解锁的、可定制的 PC，专为游戏优化，还能够安装自定义应用甚至其他操作系统。 此次发布代表了 Valve 进入客厅游戏市场的重大举措，直接与 PlayStation 和 Xbox 等传统游戏主机竞争。随机预订系统解决了黄牛党长期以来存在的问题，以及限时发布对网络速度快或使用脚本的玩家造成的不公平困扰。 Steam Machine 采用定制的 Newell Nucleus 处理器，基于 AMD Zen 4 架构设计，六核十二线程，30W TDP，最高可 boost 至 4.8 GHz。定价从 1049 美元/879 英镑起，反映了自 2023 年以来从全球制造商采购的组件成本。

hackernews · theschwa · Jun 22, 17:09

**背景**: Steam Machine 是 Valve 将 PC 游戏带入客厅的尝试，通过专用设备弥合传统游戏主机与定制 PC 之间的差距。该设备运行 SteamOS，并采用可更换前面板的物理设计。随机预订系统取代了传统的先到先得模式，后者经常导致黄牛使用脚本抢货。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.lttlabs.com/articles/2026/06/22/the-newell-nucleus-steam-machine-ltt-companion-article">The Newell Nucleus: Steam Machine LTT Companion Article | LTT Labs</a></li>
<li><a href="https://www.tomshardware.com/video-games/console-gaming/valve-opens-steam-machine-reservations-details-usd1-049-starting-price-randomized-queue-to-stop-scalpers-and-limited-inventory">Valve opens Steam Machine reservations ... | Tom's Hardware</a></li>
<li><a href="https://www.rockpapershotgun.com/steam-machine-prices-start-at-879-1049-valve-confirm-as-randomised-reservations-open-for-the-steamos-pc">Steam Machine prices start at £879 / $1049... | Rock Paper Shotgun</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极，用户将随机预订系统视为比限时发售更公平的替代方案。许多评论者赞扬 Valve 保持硬件解锁的承诺，有用户写道「我们有什么权利告诉你怎么用你的电脑？」有人对 1049 美元的起始价格表示担忧，Valve 解释这反映了组件成本和他们对 PC 硬件价格趋势的分析。

**标签**: `#valve`, `#steam-machine`, `#gaming-hardware`, `#product-launch`, `#consumer-electronics`

---

<a id="item-8"></a>
## [加拿大计划到 2040 年建设最多 10 座核反应堆](https://www.cbc.ca/news/politics/federal-nuclear-strategy-9.7244509) ⭐️ 7.0/10

加拿大宣布计划到 2040 年建设最多 10 座核反应堆，被称为"核能复兴"，以在可再生能源扩张的同时满足基荷能源需求。 这代表加拿大能源政策的重大转变，利用该国的 CANDU 反应堆技术和铀储备，为安大略省和萨斯喀彻温省等大量投资可变可再生能源的省份提供稳定的基荷电力。 该计划依托加拿大现有的 CANDU 反应堆技术以及目前正在建设的达灵顿新核项目。社区评论对 2040 年的时间表表示怀疑，部分人士将其与英国欣克利角项目相比，该项目经历了严重的延误和成本超支。

hackernews · geox · Jun 22, 19:06

**背景**: 基荷能源是指无论天气条件如何都必须全天候满足的最低电力需求。与太阳能和风能不同，核能提供持续可靠的发电，使其适合满足基荷需求。CANDU（加拿大氚铀）反应堆是加拿大设计的加压重水反应堆技术，已出口到全球。加拿大拥有世界上最大的铀储量之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wattnow.io/2026/03/10/energy-baseload-definition-calculation-and-how-to-reduce-this-phantom-consumption/">Energy baseload : definition , calculation and how to reduce... - Wattnow</a></li>

</ul>
</details>

**社区讨论**: 讨论显示情绪复杂——支持者指出加拿大的强大核专业知识、铀储备和达灵顿项目证明该计划是可行的。然而，批评者认为时间表不切实际，指出英国欣克利角项目从宣布到预计完工用了十多年时间，成本超支严重，表明加拿大的核反应堆可能要到 2070-2080 年才能投入使用。

**标签**: `#nuclear-energy`, `#canada`, `#energy-policy`, `#infrastructure`, `#climate-change`

---

<a id="item-9"></a>
## [Oak：为 AI 代理设计的 Git 替代方案](https://oak.space/oak/oak) ⭐️ 7.0/10

Oak 是一个专为 AI 代理设计的早期版本控制系统，具有虚拟挂载功能，无需完整复制仓库即可工作，支持并行代理工作流程而无需下载所有内容。开发团队已经使用 Oak 构建 Oak 数月，且没有使用 Git 备份。 这很重要，因为它解决了 AI 代理工作流程中潜在的效率瓶颈，可能降低 token 成本，并使多个代理能够同时在同一仓库上工作，而无需完整克隆或工作树的开销。它代表了一种专门为 AI 代理调整版本控制的新颖方法。 Oak 仍处于早期开发阶段，没有 Windows 构建版本，且缺少许多功能如 CI、issues 和评论。该系统使用虚拟挂载来提供对仓库的远程访问而无需本地副本，但这也意味着与现有 Git 生态系统的完全不兼容。

hackernews · zdgeier · Jun 22, 15:37

**背景**: 像 Git 这样的版本控制系统跟踪代码库的变更，使多个开发人员或代理能够协作。传统的 Git 需要完整的仓库副本（克隆）或工作树，这对于需要并行处理多个任务的 AI 代理来说可能既慢又资源密集。虚拟挂载是一种允许访问远程文件系统而无需在本地复制所有数据的技术，可能会提高代理工作流程的效率。

**社区讨论**: 社区讨论提出了质疑的观点。批评者认为 AI 代理已经在训练数据中内置了 Git 知识，质疑是否需要专门的工具。其他人指出，瓶颈通常在于人类决策而非代码生成速度。还有人对 token 减少的声明以及为什么需要一个全新的 VCS（当 Git 的 porcelain 模式可能解决类似问题）表示担忧。

**标签**: `#version-control`, `#ai-agents`, `#developer-tools`, `#git-alternative`, `#open-source`

---

<a id="item-10"></a>
## [警察局长滥用 Flock 车牌识别器无证追踪女性](https://ipvm.com/reports/police-chiefs-track) ⭐️ 7.0/10

Flock Safety 提供人工智能自动车牌识别器，连接到全国性数据库。调查发现，警察局长将这种追踪滥用描述为"罕见"，同时又承认这是发生的"最常见的滥用形式"。

hackernews · jhonovich · Jun 22, 19:13

**背景**: Flock Safety 是一家向美国执法机构提供车牌识别器（LPR）摄像头的公司。这些摄像头自动捕捉车牌并将数据输入共享数据库。车牌识别器因对大规模监控的担忧以及缺乏适当监督机制或逮捕令要求可能导致的滥用风险而一直存在争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tiktok.com/discover/flock-safety-license-plate-reader">Flock Safety License Plate Reader | TikTok</a></li>
<li><a href="https://www.fox35orlando.com/news/mount-dora-police-flock-license-plate-reader-theft-recorded-suspect-custody">Police: Flock license plate reader in Mount Dora... | FOX 35 Orlando</a></li>

</ul>
</details>

**标签**: `#privacy`, `#surveillance`, `#law-enforcement`, `#abuse`, `#policy`

---

<a id="item-11"></a>
## [雪佛龙与微软签署德州西部数据中心 20 年供电协议](https://www.chevron.com/newsroom/2026/q2/chevron-signs-20-year-power-agreement-with-microsoft-for-west-texas-data-center) ⭐️ 7.0/10

讨论中反映出社区对微软可持续发展承诺的显著质疑。评论者强调使用 Solar Turbines（燃气轮机制造商）追求碳负排放目标的讽刺意味。社区对二叠纪盆地的负天然气价格也感到困惑，生产商必须付费才能让天然气被拉走。总体情绪质疑微软如何将其数千兆瓦新化石燃料消耗与环境承诺相协调。

hackernews · cdrnsf · Jun 22, 13:43

**背景**: Microsoft operates the world's largest cloud infrastructure and has committed to being carbon negative by 2030. The Texas grid (ERCOT) is unique as it operates independently from major US grids and relies on investor-driven generation decisions. The Permian Basin, spanning West Texas and southeastern New Mexico, is one of the most prolific oil and gas regions in the United States, producing significant quantities of associated natural gas alongside crude oil.

**社区讨论**: 讨论中反映出社区对微软可持续发展承诺的显著质疑。评论者强调使用 Solar Turbines（燃气轮机制造商）追求碳负排放目标的讽刺意味。社区对二叠纪盆地的负天然气价格也感到困惑，生产商必须付费才能让天然气被拉走。总体情绪质疑微软如何将其数千兆瓦新化石燃料消耗与环境承诺相协调。

**标签**: `#data-centers`, `#energy-infrastructure`, `#sustainability`, `#microsoft`, `#texas-grid`

---

<a id="item-12"></a>
## [OpenAI 推出 Daybreak 安全工具助力漏洞管理](https://openai.com/index/daybreak-securing-the-world) ⭐️ 7.0/10

OpenAI 推出了 Daybreak 安全工具套件，其中包含 Codex Security 和 GPT-5.5-Cyber，旨在帮助组织大规模发现、验证和修复漏洞。 这代表了自动网络安全领域的重大进展，可能会改变组织大规模处理漏洞管理的方式。然而，这些人工智能驱动的工具在现实安全运营中的有效性仍有待验证。 Daybreak 套件包含专门针对安全任务训练的专用人工智能模型。Codex Security 专注于识别代码漏洞，而 GPT-5.5-Cyber 似乎是专门用于网络防御任务的专用模型。

rss · OpenAI News · Jun 22, 10:00

**背景**: Daybreak 是 OpenAI 首个专注于企业漏洞管理的专用安全产品线。这些工具利用人工智能自动化传统上需要大量人力资源的软件系统安全漏洞发现和修复过程。

**标签**: `#ai-security`, `#vulnerability-detection`, `#openai-products`, `#cybersecurity`, `#automated-patching`

---

<a id="item-13"></a>
## [AWS 多模态 AI 可搜索航空影像技术](https://aws.amazon.com/blogs/machine-learning/embed-the-world-multimodal-ai-for-searchable-aerial-imagery-at-scale/) ⭐️ 7.0/10

AWS 工程师详细介绍了其基于 Amazon Bedrock 和 Amazon Nova 构建的多模态 AI 系统，用于大规模可搜索航空影像，并展示了跨嵌入模型和搜索策略的比较实验以及 F1 基准测试结果。 该系统使用户能够通过自然语言查询搜索航空影像，而无需依赖传统元数据标记，从而彻底改变了地理空间数据的可发现性和可用性。该技术现已演化为 Vexcel Intelligence 产品，为全球 45+国家的航空影像库提供可搜索的向量嵌入 API。 实验比较了嵌入模型、融合策略、标注方法和搜索方法四种配置。Amazon Nova Multimodal Embeddings 在两项基准查询中均获得最高 F1 分数。评估方法基于 OpenStreetMap 真实数据构建，系统架构运行在 Amazon Bedrock 和 Amazon OpenSearch Serverless 上。

rss · AWS Machine Learning Blog · Jun 22, 16:32

**背景**: 多模态嵌入是一种将图像和文本映射到同一向量空间的技术，使语义搜索成为可能。航空影像与卫星影像类似，但通常包含更高分辨率的顶视图和 45 度倾斜视图。Amazon Bedrock 是 AWS 的全托管 AI 平台，提供对基础模型（包括 Nova 系列）的 API 访问。Vexcel 拥有覆盖 45+国家的全球航空影像库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vexceldata.com/intelligence/">Vexcel Intelligence | Vexcel Data Program</a></li>
<li><a href="https://aws.amazon.com/blogs/machine-learning/embed-the-world-multimodal-ai-for-searchable-aerial-imagery-at-scale/">Embed the world: Multimodal AI for searchable aerial imagery at scale</a></li>

</ul>
</details>

**标签**: `#multimodal-ai`, `#semantic-search`, `#geospatial-ai`, `#amazon-bedrock`, `#computer-vision`

---

<a id="item-14"></a>
## [NVIDIA 发布新型 AI 软件助力科学研究](https://blogs.nvidia.com/blog/ai-for-science-software-cuda/) ⭐️ 7.0/10

NVIDIA 在汉堡举行的 ISC 大会上发布了三款新型 AI 软件工具：DAQIRI 库、ALCHEMI NIM 微服务以及即将推出的 cuPhoton 参考代码，这些工具旨在加速化学、材料发现和暗物质搜索等科学领域的研究。 这些软件工具弥合了 AI 研究与实验科学之间的差距，使计算化学家、材料科学家和天体物理学家能够更高效地处理来自望远镜、X 射线和激光实验的复杂多维数据。 NVIDIA cuPhoton 是一款用于光子模拟的参考代码，帮助科学家从望远镜、X 射线和激光实验收集的多维数据中提取洞察。ALCHEMI NIM 微服务提供预构建的优化推理端点，可在 NVIDIA 加速基础设施上部署 AI 模型。

rss · NVIDIA Blog · Jun 22, 13:00

**背景**: ISC（国际超级计算）大会是德国汉堡举办的年度重要活动，汇聚了高性能计算领域的专家。NVIDIA 的新软件工具针对多个科学领域：DAQIRI 用于化学应用，cuPhoton 用于材料科学和天文学中的光子模拟，ALCHEMI NIM 用于科学研究工作流程中的加速 AI 推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/ai-for-science-software-cuda/">From Materials Simulation to Experimental Astronomy... | NVIDIA Blog</a></li>
<li><a href="https://nvidia.github.io/cuda-quantum/latest/using/backends/sims/photonics.html">Photonics Simulators — NVIDIA CUDA-Q documentation</a></li>

</ul>
</details>

**标签**: `#AI for Science`, `#NVIDIA`, `#Computational Chemistry`, `#Materials Science`, `#High-Performance Computing`

---

<a id="item-15"></a>
## [CCCL Runtime：面向 CUDA 的现代 C++运行时](https://developer.nvidia.com/blog/cccl-runtime-a-modern-c-runtime-for-cuda/) ⭐️ 7.0/10

此运行时通过提供更高级、更符合 C++习惯的接口简化了 CUDA 开发，使 GPU 计算更容易被开发者上手。它惠及高性能计算社区、人工智能/机器学习研究人员以及希望获得更高生产力的通用 GPU 开发者。 CCCL 3.2 引入了新的惯用 C++接口，用于核心 CUDA 运行地和驱动程序功能。这些包括 CUDA 运行时句柄的包装类型，支持 get()、接受本机句柄的构造函数、release()和 from_native_handle 辅助函数。Python 绑定也支持与本机 CUDA 句柄的互操作性。

rss · NVIDIA Developer Blog · Jun 22, 16:00

**背景**: CUDA（统一计算设备架构）是 NVIDIA 的并行计算平台，使开发者能够利用 GPU 进行通用计算。原始的 CUDA C++ API 是 C 风格的，需要手动管理内存和编写样板代码。CCCL 通过提供现代 C++抽象来解决这一问题，同时保持与现有 CUDA 代码的性能兼容性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/cccl-runtime-a-modern-c-runtime-for-cuda/">CCCL Runtime : A Modern C++ Runtime for CUDA | NVIDIA Technical...</a></li>
<li><a href="https://github.com/NVIDIA/cccl/releases">Releases · NVIDIA/ cccl</a></li>
<li><a href="https://nvidia.github.io/cccl/">CUDA Core Compute Libraries — cccl 3.1 documentation</a></li>

</ul>
</details>

**标签**: `#CUDA`, `#GPU Computing`, `#C++`, `#NVIDIA`, `#High Performance Computing`

---

<a id="item-16"></a>
## [NVIDIA DAQIRI 实现高速数据采集的实时 AI 处理](https://developer.nvidia.com/blog/enable-real-time-ai-for-high-speed-data-acquisition-with-daqiri/) ⭐️ 7.0/10

NVIDIA 发布了 DAQIRI（集成实时仪器数据采集），这是一个软件定义的解决方案，可将高带宽探测器流直接桥接到 NVIDIA GPU，消除了传统的“先存储后处理”工作流程，从而在数据采集过程中实现实时 AI 推理。 这一突破对科学研究和药物发现具有重要意义，因为实时 AI 推理可以加速发现过程。例如，AlphaFold2 在 2020 年通过预测蛋白质结构革新了药物发现，但依赖于 50 年来收集的 170,000 个蛋白质结构——DAQIRI 使这类 AI 能够在数据流实时输入时运行，从而大幅缩短发现周期。 DAQIRI 消除了数据采集管道中“先存储”的瓶颈，允许仪器在流式处理中运行 AI 推理并实时响应。在 CERN 的 ATLAS 实验中，由于存储限制，通常只能存储不到 2%的碰撞数据——DAQIRI 能够实时选择哪些数据值得保存。该解决方案面向药物发现、粒子物理和工业应用中的下一代科学仪器。

rss · NVIDIA Developer Blog · Jun 22, 15:00

**背景**: 数据采集（DAQ）系统传统上在处理之前先收集传感器数据并存储——“先存储”的方法为 AI 推理带来了延迟瓶颈。粒子探测器等高速科学仪器产生数据的速度远快于存储系统的写入速度，使得实时处理变得必要。NVIDIA GPU 提供了在高带宽数据流上进行实时 AI 推理所需的加速计算能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/enable-real-time-ai-for-high-speed-data-acquisition-with-daqiri/">Enable Real - Time AI for High-Speed Data Acquisition with DAQIRI</a></li>
<li><a href="https://github.com/NVIDIA/daqiri">GitHub - NVIDIA / daqiri : DAQIRI connects high bandwidth streaming...</a></li>
<li><a href="https://www.theregister.com/systems/2026/06/22/nvidia-gets-all-agentic-about-supercomputing-for-scientific-research/5259553">Nvidia gets all agentic about supercomputing for scientific research</a></li>

</ul>
</details>

**标签**: `#real-time AI`, `#data acquisition`, `#NVIDIA`, `#drug discovery`, `#scientific computing`

---

<a id="item-17"></a>
## [Meta 意外内部暴露员工按键数据](https://www.wired.com/story/meta-accidentally-let-employees-access-each-others-keystroke-data/) ⭐️ 7.0/10

Meta 意外暴露了其有争议的员工追踪计划中收集的内部员工按键数据，该计划原本用于收集员工的打字模式来训练 AI 模型。员工此前曾对此计划表示担忧。 此事件引发了对大型科技公司工作场所隐私和内部数据安全的严重担忧。意外暴露凸显了收集敏感员工数据用于 AI 训练的风险，特别是在员工已对此做法表示担忧的情况下。 收集的按键数据包括员工打字的时间信息，这些数据可用于按键动力学分析——这是一种基于用户独特打字模式识别用户身份的生物特征技术。这类数据被认为是敏感的，因为它可以揭示个人的行为特征。

rss · WIRED AI · Jun 22, 20:28

**背景**: 按键动力学是一种行为生物特征技术，使用机器学习分析打字模式来进行用户身份验证或识别。当有足够的数据训练时，这些系统在检测身份异常方面可以达到 90%以上的准确率。此事件与关于工作场所监控和企业数据收集实践的更广泛讨论相关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2406.15335">Keystroke Dynamics Against Academic Dishonesty in the Age of LLMs</a></li>
<li><a href="https://medium.com/@tudorache.a.bogdan/ml-models-for-user-recognition-using-keystroke-dynamics-e0665bc18cad">ML models for User Recognition using Keystroke Dynamics | Medium</a></li>
<li><a href="https://aptahire.ai/transparent-fair-ai-hiring-2/">Keystroke Dynamics and Machine Learning: How AI Analyzes Typing...</a></li>

</ul>
</details>

**标签**: `#privacy`, `#workplace surveillance`, `#AI ethics`, `#data breach`, `#Meta`

---

<a id="item-18"></a>
## [将 Moebius 0.2B 图像修复模型移植到浏览器运行](https://simonwillison.net/2026/Jun/22/porting-moebius/#atom-everything) ⭐️ 7.0/10

Simon Willison 成功将 Moebius 0.2B 轻量级图像修复模型移植到浏览器中使用 WebGPU 运行，创建了一个功能演示，用户可以标记图像中要移除的区域，模型会自动生成应该填充的内容。 这证明了 0.2B 参数模型可以在浏览器中客户端运行，这对于设备端 AI 和边缘计算应用来说是重要的进步。它表明实际的浏览器端机器学习推理可以用于真实的图像编辑任务。 Willison 使用 ONNX Runtime Web 的 WebGPU 后端（位于 Transformers.js 之下）来移植模型。原始的 Moebius 需要 PyTorch 和 NVIDIA CUDA，但移植后的版本完全在浏览器中运行，无需服务端处理。

rss · Simon Willison · Jun 22, 23:43

**背景**: WebGPU 是一个新的网页图形 API，使浏览器能够直接进行高性能 GPU 计算，支持现代图形和计算工作负载。图像修复是一种深度学习技术，模型会用语义上合理的内容填充图像中缺失或不需要的区域。Moebius 模型是一个 0.2B 参数模型，据称能达到 10B 级别的性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/WebGPU_API">WebGPU API - Web APIs | MDN</a></li>
<li><a href="https://arxiv.org/html/2401.03395">Deep Learning -based Image and Video Inpainting : A Survey</a></li>

</ul>
</details>

**标签**: `#WebGPU`, `#image-inpainting`, `#browser-machine-learning`, `#edge-AI`, `#Web development`

---

<a id="item-19"></a>
## [AI 安全需要与传统网络安全不同的方法](https://www.latent.space/p/gray-swan) ⭐️ 7.0/10

OpenAI 董事会成员 Zico Kolter 与 Gray Swan CEO Matt Fredrikson 在 Latent Space 播客中解释了为什么 AI 安全不仅仅是'使用 AI 的网络安全'，并探讨了 AI 安全与传统网络安全的根本区别。 随着 AI 系统特别是大语言模型(LLM)被嵌入关键系统，传统的网络安全方法已不足以保护这些非确定性系统。AI 安全的独特性需要全新的防护思路和方法论，这对 AI 开发者和安全专业人员都具有重要指导意义。 AI 系统具有非确定性特征，同样的输入可能产生不同输出，这与传统软件的确定性行为形成鲜明对比。Red-teaming(红队测试)在 AI 领域的应用不仅是技术稳健性测试，还包括对语言模型作为社会嵌入式系统的评估。

rss · Latent Space · Jun 22, 21:06

**背景**: Red-teaming 是一种主动寻找系统漏洞的安全测试方法，源于军事领域的红蓝对抗演习。在 AI 领域，红队测试通过故意尝试破坏 LLM 来评估其安全性。Claude Mythos 是 Anthropic 推出的 AI 安全代理，曾在单次运行中发现 271 个 Firefox 漏洞。Gray Swan 是一家专注于 AI 安全的公司，其 CEO Matt Fredrikson 与 OpenAI 董事会成员 Zico Kolter 共同探讨了这一新兴领域的差异化需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@shafiqulsumon007/red-teaming-large-language-models-how-to-break-ai-before-attackers-do-ad3f6a8c3dde">Red Teaming Large Language Models : How to Break AI ... | Medium</a></li>
<li><a href="https://arxiv.org/html/2602.18483">Red Teaming LLMs as Socio-Technical Practice: From Exploration...</a></li>
<li><a href="https://agentconn.com/blog/claude-mythos-ai-security-agent-review/">Claude Mythos : AI Security Agent That Found 271... - AgentConn Blog</a></li>

</ul>
</details>

**标签**: `#AI security`, `#red-teaming`, `#cybersecurity`, `#LLM safety`, `#AI governance`

---

<a id="item-20"></a>
## [libvfio-user：虚拟机监视器的外部设备仿真库](https://github.com/nutanix/libvfio-user) ⭐️ 7.0/10

这解决了专业化用例的真实问题，即仿真实现与 QEMU 运行时环境不匹配的情况，例如 SPDK 用于在单个进程中处理多个 VM 的虚拟磁盘。它使得设备实现可以在多个 VMM 之间重复使用，而无需修改 QEMU。 vfio-user 协议基于内核的 VFIO 框架建模，采用客户端-服务器架构，客户端运行在 VMM 中，服务器运行在单独的进程中。该库支持 C 和 Python 实现 PCI 设备，Rust 也可能得到支持。

rss · Hacker News - Show HN · Jun 22, 21:41

**背景**: VFIO(虚拟功能 I/O)是一个 Linux 内核框架，允许用户空间程序直接访问硬件设备。QEMU 传统上在单个进程中运行所有仿真。SPDK(存储性能开发套件)是一个用于高性能存储应用程序的框架，需要与 QEMU 提供的不同的运行时环境。vfio-user 协议使这些专业化实现能够在外部运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/nutanix/libvfio-user">GitHub - nutanix/ libvfio - user : framework for emulating devices in...</a></li>
<li><a href="https://www.qemu.org/docs/master/interop/vfio-user.html">vfio - user Protocol Specification — QEMU documentation</a></li>
<li><a href="https://spdk.io/doc/">SPDK : Storage Performance Development Kit</a></li>

</ul>
</details>

**标签**: `#virtualization`, `#device-emulation`, `#QEMU`, `#VFIO`, `#SPDK`

---

<a id="item-21"></a>
## [TIRx：面向前沿 ML 内核的开源编译器栈](https://tvm.apache.org/2026/06/22/tirx) ⭐️ 7.0/10

Apache TVM 发布了 TIRx，这是一款专门用于处理不断演进的前沿机器学习内核的新型开源编译器栈。该版本包含内核库和基准测试，提供涵盖 GEMM、注意力风格内核以及 Blackwell GPU 低精度算子的端到端示例。 这很重要，因为前沿 ML 模型需要专门的内核优化，而传统编译器在处理这些优化时效率较低。TIRx 提供了一个统一的、可编程的软件栈，使硬件供应商、编译器工程师和 ML 研究人员能够协作优化尖端 ML 工作负载。 TIRx 是 Apache TVM 采用的 Python 优先开发方法的一部分，能够快速定制 ML 编译器管道。该栈支持通用部署，可将模型打包成最小的可部署模块，目标是 NVIDIA Blackwell 等现代 GPU 架构。

rss · Lobsters - AI · Jun 22, 22:49

**背景**: Apache TVM 是一个重要的开源 ML 编译器框架，已开发多年。前沿 ML 内核指的是最先进 AI 模型中的核心计算操作，例如 Transformer 中的注意力机制和通用矩阵乘法（GEMM）。随着新模型架构的出现，这些内核发展迅速，需要编译器能够快速适应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tvm.apache.org/2026/06/22/tirx">TIRx: An Open Compiler Stack for Evolving Frontier ML Kernels</a></li>
<li><a href="https://github.com/apache/tvm">GitHub - apache / tvm : Open Machine Learning Compiler Framework</a></li>
<li><a href="https://tvm.apache.org/docs/">Apache TVM Documentation — tvm 0.25.dev0 documentation</a></li>

</ul>
</details>

**标签**: `#machine-learning`, `#compilers`, `#tvm`, `#ml-compilers`, `#open-source`

---

<a id="item-22"></a>
## [Netflix 如何实时绘制数千个微服务的拓扑图](https://www.infoq.cn/article/kp5s7thcxtELg8TpdQYY?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Netflix 工程师解释了他们在生产环境中实时可视化和监控数千个相互连接的微服务的方法。 这解决了一个常见但具有挑战性的分布式系统问题——实时拓扑映射帮助团队了解服务依赖关系，快速识别大型微服务架构中的瓶颈并进行故障排查。 该方法涉及从分布式追踪系统收集追踪数据，以构建实时拓扑图，展示数千个微服务之间的服务关系、请求流和性能指标。

rss · InfoQ 中文站 · Jun 22, 19:07

**背景**: Netflix 运营着数千个处理视频流、推荐系统和用户管理的微服务。管理如此复杂的分布式系统需要有效的可视化和监控工具来确保可靠性和性能。Zipkin 等分布式追踪系统收集时序数据，用于排查服务架构中的延迟问题，而拓扑可视化则提供服务的交互式依赖关系和健康指标视图。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zipkin.io/">OpenZipkin · A distributed tracing system</a></li>
<li><a href="https://cwiki.apache.org/confluence/display/ZIPKIN/Netflix">Netflix - ZIPKIN - Apache Software Foundation</a></li>

</ul>
</details>

**标签**: `#microservices`, `#distributed systems`, `#topology visualization`, `#Netflix`, `#monitoring`

---

<a id="item-23"></a>
## [Discord 以自动化重构数据库运维，以管理超大规模的 ScyllaDB](https://www.infoq.cn/article/hsg1FAk30lT5KVpIpDf1?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

这非常重要，因为 Discord 服务数亿用户，在如此大规模下人工数据库运维变得难以持续。自动化能够实现更快的恢复、更一致的配置，并减少关键基础设施中的人为错误。 ScyllaDB 是一款高性能的 NoSQL 数据库，与 Apache Cassandra 兼容，提供低延迟的数据处理。Discord 的实现需要在保持用户期望的速度和可靠性的同时处理海量数据。

rss · InfoQ 中文站 · Jun 22, 14:44

**背景**: ScyllaDB 是一款开源的 NoSQL 数据库，以高性能和低延迟著称，设计为 Apache Cassandra 的优化版本。Discord 作为主要通信平台，其基础设施每天必须处理数百万并发连接和消息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dools.cc/docs/scylladb/index">ScyllaDB 参考文档-高性能 NoSQL 数 据 库 | dools.cc</a></li>
<li><a href="https://blog.csdn.net/weixin_43501634/article/details/134755568">ScyllaDB 基础入门-CSDN博客</a></li>
<li><a href="https://www.cnblogs.com/superscfan/p/12256951.html">Module- ScyllaDB 技术文档 - SuperScfan - 博客园</a></li>

</ul>
</details>

**标签**: `#数据库运维`, `#ScyllaDB`, `#自动化`, `#DevOps`, `#分布式系统`

---

<a id="item-24"></a>
## [快手 AI 赋能功能开关全生命周期治理方案](https://www.infoq.cn/article/qAbbFlvzvDM2OZD9ulkE?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

快手架构团队分享了利用 AI 技术实现功能开关全生命周期治理的方案，通过自动发现和消亡无用开关的自毁机制来消除技术债务。 关键创新在于“自毁”机制：AI 自动识别已不再使用的开关，并触发其从代码库中移除，减少手动清理工作量，防止技术债务累积。

rss · InfoQ 中文站 · Jun 22, 14:16

**背景**: 功能开关是软件系统中用于控制代码路径执行的条件开关，无需部署即可控制功能启用。它们支持渐进式发布和 A/B 测试，但如果不加管理就会产生技术债务。随着系统扩展，成百上千个开关可能累积，使维护变得困难，增加开发者的认知负担。传统上管理这种技术债务需要手动追踪开关使用情况并移除过时的代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://flagshark.com/blog/feature-flag-technical-debt-guide/">The Complete Guide to Managing Feature Flag Technical Debt</a></li>
<li><a href="https://www.getunleash.io/blog/using-feature-flags-to-manage-technical-debt">Using feature flags to manage technical debt</a></li>

</ul>
</details>

**标签**: `#feature-flags`, `#devops`, `#ai-engineering`, `#platform-engineering`, `#technical-debt`

---

<a id="item-25"></a>
## [内核级的真相：为什么 eBPF 正在取代用户空间 Agent 成为安全可观测性的首选](https://www.infoq.cn/article/spibFV8QPwbvac8LAluZ?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

文章探讨了 eBPF（扩展伯克利包过滤器）技术如何在内核层面实现安全可观测性，以及为何它正在取代传统的基于用户空间 Agent 的安全监控方案。 这一转变代表了安全监控实现方式的根本性变化，从用户空间转向内核级可见性，以获得更好的性能、更低的开销和更全面的系统事件捕获。 eBPF 直接在内核上下文中运行程序而无需修改内核源代码，实现了 CO-RE（一次编译到处运行）以支持跨内核版本的可移植性。XDP（快速数据路径）和环形缓冲区等技术提供了高性能网络处理和高效的事件传递，相比传统的 perf 缓冲区具有更低的开销。

rss · InfoQ 中文站 · Jun 22, 10:20

**背景**: eBPF 是一种 Linux 内核技术，允许在内核空间运行沙盒程序而无需修改内核源代码。传统的安全监控使用作为独立进程运行的用户空间代理，这种方式开销更高且可能错过内核级事件。eBPF 的内核级方法可以在数据路径的更早阶段拦截系统调用和网络数据包，提供更好的可见性和更快的响应时间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.ebpf.io/concepts/core/">BPF CO - RE - eBPF Docs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Express_Data_Path">Express Data Path - Wikipedia</a></li>
<li><a href="https://kubefront.net/system/ebpf/ring-buffer-vs-perf-buffer/">eBPF Ring Buffer vs Perf Buffer | KubeFront</a></li>

</ul>
</details>

**标签**: `#eBPF`, `#安全可观测性`, `#内核技术`, `#系统监控`, `#云原生安全`

---

<a id="item-26"></a>
## [英伟达 CEO 黄仁勋盛赞华为为 AI 芯片领域强劲竞争对手](https://t.me/zaihuapd/42107) ⭐️ 7.0/10

英伟达创始人黄仁勋 7 月 16 日在北京媒体会上表示，任何轻视华为或中国制造能力的人都极其天真，称华为芯片设计能力极为优秀，并强调华为在系统工程、网络工程和云计算领域的卓越实力。 英伟达创始人的这一公开表态代表了美国主要科技企业对华为作为人工智能芯片市场重要竞争对手的看法，反映出在美中地缘政治紧张局势升级之际，英伟达如何看待华为这一强劲竞争对手。 黄仁勋用反问的方式向媒体质疑：世界上哪家手机公司制造的手机比华为更先进？哪家公司研发的蜂窝通信技术能和华为一样好甚至更好？他还指出，许多人工智能开发人员在使用华为时遇到困难，因为其生态系统尚未准备好完全取代英伟达。

telegram · zaihuapd · Jun 22, 09:05

**背景**: 近年来，华为积极发展昇腾 AI 芯片系列，昇腾 950 的发布标志着国产算力迎来重大突破。华为云 CloudMatrix 384 昇腾 AI 云服务已全面上线。公司正在构建完整的 AI 生态系统，包括昇腾处理器、Atlas 计算框架和云服务，以挑战英伟达在 AI 芯片市场的主导地位。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.toutiao.com/topic/7552715201087277098/">华 为 昇 腾 到什么形号了-今日头条</a></li>
<li><a href="https://m-robo.datayes.com/feed/detail?id=376625">910C渐近： 华 为 昇 腾 计算产业及供应商全景梳理</a></li>
<li><a href="https://www.nbd.com.cn/articles/2026-04-24/4358607.html">nbd.com.cn/articles/2026-04-24/4358607.html</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#Huawei`, `#AI Chips`, `#US-China Tech Competition`, `#Industry Commentary`

---

<a id="item-27"></a>
## [48 位中国开发者举报苹果涉嫌垄断](https://m.nbd.com.cn/articles/2026-06-22/4433380.html) ⭐️ 7.0/10

48 位中国 iOS 开发者于 2026 年 6 月 22 日向国家市场监督管理总局提交举报信，指控苹果未兑现“中国市场 App Store 费率不高于其他市场整体水平”的承诺。尽管苹果今年 3 月下调了费率，但中国开发者仍缺乏第三方分发和支付渠道。 此次举报将“苹果税”的费率差异与中外市场开放不平衡问题推向监管焦点。中国作为苹果全球第二大 iOS 市场，此次举报可能为苹果如何处理全球开发者权益和平台准入树立先例。 Apple 于 2026 年 3 月将中国 App Store 佣金从 30%下调至 25%，但仍高于欧盟费率（标准企业 17%、小型企业 10%）。与巴西已开放第三方应用商店不同，中国开发者仍无法使用替代支付系统或在官方商店外部分发应用。

telegram · zaihuapd · Jun 22, 14:57

**背景**: “苹果税”指 Apple 对 App Store 应用内购买收取的佣金。Apple 面临全球监管压力，欧盟于 2024 年强制 Apple 允许第三方应用商店和替代支付。巴西也成为开放第三方分发的主要市场之一。2026 年 3 月的费率下调是 Apple 在中国市场的首次降价。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.globalpeople.com.cn/n4/2026/0313/c305922-21644910.html">“ 苹 果 税 ”在中国调降，推动数字生态更加公平--热评-环球人物网</a></li>
<li><a href="https://36kr.com/p/2779815577486212">被马斯克吐槽的” 苹 果 税 ”，最高 税 率 就是在中国-36氪</a></li>
<li><a href="https://post.smzdm.com/p/axk7kd6w/">苹 果 2026年3月起下调中国App Store 佣 金 至25...</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#App Store`, `#Apple`, `#platform regulation`, `#developer rights`

---