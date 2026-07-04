---
layout: default
title: "Horizon Summary: 2026-07-04 (ZH)"
date: 2026-07-04
lang: zh
---

> From 137 items, 15 important content pieces were selected

---

1. [Hugging Face Diffusers v0.39.0 引入 NVIDIA Cosmos 3 支持 Physical AI](#item-1) ⭐️ 8.0/10
2. [欧洲议会议员遭 Pegasus 间谍软件入侵](#item-2) ⭐️ 8.0/10
3. [Anthropic 指控阿里巴巴发动史上最大规模 AI 蒸馏攻击](#item-3) ⭐️ 8.0/10
4. [Costco：反亚马逊的仓储模式](#item-4) ⭐️ 7.0/10
5. [Starlink 在非洲的快速普及](#item-5) ⭐️ 7.0/10
6. [FreeBSD 内核内存 Bug 调查与修复](#item-6) ⭐️ 7.0/10
7. [PostgreSQL 与 OOM killer：为何 Ubicloud 使用严格内存超额分配](#item-7) ⭐️ 7.0/10
8. [Anthropic 推出 Claude Science AI 工作台，进军药物研发领域](#item-8) ⭐️ 7.0/10
9. [设备复活死亡捐献者眼球 或使眼球移植成为可能](#item-9) ⭐️ 7.0/10
10. [Current AI 发布开源 AI 差距地图](#item-10) ⭐️ 7.0/10
11. [OpenAI 和 Anthropic 开发自研 AI 芯片挑战 NVIDIA](#item-11) ⭐️ 7.0/10
12. [Claude Fable 5 重新上线体验缩水 安全误判遭开发者吐槽](#item-12) ⭐️ 7.0/10
13. [华为发布 Atlas 350 加速卡：昇腾 950PR，算力达 H20 近三倍](#item-13) ⭐️ 7.0/10
14. [阿里下令全员卸载 Claude 7 月 10 日生效](#item-14) ⭐️ 7.0/10
15. [阿图因 AI 在 CyberGym 基准测试中超越 Claude Mythos](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Hugging Face Diffusers v0.39.0 引入 NVIDIA Cosmos 3 支持 Physical AI](https://github.com/huggingface/diffusers/releases/tag/v0.39.0) ⭐️ 8.0/10

Hugging Face 发布了 diffusers v0.39.0 版本，其中最大的亮点是引入了 NVIDIA 的 Cosmos 3 作为 Physical AI 的统一世界基础模型。Cosmos 3 采用混合 Transformer（MoT）架构，将世界生成、物理推理和动作生成整合到一个全能模型中，取代了之前版本中独立的 Predict、Reason 和 Transfer 模型。 此版本代表了 Physical AI 领域的重大进展，通过将生成、推理和动作能力整合到单一统一模型中。MoT 架构使模型能够针对不同输入处理多种策略，同时保持共享表示空间，这可能加速开发能够感知和与物理世界交互的自主机器。 Cosmos3OmniTransformer 并行运行 Qwen 风格的语言模型和扩散生成路径，并通过 3D 多模态 RoPE 连接。此版本还包含视频到视频生成、动作条件生成和声音编码器。其他新增管道包括 Ideogram 4（流匹配文本到图像）、Krea 2（单流 MMDiT）、DreamLite（字节跳动文本到图像）和 PRX Pixel（像素空间生成）。

github · sayakpaul · Jul 3, 08:55

**背景**: Physical AI 是指能够感知、理解并在真实物理世界中执行复杂动作的 AI 系统，将数字 AI 与感知和执行动作的硬件相连接。世界基础模型（WFM）是 Physical AI 的关键组成部分，通过基于视频的观察提供环境的视觉理解。混合 Transformer（MoT）是一种架构，将多个 Transformer 块组合在一起，针对不同输入启用适当的处理策略，同时保持共享表示空间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/glossary/generative-physical-ai/">What is Physical AI? | NVIDIA Glossary</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/mixture-of-transformers/">Mixture of Transformers (MoT) Definition & Architecture | NVIDIA</a></li>
<li><a href="https://arxiv.org/html/2501.03575v1?ref=whoisyan.com">Cosmos World Foundation Model Platform for Physical AI</a></li>

</ul>
</details>

**标签**: `#diffusion-models`, `#physical-ai`, `#nvidia`, `#computer-vision`, `#multimodal-ai`, `#machine-learning`

---

<a id="item-2"></a>
## [欧洲议会议员遭 Pegasus 间谍软件入侵](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

研究组织 Citizen Lab 确认，欧洲议会议员斯蒂里奥斯·库洛格 lou 的 iPhone 于 2022 年 10 月 21 日以及 2023 年 3 月 6 日至 7 日被成功植入 Pegasus 间谍软件，表明欧洲情报机构可能是此次攻击的幕后黑手。 这是对政府级间谍软件针对欧盟民选官员的重大滥用，引发了对民主监控和成员国法治的严重关切。此事件凸显了 Pegasus 不仅被用于针对记者和活动人士，还被用于针对欧盟内部的政治人物。 取证分析发现，首次感染与此前已确认的 Pegasus 活动存在重叠，该活动针对欧洲的俄罗斯和白俄罗斯语流亡记者及活动人士。同一部设备可能同时泄露了机密个人医疗信息和机密政府文件，引发了对欧洲议会设备分离政策的质疑。

hackernews · ledoge · Jul 3, 20:38

**背景**: Pegasus 是由以色列 NSO 集团开发的高级间谍软件，可通过零点击漏洞部署，无需用户任何操作即可入侵设备。Citizen Lab 是多伦多大学蒙克全球事务与公共政策学院的研究部门，专门调查针对记者、政治人物和人权活动人士的间谍软件攻击。希腊、波兰和意大利等多个欧洲国家都曾发生涉及滥用 Pegasus 针对记者、政治人物和公民的丑闻。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://citizenlab.ca/">The Citizen Lab - The Citizen Lab</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab</a></li>
<li><a href="https://www.kaspersky.com/resource-center/definitions/what-is-zero-click-malware">Zero - Click Exploits</a></li>

</ul>
</details>

**社区讨论**: 社区评论者指出，这与此前针对流亡记者的 Pegasus 活动存在重叠，并质疑欧洲议会为何缺乏设备分离政策。有些人强调，类似的 Pegasus 滥用事件曾在希腊、波兰和意大利发生，一些以色列公司因广泛滥用而切断了与欧洲客户的联系。关于这是否应被定性为针对欧洲议会的特定攻击，还是更广泛的国内监控模式的一部分，存在争议。

**标签**: `#cybersecurity`, `#spyware`, `#pegasus`, `#surveillance`, `#european-parliament`, `#privacy`

---

<a id="item-3"></a>
## [Anthropic 指控阿里巴巴发动史上最大规模 AI 蒸馏攻击](https://t.me/zaihuapd/42327) ⭐️ 8.0/10

Anthropic 指控阿里巴巴发动了 AI 历史上已知最大规模的"蒸馏攻击"，称该公司使用约 2.5 万个欺诈账户，在 2026 年 4 月 22 日至 6 月 5 日期间与 Claude 进行了超过 2880 万次交互，以提取模型能力。 这代表了中美 AI 公司之间 AI 知识产权纠纷的重大升级，可能为 AI 模型保护如何监管开创先例。所谓的攻击规模（2880 万次交互）超过了以往的事件，可能影响中美科技竞争格局。 Anthropic 致信美国参议院银行委员会详细说明了这些指控。攻击涉及阿里巴巴及其 AI 实验室 Qwen。蒸馏是一种用更弱的模型学习更强模型的输出以复制其能力的技术。

telegram · zaihuapd · Jul 3, 06:21

**背景**: 模型蒸馏是一种合法的 AI 训练技术，其中较小的"学生"模型学习模仿较大的"教师"模型的行为和知识。未经授权进行蒸馏可能构成知识产权盗窃。阿里巴巴的 Qwen 是 2023 年推出的主要中国 AI 模型系列，最初名为通义千问，已成为中国的领先开源 AI 模型之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gaussianwaves.com/2025/02/model-distillation-explained-how-deepseek-leverages-the-technique-for-ai-success/">Model Distillation Explained: How DeepSeek Leverages the ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI_IP_theft`, `#Anthropic_Claude`, `#Alibaba_Qwen`, `#US_China_AI_competition`, `#model_distillation`

---

<a id="item-4"></a>
## [Costco：反亚马逊的仓储模式](https://phenomenalworld.org/analysis/the-anti-amazon/) ⭐️ 7.0/10

一篇分析文章将 Costco 的仓储自提模式与亚马逊的送货上门模式进行比较，突出了 Costco 如何通过让顾客自行运输商品来避免最后一英里配送问题。 最后一英里配送问题指的是将包裹从配送中心送到客户家门口的复杂且昂贵的最后一段路程，亚马逊必须为每个订单解决这一问题，而 Costco 则将这一负担转移给自行批量取货的顾客。 关键在于，亚马逊需要用卡车逐一送货上门，而 Costco 则用卡车将整托盘货物送到面向消费者的仓库，然后由顾客自己开车将商品运回家。这两种模式在物流成本结构上存在本质差异。

hackernews · bookofjoe · Jul 3, 15:14

**背景**: 最后一英里配送问题被广泛认为是电子商务物流中最复杂且最昂贵的部分，通常占配送总成本的很大比例。Costco 采用仓储会员店模式，顾客支付年度会员费后在实体店批量购物，直接取货而非等待送货上门。这种模式使 Costco 成为全球最大的零售商之一，同时保持相对较低的价格。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://onfleet.com/blog/last-mile-problem/">The Last Mile Delivery Problem : Here's How to Solve it</a></li>

</ul>
</details>

**社区讨论**: 社区成员讨论了物流权衡问题，部分人质疑鉴于顾客需要开车前往门店，Costco 的模式是否真正具有社会价值。另一些人引用工程格言：「智者解决问题，贤者避免问题」，认为 Costco 的做法体现了设计上的智慧。部分批评了仓储零售的汽车中心主义，而另一些人为其辩护，认为这对于喜欢每月批量购物的郊区消费者来说很实用。

**标签**: `#retail`, `#business-model`, `#logistics`, `#e-commerce`, `#systems-thinking`

---

<a id="item-5"></a>
## [Starlink 在非洲的快速普及](https://www.economist.com/middle-east-and-africa/2026/07/02/africans-are-turning-to-starlink) ⭐️ 7.0/10

《经济学人》报道了 Starlink 在非洲的快速普及，卫星互联网服务正在被之前无法获得传统有线基础设施服务的人群所接受。 这种普及代表了服务不足人群数字接入的重大转变，可能在铺设电缆或光纤基础设施不切实际或不可能的地区弥合数字鸿沟。 Starlink 使用低地球轨道(LEO)卫星，延迟时间为 25-60 毫秒，而传统地球静止轨道卫星互联网的延迟高达 600 毫秒。该服务在美国每月约需 55 美元，在电力不稳定的地区可以使用汽车充电器等替代电源运行。

hackernews · bookofjoe · Jul 3, 21:08

**背景**: Starlink 是 SpaceX 的卫星互联网星座，使用低地球轨道卫星向偏远地区提供宽带互联网。与在地球上方 35,786 公里轨道运行的传统地球静止轨道卫星不同，Starlink 的卫星在 540-570 公里轨道运行，大大降低了延迟。这项技术使得在铺设传统电缆或光纤基础设施在经济上不可行的地区也能接入互联网。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Starlink">Starlink - Wikipedia</a></li>
<li><a href="https://www.satelliteinternet.com/providers/starlink/">Starlink Internet Plans and Cost [2026]</a></li>

</ul>
</details>

**社区讨论**: 评论强调了 Starlink 的使命驱动特性，一位前工程师强调其作为"平等工具"为服务不足人群带来互联网的作用。南非用户解释了严重的基础设施挑战，包括每天长达 10 小时的停电。其他人将 Starlink 与非洲移动电话跳过有线基础设施的跨越式发展相比，认为 Starlink 为农村互联网接入填补了类似的空白。

**标签**: `#Starlink`, `#satellite internet`, `#Africa`, `#digital divide`, `#infrastructure`

---

<a id="item-6"></a>
## [FreeBSD 内核内存 Bug 调查与修复](https://crocidb.com/post/freebsd-ate-my-ram/) ⭐️ 7.0/10

一名开发者调查并修复了 FreeBSD 内核中的一个 bug，该 bug 导致 vm_map 子系统中未使用的内存页面未被正确释放，从而导致内存使用量报告膨胀。相关修复已被合并到上游代码库。 该 bug 位于内核的虚拟内存映射（vm_map）系统中，未使用的内存页面未被正确释放回系统。开发者通过内核内存调试工具和 vmstat 追踪了这个问题，找到了 Accounting 不正确的位置。

hackernews · theanonymousone · Jul 3, 19:08

**背景**: FreeBSD 使用一个名为 vm_map 的虚拟内存子系统来管理内核虚拟地址空间。区域分配器将内核虚拟内存（KVM）分割成不同内核结构的常量大小块。可以使用 vmstat -m 查看按区域划分的 KVM 利用率。这个 bug 导致系统报告的“已用”内存比实际更多。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.freebsd.org/en/books/arch-handbook/vm/">Chapter 7. Virtual Memory System | FreeBSD Documentation Portal</a></li>
<li><a href="https://man.freebsd.org/cgi/man.cgi?query=vm_map">vm_map</a></li>
<li><a href="https://forums.freebsd.org/threads/memory-management-freebsd-kernel.84787/">Memory management FreeBSD kernel | The FreeBSD Forums</a></li>

</ul>
</details>

**社区讨论**: 社区对这篇高质量的技术深入分析表示赞赏，一位评论者感谢作者的分享，另一位祝贺他们成功将修复合并到上游。还有关于内存 Accountingheuristics 的讨论——一位评论者质疑为什么精确的内存统计需要启发式方法而不是精确数字，指出“系统使用的内存始终是总量减去可用内存”。

**标签**: `#freebsd`, `#debugging`, `#memory`, `#systems-programming`, `#operating-systems`

---

<a id="item-7"></a>
## [PostgreSQL 与 OOM killer：为何 Ubicloud 使用严格内存超额分配](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 7.0/10

Ubicloud 解释了他们在生产环境中对 PostgreSQL 使用严格内存超额分配(vm.overcommit_memory=2)来避免 OOM killer 问题的运营决策，尽管作者后来承认标题过于激进，且这种做法在某些场景下会产生副作用。 这对大规模管理 PostgreSQL 的数据库管理员和 DevOps 工程师非常重要，因为 OOM killer 可能在内存压力下导致不可预测的数据库崩溃。讨论强调了内存超额分配模式之间的实际权衡。 严格超额分配模式(vm.overcommit_memory=2)根据实际物理内存+swap 强制执行内存分配硬限制，拒绝超过此阈值的分配。社区成员警告说，这可能会阻止 fork 操作，并在应用程序与 PostgreSQL 部署在同一台机器上时导致系统不稳定。

hackernews · furkansahin · Jul 3, 13:00

**背景**: Linux 内存超额分配是内核的一个特性，允许进程分配比物理可用内存更多的虚拟内存。OOM(内存耗尽)killer 是 Linux 内核的一种机制，当系统内存耗尽时会终止进程。内存超额分配有三种模式：模式 0(启发式，默认值)、模式 1(始终超额分配)和模式 2(永不超额分配，即严格模式)。模式 2 可能导致 malloc()失败而不是触发 OOM killer。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kernel.org/doc/html/v6.13/mm/overcommit-accounting.html">Overcommit Accounting — The Linux Kernel documentation</a></li>
<li><a href="https://www.baeldung.com/linux/overcommit-modes">Linux Overcommit Modes | Baeldung on Linux</a></li>

</ul>
</details>

**社区讨论**: 讨论显示情绪复杂——虽然一些人认同对数据库使用严格超额分配的方法，但其他人警告说会产生副作用，包括阻止 fork 操作和系统不稳定。社区成员 Bender 强调在生产部署前要在 QA/Perf 环境中进行测试。作者 ozgune 承认标题过于激进，许多场景可能会产生意外的副作用。

**标签**: `#postgresql`, `#linux`, `#memory-management`, `#oom-killer`, `#devops`, `#systems`

---

<a id="item-8"></a>
## [Anthropic 推出 Claude Science AI 工作台，进军药物研发领域](https://www.theverge.com/ai-artificial-intelligence/961311/anthropic-claude-science-ai-drug-development) ⭐️ 7.0/10

Anthropic 发布了 Claude Science，这是一款面向科学家的新型 AI 工作台，可将分散的工具和数据集整合到统一环境中用于药物研发，并可生成图表和可视化内容。 这标志着 Anthropic 大规模进军科学研究和药物研发领域，反映了主要 AI 公司在医疗健康领域的战略布局。此举使 Claude 成为现有科学研究工具的竞争对手，并可能加速制药研究的工作流程。 Claude Science 在「The Briefing: AI for Science」活动上发布。该平台旨在统一科学研究中分散的工具景观，允许科学家在单一界面中访问多个数据集和工具，同时自动生成图表。

rss · The Verge AI · Jul 3, 13:56

**背景**: 传统药物研发涉及复杂的工作流程，包含许多互不连接的工具和数据库。谷歌 DeepMind 和微软等 AI 公司一直在加大对科学研究应用的投资，利用机器学习加速分子发现、预测蛋白质结构和优化临床试验。Anthropic 进入该领域紧随竞争对手的类似举措。

**标签**: `#AI`, `#Anthropic`, `#drug development`, `#scientific research`, `#product launch`

---

<a id="item-9"></a>
## [设备复活死亡捐献者眼球 或使眼球移植成为可能](https://www.technologyreview.com/2026/07/03/1140148/a-device-that-revives-eyeballs-from-dead-donors-could-make-eye-transplants-possible/) ⭐️ 7.0/10

这一突破可能使数百万患有不可逆失明的人恢复视力。全眼球移植曾被尝试过但失败了，因为移植的眼球无法看到东西——主要原因是视神经再生方面的挑战。 该设备使用灌注和保存技术维持和复活死亡捐献者的眼球。类似的器官保存设备如 LifePort 通过循环保存溶液、给器官充氧并维持适当温度来防止退化。

rss · MIT Technology Review · Jul 3, 17:34

**背景**: 全眼球移植一直是眼科领域的前沿，有望为不可逆失明提供变革性的治疗方法。然而，巨大的挑战仍然存在，包括需要视神经再生来恢复视力。之前移植尝试中的眼球因退化和神经连接失败而无法看到。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11212585/">Whole - eye transplantation : Current challenges and future...</a></li>
<li><a href="https://www.frontiersin.org/journals/medicine/articles/10.3389/fmed.2025.1691259/full">Frontiers | Allogeneic whole - eye transplantation : advancements...</a></li>
<li><a href="https://www.organ-recovery.com/always-listening-always-innovating/">Always Listening, Always Innovating: ORS... - Organ Recovery Systems</a></li>

</ul>
</details>

**标签**: `#medical research`, `#eye transplant`, `#organ donation`, `#biomedical device`, `#vision restoration`

---

<a id="item-10"></a>
## [Current AI 发布开源 AI 差距地图](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 7.0/10

获得 4 亿美元资金支持的非营利组织 Current AI 发布了开源 AI 差距地图 v0.1，索引了来自 228 个组织的 421 个产品，涵盖软件工具、模型、数据集和硬件类别。 这个全面的目录为 AI 社区了解开源 AI 生态系统的现状提供了有价值的参考，尽管它主要是一项文档和编目工作，而非技术突破。 差距地图将产品分为 14 个类别，跨越 3 个技术栈层（模型组件、产品/UX 和基础设施）。底层数据以 MIT 许可证发布在 GitHub 上，包含 1,184 个 YAML 文件和 16,185 个被追踪的 GitHub 仓库。

rss · Simon Willison · Jul 3, 22:04

**背景**: Current AI 于 2025 年 2 月在巴黎人工智能行动峰会上作为非营利组织成立，目标是"为人工智能建立公共选择方案"。该组织已获得 4 亿美元的承诺资金。这个差距地图是他们绘制开源 AI 领域图景的首个主要公开成果。

**标签**: `#open-source-ai`, `#ai-ecosystem`, `#resources`, `#tools`, `#datasets`

---

<a id="item-11"></a>
## [OpenAI 和 Anthropic 开发自研 AI 芯片挑战 NVIDIA](https://www.infoq.cn/article/MOqFJbvWYlJ9PXcfdfCC?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

这直接挑战了 NVIDIA 在 AI 芯片市场的主导地位，其 Blackwell 芯片售价高达每片 3 万至 4 万美元。如果成功开发自研芯片，将大幅降低 AI 基础设施成本，打破 NVIDIA 的价格垄断地位，可能重塑整个 AI 硬件生态系统。 NVIDIA 的 H100 GPU 售价高达 4 万美元，约是 AMD 竞品 MI300X（1 万至 1.5 万美元）价格的四倍。Anthropic 已从 OpenAI 芯片部门挖来 Clive Chan 负责芯片开发工作。OpenAI 与 Broadcom 合作开发了 Jalapeño 芯片，标志着 AI 行业向定制硅片的重大转变。

rss · InfoQ 中文站 · Jul 3, 18:00

**背景**: NVIDIA 凭借其 CUDA 生态系统和高性能 GPU 主导 AI 芯片市场，使得竞争对手难以进入。NVIDIA GPU 的高昂成本（H100：2.7 万至 4 万美元；Blackwell：3 万至 4 万美元）已成为 AI 公司扩大规模的重大瓶颈。谷歌、亚马逊和微软等主要科技公司已经开发了定制芯片，而 OpenAI 和 Anthropic 现在也纷纷效仿，以减少对单一供应商的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2024/03/19/nvidias-blackwell-ai-chip-will-cost-more-than-30000-ceo-says.html">Nvidia's Blackwell AI chip will cost more than $30,000, CEO says</a></li>
<li><a href="https://www.reddit.com/r/hardware/comments/1ahgu7q/nvidias_h100_ai_gpus_cost_up_to_four_times_more/">r/hardware on Reddit: Nvidia's H100 AI GPUs cost up to four times more than AMD's competing MI300X — AMD's chips cost $10 to $15K apiece; Nvidia's H100 has peaked beyond $40,000: Report</a></li>
<li><a href="https://techcrunch.com/2026/07/02/anthropic-is-discussing-a-new-custom-chip-with-samsung/">Anthropic is discussing a new custom chip with Samsung</a></li>
<li><a href="https://blockonomi.com/anthropic-eyes-custom-ai-chip-development-with-samsung-as-manufacturing-partner/">Anthropic Eyes Custom AI Chip Development with Samsung as ...</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#NVIDIA`, `#OpenAI`, `#Anthropic`, `#Hardware`

---

<a id="item-12"></a>
## [Claude Fable 5 重新上线体验缩水 安全误判遭开发者吐槽](https://www.bleepingcomputer.com/news/artificial-intelligence/claude-fable-relaunch-disappoints-users-with-nerfed-performance/) ⭐️ 7.0/10

Anthropic 在美国解除出口管制后恢复了 Claude Fable 5 的全球访问权限，但用户报告体验大幅缩水，包括 7 月 7 日前每周 50%的配额限制，以及频繁的安全误判导致代码处理自动降级到 Opus 4.8 等旧版模型。 这对于依赖 Claude Fable 5 进行复杂编码任务的开发者影响很大，因为安全误判频繁中断正常开发工作，迫使用户花了旗舰模型的钱却得到较旧、能力较弱的替代模型。 模型本身的性能并未被削弱，只是安全分类器的阈值设置过于激进。API 和企业按量付费用户可以完全访问 Claude Fable 5，而订阅用户在 7 月 7 日前面临 50%的配额限制，之后 Fable 5 将转为按量付费。

telegram · zaihuapd · Jul 3, 07:20

**背景**: 2024 年 6 月，美国商务部对 Claude Fable 5 实施出口管制，限制其全球可用性。6 月 12 日管制解除后，Anthropic 得以恢复访问。Claude Fable 5 是 Anthropic 的旗舰模型，专为复杂推理和编码任务设计，而 Opus 4.8 是一款更保守的备用模型，具有更严格的安全措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropic-restores-claude-fable-5-as-us-lifts-export-controls">Anthropic restores Claude Fable 5 as US lifts... | Tom's Hardware</a></li>
<li><a href="https://www.techtimes.com/articles/319576/20260702/claude-fable-5-debugging-scores-drop-70-safety-classifier-reroutes-tasks-weaker-fallback-model.htm">Claude Fable 5 Debugging Scores Drop 70%: Safety Classifier...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Anthropic`, `#Claude`, `#Developer Tools`, `#API`

---

<a id="item-13"></a>
## [华为发布 Atlas 350 加速卡：昇腾 950PR，算力达 H20 近三倍](https://t.me/zaihuapd/42329) ⭐️ 7.0/10

在 2026 年华为中国合作伙伴大会上，华为正式发布了搭载全新昇腾 950PR 处理器的人工智能训练推理加速卡 Atlas 350。该产品是目前国内唯一支持 FP4 低精度推理的加速卡，单卡算力达到英伟达 H20 的 2.87 倍，HBM 容量达 112GB。 此次发布标志着华为在 AI 加速卡市场强势挑战英伟达的主导地位。FP4 支持和大容量 HBM 可能大幅降低 AI 推理成本，支持更大参数模型部署，推动中国 AI 硬件自主可控进程。 Atlas 350 算力达英伟达 H20 的 2.87 倍，配备 112GB HBM，支持 70B 参数模型单卡加载，向量算力和互联带宽较前代大幅提升。但这些数据为华为官方声称，尚未得到独立验证。

telegram · zaihuapd · Jul 3, 08:35

**背景**: FP4 是一种 4 位浮点精度格式，可在保持可接受推理精度的同时降低计算复杂度，显著提高能效。高带宽内存（HBM）是一种 3D 堆叠内存技术，相比传统内存提供更高带宽，对数据密集型 AI 工作负载至关重要。英伟达于 2025 年中期推出 NVFP4 优化低精度推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.micron.com/products/memory/hbm">High-bandwidth memory (HBM) | Micron Technology Inc.</a></li>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision ...</a></li>

</ul>
</details>

**标签**: `#AI_hardware`, `#Huawei`, `#Ascend_950PR`, `#AI_accelerator`, `#China_tech`

---

<a id="item-14"></a>
## [阿里下令全员卸载 Claude 7 月 10 日生效](https://t.me/zaihuapd/42334) ⭐️ 7.0/10

阿里巴巴内部宣布反向禁用 Claude，要求员工卸载 Anthropic 相关产品，包括 Sonnet、Opus、Fable 等模型以及 Claude Code，禁令将于 7 月 10 日生效。此举逆转了阿里此前报销员工使用 Claude、GPT、Gemini 等外部 AI 模型费用的政策。 这标志着中美科技在 AI 领域的紧张关系显著升级。史无前例的禁令表明，虚假账户滥用指控如何迅速恶化主要科技公司之间的关系，可能重塑中国公司获取西方 AI 工具的方式。 Anthropic 曾指控阿里在 4 月 22 日至 6 月 5 日期间使用约 2.5 万个虚假账号与 Claude 交互超 2800 万次，随后收紧了风控措施。禁令特别针对所有 Anthropic 产品，包括 Claude Code AI 编程助手。

telegram · zaihuapd · Jul 3, 13:00

**背景**: 阿里此前对外部 AI 工具持开放政策，报销员工使用 Claude、GPT 和 Gemini 的费用。Claude Code 是 Anthropic 开发的 AI 驱动编码助手，帮助开发者构建功能、修复错误和自动化开发任务。虚假账户滥用指控是迄今为止报道的最大规模 AI 模型操纵案例之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.claude.com/docs/zh-CN/overview">概述 - Claude Code Docs</a></li>
<li><a href="https://www.cnblogs.com/knqiufan/p/19449849">Claude Code 完全指南：使用方式、技巧与最佳实践 - knqiufan - 博客园</a></li>

</ul>
</details>

**标签**: `#AI`, `#Alibaba`, `#Anthropic`, `#US-China Tech Relations`, `#Industry News`

---

<a id="item-15"></a>
## [阿图因 AI 在 CyberGym 基准测试中超越 Claude Mythos](https://mp.weixin.qq.com/s/BzU7g-2iG7d6h4ViwMhxyg) ⭐️ 7.0/10

腾讯玄武实验室的阿图因 AI 在加州大学伯克利分校的 CyberGym 网络安全基准测试中获得 84.0% 的得分，超越 Anthropic 的 Claude Mythos，同时使用预算不到后者的 0.1%。还在 curl、OpenSSL、Python cryptography 等重要开源项目中发现了 Mythos 未检出的多个高危逻辑漏洞。 这表明可本地部署的开源模型能够在漏洞检测方面超越昂贵的前沿模型，可能使先进的 AI 安全工具更加普及。以极低的成本实现相似或更好的效果，可能会显著影响组织进行软件安全审计的方式。 阿图因 AI 基于智谱 AI 的 GLM-5.1 构建，这是一个拥有 7440 亿参数的开源混合专家模型。检测到的最高漏洞严重程度评分为 9.3，在伯克利 BVI 真实世界漏洞榜单中，阿图因 AI 的严重漏洞严重程度排名第 1，总数排名第 5。

telegram · zaihuapd · Jul 3, 16:12

**背景**: CyberGym 是加州大学伯克利分校推出的综合基准测试，用于评估 AI 智能体在大型代码库中发现和利用真实软件漏洞的能力。GLM-5.1 是智谱 AI 的最新开源模型，具有 8 小时自主任务执行能力。Project Glasswing 是 Anthropic 的倡议，使用 Claude Mythos 扫描关键开源软件基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rdi.berkeley.edu/blog/cybergym/">Center for Responsible, Decentralized Intelligence at Berkeley</a></li>
<li><a href="https://pandaily.com/zhipu-unveils-glm-5-1-its-most-advanced-open-source-model-with-8-hour-autonomous-task-capability">Zhipu Unveils GLM-5.1, Its Most Advanced Open-Source Model with 8-Hour Autonomous Task Capability - Pandaily</a></li>
<li><a href="https://www.anthropic.com/project/glasswing">Project Glasswing \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI security`, `#cybersecurity`, `#vulnerability detection`, `#benchmark`, `#Tencent`, `#GLM`, `#Claude`

---