---
layout: default
title: "Horizon Summary: 2026-08-03 (EN)"
date: 2026-08-03
lang: en
---

> From 111 items, 6 important content pieces were selected

---

1. [Karpathy's Pelican: AI Physical World Benchmark](#item-1) ⭐️ 7.0/10
2. [Kakehashi: Run macOS Binaries on Linux ARM](#item-2) ⭐️ 7.0/10
3. [F*: Industrial-Grade Proof-Oriented Programming Language](#item-3) ⭐️ 7.0/10
4. [eBay Security Team Harassment Campaign Leads to $56M Settlement](#item-4) ⭐️ 7.0/10
5. [Shitty Terminal: Intentional Unsafe Rust for Speed](#item-5) ⭐️ 7.0/10
6. [Microplastics Found in 92% of Deep-Sea Hydrothermal Vent Animals](#item-6) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Karpathy's Pelican: AI Physical World Benchmark](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 7.0/10

Andrej Karpathy shared an AI-generated pelican image that has emerged as a new benchmark for testing models' understanding of the physical world, sparking substantive community debate about reproducibility and AI evaluation methodologies. This represents a shift from traditional benchmarks to qualitative tests that better expose AI models' understanding of physical reality, spatial relationships, and practical constraints - capabilities that remain challenging even for frontier LLMs. The pelican serves as a qualitative benchmark requiring subjective evaluation, not just quantitative metrics. Frontier models still struggle with basic physical tasks like creating a playable pinball game, often placing walls that block launch chutes or orienting flippers incorrectly.

hackernews · delichon · Aug 2, 04:05

**Background**: Andrej Karpathy is a prominent AI researcher who was a founding member of OpenAI and later served as Director of AI at Tesla, leading the Autopilot computer vision team. Physical world understanding in AI refers to a model's ability to comprehend spatial relationships, physical constraints, and cause-and-effect in real-world scenarios - capabilities that remain difficult to evaluate with existing benchmarks.

<details><summary>References</summary>
<ul>
<li><a href="https://karpathy.ai/">Andrej Karpathy</a></li>
<li><a href="https://github.com/SHI-Labs/physical-ai-bench">GitHub - SHI-Labs/physical-ai-bench: [CVPR 2026 Oral] PAI ...</a></li>
<li><a href="https://arxiv.org/abs/2501.16411">[2501.16411] PhysBench: Benchmarking and Enhancing Vision ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree the pelican represents a valuable qualitative benchmark, though some question its reproducibility since the original prompt wasn't shared. Others noted that even frontier models like Opus 5 still struggle with basic physical tasks like arranging pinball game elements correctly, and that some models may be specifically trained for certain tasks like three.js code generation rather than demonstrating general physical understanding.

**Tags**: `#AI`, `#machine learning`, `#image generation`, `#benchmarks`, `#Andrej Karpathy`

---

<a id="item-2"></a>
## [Kakehashi: Run macOS Binaries on Linux ARM](https://github.com/wie-project/kakehashi) ⭐️ 7.0/10

Kakehashi is an experimental userspace project that enables macOS CLI binaries to run natively on Linux ARM machines. It currently has working prototypes for 7-Zip (passing multi-threaded compression tests on an 8k-file tree) and curl (with over 200 commands passing automated Docker tests). This project demonstrates the feasibility of running macOS applications on Linux ARM, which could enable cross-platform compatibility similar to how WINE/Proton allows Windows apps on Linux. The developer also mentioned interest in potential AU (Audio Unit) plugin support through a yabridge-like implementation, which could benefit Linux audio production workflows. Performance benchmarks show 7-Zip running approximately 5.2x slower than native Linux execution, though the developer has outlined a clear optimization plan. The project operates entirely in userspace rather than kernel space, avoiding the complexity of kernel-level virtualization.

hackernews · vlad_kalinkin · Aug 2, 16:26

**Background**: Binary translation is a virtualization technique that converts machine code from one instruction set architecture (ISA) to another, allowing executables designed for one system to run on a different system. Userspace refers to the memory area where application software executes, in contrast to kernel space where the operating system kernel runs. The Darling project is an existing macOS compatibility layer for Linux that currently has an open PR for ARM64 support.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Binary_translation">Binary translation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/User_space_and_kernel_space">User space and kernel space - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments show enthusiasm for the project, with users suggesting collaboration opportunities with the Darling project and expressing interest in potential AU plugin support. Some technical questions were raised about the approach compared to game decompilation methods, and concerns were noted about the early-stage nature of the solution.

**Tags**: `#macos`, `#linux`, `#arm`, `#binary-translation`, `#open-source`

---

<a id="item-3"></a>
## [F*: Industrial-Grade Proof-Oriented Programming Language](https://fstar-lang.org/) ⭐️ 7.0/10

F* is a general-purpose proof-oriented programming language used for formal verification in industry, with notable applications in HACL* and verified TLS implementations. This matters because F* enables developers to prove critical properties of their code mathematically, reducing bugs in security-sensitive software. Its use in real-world projects like verified TLS demonstrates practical industrial applicability. F* combines dependent types and refinement types to allow precise specifications. It supports interop with external C libraries, enabling incremental migration of existing C codebases—a practical feature noted by users.

hackernews · ducktective · Aug 2, 12:31

**Background**: Formal verification uses mathematical methods to prove software correctness. Dependent types allow types to constrain values more precisely (e.g., an array type that knows its length). Refinement types add predicates to existing types to express preconditions and postconditions. F* builds on these concepts to provide a practical verification framework used by major projects.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dependent_type">Dependent type - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Refinement_type">Refinement type</a></li>
<li><a href="https://en.wikipedia.org/wiki/Formal_verification">Formal verification - Wikipedia</a></li>

</ul>
</details>

**Discussion**: 评论强调了网站可用性问题——用户难以在首页找到代码示例和语法文档。其他人则赞赏 F* 调用外部库和增量迁移 C 代码库的能力。对于刚接触函数式编程的开发者来说，工业应用和使用案例仍存在疑问。

**Tags**: `#programming-languages`, `#formal-verification`, `#proof-assistants`, `#functional-programming`, `#fstar`

---

<a id="item-4"></a>
## [eBay Security Team Harassment Campaign Leads to $56M Settlement](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 7.0/10

eBay's security team conducted a systematic harassment campaign against a Massachusetts couple who ran an eBay criticism blog, resulting in a $56 million settlement and prison sentences for executives including a 57-month term for former Senior Director Jim Baugh. This case reveals potential abuse of corporate security resources and raises questions about whether similar intimidation tactics were used against other critics, particularly given the involvement of former police captains in the security team. Seven members of eBay's security team, including former police captains, worked together to harass and intimidate the Steiners according to prosecutors. The harassment included sending disturbing items like a funeral wreath and sex toys to the victims' home.

hackernews · JumpCrisscross · Aug 2, 19:19

**Background**: The case centers on eBay's Global Security Team which was tasked with protecting the company's interests but instead engaged in illegal harassment. The victims, the Steiners, operated a blog that was critical of eBay's policies. This case is part of a broader discussion about corporate intimidation tactics and accountability.

**Discussion**: Comments express skepticism that this was an isolated incident, with users questioning whether other eBay critics were targeted. One comment draws a parallel to human behavior patterns where unsupervised people with low detection risk behave badly. Some also note tangential concerns about eBay's high fees compared to competitors.

**Tags**: `#corporate-misconduct`, `#ebay`, `#legal`, `#harassment`, `#tech-industry`

---

<a id="item-5"></a>
## [Shitty Terminal: Intentional Unsafe Rust for Speed](https://github.com/pg83/shitty) ⭐️ 7.0/10

A terminal emulator project called 'shitty' was released on GitHub that deliberately uses memory-unsafe Rust code (unsafe Rust blocks) to achieve faster performance than conventional terminal emulators. This challenges the conventional wisdom in the Rust community that memory safety should always take precedence over performance. It sparks debate about whether performance-critical applications should accept the risks of memory-unsafety for speed gains. The project uses 'unsafe Rust' blocks to bypass Rust's compile-time memory safety guarantees, essentially treating Rust as a 'better C'. The name 'shitty' appears to be a provocative play on 'kitty', another fast GPU-accelerated terminal emulator.

rss · Hacker News - Show HN · Aug 2, 23:05

**Background**: Rust is a systems programming language known for its memory safety guarantees enforced at compile time, which prevents many common bugs like null pointer dereferences and buffer overflows. However, Rust provides an 'unsafe' mode that allows developers to bypass these safety guarantees for performance-critical code. The 'kitty' terminal emulator is an existing fast, GPU-accelerated terminal written in a mix of C, Python, and Go.

<details><summary>References</summary>
<ul>
<li><a href="https://doc.rust-lang.org/book/ch20-01-unsafe-rust.html">Unsafe Rust - The Rust Programming Language</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kitty_(terminal_emulator)">kitty (terminal emulator) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#terminal-emulator`, `#rust`, `#performance-optimization`, `#systems-programming`, `#unsafe-code`

---

<a id="item-6"></a>
## [Microplastics Found in 92% of Deep-Sea Hydrothermal Vent Animals](https://www.yahoo.com/news/science/articles/most-isolated-environments-microplastics-finding-020000452.html) ⭐️ 7.0/10

Korean researchers from the Korea Institute of Bioscience and Biotechnology discovered microplastics in 92% of animals (snails and mussels) collected near hydrothermal vents at approximately 2000 meters depth in the Southwest Pacific and Indian Oceans, with an average of 3.42 polystyrene pieces per animal. This finding demonstrates that microplastic pollution has reached even the most isolated marine ecosystems on Earth, highlighting the pervasive nature of plastic contamination and raising concerns about impacts on deep-sea biodiversity and food webs. Filter-feeding mussels showed uniform microplastic distribution throughout their bodies, while herbivorous snails concentrated particles in their digestive organs. Indian Ocean samples showed higher microplastic concentrations than Pacific Ocean samples, suggesting regional variations in pollution transport.

telegram · zaihuapd · Aug 2, 11:00

**Background**: Hydrothermal vents are deep-sea ecosystems discovered in 1977 that support complex communities without sunlight, using chemosynthesis where bacteria harvest energy from chemical reactions involving hydrogen sulfide. Microplastics are plastic particles smaller than 5mm that have become ubiquitous pollutants in marine environments, with detection methods still lacking full standardization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hydrothermal_vent">Hydrothermal vent - Wikipedia</a></li>
<li><a href="https://www.marinebio.org/oceans/deep-sea/hydrothermal-vents/">Hydrothermal Vents & Chemosynthetic Ecosystems | MarineBio ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Microplastics">Microplastics - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#microplastics`, `#marine pollution`, `#deep-sea environment`, `#environmental science`, `#hydrothermal vents`

---