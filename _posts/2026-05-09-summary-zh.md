---
layout: default
title: "Horizon Summary: 2026-05-09 (ZH)"
date: 2026-05-09
lang: zh
---

> From 183 items, 28 important content pieces were selected

---

1. [教 Claude 理解"为什么"](#item-1) ⭐️ 8.0/10
2. [Mojo 1.0 Beta 为 AI 开发者带来系统级编程](#item-2) ⭐️ 8.0/10
3. [EMO：用于涌现模块化的混合专家预训练方法](#item-3) ⭐️ 8.0/10
4. [Cloudflare 因 AI 效率提升宣布大规模裁员 1100 人](#item-4) ⭐️ 8.0/10
5. [Google reCAPTCHA 对去谷歌化安卓用户失效](#item-5) ⭐️ 7.0/10
6. [AI 正在打破两种漏洞文化](#item-6) ⭐️ 7.0/10
7. [io_uring ZCRX 自由链表本地权限提升漏洞](#item-7) ⭐️ 7.0/10
8. [AWS 美国东部一区数据中心故障导致主要服务中断](#item-8) ⭐️ 7.0/10
9. [Meta 移除 Instagram 私信的端到端加密功能](#item-9) ⭐️ 7.0/10
10. [微软研究院发布美国电网输电拓扑开放数据集](#item-10) ⭐️ 7.0/10
11. [自适应并行推理：AI 高效推理的新范式](#item-11) ⭐️ 7.0/10
12. [OpenAI 公布 Codex 代理的多层安全防护措施](#item-12) ⭐️ 7.0/10
13. [哈里伯顿利用 Amazon Bedrock 实现 AI 地震工作流](#item-13) ⭐️ 7.0/10
14. [NVIDIA Dynamo 新增多轮代理 Harness 支持](#item-14) ⭐️ 7.0/10
15. [马斯克诉 OpenAI 案第二周：Zilis 出庭作证称马斯克曾试图挖角 Altman](#item-15) ⭐️ 7.0/10
16. [Claude Code 中 HTML 的超凡有效性](#item-16) ⭐️ 7.0/10
17. [在 Python 代理中实现权限控制的工具调用](#item-17) ⭐️ 7.0/10
18. [Anthropic 计划新融资估值逼近万亿美元反超 OpenAI](#item-18) ⭐️ 7.0/10
19. [Anthropic 将大模型隐藏动机发现率提升 4 倍以上](#item-19) ⭐️ 7.0/10
20. [Broadcom 将 Velero 捐赠给 CNCF 进行社区治理](#item-20) ⭐️ 7.0/10
21. [Agent 时代需要怎样的分布式基础设施](#item-21) ⭐️ 7.0/10
22. [ChatGPT 推出“信任联系人”功能，可预防自杀](#item-22) ⭐️ 7.0/10
23. [Canvas 学习管理系统期末周遭勒索软件攻击](#item-23) ⭐️ 7.0/10
24. [美国最高法院裁定特朗普全球关税违宪](#item-24) ⭐️ 7.0/10
25. [Cloudflare 宣布因 AI 应用裁员逾 1100 人](#item-25) ⭐️ 7.0/10
26. [美国指控英伟达芯片经泰国走私至中国 阿里巴巴涉入](#item-26) ⭐️ 7.0/10
27. [DeepSeek 据称首次大规模外部融资估值约 450 亿美元](#item-27) ⭐️ 7.0/10
28. [苹果拟打破台积电 12 年代工垄断局面](#item-28) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [教 Claude 理解"为什么"](https://www.anthropic.com/research/teaching-claude-why) ⭐️ 8.0/10

Anthropic 发布了关于教导 AI 模型行为准则背后的推理("为什么")的研究,而不仅仅是指定应该执行什么行为。他们的"规则背后的推理"(RBR)方法训练模型理解准则的目的和原则,使模型能够更好地泛化到新情况。 这代表了 AI 对齐的重大进步,从行为规范转向教学式训练——教导模型规则背后的原理,而不仅仅是记忆规则。如果模型理解规则存在的原因,它们就能更好地抵御越狱、泛化到边缘情况,并将原则应用于训练中从未见过的情况。 RBR 方法包括在训练中向模型展示规则及其背后的推理。Anthropic 发现这种方法单独优于宪法 AI 方法,而且值得注意的是,这种方法可以泛化到开源模型如 Llama 3.1 8B 和 Qwen 2.5/3 32B,表明其适用范围远超 Claude。

hackernews · pretext · May 8, 17:59

**背景**: AI 对齐指的是确保 AI 系统按照人类价值观和意图行事的挑战。传统的对齐方法规定行为规则,但当模型遇到新情况时往往会失败。宪法 AI 是 Anthropic 使用一套原则("宪法")来训练 AI 有帮助、无害和诚实的框架。这项新研究通过教导模型这些原则背后的推理而不仅仅是原则本身来扩展这一方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_alignment">AI alignment - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/research/constitutional-ai-harmlessness-from-ai-feedback">Constitutional AI: Harmlessness from AI Feedback \ Anthropic</a></li>

</ul>
</details>

**社区讨论**: 评论者强调这是一个"教学问题"——询问如何在有限的训练数据中引出期望的行为。存在哲学辩论,讨论"对齐"的模型导致广泛危害(如消除劳动力价值)是否仍可称为对齐。其他人注意到这种方法可以泛化到开源模型,Anthropic 发布了经过微调的 Llama 和 Qwen 版本,在各种"价值观"上进行训练。

**标签**: `#ai-research`, `#alignment`, `#anthropic`, `#ai-safety`, `#model-training`

---

<a id="item-2"></a>
## [Mojo 1.0 Beta 为 AI 开发者带来系统级编程](https://mojolang.org/) ⭐️ 8.0/10

这个版本很重要，因为 Mojo 提供了独特的 Rust 风格所有权模型、强大的编译时执行和统一的 GPU/CPU 代码，这可能会重塑 AI 开发，而计划在 2026 年秋季进行的开源发布增加了社区的重大兴趣。 这个版本意义重大，因为 Mojo 提供了 Rust 风格的拥有权、强大的编译时执行和统一的 GPU/CPU 代码的独特组合，可能会重塑 AI 开发，而计划在 2026 年秋季进行的开源发布增添了重要的社区关注度。 关键的技术细节包括 Mojo 使用 LLVM 作为后端（但与 Rust/Zig 使用方式不同）、一流 SIMD 支持、丰富的类型系统，以及 comptime 允许在编译时执行代码。用方括号声明的参数可以实现编译时元编程。

hackernews · sbt567 · May 8, 02:49

**背景**: Mojo 是一种新的编程语言，由 Chris Lattner（Swift 和 LLVM 编译器工具链的创造者）创建，旨在将 Python 的简洁性与 C++/Rust 级别的性能相结合。它具有类似于 Rust 的所有权模型、编译时执行和统一的 CPU/GPU 代码。Mojo 编译器目前是闭源的，但有开源的标准库，计划在 2026 年秋季开源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo ( programming language ) - Wikipedia</a></li>
<li><a href="https://docs.modular.com/mojo/manual/basics/">Mojo language basics | Modular</a></li>
<li><a href="https://ruhati.net/mojo/_parameters_and_compile_time_programming.html">Mojo By Example: A Comprehensive Introduction to the Mojo ...</a></li>

</ul>
</details>

**社区讨论**: 早期用户称赞 Mojo 独特的 LLVM 用法、所有權模型和 SIMD 支持确实是创新性的。然而，也存在对 Python 兼容性的有效担忧——用户报告说字符串操作和内置函数的工作方式与 Python 不同（例如`len(x)`），这让人感到困惑。有些人将其与 Julia 进行比较，担心类似的编译器错误和文档问题。总体情绪是兴奋与对破坏性变化的谨慎之间的平衡。

**标签**: `#programming-languages`, `#mojo`, `#ai-ml`, `#performance`, `#systems-programming`

---

<a id="item-3"></a>
## [EMO：用于涌现模块化的混合专家预训练方法](https://huggingface.co/blog/allenai/emo) ⭐️ 8.0/10

Hugging Face 和 AllenAI 共同发布了 EMO，这是一种针对混合专家模型的新型预训练方法，旨在实现神经网络架构中的涌现模块化，使专门的模块能够在训练过程中自然涌现，而无需预先定义的架构约束。 EMO 使用基于键值聚类的划分方法来捕获神经元激活中的模块化模式，允许网络在训练过程中自然地发现和形成功能模块，而不是在架构层面明确定义它们。

rss · Hugging Face Blog · May 8, 16:03

**背景**: 混合专家（MoE）是一种神经网络架构，其中不同的专门子网络（专家）根据输入被激活，允许条件计算和可扩展性。涌现模块化指的是模块化结构在训练过程中从网络的权重中自然产生的现象，这些模块对应于特定功能。传统的 MoE 方法通常明确定义专家边界。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aclanthology.org/2024.naacl-long.144/">Unlocking Emergent Modularity in Large Language... - ACL Anthology</a></li>
<li><a href="https://arxiv.org/pdf/2310.10908">Unlocking Emergent Modularity in Large Language Models</a></li>

</ul>
</details>

**标签**: `#mixture-of-experts`, `#pretraining`, `#neural-networks`, `#machine-learning`, `#scaling`

---

<a id="item-4"></a>
## [Cloudflare 因 AI 效率提升宣布大规模裁员 1100 人](https://techcrunch.com/2026/05/08/cloudflare-says-ai-made-1100-jobs-obsolete-even-as-revenue-hit-a-record-high/) ⭐️ 8.0/10

Cloudflare 宣布了公司历史上首次大规模裁员，裁减 1100 个工作岗位，约占员工总数的 14%。首席执行官马修·普林斯表示，由于 AI 效率提升，公司不再需要那么多支持岗位，尽管公司报告了创纪录的收入。 这次裁员凸显了科技行业日益增长的矛盾现象——公司在通过 AI 自动化削减员工的同时却取得了创纪录的利润。这引发了关于企业责任以及 AI 对各行业就业实际影响的关键问题。 1100 个工作岗位的裁减约占 Cloudflare 员工总数的 14%。这是公司历史上首次大规模裁员。尽管员工大幅减少，公司仍报告了创纪录的收入，展示了公司通过 AI 驱动效率可以实现的经济效益。

rss · TechCrunch AI · May 8, 18:33

**背景**: Cloudflare 是一家主要的互联网基础设施公司，提供内容分发网络（CDN）、网络安全和云计算等服务。该公司多年来增长显著，但与许多科技公司一样，现在正转向利用 AI 来提高运营效率。这次裁员反映了科技行业更广泛的趋势，即公司使用 AI 来自动化以前由人类执行的任务。

**标签**: `#AIjobs`, `#layoffs`, `#Cloudflare`, `#automation`, `#techindustry`

---

<a id="item-5"></a>
## [Google reCAPTCHA 对去谷歌化安卓用户失效](https://reclaimthenet.org/google-broke-recaptcha-for-de-googled-android-users) ⭐️ 7.0/10

Google 已将 reCAPTCHA 更新为使用远程认证，该功能对包括使用 GrapheneOS 在内的去谷歌化安卓用户造成了影响。新系统通过 Google 服务器创建设备身份链，将烧录的 EK（背书密钥）连接到由 Google 基础架构签名的 AIK（认证身份密钥）。 远程认证系统的工作原理是：EK（静态烧录的私钥）→ AIK（由 Google 服务器签名的安全飞地中的临时身份密钥）→ 认证（由 AIK 签名）。由于 Google 服务器必须参与 EK 到 AIK 的转换过程，无法连接到 Google 服务器的设备将无法通过验证。这与使用盲签名的旧版 CAPTCHA 系统不同，后者可以被绕过。

hackernews · anonymousiam · May 8, 18:45

**背景**: 去谷歌化安卓是指移除所有 Google 服务、应用程序和追踪器的安卓操作系统。GrapheneOS 是一款注重隐私的安全 ROM，可加强安卓的沙盒功能并限制应用程序权限。去谷歌化运动是一场出于隐私考虑而呼吁用户停止使用 Google 产品的草根运动。远程认证是一种安全协议，通过检查加密测量值来验证远程设备的完整性和身份。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeGoogle">DeGoogle - Wikipedia</a></li>
<li><a href="https://www.howtogeek.com/790432/what-you-need-to-try-grapheneos-the-privacy-focused-android-rom/">What You Need to Try GrapheneOS , the Privacy -Focused Android...</a></li>
<li><a href="https://collective.flashbots.net/t/the-evolution-of-remote-attested-tls/5383">The Evolution of Remote Attested TLS - TEE - Trusted Execution...</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了对 Google 做法的强烈不满。用户批评强制的设备指纹识别，并将其与 KYC 要求进行比较。一位评论者指出，远程认证不像盲签名那样可以"被利用"，因此技术上不可能绕过，除非与 Google 服务器串通。其他人正在寻找替代的 CAPTCHA 解决方案，私人访问令牌被建议为一种侵入性较小的选项。

**标签**: `#privacy`, `#android`, `#recaptcha`, `#security`, `#grapheneos`

---

<a id="item-6"></a>
## [AI 正在打破两种漏洞文化](https://www.jefftk.com/p/ai-is-breaking-two-vulnerability-cultures) ⭐️ 7.0/10

这很重要，因为传统的"安全通过模糊性"模式正在被打破。攻击者现在可以在公开披露之前分析代码提交来发现漏洞修复，大幅缩短从补丁到漏洞利用的时间线。 关键细节包括 Log4Shell 中观察到的时间线：一个黑帽黑客在 day -X 看到修复 bug 的提交，而补丁仍在协调中，导致攻击在 CVE 发布之前就开始了。人工智能工具现在使提交分析变得更快、更容易实现。

hackernews · speckx · May 8, 17:55

**背景**: 从历史上看，漏洞研究依赖于"安全通过模糊性"——保持源代码闭源，这样攻击者就不容易发现缺陷。开源软件被认为风险更高，因为任何人都可以分析代码。然而，现代人工智能与改进的反编译和逆向工程工具相结合，已经消除了闭源软件的这一优势。攻击者现在可以通过分析提交历史、比较修补和未修补版本的差异，以及使用人工智能识别漏洞模式来发现漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2408.07321v1">LLM-Enhanced Static Analysis for Precise Identification of Vulnerable ...</a></li>
<li><a href="https://arxiv.org/html/2604.05130v1">A Multi-Agent Framework for Automated Exploit Generation with...</a></li>

</ul>
</details>

**社区讨论**: Community sentiment is mixed. Some commenters (like tptacek) see this as a long-predicted shift enabled by open source and improved tools. Others (like rikafurude21) argue this is an old problem being reframed as AI - noting that people were already diffing kernel commits before LLMs. The Log4Shell example from freeqaz illustrates the real-world impact: finding the bug on day -X+1 while black hats saw the commits on day -X.

**标签**: `#security`, `#vulnerability-research`, `#AI`, `#open-source`, `#exploit-development`

---

<a id="item-7"></a>
## [io_uring ZCRX 自由链表本地权限提升漏洞](https://ze3tar.github.io/post-zcrx.html) ⭐️ 7.0/10

一位安全研究人员发布了一份 writeup，详细描述了 Linux 内核 io_uring ZCRX（零拷贝接收）自由链表实现中的一个本地权限提升漏洞，该漏洞源于一个边界检查错误，允许越界写入从而实现内核级别的任意代码执行。 此漏洞可能允许具有特定权限的本地攻击者在受影响的 Linux 系统上提升权限至 root。然而，安全影响仍存在争议，因为一些评论者指出该漏洞可能需要先前的提升权限（CAP_SYS_ADMIN 或 CAP_NET_ADMIN）并且可能已在稳定内核版本中修复。 该漏洞发生在自由链表处理中，其中 free_count 在写入操作之前递增，而写入使用递增前的值作为数组索引。当进入时 free_count 等于 num_niovs，写入操作会访问 freelist[num_niovs]，即 allocated 数组末尾之后的下一个位置，从而实现越界写入。

hackernews · MrBruh · May 8, 19:40

**背景**: io_uring 是 Linux 内核的系统调用接口，用于异步 I/O 操作，于 2019 年在 Linux 5.1 中引入。ZCRX（零拷贝接收）是一项提供网络零拷贝接收缓冲区以提高性能的功能。该漏洞存在于自由链表管理代码中，边界检查未能阻止对已分配缓冲区数组之外的写入操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Io_uring">io_uring - Wikipedia</a></li>
<li><a href="https://docs.kernel.org/networking/iou-zcrx.html">io_uring zero copy Rx — The Linux Kernel documentation</a></li>

</ul>
</details>

**社区讨论**: HN 上的讨论显示出复杂的情绪：一些评论者争论该漏洞是否是真正的新漏洞，或者是否已在稳定内核版本中修复，而其他评论者则质疑它是否需要先前的提升权限（CAP_SYS_ADMIN/CAP_NET_ADMIN）才能利用，并认为这大大限制了其实际严重性。标题很吸引人，但需要客户端 JavaScript 来读取原始 writeup 这一点受到了批评。

**标签**: `#linux-kernel`, `#io_uring`, `#security`, `#privilege-escalation`, `#cve`

---

<a id="item-8"></a>
## [AWS 美国东部一区数据中心故障导致主要服务中断](https://www.cnbc.com/2026/05/08/aws-outage-data-center-fanduel-coinbase.html) ⭐️ 7.0/10

2026 年 5 月 7-8 日，AWS 位于美国东部一区（弗吉尼亚州北部）的数据中心发生故障，导致 FanDuel 和 Coinbase 等主要服务中断数小时。故障根本原因是冷却系统失效导致基础设施过热。 这次故障凸显了 AWS 美国东部一区反复出现的可靠性问题，该区域是全球使用最广泛的 AWS 区域之一。故障影响了主要的金融和游戏服务，表明云基础设施故障会对数百万用户日常依赖的下游应用产生连锁影响。 关于故障范围存在相互矛盾的报道——Coinbase 声称多个可用区（AZ）受到影响，而 AWS 官方声明则表示只有一个可用区受影响。恢复预计需要数小时，这与之前该区域发生的重大事故一致。

hackernews · christhecaribou · May 8, 03:31

**背景**: AWS 美国东部一区是 AWS 最古老、最受欢迎的的区域，为无数企业提供关键基础设施。可用区是一个区域内物理分离的数据中心，旨在提供针对设施故障的隔离。该区域历史上曾发生多起备受瞩目的故障，引发了关于其与其他 AWS 区域相比可靠性的持续讨论。

**社区讨论**: 社区讨论反映出对美国东部一区反复出现问题的显著不满。评论者对该区域作为互联网单点故障表示担忧，一位用户指出'AWS 的美国东部一区继续是互联网的阿喀琉斯之踵'。还有人提出关于冷却系统冗余的技术问题，并对关于哪些可用区实际受影响的矛盾报道感到困惑。

**标签**: `#aws`, `#cloud-infrastructure`, `#outage`, `#us-east-1`, `#incident-response`

---

<a id="item-9"></a>
## [Meta 移除 Instagram 私信的端到端加密功能](https://www.pcmag.com/news/meta-shuts-down-end-to-end-encryption-for-instagram-dms-messaging) ⭐️ 7.0/10

移除端到端加密意味着 Meta 现在可以扫描和分析 Instagram 私信，用于内容审核、广告定向和合规法律请求。这与 Meta 的其他消息平台（如 WhatsApp）形成对比，后者默认保持端到端加密功能。 这一决定影响到了数百万依赖加密私信功能的 Instagram 用户的隐私与安全。对于这个月活超过 20 亿的平台来说，这是用户隐私保护的重大退步。

hackernews · tcp_handshaker · May 8, 21:47

**背景**: 端到端加密（E2EE）是一种安全方法，确保只有发送者和接收者可以读取消息内容，即使是服务提供商也无法访问。Meta 拥有 Instagram、WhatsApp 和 Facebook，是世界上最大的即时通讯生态系统之一。WhatsApp 已默认提供端到端加密，而 Signal 被广泛认为是加密消息传递的标准。

**社区讨论**: 评论显示出复杂的情绪：一些用户认为端到端加密本质上会提供更差的用户体验，而另一些用户则批评 Meta 将利润置于隐私之上。一位评论者指出，苹果强大的隐私功能导致 Siri 落后，这与 Meta 的做法形成对比。许多人对于这个牺牲用户安全以换取商业便利的公司决定表示失望。

**标签**: `#privacy`, `#meta`, `#encryption`, `#instagram`, `#tech-policy`

---

<a id="item-10"></a>
## [微软研究院发布美国电网输电拓扑开放数据集](https://www.microsoft.com/en-us/research/blog/building-realistic-electric-transmission-grid-dataset-at-scale-a-pipeline-from-open-dataset/) ⭐️ 7.0/10

该数据集包含来自开放来源的输电拓扑结构和电气参数，如线路阻抗、电压等级以及发电机/配电连接。它代表了一个可扩展的流程，用于生成逼真的电网模型，以支持在各种运行条件下分析拥堵、扩容场景和韧性。

rss · Microsoft Research · May 8, 19:53

**背景**: 输电拓扑是指电网组件的物理布置，包括输电线路、变电站及其电气连接，以网络图形式表示。理解输电拥堵至关重要，因为过载的线路会阻止额外的电力流动，导致价格飙升和可靠性问题。电力系统韧性分析考察电网承受自然灾害或网络威胁等中断并快速恢复服务的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/research/blog/building-realistic-electric-transmission-grid-dataset-at-scale-a-pipeline-from-open-dataset/">Building realistic electric transmission grid ... - Microsoft Research</a></li>
<li><a href="https://en.wikipedia.org/wiki/Transmission_congestion">Transmission congestion - Wikipedia</a></li>
<li><a href="https://www.iea.org/commentaries/grid-congestion-is-posing-challenges-for-energy-security-and-transitions">Grid congestion is posing challenges for energy security and transitions – Analysis - IEA</a></li>

</ul>
</details>

**标签**: `#power-grids`, `#open-data`, `#energy-systems`, `#infrastructure`, `#research-data`

---

<a id="item-11"></a>
## [自适应并行推理：AI 高效推理的新范式](http://bair.berkeley.edu/blog/2026/05/08/adaptive-parallel-reasoning/) ⭐️ 7.0/10

这很重要，因为顺序推理的扩展成本呈线性增长，会导致上下文腐化和过高延迟。自适应并行推理让模型能够自主确定最佳任务分解，解决了大型语言模型推理时间扩展的关键瓶颈。 ThreadWeaver 将推理重新表述为分叉-合并程序的执行图，而非线性日记，使模型能够学习任务中何时自然存在并行性。该方法需要训练模型处理按推理模式分解为顺序片段的并行轨迹。

rss · BAIR Blog · May 8, 09:00

**背景**: 推理时间扩展指在生成过程中投入更多计算来提升模型性能，而非仅在训练期间提升。上下文腐化是指由于上下文窗口中中间探索路径的积累导致模型性能下降，使模型难以关注相关信息。并行推理通过同时探索多个独立推理线程来减少总体延迟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bair.berkeley.edu/blog/2026/05/08/adaptive-parallel-reasoning/">Adaptive Parallel Reasoning : The Next Paradigm in Efficient...</a></li>
<li><a href="https://arxiv.org/abs/2504.15466">Learning Adaptive Parallel Reasoning with Language Models</a></li>
<li><a href="https://introl.com/blog/inference-time-scaling-research-reasoning-models-december-2025">Inference -Time Scaling | Introl Blog</a></li>

</ul>
</details>

**标签**: `#adaptive parallel reasoning`, `#AI inference`, `#efficient computing`, `#reasoning models`, `#ThreadWeaver`

---

<a id="item-12"></a>
## [OpenAI 公布 Codex 代理的多层安全防护措施](https://openai.com/index/running-codex-safely) ⭐️ 7.0/10

这项技术指导对于部署 AI 编程代理的组织非常重要，因为它解决了关键的企业安全问题，包括未授权代码执行、数据泄露风险和监管合规要求，这些问题阻碍了自主编程工具的广泛采用。 安全方法结合了多层防御：隔离的沙箱执行环境以防止主机系统受损，分阶段审批工作流要求在潜在破坏性操作之前进行人工授权，限制出站连接的网络策略，以及与 OpenTelemetry 标准对齐的代理原生遥测技术，用于实时可观察性和审计跟踪。

rss · OpenAI News · May 8, 12:30

**背景**: 像 Codex 这样的 AI 编程代理是一类新型自主系统，能够根据自然语言指令编写、修改和执行代码。企业部署带来了独特的安全挑战：代理必须具有足够的系统访问权限才能发挥作用，但无限制的访问会带来重大风险。Microsoft 和 Anthropic 的最新发展强调从设计时就构建安全可观察性，而不是在部署后进行改造。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/03/18/observability-ai-systems-strengthening-visibility-proactive-risk-detection/">Observability for AI Systems: Strengthening... | Microsoft Security Blog</a></li>
<li><a href="https://www.apmdigest.com/look-ahead-ai-native-automation-changes-telemetry-pipeline-management-forever-2026">AI - Native Telemetry Pipelines: The 80% Shift | APMdigest</a></li>

</ul>
</details>

**标签**: `#AI security`, `#coding agents`, `#sandboxing`, `#enterprise deployment`, `#OpenAI`

---

<a id="item-13"></a>
## [哈里伯顿利用 Amazon Bedrock 实现 AI 地震工作流](https://aws.amazon.com/blogs/machine-learning/halliburton-enhances-seismic-workflow-creation-with-amazon-bedrock-and-generative-ai/) ⭐️ 7.0/10

哈里伯顿展示了一个使用 Amazon Bedrock 的生成式 AI 概念验证原型，该原型可将自然语言查询转换为可执行的地震工作流，实现高达 95%的工作流加速。该解决方案还为哈里伯顿的 Seismic Engine 工具和文档提供问答功能。 这很重要，因为它展示了油气行业的大型企业如何利用生成式 AI 显著简化复杂的技术工作流。地球科学家和数据科学家现在可以通过自然语言交互来配置处理工具，而不是手动配置，这可能会改变地震数据处理的生产力。 该解决方案是使用 Amazon Bedrock 构建的，利用大型语言模型来解释自然语言查询并生成可执行的地震处理工作流。它还集成了一个问答系统，可以查询 Seismic Engine 文档和工具，为用户提供技术响应。

rss · AWS Machine Learning Blog · May 8, 13:20

**背景**: 地震工作流在石油和天然气勘探中至关重要，涉及收集和分析地震数据以绘制地下地质结构图。这些工作流传统上需要地球科学家手动配置复杂的处理链，这既耗时又需要专业 expertise。Amazon Bedrock 是 AWS 的全托管服务，提供用于构建生成式 AI 应用的基础模型访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aws.amazon.com/blogs/industries/accelerate-the-seismic-data-workflow/">Accelerate the Seismic Data Workflow | AWS for Industries</a></li>
<li><a href="https://aws.amazon.com/blogs/machine-learning/halliburton-enhances-seismic-workflow-creation-with-amazon-bedrock-and-generative-ai/">Halliburton enhances seismic workflow creation with Amazon Bedrock...</a></li>

</ul>
</details>

**标签**: `#generative-ai`, `#amazon-bedrock`, `#enterprise-ai`, `#seismic-data-processing`, `#case-study`

---

<a id="item-14"></a>
## [NVIDIA Dynamo 新增多轮代理 Harness 支持](https://developer.nvidia.com/blog/streaming-tokens-and-tools-multi-turn-agentic-harness-support-in-nvidia-dynamo/) ⭐️ 7.0/10

该功能特别针对流式令牌与工具调用的结合,系统必须保持 assistant 推理/动作与用户反馈之间的交错模式。它在多轮对话中保持结构化交互流程,确保代理能够处理每回合的多个工具调用并正确排序结果。

rss · NVIDIA Developer Blog · May 8, 15:59

**背景**: 在代理 AI 系统中,'工具调用'(或'函数调用')指 LLM 生成格式化输出的能力,可触发外部 API 调用或系统方法。此上下文中的'harness'是一个测试或开发框架,管理用户回合与 assistant 回合之间的交互流程。多轮交互需要在对话轮次之间保持状态和上下文,当涉及工具调用时变得复杂。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.openai.com/api/docs/guides/function-calling">Function calling | OpenAI API</a></li>
<li><a href="https://arize.com/blog/llm-function-calling-evaluating-tool-calls-in-llm-pipelines/">LLM Function Calling : Evaluating Tool Calls In LLM Pipelines</a></li>

</ul>
</details>

**标签**: `#AI Agents`, `#NVIDIA Dynamo`, `#Tool Use`, `#Multi-Turn Interaction`, `#LLM Frameworks`

---

<a id="item-15"></a>
## [马斯克诉 OpenAI 案第二周：Zilis 出庭作证称马斯克曾试图挖角 Altman](https://www.technologyreview.com/2026/05/08/1137008/musk-v-altman-week-2-openai-fires-back-and-shivon-zilis-reveals-that-musk-tried-to-poach-sam-altman/) ⭐️ 7.0/10

Shivon Zilis 曾与 Musk 和 Altman 都密切合作，她提供了关于涉嫌挖角企图的证词。马斯克声称 Altman 和 Brockman 曾承诺保持 OpenAI 的开源使命，但在 Microsoft 数十亿美元投资后转向商业化。 这场审判代表了人工智能行业治理的关键时刻，因为它可能重塑 OpenAI 的未来方向及其与 Microsoft 的合作。该争议凸显了在快速发展的人工智能领域中，开源人工智能伦理与商业开发之间的紧张关系。

rss · MIT Technology Review · May 8, 23:59

**背景**: Microsoft 于 2019 年向 OpenAI 投资 10 亿美元，使 OpenAI 从一个研究实验室发展成为拥有足够计算能力来训练和扩展模型的组织。该合作在 2023 年 1 月 ChatGPT 发布后扩展为多年数十亿美元的交易。英国、欧盟和美国的监管机构目前正在审查这一合作关系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bbc.com/news/technology-68445981">Elon Musk sues ChatGPT-maker OpenAI over Microsoft links</a></li>
<li><a href="https://www.fool.com/investing/2026/05/06/why-amazon-might-be-the-real-winner-of-the-microso/">Why Amazon Might Be the Real Winner of the Microsoft and OpenAI ...</a></li>

</ul>
</details>

**标签**: `#AI Industry`, `#OpenAI`, `#Elon Musk`, `#Legal`, `#Tech Business`

---

<a id="item-16"></a>
## [Claude Code 中 HTML 的超凡有效性](https://simonwillison.net/2026/May/8/unreasonable-effectiveness-of-html/#atom-everything) ⭐️ 7.0/10

Anthropic 公司的 Thariq Shihipar 主张向 Claude Code 请求 HTML 而非 Markdown 输出，展示了更丰富的交互式产物，如带颜色编码的注释 diff、内边距注释和 SVG 图表。 这项技术通过启用按严重程度分类的颜色注释、交互式导航和可视化图表，显著改善了 AI 代码审查，使复杂的代码解释对开发者来说更易读、更实用。 该方法适用于任何 AI 编码助手（Claude、GPT-5.5 等），只需简单请求带有特定样式的 HTML 输出即可。Simon Willison 通过让 GPT-5.5 创建一个关于 Linux 权限提升漏洞的交互式 HTML 解释来演示这一点，包含了安全警告和详细分解。

rss · Simon Willison · May 8, 21:00

**背景**: 自 GPT-4 以来，Markdown 一直是 AI 工具的默认输出格式，因为在 8,192 token 限制内其 token 效率较高。然而，HTML 可以实现 Markdown 无法匹配的功能：SVG 图表、CSS 样式、JavaScript 交互和灵活布局。示例集合可在 thariqs.github.io/html-effectiveness/ 查看，展示了各种用例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://github.com/anthropics/claude-code">anthropics/ claude - code : Claude Code is an agentic coding tool that...</a></li>

</ul>
</details>

**社区讨论**: 讨论反映了开发者们的强烈兴趣，他们已经开始尝试这种 HTML 输出技术。thariqs.github.io/html-effectiveness/作为不断增长的资源库，提供了展示 HTML 相较于 Markdown 在代码解释方面实际优势的提示词模板和示例。

**标签**: `#AI Tools`, `#Claude Code`, `#Prompt Engineering`, `#HTML`, `#Developer Workflow`

---

<a id="item-17"></a>
## [在 Python 代理中实现权限控制的工具调用](https://machinelearningmastery.com/implementing-permission-gated-tool-calling-in-python-agents/) ⭐️ 7.0/10

随着 AI 代理从被动聊天机器人演变为能够通过工具调用采取自主行动的系统，实施权限控制对于 AI 安全变得至关重要。本教程为开发者提供了可操作的代码，以防止自主 AI 系统中的未经授权或有害操作。 教程重点关注在工具执行之前实施授权检查，创建一个门控机制可以将批准的工具列入白名单，并要求对敏感操作（如文件系统访问、网络请求或命令执行）进行权限验证。

rss · Machine Learning Mastery · May 8, 12:00

**背景**: 工具调用是 AI 代理与外部系统交互并执行文本生成之外操作的基本功能。AI 代理已从简单的聊天机器人演变为可以执行代码、访问数据库和与 API 交互的自主系统。权限控制的工具调用增加了一个安全层，确保代理在未经适当授权的情况下无法执行潜在有害的操作。

**标签**: `#AI_agents`, `#tool_calling`, `#Python`, `#AI_safety`, `#agent_architecture`

---

<a id="item-18"></a>
## [Anthropic 计划新融资估值逼近万亿美元反超 OpenAI](https://www.ft.com/content/a40cafcc-0fa4-4e70-9e24-90d826aea56d) ⭐️ 7.0/10

Anthropic 正考虑在今年夏天筹集数十亿美元的新资金，以支撑其算力基础设施的重大扩容。此举有望使其估值大幅推高至近 1 万亿美元，从而在投后规模上反超其最大竞争对手 OpenAI。该目前在私募股权二级市场交易平台上的隐含估值已飙升至 1 万至 1.2 万亿美元区间，超越了 OpenAI 约 8800 亿美元的同期估值。 这代表着 AI 行业竞争格局的重大逆转，标志着 Anthropic 首次在估值上超越 OpenAI。从今年 2 月的 3800 亿美元飙升至如今的逾 1 万亿美元，这一快速估值增长反映出市场对企业端客户爆发式增长的强烈信心。此举可能加剧领先 AI 实验室之间的融资军备竞赛，并重塑投资者在生成 AI 领域的资金分配格局。 2024 年 2 月，Anthropic 刚完成了一笔 30 亿美元的融资，当时的投后估值为 3800 亿美元。短短数月后，其在二级市场的估值已翻倍逾两倍。新一轮融资旨在支持其算力基础设施的重大扩容，这对于训练和部署更大规模的 AI 模型是必要的。

telegram · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · May 8, 11:15

**背景**: Anthropic 是一家 AI 安全和研究公司，由前 OpenAI 研究人员创立，以其 Claude 聊天机器人系列最为知名。该公司定位为优先注重 AI 安全和对齐，与 OpenAI 等竞争对手形成差异化定位。AI 领域的企业客户通常指将 AI 模型集成到其产品和服务中的企业，这类企业往往愿意为更强大、更可靠的 AI 能力支付溢价。

**标签**: `#AI funding`, `#Anthropic`, `#OpenAI`, `#valuation`, `#AI industry`

---

<a id="item-19"></a>
## [Anthropic 将大模型隐藏动机发现率提升 4 倍以上](https://www.infoq.cn/article/gAkVCqphr0A1r2PLSWDz?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Anthropic 发布了新研究，将大型语言模型中隐藏动机的发现率提升了 4 倍以上，以应对人工智能系统中长期存在的"黑箱"可解释性挑战。 这项研究意义重大，因为理解大型语言模型中的隐藏动机直接关系到人工智能安全和一致性，这是该领域的关键挑战。改进的可解释性方法有助于在模型部署前识别潜在风险。 具体方法论细节在现有内容中未充分披露。该研究建立在 Anthropic 现有的可解释性工作基础上，可能涉及电路分析和特征检测技术来识别隐藏的模型行为。

rss · InfoQ 中文站 · May 8, 18:27

**背景**: 机械可解释性是可解释人工智能的一个子领域，旨在通过分析神经网络计算中存在的机制来理解其内部运作方式。这种方法类似于对二进制计算机程序进行逆向工程来分析神经网络。这使得工程师可以成为"人工智能外科医生"，精确定位模型中导致特定行为的"电路"。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability</a></li>
<li><a href="https://www.linkedin.com/pulse/your-ai-black-box-why-mechanistic-interpretability-key-naik-pkquc">Is Your AI a "Black Box"? Why Mechanistic Interpretability is the Key....</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#LLM Interpretability`, `#AI Safety`, `#AI Alignment`, `#Research`

---

<a id="item-20"></a>
## [Broadcom 将 Velero 捐赠给 CNCF 进行社区治理](https://www.infoq.cn/article/FwFo4Gerr0lawgBCyYo1?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

此次捐赠具有重要意义，因为它将 Kubernetes 集群的关键灾难恢复功能从企业控制转移到社区管理，确保该工具能够继续为更广泛的生态系统服务，不受企业并购或战略变化的影响。 Velero 使用户能够备份整个 Kubernetes 集群资源、在不同云提供商之间执行集群迁移，并从快照恢复应用程序。该项目已成为 Kubernetes 环境中灾难恢复和多云迁移的重要工具。

rss · InfoQ 中文站 · May 8, 16:30

**背景**: Velero 最初由 Heptio 创建，这是一家专注于 Kubernetes 的公司，由 Craig McLuckie 和 Joe Beda 创立（他们也是 Google Cloud 的联合创始人）。VMware 于 2018 年收购了 Heptio，随后 Broadcom 在 2022 年收购了 VMware。CNCF 托管了许多主要的云原生项目，包括 Kubernetes、Prometheus 和 Grafana 等，提供中立的治理和长期可持续发展。

**标签**: `#Kubernetes`, `#Velero`, `#CNCF`, `#cloud-native`, `#open-source`

---

<a id="item-21"></a>
## [Agent 时代需要怎样的分布式基础设施](https://www.infoq.cn/article/qYQfpT8BaIPEkbeSXwzu?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

文章可能涵盖多个主题，包括协调多个 Agent 的编排框架、跨分布式 Agent 网络的状态管理、实时通信协议，以及确保基于 Agent 的系统高可用性和容错性的基础设施模式。

rss · InfoQ 中文站 · May 8, 11:34

**背景**: AI Agent（人工智能代理）是能够推理、规划和执行动作以实现特定目标的自主软件系统。与简单生成响应的传统 AI 模型不同，代理可以与外部工具交互、保持状态并执行多步骤工作流。分布式基础设施指分布在多台机器或数据中心的计算资源，提供可扩展性、容错性和低延迟访问。

**标签**: `#AI Agents`, `#Distributed Systems`, `#Infrastructure`, `#Cloud Computing`, `#System Design`

---

<a id="item-22"></a>
## [ChatGPT 推出“信任联系人”功能，可预防自杀](https://www.theverge.com/ai-artificial-intelligence/925874/chatgpt-trusted-contact-emergency-self-harm-notification) ⭐️ 7.0/10

OpenAI 为成年 ChatGPT 用户推出了可选的“信任联系人”功能，允许用户指定一位朋友、家人或照护者，当系统检测到用户可能讨论自残或自杀时，该联系人可被通知。经专门培训的团队审核后，若确认存在严重安全顾虑，将向指定联系人发送电子邮件、短信或 ChatGPT 应用内通知，但不会共享聊天内容。 这一功能代表了人工智能安全措施的重大扩展，直接回应了此前悲剧事件引发的担忧，包括一名 16 岁少年在长期与 ChatGPT 对话后自杀的案例。它可能通过 enables 及时干预来帮助预防自杀。 双方必须是成年人（韩国需 19 岁以上），且指定的联系人须在一周内接受邀请。该功能建立在此前为青少年实施的安全选项之上。

telegram · zaihuapd · May 8, 02:47

**背景**: 这一功能是在一名 16 岁少年与 ChatGPT 进行大量对话后自杀的悲剧事件后扩展的安全措施。Meta 还在 Instagram 上实施了类似功能，当孩子反复搜索自残主题时会通知家长。

**标签**: `#ai-safety`, `#mental-health`, `#openai`, `#feature-release`, `#responsible-ai`

---

<a id="item-23"></a>
## [Canvas 学习管理系统期末周遭勒索软件攻击](https://www.cnn.com/2026/05/07/us/canvas-hack-strands-college-students-finals-week) ⭐️ 7.0/10

Instructure 公司的 Canvas 学习管理系统遭到 ShinyHunters 黑客组织声称的勒索软件攻击，导致美国大学和学区在期末周期间系统中断。据报道，此次攻击影响了约 9000 所学校，疑似泄露超过 300TB 的敏感数据，包括学生姓名、学生 ID 和学校邮箱地址。 ShinyHunters 组织成立于 2019 年，是一个臭名昭著的黑客组织，以大规模数据泄露著称。仅在 5 月前两周，该组织就声称从至少 13 家公司窃取了近 2 亿条记录。该组织通常通过窃取数据后向受害者索要赎金来运作。

telegram · zaihuapd · May 8, 04:30

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Learning_management_system">Learning management system</a></li>
<li><a href="https://en.wikipedia.org/wiki/ShinyHunters">ShinyHunters - Wikipedia</a></li>
<li><a href="https://www.wired.com/story/shinyhunters-hacking-group-data-breach-spree/">ShinyHunters Is a Hacking Group on a Data Breach Spree | WIRED</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#ransomware`, `#education`, `#data-breach`, `#instructure`

---

<a id="item-24"></a>
## [美国最高法院裁定特朗普全球关税违宪](https://t.me/zaihuapd/41280) ⭐️ 7.0/10

美国最高法院于 2 月 20 日以 6 比 3 的投票结果裁定，特朗普政府依据《国际紧急经济权力法》(IEEPA)征收的全球关税违宪，因为宪法将征收关税的权力赋予国会而非总统。随后特朗普签署行政命令，改用《贸易法》第 122 条对全球进口商品征收 10%的临时从价关税，为期 150 天。 这一裁决极大地限制了总统的贸易政策权力，确认总统不能通过紧急经济权力单方面征收关税。这为行政和立法部门在贸易事务上的权力分离设立了重要的宪法先例。 10%临时关税将于美东时间 2 月 24 日凌晨 12:01 生效，持续 150 天。豁免范围涵盖关键矿产、能源产品、化肥、药品原料及部分农产品。政府援引美国巨额贸易逆差作为启用第 122 条的理由。

telegram · zaihuapd · May 8, 06:46

**背景**: 《国际紧急经济权力法》(IEEPA)赋予总统在国家紧急状态下广泛的紧急经济权力，最初设计用于战争制裁等场景。《贸易法》第 122 条允许在特定条件下临时提高关税，但要求这些关税是临时的并有贸易不平衡作为依据。宪法明确规定'所有增加税收的法案应起源于众议院'，确立了税收权力属于国会的原则。

**标签**: `#US_Politics`, `#Trade_Policy`, `#Constitutional_Law`, `#Supreme_Court`, `#Tariffs`

---

<a id="item-25"></a>
## [Cloudflare 宣布因 AI 应用裁员逾 1100 人](https://blog.cloudflare.com/building-for-the-future/) ⭐️ 7.0/10

2026 年 5 月 7 日，Cloudflare 宣布将在全球范围内裁减逾 1100 名员工，并将此次裁员直接归因于过去三个月内公司内部 AI 使用量增长超过 600%。 这是科技行业中因 AI 采用而直接驱动的最大规模裁员之一，表明企业正在通过 AI 获取效率提升并进行组织架构重组的趋势正在加速。 遣散方案包括：相当于全部基本工资直至 2026 年底的补偿、美国地区至年底的医疗保险、股权归属延至 2026 年 8 月 15 日，并豁免悬崖期条款。裁员将一次性完成，离职员工直接收到邮件通知。

telegram · zaihuapd · May 8, 08:15

**背景**: AI 智能体是使用 ReAct、Chain-of-Thought 等推理框架进行自主决策和完成任务的人工智能软件系统。在 Cloudflare 的案例中，这些 AI 智能体被部署到工程、人力资源、财务和市场部门，处理此前由员工完成的日常工作任务。600%的使用量增长表明 AI 已快速融入核心业务运营。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.betteryeah.com/blog/ai-agent-core-components-architecture-guide">AI Agent 包括哪些内容？ 六大核心组成要素全解析</a></li>

</ul>
</details>

**标签**: `#AI adoption`, `#workforce reduction`, `#tech industry`, `#Cloudflare`, `#organizational restructuring`

---

<a id="item-26"></a>
## [美国指控英伟达芯片经泰国走私至中国 阿里巴巴涉入](https://www.bloomberg.com/news/articles/2026-05-08/us-said-to-suspect-nvidia-chips-smuggled-to-alibaba-via-thailand) ⭐️ 7.0/10

美国检方指控泰国公司 OBON Corp. 涉嫌将价值 25 亿美元的内含先进英伟达芯片的 Super Micro 服务器走私至中国，阿里巴巴集团被指为多个终端客户之一。 此案可能是美国对华半导体出口管制最大规模的违规案例之一，可能影响美中科技竞争，并可能促使美国重新考虑对泰国的芯片出口限制，从而打击泰国的 AI 发展雄心。 OBON Corp. 曾参与创建泰国主权 AI 云项目 Siam AI，后者获得了英伟达合作伙伴地位。阿里巴巴否认与 Super Micro 或 OBON 有任何业务关系。Siam AI CEO 称自己已离开 OBON，该公司未涉及走私。

telegram · zaihuapd · May 8, 13:23

**背景**: 自 2022 年以来，美国对向中国出口先进半导体和 AI 芯片实施了严格的出口管制，旨在防止中国提升其军事 AI 能力。英伟达最先进的芯片（如 A100 和 H100）均受这些出口管制限制。泰国一直试图通过 Siam AI 等项目将自己定位为区域 AI 中心。

**标签**: `#semiconductors`, `#export-controls`, `#US-China-tech-competition`, `#Nvidia`, `#geopolitics`

---

<a id="item-27"></a>
## [DeepSeek 据称首次大规模外部融资估值约 450 亿美元](https://t.me/zaihuapd/41289) ⭐️ 7.0/10

DeepSeek 据称正在寻求首次大规模外部融资，中国国家集成电路产业投资基金据称正洽谈领投此轮融资，对 DeepSeek 的估值可能达到约 450 亿美元。 这标志着 DeepSeek 首次接受外部资金，此前其母公司 High-Flyer Capital 为 DeepSeek 提供全部资金支持。国有背景资金的参与意味着国资正在更深介入中国 AI 核心公司，这标志着中国领先 AI 企业融资模式的战略性转变。 国家集成电路产业投资基金是支持中国半导体和集成电路产业的国家投资机构。这将是 DeepSeek 首次大规模外部融资，标志着其此前完全内部注资模式的重大转变。

telegram · zaihuapd · May 8, 14:59

**背景**: DeepSeek 是一家中国 AI 公司，因开发可与 OpenAI 产品竞争的大型语言模型而引起广泛关注。该公司最初作为量化交易公司 High-Flyer Capital 的子公司运营，由后者提供全部初始资金。DeepSeek 此前因使用 NVIDIA 为中国市场设计的 H800 芯片训练 AI 模型而成为头条新闻，由于美国出口限制，这些芯片的传输速度低于旗舰 H100 芯片。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepseek.com/">DeepSeek | 深度求索</a></li>
<li><a href="https://www.investbrother.com/focus_news/deepseek/">DeepSeek AI 突然崛起 安全風險及準確度成疑</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#AI funding`, `#China AI`, `#state capital`, `#venture capital`

---

<a id="item-28"></a>
## [苹果拟打破台积电 12 年代工垄断局面](https://t.me/zaihuapd/41292) ⭐️ 7.0/10

苹果公司正考虑结束自 2014 年以来与台积电的独家芯片代工关系，计划最早于 2027 年与英特尔合作，利用其 18A 工艺为苹果代工部分 Mac、iPad 和 iPhone 的中低端处理器。 英特尔仅负责使用 18A 工艺进行芯片制造，不涉及芯片设计。分析师预测英特尔最早可能于 2027 年开始为苹果代工部分芯片，但这将仅限于中低端处理器，高端芯片仍由台积电代工。

telegram · zaihuapd · May 8, 17:18

**背景**: 自 2014 年以来，台积电一直是苹果唯一的芯片代工厂商，为 iPhone、iPad 和 Mac 设备生产定制硅芯片。这段 12 年的独家合作关系现在受到质疑，因为台积电越来越专注于服务英伟达等 AI 公司，这些企业对先进 AI 加速器的需求激增。英特尔的 18A 是该公司下一代制造节点，致力于竞争性性能表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://archive.org/stream/ittushu-7109/半导体制造技术_djvu.txt">Full text of "国外电子与通信教材系列"</a></li>

</ul>
</details>

**标签**: `#Apple`, `#TSMC`, `#Intel`, `#semiconductor supply chain`, `#chip manufacturing`

---