---
layout: default
title: "Horizon Summary: 2026-08-03 (ZH)"
date: 2026-08-03
lang: zh
---

> From 111 items, 6 important content pieces were selected

---

1. [Karpathy 的 Pelican：AI 物理世界理解新基准](#item-1) ⭐️ 7.0/10
2. [Kakehashi：在 Linux ARM 上运行 macOS 可执行程序](#item-2) ⭐️ 7.0/10
3. [F*：面向证明的工业级编程语言](#item-3) ⭐️ 7.0/10
4. [eBay 安全团队骚扰 campaign 导致 5600 万美元和解](#item-4) ⭐️ 7.0/10
5. [Shitty 终端：故意使用不安全 Rust 代码追求性能](#item-5) ⭐️ 7.0/10
6. [微塑料侵入深海热液喷口 92%动物体内检出](#item-6) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Karpathy 的 Pelican：AI 物理世界理解新基准](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 7.0/10

Andrej Karpathy 分享了一张 AI 生成的鹈鹕图像，该图像已成为测试模型物理世界理解能力的新基准，引发了关于可重复性和 AI 评估方法的实质性社区讨论。 鹈鹕图像作为定性基准需要主观评估，而不仅仅是定量指标。前沿模型在创建可玩的弹珠游戏等基本物理任务上仍然困难，经常放置挡住弹射槽的墙壁或方向错误的挡板。

hackernews · delichon · Aug 2, 04:05

**背景**: Andrej Karpathy 是一位著名的 AI 研究人员，是 OpenAI 的创始成员，后来在特斯拉担任 AI 总监，负责 Autopilot 计算机视觉团队。AI 中的物理世界理解指的是模型理解现实场景中空间关系、物理约束和因果关系的能力——这些能力用现有基准很难评估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://karpathy.ai/">Andrej Karpathy</a></li>
<li><a href="https://github.com/SHI-Labs/physical-ai-bench">GitHub - SHI-Labs/physical-ai-bench: [CVPR 2026 Oral] PAI ...</a></li>
<li><a href="https://arxiv.org/abs/2501.16411">[2501.16411] PhysBench: Benchmarking and Enhancing Vision ...</a></li>

</ul>
</details>

**社区讨论**: Commenters largely agree the pelican represents a valuable qualitative benchmark, though some question its reproducibility since the original prompt wasn't shared. Others noted that even frontier models like Opus 5 still struggle with basic physical tasks like arranging pinball game elements correctly, and that some models may be specifically trained for certain tasks like three.js code generation rather than demonstrating general physical understanding.

**标签**: `#AI`, `#machine learning`, `#image generation`, `#benchmarks`, `#Andrej Karpathy`

---

<a id="item-2"></a>
## [Kakehashi：在 Linux ARM 上运行 macOS 可执行程序](https://github.com/wie-project/kakehashi) ⭐️ 7.0/10

Kakehashi 是一个实验性的用户空间项目，可以在 Linux ARM 机器上原生运行 macOS 命令行可执行程序。目前已有 7-Zip（通过 8k 文件树的多线程压缩测试）和 curl（超过 200 个命令通过自动化 Docker 测试）的可用原型。 这个项目展示了在 Linux ARM 上运行 macOS 应用程序的可行性，类似于 WINE/Proton 在 Linux 上运行 Windows 应用程序的跨平台兼容性。开发者还提到通过类似 yabridge 的实现支持 AU（音频单元）插件的潜在可能性，这可能有利于 Linux 音频制作工作流程。 性能基准测试显示 7-Zip 的运行速度比本地 Linux 执行慢约 5.2 倍，尽管开发者已制定明确的优化计划。该项目完全在用户空间而非内核空间运行，避免了内核级虚拟化的复杂性。

hackernews · vlad_kalinkin · Aug 2, 16:26

**背景**: 二进制翻译是一种虚拟化技术，将一种指令集架构（ISA）的机器代码转换到另一种，允许为某个系统设计的可执行文件在另一个系统上运行。用户空间是指应用程序软件执行的内存区域，与运行操作系统内核的内核空间不同。Darling 项目是一个现有的 Linux macOS 兼容层，目前有针对 ARM64 支持的开放拉取请求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Binary_translation">Binary translation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/User_space_and_kernel_space">User space and kernel space - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论显示对这个项目充满热情，用户建议与 Darling 项目合作，并表示对潜在的 AU 插件支持感兴趣。一些技术问题被提出与游戏反编译方法进行比较，并注意到解决方案仍处于早期阶段的担忧。

**标签**: `#macos`, `#linux`, `#arm`, `#binary-translation`, `#open-source`

---

<a id="item-3"></a>
## [F*：面向证明的工业级编程语言](https://fstar-lang.org/) ⭐️ 7.0/10

F* 是一种面向证明的通用编程语言，用于工业级形式验证，在 HACL* 和已验证的 TLS 实现中有显著应用。 这很重要，因为 F* 使开发者能够数学地证明代码的关键属性，减少敏感安全软件的错误。它在真实项目（如已验证的 TLS）中的使用展示了实际的工业适用性。 F* 结合了依赖类型和细化类型，以允许精确的规范。它支持与外部 C 库的互操作，能够增量迁移现有的 C 代码库——这是用户注意到的一个实用功能。

hackernews · ducktective · Aug 2, 12:31

**背景**: 形式验证使用数学方法来证明软件的正确性。依赖类型允许类型更精确地约束值（例如，知道其长度的数组类型）。细化类型为现有类型添加谓词来表示前置条件和后置条件。F* 基于这些概念提供了一个实用的验证框架，被主要项目采用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dependent_type">Dependent type - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Refinement_type">Refinement type</a></li>
<li><a href="https://en.wikipedia.org/wiki/Formal_verification">Formal verification - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论强调了网站可用性问题——用户难以在首页找到代码示例和语法文档。其他人则赞赏 F* 调用外部库和增量迁移 C 代码库的能力。对于刚接触函数式编程的开发者来说，工业应用和使用案例仍存在疑问。

**标签**: `#programming-languages`, `#formal-verification`, `#proof-assistants`, `#functional-programming`, `#fstar`

---

<a id="item-4"></a>
## [eBay 安全团队骚扰 campaign 导致 5600 万美元和解](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 7.0/10

eBay 的安全团队对一个经营 eBay 批评博客的马萨诸塞州夫妇进行了系统性骚扰 campaign，导致 5600 万美元的和解金，包括前高级总监 Jim Baugh 在内的多名高管被判处监禁，其中一人获刑 57 个月。 此案揭示了企业安全资源可能被滥用的问题，并引发了关于类似恐吓 tactics 是否被用于其他批评者的疑问，特别是考虑到安全团队中有前警察局长参与。 据检察官称，eBay 安全团队的七名成员（包括前警察局长）共同合作骚扰和恐吓 Steiners 夫妇。骚扰活动包括向受害者家中寄送令人不安的物品，如葬礼花圈和性玩具。

hackernews · JumpCrisscross · Aug 2, 19:19

**背景**: 此案的核心是 eBay 的全球安全团队，该团队原本负责保护公司利益，但却从事非法骚扰活动。受害者 Steiners 夫妇经营一个批评 eBay 政策的博客。此案是关于企业恐吓 tactics 和问责制的更广泛讨论的一部分。

**社区讨论**: 评论对此案是否为孤立事件表示怀疑，用户质疑 eBay 是否还针对其他批评者。一条评论将此与人类行为模式进行类比，即缺乏监督且被发现的概率较低的人会表现不佳。也有一些评论顺便提到对 eBay 高费用的担忧，与竞争对手相比。

**标签**: `#corporate-misconduct`, `#ebay`, `#legal`, `#harassment`, `#tech-industry`

---

<a id="item-5"></a>
## [Shitty 终端：故意使用不安全 Rust 代码追求性能](https://github.com/pg83/shitty) ⭐️ 7.0/10

GitHub 上发布了一个名为 shitty 的终端模拟器项目，该项目故意使用内存不安全的 Rust 代码（unsafe Rust 代码块）来实现比传统终端模拟器更快的性能。 这挑战了 Rust 社区的 conventional wisdom，即内存安全应该始终优先于性能。它引发了关于性能关键型应用程序是否应该为了速度而接受内存不安全风险的争论。 该项目使用 unsafe Rust 代码块来绕过 Rust 在编译时的内存安全保证，从本质上将 Rust 当作更好的 C 来使用。shitty 这个名字似乎是对 kitty（另一个快速的 GPU 加速终端模拟器）的挑衅性戏仿。

rss · Hacker News - Show HN · Aug 2, 23:05

**背景**: Rust 是一种系统编程语言，以其在编译时强制执行的内存安全保证而闻名，这可以防止许多常见的错误，如空指针解引用和缓冲区溢出。然而，Rust 提供了一种 unsafe 模式，允许开发人员绕过这些安全保证来处理性能关键的代码。kitty 终端模拟器是一个现有的快速、GPU 加速的终端，使用 C、Python 和 Go 混合编写。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://doc.rust-lang.org/book/ch20-01-unsafe-rust.html">Unsafe Rust - The Rust Programming Language</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kitty_(terminal_emulator)">kitty (terminal emulator) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#terminal-emulator`, `#rust`, `#performance-optimization`, `#systems-programming`, `#unsafe-code`

---

<a id="item-6"></a>
## [微塑料侵入深海热液喷口 92%动物体内检出](https://www.yahoo.com/news/science/articles/most-isolated-environments-microplastics-finding-020000452.html) ⭐️ 7.0/10

韩国生物科学与生物技术研究院的研究人员在西南太平洋和印度洋约 2000 米深的深海热液喷口附近，从蜗牛和贻贝等 4 种动物体内检出微塑料，检出率 92%，平均每只含 3.42 片聚苯乙烯。 这一发现表明微塑料污染已蔓延至地球上最偏远的海洋生态系统，凸显了塑料污染的无孔不入，并引发了对深海生物多样性和食物网潜在影响的担忧。 滤食性贻贝体内微塑料分布均匀，而食草性蜗牛的微塑料集中于消化器官。印度洋样本的微塑料浓度高于太平洋样本，表明污染传输存在区域差异。

telegram · zaihuapd · Aug 2, 11:00

**背景**: 热液喷口是 1977 年发现的深海生态系统，在没有阳光的情况下通过化学合成支持复杂群落，细菌从硫化氢等化学反应的化学能中获取能量。微塑料是小于 5 毫米的塑料颗粒，已成为海洋环境中普遍存在的污染物，检测方法尚未完全标准化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hydrothermal_vent">Hydrothermal vent - Wikipedia</a></li>
<li><a href="https://www.marinebio.org/oceans/deep-sea/hydrothermal-vents/">Hydrothermal Vents & Chemosynthetic Ecosystems | MarineBio ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Microplastics">Microplastics - Wikipedia</a></li>

</ul>
</details>

**标签**: `#microplastics`, `#marine pollution`, `#deep-sea environment`, `#environmental science`, `#hydrothermal vents`

---