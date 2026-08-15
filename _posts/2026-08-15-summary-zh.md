---
layout: default
title: "Horizon Summary: 2026-08-15 (ZH)"
date: 2026-08-15
lang: zh
---

> From 148 items, 25 important content pieces were selected

---

1. [苹果宣布 CEO 交接：库克卸任，特努斯接任](#item-1) ⭐️ 8.0/10
2. [PostgreSQL 修复高危 to_char 漏洞可执行任意代码](#item-2) ⭐️ 8.0/10
3. [Qwen 3.8 27B 发布：本地推理模型新成员](#item-3) ⭐️ 7.0/10
4. [Going Dark 问题：加密时代的执法黑客行动](#item-4) ⭐️ 7.0/10
5. [RISC-V 架构设计的关键分析](#item-5) ⭐️ 7.0/10
6. [Why does Opus 5 feel worse to work with?](#item-6) ⭐️ 7.0/10
7. [谷歌通过同态加密实现隐私 AI 的实际应用](#item-7) ⭐️ 7.0/10
8. [Firefox 成为最后一个仍支持 uBlock Origin 的主流浏览器](#item-8) ⭐️ 7.0/10
9. [Mixedbread 发布 Toast 1：专为多轮搜索设计的专业 LLM](#item-9) ⭐️ 7.0/10
10. [GLM-5.3 展现前沿编码能力与新兴网络安全研究技能](#item-10) ⭐️ 7.0/10
11. [印尼首个大学 AI 中心在 UGM 日惹成立](#item-11) ⭐️ 7.0/10
12. [法国 Kog 优化 GPU 用于智能体 AI，声称推理提速 30 倍](#item-12) ⭐️ 7.0/10
13. [苹果与阿里巴巴合作开发中国定制 AI 模型](#item-13) ⭐️ 7.0/10
14. [Z.ai 仅通过规模化后训练发布 GLM-5.3 实现重大性能提升](#item-14) ⭐️ 7.0/10
15. [Needle 2：4500 万参数工具调用模型仅 14MB](#item-15) ⭐️ 7.0/10
16. [世界首个超导量子热引擎演示成功](#item-16) ⭐️ 7.0/10
17. [使用 LLM"幻觉"技术进行标签分类](#item-17) ⭐️ 7.0/10
18. [谷歌 DeepMind 发布 Gemini 3.7 Flash 性能直逼旗舰价格大降](#item-18) ⭐️ 7.0/10
19. [DeepSeek 开源 Harness 框架：全面插件化](#item-19) ⭐️ 7.0/10
20. [AI 编程工具进入生产环境：从会用到驾驭的真实挑战](#item-20) ⭐️ 7.0/10
21. [AI 实验室每年测试 300 万人体组织样本，或将替代动物测试](#item-21) ⭐️ 7.0/10
22. [苹果寻求最高法院审查 App Store 收费裁决，已获暂停执行](#item-22) ⭐️ 7.0/10
23. [小红书开源 280B MoE 模型 dots3-note](#item-23) ⭐️ 7.0/10
24. [谷歌被令取消第三方应用商店安装障碍](#item-24) ⭐️ 7.0/10
25. [苹果联手阿里开发中国专属 AI 大模型](#item-25) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [苹果宣布 CEO 交接：库克卸任，特努斯接任](https://t.me/zaihuapd/43191) ⭐️ 8.0/10

苹果宣布现任 CEO 蒂姆·库克将出任董事会执行董事长，现任硬件工程高级副总裁约翰·特努斯将于 2026 年 9 月 1 日起接任 CEO 一职。 董事会一致批准了这一交接计划。库克将在整个夏季继续担任 CEO 以确保平稳过渡。现任董事长阿瑟·莱文森将转任首席独立董事，特努斯将于 2026 年 9 月 1 日加入董事会。

telegram · zaihuapd · Aug 14, 11:00

**背景**: 约翰·特努斯于 2001 年加入苹果，2013 年升任硬件工程副总裁，2021 年进入苹果高管团队。近年来他负责 iPhone、Mac、iPad 和 AirPods 的研发工作。蒂姆·库克自 2011 年起担任 CEO，接替了史蒂夫·乔布斯。

**标签**: `#apple`, `#leadership-change`, `#tim-cook`, `#corporate-news`, `#tech-industry`

---

<a id="item-2"></a>
## [PostgreSQL 修复高危 to_char 漏洞可执行任意代码](https://www.postgresql.org/support/security/CVE-2026-14669/) ⭐️ 8.0/10

PostgreSQL 项目披露了关键漏洞 CVE-2026-14669，该漏洞存在于 to_char(timestamptz) 函数中。漏洞源于处理超长的 POSIX 时区缩写时可触发堆缓冲区溢出，使拥有数据库账户的攻击者能够以 PostgreSQL 服务进程的操作系统权限执行任意代码。 这是一个高危漏洞（CVSS 8.8），影响全球最广泛使用的开源数据库之一。虽然利用该漏洞需要低权限数据库账户而非无需认证，但能够以服务级权限执行任意代码对任何运行受影响 PostgreSQL 版本的组织都构成严重安全风险。 该漏洞影响 PostgreSQL 14.x 至 18.x 版本，具体为 14.24、15.19、16.15、17.11 和 18.6 之前的版本。由于 18.5 因回归问题未正式发布，18.x 用户应直接升级至 18.6。与主版本升级不同，这些小版本更新无需数据库转储或 pg_upgrade，仅需更新程序文件并重启服务。

telegram · zaihuapd · Aug 14, 14:35

**背景**: PostgreSQL 中的 to_char() 函数用于将时间戳值转换为格式化的字符串，其中 timestamptz 变体处理带时区的时间戳。POSIX 时区缩写遵循特定格式，包含名称部分（通常为 3-4 个字母）和偏移量。当时区缩写超过预期长度限制时，会发生堆缓冲区溢出，可能允许攻击者利用内存损坏来执行代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/pgupgrade.html">PostgreSQL: Documentation: 18: pg_upgrade</a></li>
<li><a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones">List of tz database time zones - Wikipedia</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#security`, `#vulnerability`, `#CVE-2026-14669`, `#database`

---

<a id="item-3"></a>
## [Qwen 3.8 27B 发布：本地推理模型新成员](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 7.0/10

阿里巴巴 Qwen 团队在 Hugging Face 上发布了 Qwen 3.8 27B，这是一款新型本地大型语言模型，在推理性能方面与谷歌的 Gemma 4 相当，详细的社区基准测试显示了特定硬件的性能指标。 这一发布标志着本地 AI 模型能力的重要进步，表明非美国 AI 开发者也能生产出具有竞争推理能力的模型，这些模型可以在消费级硬件上运行。 社区基准测试显示，使用 ninfer 推理引擎在 RTX 5090 GPU 上该模型每秒可生成约 138 个 tokens，尽管与 Gemma 4 相比需要 5 倍更多的 tokens 和 12 分 30 秒来完成推理任务。

hackernews · erdaltoprak · Aug 14, 15:00

**背景**: Qwen 是阿里云的大型语言模型系列，参数规模从紧凑型到数万亿不等。本地 AI 模型完全在个人设备上运行，而非云服务，提供更强的隐私保护和离线能力。Gemma 4 则代表谷歌在这一竞争领域的先进开放模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://huggingface.co/Qwen">Org profile for Qwen on Hugging Face, the AI community building the...</a></li>

</ul>
</details>

**社区讨论**: 社区反馈强调与 Gemma 4 相比的 VRAM 效率问题，有用户注意到模型处理推理时的独特'思维追踪'模式。积极反馈则强调该模型在消费级硬件上的强大推理能力。

**标签**: `#AI`, `#LLM`, `#Qwen`, `#local AI`, `#model benchmarking`

---

<a id="item-4"></a>
## [Going Dark 问题：加密时代的执法黑客行动](https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/) ⭐️ 7.0/10

密码工程博客发布分析文章，探讨"Going Dark"问题——执法机构通过软件漏洞进行黑客行动是否能弥补加密技术的限制，并回顾了从物理线路到现代加密的窃听技术发展历史。 这很重要，因为加密技术已经变得如此强大，以至于执法机构即使拥有法律授权也常常无法破解，这引发了关于平衡安全与执法获取权的持续政策讨论。其利害关系涉及公共安全和通信基础设施的整体安全性。 该分析探讨了执法机构是否能越来越多地依赖利用软件漏洞而非后门来获取信息，但指出存在重大安全权衡担忧，以及美国系统被削弱后可能被外国对手利用的风险。

hackernews · vslira · Aug 14, 20:52

**背景**: "Going Dark"问题指的是加密软件变得如此安全，以至于政府即使拥有法律授权也常常无法破解的挑战。这一问题日益普遍，已引发多轮政策讨论。安全专家通常反对后门，原因是"最不可信国家问题"——为执法机构创建的任何漏洞都可能被对手利用——以及削弱整体网络安全基础设施的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theiacp.org/resources/critical-issues-encryption-going-dark">Critical Issues: Encryption & Going Dark</a></li>
<li><a href="https://repository.law.umich.edu/mjlr/vol50/iss2/5/">"Shedding Light on the "Going Dark" Problem and the Encryption Debate" by John Mylan Traylor</a></li>
<li><a href="https://www.schneier.com/blog/archives/2026/07/end-to-end-encryption-and-going-dark.html">End-to-End Encryption and "Going Dark" - Schneier on Security</a></li>

</ul>
</details>

**社区讨论**: 评论者提供了宝贵的历史背景——指出在计算机化系统之前，电话窃听需要物理线路，在纽约市每年花费约 100 万美元。其他评论者对软件漏洞是否真的在减少表示担忧，有人认为人工智能生成的代码可能引入更多漏洞而非更少，质疑漏洞发现能力将持续改善的假设。

**标签**: `#cryptography`, `#encryption`, `#law-enforcement`, `#privacy`, `#security`

---

<a id="item-5"></a>
## [RISC-V 架构设计的关键分析](https://dmitry.gr/?r=06.%20Thoughts&proj=12.%20RV) ⭐️ 7.0/10

发表了一篇关于 RISC-V 架构的技术批评文章，分析了其设计选择以及作为开放 ISA 标准的战略重要性。 这一批评很重要，因为 RISC-V 正成为 ARM 和 x86 等专有架构日益重要的开放标准替代方案，了解其技术局限性对于做出明智的采用决策至关重要。 该批评审视了 RISC-V 中的具体技术设计决策，包括可能并非所有用例都最优的指令编码和架构选择。讨论指出，目前最快的 RISC-V CPU 在速度、功耗或芯片面积方面尚不能与最优秀的芯片相比。

hackernews · kaycebasques · Aug 14, 22:38

**背景**: RISC-V 是一种开源的指令集架构(ISA)，定义了软件与 CPU 层面硬件的交互方式。与 ARM 或 x86 等专有 ISA 不同，RISC-V 可以免费供任何人使用，无需授权费用。ISA 是软件和硬件之间的抽象模型接口，指定处理器的功能及其实现方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Instruction_set_architecture">Instruction set architecture - Wikipedia</a></li>
<li><a href="https://www.arm.com/glossary/isa">What is Instruction Set Architecture (ISA)?</a></li>

</ul>
</details>

**社区讨论**: 社区评论显示出多元观点。有些人强调 RISC-V 的战略价值在于其不受限制的开放标准地位，而非技术优势，中国正是因此大力投资。另一些作为业余 CPU 设计师的人则欣赏 RISC-V 得到主流编译器的支持且在法律上可访问。一个共同的主题是期望可能不切实际——RISC-V 目前虽然在各方面都不如其他架构，但却提供了一个有价值的开放基础。

**标签**: `#RISC-V`, `#hardware-design`, `#open-source`, `#ISA`, `#CPU-architecture`

---

<a id="item-6"></a>
## [Why does Opus 5 feel worse to work with?](https://mun-logadan.github.io/why-does-opus-5-feel-worse/) ⭐️ 7.0/10

Hacker News discussion analyzing user dissatisfaction with Claude Opus 5's communication style and speculating that AI post-training may be shifting toward agent-centric rather than human-centric optimization.

hackernews · numeri · Aug 14, 10:12

**标签**: `#AI`, `#Claude`, `#Anthropic`, `#LLM UX`, `#model training`

---

<a id="item-7"></a>
## [谷歌通过同态加密实现隐私 AI 的实际应用](https://blog.google/security/how-google-is-making-private-ai-practical-with-homomorphic-encryption/) ⭐️ 7.0/10

谷歌讨论了他们在使同态加密实际应用于隐私 AI 推理方面的工作，这使得对加密数据的计算无需先解密即可进行。 这一发展可能实现隐私保护的 AI 服务，使敏感数据在整个处理流程中保持加密状态，可能在医疗、金融和其他隐私敏感行业启用新的用例。 一位拥有隐私保护机器学习硕士学位的评论者指出，同态加密在推理任务上具有非常高的计算开销（约 1000 倍的资源消耗），使其在商业上不可行。其他人则指出这会带来显著增加的能源消耗带来的环境问题。

hackernews · u1hcw9nx · Aug 14, 15:43

**背景**: 同态加密是一种加密形式，允许在加密数据上直接执行计算，而无需先解密。计算结果保持加密状态，解密后产生的输出与对未加密数据执行的操作结果相同。AI 推理是训练好的 AI 模型使用新输入数据实时生成输出的阶段。将这些技术结合在一起可以实现处理敏感数据而不暴露原始数据的 AI 服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Homomorphic_encryption">Homomorphic encryption</a></li>
<li><a href="https://cloud.google.com/discover/what-is-ai-inference">What is AI inference? How it works and examples | Google Cloud</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一。虽然有些人承认这一技术进步，但其他人强调鉴于谷歌的声誉，追求隐私技术的做法具有讽刺意味。最实质性的技术批评集中在约 1000 倍的计算开销使其商业上不可行，再加上能源消耗增加带来的重大环境问题。怀疑论者还指出，在个人硬件上本地运行 AI 比任何基于云的解决方案都能提供更好的隐私保护。

**标签**: `#homomorphic-encryption`, `#privacy`, `#machine-learning`, `#google`, `#security`

---

<a id="item-8"></a>
## [Firefox 成为最后一个仍支持 uBlock Origin 的主流浏览器](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 7.0/10

在谷歌实施 Manifest V3 后，Firefox 成为最后一个仍支持完整版 uBlock Origin 的主流浏览器，该版本有效限制了 Chrome 及其衍生浏览器的广告拦截功能。 这很重要，因为它影响到数百万依赖广告拦截器来保护隐私和改善浏览体验的用户。它还突出了浏览器供应商与广告拦截生态系统之间持续的紧张关系，谷歌的 Manifest V3 因损害用户选择权而受到隐私倡导者的批评。 在 Manifest V3 下，webRequestBlocking 权限仅适用于企业级侧载扩展，普通用户无法使用完整的广告拦截功能。Firefox 保持对完整版 uBlock Origin 的支持，并对热门扩展进行安全审查，以确保没有恶意软件被植入。

hackernews · DemiGuru · Aug 14, 19:03

**背景**: Manifest V3 是 Chrome 的新扩展平台，用 declarativeNetRequest 取代了 webRequest API，限制了扩展拦截网络请求的方式。这一变化一直存在争议，电子前沿基金会（EFF）批评它损害了隐私、安全和创新。uBlock Origin 是最受欢迎的广告拦截扩展之一，以其高效性和广泛的过滤列表著称。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/what-is-mv3">Extensions / Manifest V 3 | Chrome for Developers</a></li>
<li><a href="https://developer.chrome.com/docs/extensions/reference/api/webRequest">chrome.webRequest | API | Chrome for Developers</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了 Firefox 对热门扩展的安全审查程序，一位用户指出 Firefox 是唯一在每次更新时审查 uBlock 代码的浏览器。一些用户提到有非官方的 uBlock Origin 移植版本可在 Manifest V3 上运行，而另一些用户则报告 uBlock Origin Lite 足以满足大多数广告拦截需求。

**标签**: `#browsers`, `#ad-blocking`, `#uBlock Origin`, `#web extensions`, `#Google Chrome`

---

<a id="item-9"></a>
## [Mixedbread 发布 Toast 1：专为多轮搜索设计的专业 LLM](https://www.mixedbread.com/blog/toast-1) ⭐️ 7.0/10

Mixedbread 发布了 Toast 1，这是一款专为多轮搜索查询设计的专业 LLM。它通过执行多轮搜索和验证来迭代搜索结果，从而提高用户的"搜索能力"。 这标志着向针对特定任务优化的专业 LLM（而非通用模型）的转变。它解决了一个真实的痛点：复杂问题通常需要 2-5 轮搜索、点击链接和验证假设——而 LLM 可能能够高效地自动化这些工作。 Toast 1 是一款基于云的模型，而非开源权重模型，这限制了本地部署选项。用户已将其与 Perplexity、配备搜索功能的 Gemini 和 Parallel AI 进行比较，作为搜索类 LLM 服务的竞争者。

hackernews · mplappert · Aug 14, 15:07

**背景**: 多轮搜索是一种 LLM 将复杂查询分解为子查询、迭代执行并聚合响应的方法。这与单次搜索不同，允许模型通过多轮迭代验证信息和优化结果。与此相关的是 ReAct 提示技术，它使用思维-行动-观察循环，使 LLM 能够有效地使用搜索引擎等外部工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ulab-uiuc/LLMRouter">GitHub - ulab-uiuc/LLMRouter: LLMRouter: An Open-Source ...</a></li>
<li><a href="https://www.promptingguide.ai/techniques/react">ReAct Prompting | Prompt Engineering Guide</a></li>
<li><a href="https://deepwiki.com/ulab-uiuc/LLMRouter/5.3.3-multi-round-routers">Multi-Round Routers | ulab-uiuc/LLMRouter | DeepWiki</a></li>

</ul>
</details>

**社区讨论**: 社区成员对专业搜索 LLM 的概念表示热情，有人指出它解决了一个真正的问题。然而，用户质疑它与 Perplexity 的差异，并批评缺乏开源权重版本。一些人还批评文章没有清楚解释 Mixedbread Search 的功能。

**标签**: `#AI`, `#LLMs`, `#search`, `#product-launch`, `#machine-learning`

---

<a id="item-10"></a>
## [GLM-5.3 展现前沿编码能力与新兴网络安全研究技能](https://z.ai/blog/glm-5.3) ⭐️ 7.0/10

GLM-5.3 展示了前沿编码能力及新兴的网络安全研究技能，包括漏洞发现、红队场景、WordPress 插件中的零日检测、RCE 漏洞利用和内核漏洞利用适配。 这代表了 AI 驱动安全研究的重大进展，引发了关于 AI 安全、负责任披露以及与 OpenAI 和 Anthropic 模型竞争的辩论。大规模发现漏洞的能力可能使安全测试民主化，但也引发了对滥用的担忧。 据报道，该模型在红队场景中对抗另一个 GLM 代理执行了完整的漏洞发现，发现了流行软件中的漏洞。Z.ai 似乎正在大规模扫描开源软件，并在 cvd.z.ai 拥有一个包含许多待披露 CVE 的漏洞数据库。一些用户注意到它仍然是基于 GLM 5.2 进行后训练增强的版本。

hackernews · pella · Aug 14, 05:19

**背景**: GLM 是由中国公司 Z.ai（也称为智谱 AI）开发的开源大型语言模型系列。涌现能力（Emergent capabilities）是指在特定规模阈值下大型 AI 模型中出现的意外技能，如多步推理和工具使用。前沿编码（Frontier coding）是指能够执行复杂软件工程任务的先进 AI 编码代理。AI 安全研究领域近期随着 Anthropic 的 Project Glasswing 等竞争项目取得了进展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM_(AI)">GLM (AI) - Wikipedia</a></li>
<li><a href="https://github.com/zai-org/GLM-5">GLM-5.2 & GLM-5.1 & GLM-5 - GitHub</a></li>
<li><a href="https://www.emergentmind.com/topics/emergent-capabilities">Emergent Capabilities in AI</a></li>

</ul>
</details>

**社区讨论**: 评论显示对该模型的安全研究能力感到兴奋，一位用户将其描述为第一个能够进行适当安全研究的模型，并表示它能无缝执行包括零日和内核漏洞在内的红队场景。一些用户将其与 OpenAI 模型进行比较，但指出还不足以吸引切换。还在讨论以量化形式在本地运行的问题，以及对大规模漏洞扫描的担忧。

**标签**: `#AI`, `#Machine Learning`, `#Cybersecurity`, `#LLM`, `#Vulnerability Research`

---

<a id="item-11"></a>
## [印尼首个大学 AI 中心在 UGM 日惹成立](https://blogs.nvidia.com/blog/ugm-indosat-nvidia-ai-technology-center/) ⭐️ 7.0/10

本周，印尼通信和数字事务部、Indosat Ooredoo Hutchison、NVIDIA 和 Gadjah Mada 大学在日惹推出了 UGM Indosat NVIDIA AI 技术中心——这是印尼首个大学人工智能技术中心。 这代表了印尼这个东南亚最大经济体的 AI 教育基础设施重大投资，解决了这个拥有超过 2.7 亿人口的国家对本地 AI 人才的迫切需求。该中心展示了 NVIDIA 对新兴市场的战略扩张，并符合印尼的国家 AI 战略。 该中心将利用 NVIDIA 的 AI 技术和专业知识，在政府建立的印尼 AI 卓越中心框架内培养本地 AI 人才。UGM 是印尼最古老、最负盛名的大学。

rss · NVIDIA Blog · Aug 14, 17:13

**背景**: 印尼一直在努力发展其 AI 能力，作为国家数字转型战略的一部分。AI 卓越中心（AI CoE）是一个中心枢纽，帮助组织制定 AI 战略、制定 AI 采用框架，并通过技术专家、行业专家和行业合作伙伴之间的合作建立内部能力。这是印尼首个大学人工智能技术中心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/ai-center-of-excellence">What is an AI center of excellence? - IBM</a></li>

</ul>
</details>

**标签**: `#AI education`, `#Indonesia`, `#NVIDIA`, `#talent development`, `#emerging markets`

---

<a id="item-12"></a>
## [法国 Kog 优化 GPU 用于智能体 AI，声称推理提速 30 倍](https://techcrunch.com/2026/08/14/kog-is-going-deeper-to-squeeze-more-inference-out-of-gpus/) ⭐️ 7.0/10

法国初创公司 Kog 开发了软件优化技术，据报道在标准数据中心 GPU 上实现了大型语言模型推理 30 倍的加速，挑战了 GPU 不适合智能体 AI 工作流程的常见观点。 这挑战了 Cerebras 等公司倡导的硬件优先方案，表明仅通过软件优化就能从现有 GPU 硬件中提取显著性能，可能会颠覆专用 AI 芯片市场，并改变企业构建 AI 推理基础设施的方式。 Kog 声称他们的优化在智能体工作流程中特别有效，这类流程涉及持续决策和多步推理，而非单次推理调用。该公司已有 200 个业务线索，并正在从小型模型扩展到大型语言模型。

rss · TechCrunch AI · Aug 14, 14:50

**背景**: GPU 最初是为图形渲染设计的，但由于其并行处理能力，已成为 AI 训练的主流。许多人认为像 Cerebras 这样的专用芯片对于高效的 AI 推理是必要的，特别是对于需要持续适应和多步推理的智能体工作流程。智能体 AI 与传统 AI 的不同之处在于，它可以根据不断变化的环境自主做出决策和调整策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/08/14/kog-is-going-deeper-to-squeeze-more-inference-out-of-gpus/">Kog is going deeper to squeeze more inference out of GPUs</a></li>
<li><a href="https://en.reflect.ee/article/french-startup-kog-is-developing-gpu-data-processing-acceleration-980e39">French startup Kog is developing GPU data processing acceleration</a></li>
<li><a href="https://endroid.com/2026/kog-gpu-inference-engine-software-optimization/">GPU Inference Engine: Kog Challenges Purpose-Built Chip Thesis</a></li>

</ul>
</details>

**社区讨论**: 行业反应不一——虽然一些人庆祝软件优化方法的验证，但其他人对 30 倍的声称持怀疑态度，并质疑它是否能扩展到具有实际工作负载的生产环境。这场辩论反映了硬件优先和软件优先 AI 基础设施策略之间更广泛的张力。

**标签**: `#AI infrastructure`, `#GPU optimization`, `#startups`, `#AI inference`, `#agentic AI`

---

<a id="item-13"></a>
## [苹果与阿里巴巴合作开发中国定制 AI 模型](https://www.theverge.com/ai-artificial-intelligence/980160/apple-intelligence-china-custom-ai-model-alibaba) ⭐️ 7.0/10

这一合作意义重大，因为它代表了中美之间日益紧张的地缘政治背景下少数的中美科技合作之一。它展示了大型科技公司在全球部署 AI 服务时如何应对不同的监管环境，尤其是在中国这样数据和 AI 监管严格的市场。 这一合作意义重大，因为它代表了中美之间日益紧张的地缘政治背景下少数的中美科技合作之一。它展示了大型科技公司在全球部署 AI 服务时如何应对不同的监管环境，尤其是在中国这样数据和 AI 监管严格的市场。 这款定制 AI 模型似乎是专门为中国市场设计的，很可能旨在符合中国严格的 AI 法规和数据本地化要求。阿里巴巴作为中国最大的云和 AI 提供商之一，带来了苹果在中国运营其 Apple Intelligence 服务所需的本地专业知识和基础设施。

rss · The Verge AI · Aug 14, 09:21

**背景**: 这一合作发生在中美在技术和 AI 方面紧张关系加剧的时期。中国有严格的规定，要求 AI 模型与社会主义价值观保持一致并接受安全审查。苹果等外国公司通常需要本地合作伙伴才能在中国运营 AI 服务，因为中国限制跨境数据流动并要求数据本地化。

**标签**: `#AI`, `#Apple`, `#Alibaba`, `#China`, `#Tech Partnerships`

---

<a id="item-14"></a>
## [Z.ai 仅通过规模化后训练发布 GLM-5.3 实现重大性能提升](https://www.marktechpost.com/2026/08/14/z-ai-ships-glm-5-3-without-retraining-the-base-model-better-at-complex-coding-and-long-horizon-tasks/) ⭐️ 7.0/10

Z.ai 于 2026 年 8 月 14 日发布 GLM-5.3，该模型复用未做任何修改的 743B GLM-5.2 基础模型。所有性能提升都来自规模化后训练，Terminal-Bench 3.0 从 4.6 提升至 28.3，DeepSWE 从 46.2 提升至 66.9。 这证明了通过规模化后训练可以单独实现复杂编码和长程任务的显著提升，而无需承担重新训练基础模型的计算成本。这种方法可能会改变 AI 实验室分配训练资源和制定模型开发策略的方式。 网络安全基准测试显示出比预期更显著的提升，CyberGym 达到 84.5%，ExploitBench 提升超过一倍至 54.4%。这些改进来自于更多的长程任务环境、更多环境类型以及更长的训练时间。模型权重预计将在约两周后发布。

rss · MarkTechPost · Aug 14, 08:03

**背景**: DeepSWE 是一个基准测试，用于衡量前沿编码智能体在来自活跃开源仓库的原创长程软件工程任务上的表现。Terminal-Bench 3.0 评估 AI 智能体在复杂终端任务上的能力。CyberGym 在 OpenSSL 和 FFmpeg 等生产软件的真实漏洞上测试 AI 系统，实现前所未有的规模化（比之前的基准大 7.5 倍）基于执行的客观评估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/datacurve-ai/deep-swe">GitHub - datacurve-ai/deep-swe: Measuring frontier coding agents on original, long-horizon engineering tasks · GitHub</a></li>
<li><a href="https://rdi.berkeley.edu/blog/cybergym/">CyberGym: Evaluating AI Agents' Real-World Cybersecurity ...</a></li>
<li><a href="https://exploitbench.ai/">ExploitBench</a></li>

</ul>
</details>

**标签**: `#AI Models`, `#Post-Training`, `#LLM Development`, `#Benchmark Performance`, `#Z.ai`

---

<a id="item-15"></a>
## [Needle 2：4500 万参数工具调用模型仅 14MB](https://www.marktechpost.com/2026/08/13/cactus-compute-needle-2-45m-parameter-tool-calling-model/) ⭐️ 7.0/10

Cactus Compute 发布了 Needle 2，这是一款开源的 4500 万参数工具调用、设备控制和结构化提取模型，打包为单个 14MB 二进制文件，可在约 28MB 内存中运行完整会话，无需 GPU 或 NPU。 这代表了边缘 AI 部署中极端模型压缩的重大成就。在如此受限的硬件环境（28MB 内存）中运行功能型工具调用模型，为嵌入式系统和物联网设备等极度受限环境中的设备端 AI 开辟了可能性。 该模型在 Seal-Tools 基准测试的两个分割中均排名第一，尽管体积极小但展现出具有竞争力的工具调用能力。它专为没有 GPU 和 NPU 的硬件设计，适合深度嵌入式应用。

rss · MarkTechPost · Aug 14, 05:45

**背景**: 工具调用（也称为函数调用）是大型语言模型调用外部函数和 API 的能力，使其从文本预测器转变为通用控制器。Seal-Tools 基准测试是用于评估 LLM 工具学习能力的数据集。该模型针对传统大型模型因硬件限制无法运行的边缘计算场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2405.08355">[2405.08355] Seal-Tools: Self-Instruct Tool Learning Dataset ... GitHub - fairyshine/Seal-Tools: The source code and dataset ... Seal-Tools: Self-instruct Tool Learning Dataset for Agent ... Seal-Tools: Self-Instruct Tool Learning Dataset for Agent ... Seal-Tools: Self-Instruct Tool Learning Dataset for Agent ... Seal-Tools/README.md at master · fairyshine/Seal-Tools arXiv:2405.08355v1 [cs.CL] 14 May 2024</a></li>
<li><a href="https://github.com/fairyshine/Seal-Tools">GitHub - fairyshine/Seal-Tools: The source code and dataset ...</a></li>

</ul>
</details>

**标签**: `#efficient-ai`, `#edge-computing`, `#model-compression`, `#tool-calling`, `#open-source`, `#embedded-ai`

---

<a id="item-16"></a>
## [世界首个超导量子热引擎演示成功](https://www.sciencedaily.com/releases/2026/08/260814011041.htm) ⭐️ 7.0/10

研究人员成功演示了世界上首个超导量子热引擎，能够在循环过程中将接近绝对零度的热量转化为有用功，该成果发表于《自然·通讯》杂志。 这一突破可能使量子计算机能够更高效地运行，因为目前连接室温电子设备到低温处理器的大量微波电缆体积庞大、成本高昂且产生噪音，未来有望将其淘汰。 该引擎利用超导电路在超冷量子条件下利用微小热量，通过受控的热力学循环输出正功，并测量了功率和效率。

rss · ScienceDaily - Artificial Intelligence · Aug 14, 12:56

**背景**: 量子计算机必须在接近绝对零度（-460°F）的温度下运行以保持量子比特的稳定性。目前它们需要大量的射频和微波电缆来进行控制和信息读取，这些电缆占用空间、引入噪音，并带来可扩展性挑战。量子热引擎是在量子尺度上将热能转化为功的装置，这一领域被称为量子热力学。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sciencedaily.com/releases/2026/08/260814011041.htm">World’s first superconducting quantum heat engine could help ...</a></li>
<li><a href="https://phys.org/news/2026-07-world-superconducting-quantum-path-larger.html">World's first superconducting quantum heat engine offers path ...</a></li>
<li><a href="https://www.nature.com/articles/s41467-026-72651-x">Initial demonstration of a quantum heat engine based on ...</a></li>

</ul>
</details>

**标签**: `#quantum computing`, `#quantum thermodynamics`, `#superconducting systems`, `#quantum hardware`, `#research breakthrough`

---

<a id="item-17"></a>
## [使用 LLM"幻觉"技术进行标签分类](https://simonwillison.net/2026/Aug/14/dont-classify-hallucinate/) ⭐️ 7.0/10

Doug Turnbull 介绍了一种技术，让 LLM 在不查看现有词汇表的情况下为内容生成新颖的、从未见过的标签（"幻觉"），然后使用向量嵌入将这些幻觉标签与现有语料库中最接近的标签进行匹配。 这种方法解决了在大型标签词汇表（如 1,856 个标签）系统中标记内容的实际问题，这些标签数量超过了 LLM 的令牌限制。它将 LLM 的创造力与向量搜索的准确性相结合，实现了可扩展的内容分类，而无需向模型输入大量的标签列表。 该技术的工作原理是提示 LLM 以特定格式生成假设性分类标签（例如"家具/客厅家具/咖啡桌"），然后使用向量嵌入相似性搜索在现有语料库中找到最接近的真实标签。提示中可以包含示例标签格式，以引导模型生成更有用的猜测。

rss · Simon Willison · Aug 14, 21:54

**背景**: 向量嵌入将文本表示为高维空间中的数值向量，其中语义相似的项目聚集在一起。这使得相似性搜索能够找到最接近的匹配项。该技术对于具有数千个标签的内容管理系统特别有用，由于令牌限制，将所有标签包含在单个 LLM 提示中是不切实际的。

**标签**: `#llm-applications`, `#tagging-classification`, `#vector-search`, `#prompt-engineering`, `#content-management`

---

<a id="item-18"></a>
## [谷歌 DeepMind 发布 Gemini 3.7 Flash 性能直逼旗舰价格大降](https://www.infoq.cn/article/plZY01etBHv3ETOYG0af?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

这一发布的重要性在于它挑战了 AI 模型性能和成本之间的传统权衡，可能使开发者和企业更容易获得先进的 AI 能力，同时迫使竞争对手重新考虑其定价策略。 Gemini 3.7 Flash 是 Gemini 3 系列中的主要智能工作模型，填补了深度推理 Pro 模型和高吞吐量 Flash-Lite 模型之间的空白。它改进了 Google Workspace 应用的工具使用，提高了复杂多技能工作流程的准确性，并在编码任务和多模态处理方面表现出色。

rss · InfoQ 中文站 · Aug 15, 00:01

**背景**: 谷歌的 Gemini 系列包括针对不同用例设计的多种模型变体——Pro 模型用于深度推理、Flash-Lite 用于高吞吐量任务，以及 Flash 模型作为平衡能力和效率的工作模型。最近 AI 模型市场竞争激烈，各大提供商不断优化，以更低的成本提供更强的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/gemini/flash/">Gemini 3.7 Flash — Google DeepMind</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/">Gemini 3.7 Flash: our most intelligent workhorse model</a></li>
<li><a href="https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/gemini/3-7-flash">Gemini 3.7 Flash | Gemini Enterprise Agent Platform | Google Cloud Documentation</a></li>

</ul>
</details>

**社区讨论**: 社交媒体上的开发者对 Gemini 3.7 Flash 的强劲性价比表示热情，有人称其为生产级多模态代理的"游戏规则改变者"。该模型在将 Figma 设计转换为代码等任务中的高效实现获得了好评。

**标签**: `#AI`, `#Google DeepMind`, `#Gemini`, `#LLM`, `#machine learning`

---

<a id="item-19"></a>
## [DeepSeek 开源 Harness 框架：全面插件化](https://www.infoq.cn/article/de9AljWc4ejW2KAyW8dD?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

DeepSeek 开源了其 Harness 框架，将模型、工具和 Agent Loop 功能以模块化插件的形式发布给 AI 开发者社区。该框架目前以开发者预览版发布，包含完整源代码。 这标志着 AI Agent 开发生态系统的重要贡献，使开发者构建 AI 应用时能够实现更灵活的集成。模块化插件架构允许开发者根据具体需求交换或重新组合模型、工具、技能和循环等功能。 Harness 框架由 Cordis 驱动，相关设计在《时空可组合性的编程范式》一文中有所描述。每个功能都实现为插件形式：模型、工具、技能、会话、沙箱、存储、循环、调度和 UI。

rss · InfoQ 中文站 · Aug 14, 14:38

**背景**: Agent Loop 是支持自主 AI Agent 持续运行的核心循环：感知→规划→执行→反思。Agent 感知情况、制定计划、执行操作、评估结果，然后重复循环直到达成目标。DeepSeek Harness 将此循环实现为模块化插件，允许开发者自定义或替换推理执行循环。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/deepseek-ai/deepseek-harness">GitHub - deepseek-ai/deepseek-harness: DeepSeek Harness: Everything is ...</a></li>
<li><a href="https://www.deepseek.com/harness/en/">DeepSeek Harness developer preview: Everything is a plugin</a></li>
<li><a href="https://pexo.ai/blog/what-is-an-ai-agent-loop-2316">What Is an AI Agent Loop ? How Autonomous Agents Plan, Act... | Pexo</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#Open Source`, `#AI Agents`, `#LLM Framework`, `#Agent Loop`

---

<a id="item-20"></a>
## [AI 编程工具进入生产环境：从会用到驾驭的真实挑战](https://www.infoq.cn/article/ydy2QDIAzQ1L314UH4qc?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

InfoQ 发布了一篇来自 AICon 会议的技术文章，探讨了在生产环境中部署 AI 编程工具的真实挑战和实践经验，涵盖了从基础使用到高级驾驭的学习曲线过程。 这篇文章解决了 AI 采用领域的一个关键空白——虽然 AI 编程助手是企业 AI 采用率最高的类别，但用户满意度却未能跟上，因此实际的生产部署见解对开发团队来说非常有价值。 文章重点关注从"会用"到"驾驭"AI 编程工具的转变，探讨生产环境中的真实碰撞点。主要挑战包括 AI 幻觉导致的包名劫持风险、有效的提示工程需求，以及在 AI 辅助工作流中维护代码质量。

rss · InfoQ 中文站 · Aug 14, 14:28

**背景**: AI 编程助手如 Cursor、Windsurf、GitHub Copilot 和 Devin 已成为企业 AI 采用率最高的类别。然而，这些工具引入了新的风险，如"包名幻觉"——AI 生成引用不存在的依赖项的代码，从而造成被称为"slopsquatting"的供应链漏洞。提示工程已成为最大化代码生成质量的关键技能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/womencodingcommunity_the-5-most-common-ai-coding-assistant-failures-activity-7382354378256515073-vIyZ">" AI Coding Assistants : The 5 Biggest Challenges and How... | LinkedIn</a></li>
<li><a href="https://en.wikipedia.org/wiki/Slopsquatting">Slopsquatting - Wikipedia</a></li>
<li><a href="https://www.vaasblock.com/news/ai-coding-assistants-cursor-windsurf-github-copilot-developer-2026/">AI Coding Assistants 2026: Cursor, Windsurf, Copilot... | VaaSBlock</a></li>

</ul>
</details>

**标签**: `#AI Coding`, `#Production Environment`, `#Software Development`, `#AIAssisted Programming`, `#Developer Tools`

---

<a id="item-21"></a>
## [AI 实验室每年测试 300 万人体组织样本，或将替代动物测试](https://www.fastcompany.com/91589344/the-worlds-largest-biological-datacenter-could-help-make-animal-testing-obsolete) ⭐️ 7.0/10

这代表了减少药物开发中动物测试依赖的重要一步。尽管约 90% 的临床试验在通过动物测试后仍告失败，业界迫切需要更贴合人体实际的测试方法，以提高药物开发成功率并加速新疗法的发现。 该系统目前由 12 个“蜂巢”机器人实验室组成，每个实验室都能培养和测试人体类器官。每年 300 万样本的总产能是美国所有临床试验产能总和的两倍，为药物候选分子的筛选提供了前所未有的规模。

telegram · zaihuapd · Aug 14, 01:48

**背景**: 类器官是在实验室中培养的三维细胞结构，可以模拟真实人体器官的结构和功能。与传统的二维细胞培养或动物模型相比，这些微型器官为药物测试提供了更符合生理学的模型。高通量筛选使研究人员能够快速测试数千种化合物，这对于高效识别有前景的药物候选分子至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.thermofisher.com/us/en/home/life-science/cell-culture/organoids-spheroids-3d-cell-culture.html">Fundamentals of 3D Cell Culture - Thermo Fisher Scientific - US</a></li>
<li><a href="https://www.cytivalifesciences.com/en/us/insights/what-is-highthroughput-screening-hts">What is highthroughput screening (HTS)?</a></li>

</ul>
</details>

**标签**: `#AI in biotechnology`, `#Drug testing alternatives`, `#Robotics in research`, `#Animal welfare`, `#Pharmaceutical innovation`

---

<a id="item-22"></a>
## [苹果寻求最高法院审查 App Store 收费裁决，已获暂停执行](https://t.me/zaihuapd/43181) ⭐️ 7.0/10

这标志着 2020 年开始的 Epic 与苹果反垄断斗争的重大升级，可能对整个移动应用生态系统及全球平台费用结构产生深远影响。最高法院的最终裁决可能重塑应用商店经济及开发者经济。 第九巡回上诉法院于 2025 年 12 月维持了对苹果的民事藐视法庭认定，即苹果对外部支付收取 27%佣金并使用“恐吓屏幕”来规避法院命令的支付竞争。原始裁决要求苹果停止屏蔽外部支付链接并取消限制开发者沟通替代购买方式的规定。

telegram · zaihuapd · Aug 14, 02:33

**背景**: Epic Games 诉苹果案始于 2020 年 8 月，当时 Epic 挑战苹果强制使用应用内支付系统并收取 30%佣金的政策。该案核心问题是苹果的 App Store 政策是否违反联邦和加州竞争法。暂停执行是法律命令，可在上诉期间暂时中止法院判决的执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Epic_Games_v._Apple">Epic Games v. Apple - Wikipedia</a></li>
<li><a href="https://law.justia.com/cases/federal/appellate-courts/ca9/25-2935/25-2935-2025-12-11.html">EPIC GAMES, INC. V. APPLE INC., No. 25-2935 (9th Cir. 2025)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Stay_of_execution">Stay of execution - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Apple`, `#App Store`, `#Epic Games`, `#Legal/Antitrust`, `#Mobile Apps`

---

<a id="item-23"></a>
## [小红书开源 280B MoE 模型 dots3-note](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 7.0/10

这具有重要意义，因为它代表了小红书的首次重大开源发布，使该模型在与其他大型 MoE 模型的竞争中处于有利地位。新的 TEMPO 强化学习方法使用自批判和测试时价值估计来训练长程智能体，在技术上是创新的，解决了现实世界智能体部署的挑战。 该模型支持混合 DSA 和 SWA 架构，提供 BF16 和 FP8 格式，并包含 MTP 投机解码。TEMPO 强化学习方法利用自批判和测试时价值估计，专门用于训练长程任务中的智能体。还发布了两个真实场景智能体基准：VibeSearchBench 和 VibeLifeBench。

telegram · zaihuapd · Aug 14, 08:27

**背景**: 混合专家（MoE）是一种架构，使用多个专业化子模型（专家），对于每个输入只激活一部分，从而能够在降低计算成本的情况下实现大容量模型。小红书是一个流行的中国生活方式和社交媒体平台。TEMPO RL 方法是一种新型强化学习方法，将自批判与测试时价值估计相结合，以改善复杂多步骤任务中的智能体表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/studio-dots-ai/dots3-note-prev">GitHub - studio-dots-ai/ dots 3 - note -prev: dots 3 note preview · GitHub</a></li>
<li><a href="https://recipes.vllm.ai/dots-studio/dots3-note-prev">dots-studio/ dots 3 - note -prev | vLLM Recipes</a></li>
<li><a href="https://book.st-hakky.com/en/news/tempo-vla-semantic-action-rl-posttrain">TEMPO Achieves and Maintains High Reward in Real-World ...</a></li>

</ul>
</details>

**标签**: `#large-language-model`, `#mixture-of-experts`, `#open-source`, `#multimodal-ai`, `#reinforcement-learning`

---

<a id="item-24"></a>
## [谷歌被令取消第三方应用商店安装障碍](https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/) ⭐️ 7.0/10

美国地区法官 James Donato 下令谷歌在一周内取消安卓第三方应用商店的安装障碍，删除包含警告弹窗的多步安装流程，法院认定这些步骤构成蓄意制造的反竞争摩擦。 这一里程碑式的裁决直接影响安卓应用分发模式，可能显著影响谷歌在移动应用生态系统中的垄断地位。这是 Epic 游戏和其他长期抱怨竞争应用商店障碍的开发者的一次重大胜利。 法院认定，谷歌要求用户先'查看'再'安装'第三方应用商店的多步流程是故意设计用来阻止普通用户的。谷歌必须使第三方市场的安装像安装普通安卓应用一样直接。

telegram · zaihuapd · Aug 14, 09:55

**背景**: 该命令源自 Epic 诉谷歌反垄断案，此前陪审团裁定谷歌在安卓应用分发上构成非法垄断。案件始于 2020 年，当时 Epic 挑战谷歌的 30%应用商店佣金和限制性政策。谷歌 Play Protect（安卓内置安全扫描系统）将继续运行，但不能再被用作阻止第三方应用商店安装的摩擦机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_Play_Protect">Google Play Protect</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#android`, `#google-play`, `#mobile-apps`, `#epic-games`, `#regulation`

---

<a id="item-25"></a>
## [苹果联手阿里开发中国专属 AI 大模型](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 7.0/10

苹果已专门为中国市场训练一款大语言模型，并获得阿里巴巴支持，一改此前依赖第三方模型的策略。Apple Intelligence 预计未来数月随 iOS 更新在华上线。 若成功获批，苹果或成为首个在华提供自有 AI 模型的外国公司，展示出科技巨头如何适应当地监管要求。该合作反映出中国庞大的智能手机市场的重要性，以及外国公司需要与本地合作伙伴合作以满足监管要求的必要性。 苹果的模型已于上个月向中国网信办提交生成式 AI 服务备案。通过这款自研模型，苹果将能更好地掌控中国市场的 AI 体验。

telegram · zaihuapd · Aug 14, 14:47

**背景**: 在中国，外国公司需要先完成网信办备案才能提供 AI 服务。截至 2025 年 7 月，全国已有 439 个 AI 模型通过备案。Apple Intelligence 是苹果公司独立开发的个人智能系统，通过强大的苹果 AI 生成式模型深度整合至 iPhone、iPad 和 Mac 芯片核心，为用户带来个性化的智能体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/1896984498073236885">AI合规必备：算法备案、大模型备案及登记全攻略【附流程+材料清单】 -...</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1941433976045700647">大模型网信办备案详细步骤说明 - 知乎</a></li>
<li><a href="https://www.apple.com/apple-intelligence/">Apple Intelligence and Siri</a></li>

</ul>
</details>

**标签**: `#Apple AI`, `#China tech market`, `#Alibaba partnership`, `#AI regulation`, `#Apple Intelligence`

---