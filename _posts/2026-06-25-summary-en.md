---
layout: default
title: "Horizon Summary: 2026-06-25 (EN)"
date: 2026-06-25
lang: en
---

> From 174 items, 25 important content pieces were selected

---

1. [OpenAI Unveils First Custom AI Chip Jalapeno with Broadcom](#item-1) ⭐️ 8.0/10
2. [Talos: Scaling Rare Disease Diagnosis with Automated Iterative Genomic Reanalysis](#item-2) ⭐️ 8.0/10
3. [Why the Frontier Ecosystem must be Open — Matei Zaharia and Reynold Xin, Databricks](#item-3) ⭐️ 8.0/10
4. [NSA Loses Access to Anthropic's Mythos Tool Amid Dispute](#item-4) ⭐️ 8.0/10
5. [AI Homework Boosts Grades but Harms Exam Performance: Study](#item-5) ⭐️ 8.0/10
6. [Anthropic Accuses Alibaba of Massive AI Model Theft](#item-6) ⭐️ 8.0/10
7. [llama.cpp b9784 Delivers Major MUL_MAT Optimizations](#item-7) ⭐️ 7.0/10
8. [Qualcomm to Acquire Modular AI for $4B](#item-8) ⭐️ 7.0/10
9. [Gemini 3.5 Flash Computer Use Issues Report](#item-9) ⭐️ 7.0/10
10. [NVIDIA 45°C Liquid Cooling Cuts Data Center Water Use to Near Zero](#item-10) ⭐️ 7.0/10
11. [John Carmack Reflects on Early id Software Management Mistakes](#item-11) ⭐️ 7.0/10
12. [Nub: Bun-like TypeScript Toolkit for Node.js](#item-12) ⭐️ 7.0/10
13. [Ethics of Copying in Design and Web Development](#item-13) ⭐️ 7.0/10
14. [AI Rewrites PostHog SQL Parser, 70x Performance Gain](#item-14) ⭐️ 7.0/10
15. [Huntington Bank Uses AWS to Redact Sensitive Data from 400M+ Documents](#item-15) ⭐️ 7.0/10
16. [Building Voice Healthcare Agent with Amazon Nova 2 Sonic](#item-16) ⭐️ 7.0/10
17. [NVIDIA Accelerates BEV Pooling on GPUs for Physical AI](#item-17) ⭐️ 7.0/10
18. [AI Researchers Continue Leaving Google for Anthropic](#item-18) ⭐️ 7.0/10
19. [US Memory Chip Company Sees Revenue Quadruple to $41.45B](#item-19) ⭐️ 7.0/10
20. [AI Companies Spend $27M in NY Congressional Race, Bores Loses Narrowly](#item-20) ⭐️ 7.0/10
21. [Anthropic Accuses Alibaba of Illegally Accessing Claude Models](#item-21) ⭐️ 7.0/10
22. [OpenAI Codex Causes Millions in SSD Costs](#item-22) ⭐️ 7.0/10
23. [Using Gini Coefficient for Edge Capacity Planning](#item-23) ⭐️ 7.0/10
24. [Why Enterprise AI Agents Die at Prototype Stage](#item-24) ⭐️ 7.0/10
25. [Micron Q3 FY2026: $41.46B Revenue, 346% YoY Growth Driven by AI](#item-25) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI Unveils First Custom AI Chip Jalapeno with Broadcom](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 8.0/10

OpenAI announced its first custom inference chip called 'Jalapeno', developed in collaboration with Broadcom. The chip was designed and brought to production in just nine months, with AI-assisted design acceleration enabled by OpenAI's own models. This marks a significant strategic move by OpenAI into custom silicon design, reducing dependence on external chip vendors like Nvidia. As one of the first major AI labs to develop their own inference chip, it signals a broader industry trend toward specialized AI hardware optimized for specific model architectures. Jalapeno is an inference chip (used for applying trained AI models, not training new ones), distinct from training accelerators. The chip was manufactured by TSMC. Some community members questioned whether the 'AI-assisted design' claim is meaningful marketing language, while others discussed innovative architectural ideas like embedding model weights directly into ROM for constant multiplication operations.

hackernews · TechCrunch AI · Jun 24, 17:47

**Background**: Inference chips are specialized ASICs designed to run trained AI models efficiently, distinct from training chips that build models. Training chips set performance ceilings while inference chips determine real-world adoption and cost. Google has been developing TPUs for years (now on 7th generation), making OpenAI's entry into custom silicon a notable catch-up move in the competitive AI infrastructure landscape.

<details><summary>References</summary>
<ul>
<li><a href="https://www.granitefirm.com/blog/us/2025/08/24/ai-inference-chips/">AI inference chips vs . training chips - Andy Lin's Long-term Stock...</a></li>
<li><a href="https://www.mpcmarkets.com.au/understanding-training-inference-chips-and-the-competitive-landscape/">Understanding Training , Inference Chips and the... - MPC Markets</a></li>
<li><a href="https://techblog.comsoc.org/2025/12/05/custom-ai-chips-powering-the-next-wave-of-intelligent-computing/">Custom AI Chips: Powering the next wave of Intelligent Computing</a></li>

</ul>
</details>

**Discussion**: Community members expressed both excitement and skepticism. Some questioned whether 'AI-accelerated design' is meaningful or just marketing hyperbole. There was discussion about TSMC manufacturing and innovative architectural ideas like embedding weights in ROM for massive parallelism. Comparisons were drawn to Google's TPUs and newer approaches like Taalas burning models directly into silicon.

**Tags**: `#AI hardware`, `#custom silicon`, `#inference chips`, `#OpenAI`, `#Broadcom`

---

<a id="item-2"></a>
## [Talos: Scaling Rare Disease Diagnosis with Automated Iterative Genomic Reanalysis](https://www.microsoft.com/en-us/research/blog/talos-scaling-rare-disease-diagnosis-with-automated-iterative-genomic-reanalysis/) ⭐️ 8.0/10

Microsoft Research has open-sourced Talos, an automated system that performs iterative genomic reanalysis to scale rare disease diagnosis. The system recovered 90% of in-scope diagnoses while presenting only 1.3 candidate variants per patient for expert review. This addresses a critical bottleneck in genomic medicine where human expert review time limits diagnostic capacity. With over half of patients remaining undiagnosed due to manual review constraints, Talos enables frequent, systematic reanalysis to be run sustainably, potentially helping millions affected by rare diseases get diagnosed. Talos uses a variant prioritization algorithm to automatically filter and rank variants across monthly iterative cycles. During each cycle, analysts only needed to review one new variant per 200 patients, demonstrating the system's efficiency in reducing manual review burden while maintaining high diagnostic yield.

rss · Microsoft Research · Jun 24, 14:00

**Background**: Genomic testing has transformed rare disease diagnosis, but the rapid pace of discovery in rare disease genomics means that previously analyzed data can yield new diagnoses when reanalyzed with updated knowledge. Traditional manual reanalysis is time-consuming and does not scale, creating a bottleneck where expert reviewers are overwhelmed by the number of candidate variants to evaluate.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nature.com/articles/s41591-026-04477-5">Automated reanalysis of genomic data for rare disease diagnostics at scale | Nature Medicine</a></li>
<li><a href="https://www.nature.com/articles/gim2017246">Making new genetic diagnoses with old data: iterative reanalysis and reporting from genome-wide data in 1,133 families with developmental disorders | Genetics in Medicine</a></li>
<li><a href="https://www.microsoft.com/en-us/research/blog/talos-scaling-rare-disease-diagnosis-with-automated-iterative-genomic-reanalysis/">Talos: Scaling rare disease diagnosis with automated, iterative genomic reanalysis - Microsoft Research</a></li>

</ul>
</details>

**Tags**: `#genomic-medicine`, `#rare-disease-diagnosis`, `#healthcare-ai`, `#automation`, `#microsoft-research`

---

<a id="item-3"></a>
## [Why the Frontier Ecosystem must be Open — Matei Zaharia and Reynold Xin, Databricks](https://www.latent.space/p/databricks) ⭐️ 8.0/10

Databricks technical leaders explain why open ecosystems are essential for the emerging AI Agent Clouds trend in enterprise AI deployment.

rss · Latent Space · Jun 24, 18:53

**Tags**: `#AI Agents`, `#Open Source`, `#Databricks`, `#Enterprise AI`, `#ML Platforms`

---

<a id="item-4"></a>
## [NSA Loses Access to Anthropic's Mythos Tool Amid Dispute](https://www.nytimes.com/2026/06/23/us/politics/nsa-lost-access-anthropic-tool.html) ⭐️ 8.0/10

The NSA has lost access to Anthropic's Mythos AI tool amid an unspecified dispute between the US intelligence agency and the leading AI company. This represents a significant conflict between government oversight and AI development. This dispute highlights the growing tension between US intelligence agencies and AI companies over access to powerful AI tools. The NSA's loss of access to Mythos could impact national security capabilities, while also raising questions about government oversight of advanced AI systems. Mythos is Anthropic's most advanced model, designed specifically for high-stakes cybersecurity environments. The tool can understand complex, multi-step threat chains that conventional security tools often miss, which explains why intelligence agencies would want access to it.

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Jun 24, 11:45

**Background**: Mythos AI is Anthropic's newest model specifically built for cybersecurity applications. It was designed to understand complex threat chains that conventional tools miss. Since its release, Mythos has triggered responses from central banks and intelligence agencies globally. Previously, there were tensions between spy agencies and the Commerce Department over who should handle AI model evaluation tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://mythos-ai.net/">Mythos AI - Claude Frontier Intelligence by Anthropic 2026</a></li>
<li><a href="https://www.nytimes.com/2026/04/22/technology/anthropics-mythos-ai.html">Anthropic’s New Mythos A.I. Model Sets Off Global Alarms ...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion reflects significant community interest in the intersection of AI policy and government oversight. Comments highlight concerns about the implications for AI safety and national security, with many users noting the importance of transparency in such disputes.

**Tags**: `#Anthropic`, `#NSA`, `#AI policy`, `#government regulation`, `#Mythos`

---

<a id="item-5"></a>
## [AI Homework Boosts Grades but Harms Exam Performance: Study](https://cepr.org/publications/dp21577) ⭐️ 8.0/10

A 30-month longitudinal study of 26,811 Chinese students in grades 7-12 found that while generative AI improved homework grades by 18% and reduced completion time by 30%, it caused a 20% decline in closed-book exam scores within 6 months and an 18-24% drop in high-stakes exam scores (Zhongkao and Gaokao), with full effects manifesting after about two years. This is significant because it provides large-scale empirical evidence that AI-assisted homework may undermine students' ability to perform in high-stakes exams, particularly for high achievers and in social sciences, challenging the assumption that AI tools always benefit learning. The study found that about 80% of AI users exhibited 'homework outsourcing' behavior - very short homework time but high scores - and bore most of the performance losses. Students who maintained homework times similar to non-AI users experienced minimal damage. Social sciences suffered the largest losses, followed by STEM and languages.

telegram · zaihuapd · Jun 24, 05:15

**Background**: Gaokao (高考) is China's national college entrance examination, a high-stakes exam that determines which universities students can attend. Zhongkao (中考) is the junior high school graduation exam used for senior high school admissions. Closed-book exams require students to answer without external materials, promoting better long-term retention compared to open-book formats. The study tracked students' performance in monthly closed-book exams where AI tools could not be used.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gaokao">Gaokao - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zhongkao">Zhongkao - Wikipedia</a></li>
<li><a href="https://www.tandfonline.com/doi/full/10.1080/13562517.2023.2289128">Does the format of an assessment (closed book or open book ...</a></li>

</ul>
</details>

**Tags**: `#AI in Education`, `#Student Performance`, `#Academic Integrity`, `#China Education`, `#Generative AI`, `#Longitudinal Study`

---

<a id="item-6"></a>
## [Anthropic Accuses Alibaba of Massive AI Model Theft](https://www.cnbc.com/2026/06/24/anthropic-alibaba-distillation-campaign.html) ⭐️ 8.0/10

Anthropic has sent a letter to the US Senate Banking Committee accusing Alibaba of conducting the largest known 'distillation attack' in history, using nearly 25,000 fraudulent accounts to interact with Claude over 28.8 million times between April 22 and June 5, 2026, to illegally extract the AI model's capabilities. This represents the first major public accusation of large-scale AI model theft between major US and Chinese tech companies, with significant implications for US-China AI competition. The timing ahead of Senate AI hearings and recent export restrictions on advanced AI models highlights the escalating tech rivalry and concerns over intellectual property protection. The attack involved Alibaba and its Qwen AI laboratory, using distillation—a technique where a weaker model learns from a stronger model's outputs to replicate its capabilities. The letter was sent to Senate Banking Committee chair Tim Scott and senior member Elizabeth Warren on June 10, ahead of congressional AI hearings. Alibaba has not yet responded to requests for comment.

telegram · zaihuapd · Jun 25, 01:36

**Background**: Model distillation is a machine learning technique where a smaller 'student' model learns from a larger 'teacher' model to replicate its capabilities efficiently. The US-China AI competition has intensified, with Washington imposing export controls on advanced AI models and accusing Beijing of intellectual property theft. In June 2026, the US Commerce Department restricted exports of Anthropic's Mythos and Fable models on national security grounds, forcing the company to disable them globally.

<details><summary>References</summary>
<ul>
<li><a href="https://www.intellectyx.com/model-distillation-ai-starter-guide-techniques-benefits-and-applications/">AI Model Distillation Guide: Techniques, Benefits & Applications</a></li>
<li><a href="https://www.datacamp.com/blog/distillation-llm">LLM Distillation Explained: Applications, Implementation & More</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI模型蒸馏`, `#中美科技竞争`, `#知识产权窃取`, `#Anthropic`, `#阿里巴巴`

---

<a id="item-7"></a>
## [llama.cpp b9784 Delivers Major MUL_MAT Optimizations](https://github.com/ggml-org/llama.cpp/releases/tag/b9784) ⭐️ 7.0/10

llama.cpp release b9784 delivers major MUL_MAT rework with 32x32 tiled weight repack, hardware-specific optimizations for Hexagon/HVX/HMX, and dynamic quantization improvements. It also fixes OLMoE and LFM models. This release provides significant performance improvements for a widely-used open-source LLM inference library, particularly on Qualcomm Hexagon hardware commonly found in mobile devices. The optimizations enable faster and more efficient on-device AI inference. Key optimizations include 32x32 tiled weight repack for better memory access patterns, vectorized q8_1 quantizer, HMX activation processing with DMA prefetch, and removal of legacy restrictions. The release also drops support for architecture versions older than v73.

github · github-actions[bot] · Jun 24, 19:55

**Background**: Qualcomm Hexagon is a family of DSP and NPU products, where HVX (Hexagon Vector Extensions) provides vector operations and HMX (Hexagon Matrix Extension) adds matrix multiplication capabilities. VTCM (Very Tightly Coupled Memory) is fast on-chip memory. OLMoE is an open-source Mixture of Experts model with 1.3B active and 6.9B total parameters.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qualcomm_Hexagon">Qualcomm Hexagon - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2409.02060">[2409.02060] OLMoE : Open Mixture - of - Experts Language Models</a></li>

</ul>
</details>

**Tags**: `#llama.cpp`, `#LLM inference`, `#performance optimization`, `#matrix multiplication`, `#embedded AI`

---

<a id="item-8"></a>
## [Qualcomm to Acquire Modular AI for $4B](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 7.0/10

Qualcomm announces acquisition of Chris Lattner's AI startup Modular for approximately $4 billion, marking a major strategic push into AI infrastructure beyond mobile and edge chips. This $4 billion acquisition represents Qualcomm's boldest move yet to diversify beyond its traditional mobile chip business into AI infrastructure. It signals Qualcomm's ambition to compete in the AI training and inference market currently dominated by NVIDIA, leveraging Modular's Mojo programming language and AI optimization technology. Modular's AI platform provides serverless inference endpoints, fine-tuning services, and training clusters for GPU portability and performance optimization. The company's core product Mojo is a Python-like programming language designed specifically for AI workloads with better performance than standard Python.

hackernews · timmyd · Jun 24, 13:49

**Background**: Chris Lattner is renowned for creating LLVM, Clang, Swift, and MLIR - foundational infrastructure in modern compilers and programming languages. After 12 years at Apple leading the Developer Tools team, Lattner founded Modular to address AI infrastructure challenges. The AI infrastructure market is currently dominated by NVIDIA's Hopper H100 and H200 GPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chris_Lattner">Chris Lattner - Wikipedia</a></li>
<li><a href="https://www.modular.com/">Modular: Inference from Kernel to Cloud</a></li>

</ul>
</details>

**Discussion**: Comments show mixed reactions - some express surprise at the acquisition timing and question the strategic fit since Qualcomm lacks products in high-end inference/training market. Others see it as a bold portfolio play moving Qualcomm beyond ARM to RISC-V and AI capabilities. There's also irony noted that Modular's founder previously criticized hardware companies for failing to build AI stacks.

**Tags**: `#acquisitions`, `#qualcomm`, `#artificial-intelligence`, `#chris-lattner`, `#modular`

---

<a id="item-9"></a>
## [Gemini 3.5 Flash Computer Use Issues Report](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/) ⭐️ 7.0/10

Google's Gemini 3.5 Flash is reported to fail at real coding tasks including incorrectly running git reset --hard when asked to commit changes, failing PDF data extraction after multiple attempts, lacking MCP (Model Context Protocol) support, and underperforming in benchmarks compared to Opus 4.8 and GPT 5.5. This matters because it reveals significant limitations of Gemini 3.5 Flash for practical software engineering tasks, raising questions about its reliability for coding workflows and highlighting gaps compared to competitors like Claude Code and Codex. Specific failures include the model running destructive git reset --hard when asked to commit changes, and admitting it 'invents data instead of doing simple data copy/reformat' after failing at PDF table extraction. Users also note missing MCP support prevents integration with external tools.

hackernews · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Jun 24, 17:21

**Background**: MCP (Model Context Protocol) is an open standard announced by Anthropic in November 2024 that provides a standardized way for AI assistants to connect to external systems including content repositories, business tools, and development environments. It has been adopted by major AI providers including OpenAI and Google DeepMind. Users compare Gemini's capabilities to Codex (OpenAI) and Claude Code (Anthropic) which can clone repos and perform static analysis.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://modelcontextprotocol.io/docs/getting-started/intro">What is the Model Context Protocol (MCP)? - Model Context Protocol</a></li>
<li><a href="https://www.anthropic.com/news/model-context-protocol">Introducing the Model Context Protocol \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Users express frustration with Gemini's coding capabilities. One user reported the model ran destructive git reset --hard instead of proper commit workflow. Another failed at PDF extraction after 15+ iterations, with the model admitting it 'invents data instead of copying'. Users want a Codex/Claude Code equivalent and question why Gemini lacks MCP support that competitors offer.

**Tags**: `#AI`, `#Gemini`, `#LLM`, `#Google`, `#software-engineering`

---

<a id="item-10"></a>
## [NVIDIA 45°C Liquid Cooling Cuts Data Center Water Use to Near Zero](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 7.0/10

NVIDIA has introduced a 45°C liquid cooling architecture for AI data centers that reduces water consumption to near zero through a closed-loop system that recirculates coolant, eliminating the need for traditional cooling towers. This is significant because traditional data centers consume massive amounts of water (about 2.6 million gallons per megawatt per year) for cooling towers, and this architecture eliminates that dependency while potentially enabling waste heat recovery for district heating applications. The cooling system operates at 45°C (113°F), which is higher than typical liquid cooling temperatures. The closed-loop design can run for years without consuming water by recirculating coolant, reducing water use from about 2.6 million gallons per megawatt per year to almost zero in suitable climates.

hackernews · nitin_flanker · Jun 24, 14:10

**Background**: Data centers traditionally rely on cooling towers that consume significant amounts of water through evaporation. The industry is shifting from air cooling to liquid-based solutions to handle rising rack power densities in AI and HPC workloads. Direct-to-chip liquid cooling and immersion cooling are existing technologies that also achieve near-zero water usage through closed-loop designs.

<details><summary>References</summary>
<ul>
<li><a href="https://interestingengineering.com/science/nvidias-servers-slash-data-center-energy">NVIDIA's 113°F cooling system brings data center water use near zero</a></li>
<li><a href="https://introl.com/blog/water-usage-efficiency-wue-ai-data-center-cooling-guide-2025">Water Usage Efficiency | Introl Blog</a></li>
<li><a href="https://gbc-engineers.com/news/direct-to-chip-vs-immersion-cooling">Direct-to-Chip vs Immersion Cooling: Which Liquid Cooling ...</a></li>

</ul>
</details>

**Discussion**: Commenters question the novelty of 45°C cooling compared to existing liquid cooling systems like NASA's Ames facility, which uses similar high-temperature water cooling at 90°F. Others find the district heating potential exciting, noting 45°C is low but workable for community heating loops, though summer heat disposal remains a challenge. Some find the article light on technical details about what makes this approach uniquely innovative.

**Tags**: `#data-center-cooling`, `#AI-infrastructure`, `#sustainability`, `#NVIDIA`, `#water-conservation`

---

<a id="item-11"></a>
## [John Carmack Reflects on Early id Software Management Mistakes](https://twitter.com/ID_AA_Carmack/status/2069799283369345247) ⭐️ 7.0/10

Legendary game developer John Carmack has shared retrospective regrets about pushing his teams too hard during id Software's early days, admitting he didn't appreciate how maturing companies need more slack and that running people at startup intensity constantly wears them out. This reflection offers valuable lessons about startup management and burnout for game developers and tech entrepreneurs. The discussion shows how Carmack's honesty about past mistakes resonates with industry veterans and provides actionable wisdom for building sustainable companies. Carmack specifically mentions that running teams at 'startup intensity' constantly was a mistake, and that companies need to adjust their pace as they mature. Some commenters connect this to the departure of Sandy Petersen and the transition from Doom to Quake's development.

hackernews · shadowtree · Jun 24, 15:56

**Background**: John Carmack is widely considered one of the most influential game developers in history, co-founding id Software and pioneering 3D first-person shooter technology with Doom (1993) and Quake (1996). His technical contributions laid the foundation for modern 3D gaming engines. id Software went from a small startup to a major game publisher, and the company's evolution reflects broader challenges in the game industry regarding scaling and company culture.

**Discussion**: The comments show general appreciation for Carmack's honesty, with some discussing whether the 'means justified the ends' given Quake's iconic status. Others reference Sandy Petersen's perspective on leaving id Software and note the contrast between Quake III Arena's energy and the later Doom 3 release. One commenter wisely notes that 'games are more important than game companies' — suggesting that the industry's evolution matters more than any individual company's fate.

**Tags**: `#game-development`, `#id-software`, `#john-carmack`, `#startup-management`, `#industry-history`

---

<a id="item-12"></a>
## [Nub: Bun-like TypeScript Toolkit for Node.js](https://github.com/nubjs/nub) ⭐️ 7.0/10

Colin McDonnell (creator of Zod) released Nub, a toolkit that augments stock Node.js with TypeScript support, module resolution hooks, and polyfills for APIs like Worker and Temporal, using a --require preload hook with an oxc-powered transpiler packaged as a Node-API add-on. Nub brings Bun-like developer experience to Node.js without replacing the runtime, making it easier for developers to migrate from Bun or get TypeScript support with minimal configuration changes. This addresses a key pain point: many developers choose Bun primarily for its better DX while still needing Node.js compatibility. Nub uses the --require preload hook to inject its transpiler and module resolution hook at startup, and adds polyfills purely additively—code ultimately runs using Node's actual engine and stdlib implementations. The oxc transpiler is a high-performance Rust-based JavaScript/TypeScript compiler from the Oxidation Compiler project.

hackernews · colinmcd · Jun 24, 14:14

**Background**: Bun is a JavaScript runtime that gained popularity for its excellent developer experience, including built-in TypeScript support and faster performance. However, many projects still need Node.js compatibility. The --require hook in Node.js allows loading a module before the main script runs, enabling Nub to intercept and transform code at runtime. oxc (Oxidation Compiler) is a collection of high-performance JavaScript tools written in Rust, part of VoidZero's vision for a unified toolchain.

<details><summary>References</summary>
<ul>
<li><a href="https://oxc.rs/">The JavaScript Oxidation Compiler</a></li>
<li><a href="https://github.com/oxc-project/oxc">GitHub - oxc -project/ oxc : A collection of high-performance JavaScript ...</a></li>

</ul>
</details>

**Discussion**: The community response is largely positive, with users praising the concept and implementation choices. One commenter noted curiosity about ESM support given the use of --require (rather than --import), which may have edge cases. A notable real-world migration testimony came from a user who merged a PR migrating their entire monorepo to Nub with zero issues and "ridiculously fast" performance.

**Tags**: `#nodejs`, `#typescript`, `#developer-tools`, `#open-source`, `#bun`

---

<a id="item-13"></a>
## [Ethics of Copying in Design and Web Development](https://ben-mini.com/2026/stealing-is-a-skill) ⭐️ 7.0/10

A blog post titled "Stealing Is a Skill" sparked heated discussion on Hacker News about the ethics of copying others' creative work in design and web development, with debate on where to draw the line between legitimate iteration and outright plagiarism. This matters because it highlights the ongoing tension between creativity and imitation in the digital age, affecting designers, developers, and creators who struggle to define originality when inspiration and copying often blur together. The discussion references specific examples like Virgil Abloh's work on Air Force 1 iterations and the concept of "Yellowism" where adding a signature supposedly makes stolen work original. Commenters also mention Dan Mall's earlier article on "stealing your way to originality" as a more thoughtful treatment of this topic.

hackernews · bewal416 · Jun 24, 13:08

**Background**: The debate touches on fundamental questions about what constitutes originality in creative work. In design and web development, practitioners often face pressure to produce new work quickly while building on existing patterns. The concept of "appropriation" in art refers to deliberately copying or borrowing from pre-existing works, sometimes transforming them into something new.

**Discussion**: Community sentiment is mixed: some dismiss copyright concerns as an "enforcer caste of the American empire" and argue that ideas cannot be owned, while others clearly distinguish between legitimate iteration (like Virgil Abloh's collaborations with Nike) and outright theft. Several commenters express concern that commercial copying has become normalized and miss the creativity of earlier, more distinctive web design.

**Tags**: `#design-ethics`, `#intellectual-property`, `#web-development`, `#creativity`, `#plagiarism`

---

<a id="item-14"></a>
## [AI Rewrites PostHog SQL Parser, 70x Performance Gain](https://posthog.com/blog/sql-parser) ⭐️ 7.0/10

A developer used AI (Claude) to completely rewrite PostHog's SQL parser, achieving a 70x performance improvement while barely examining the original code. This demonstrates a new paradigm in software engineering where LLMs can be used to rewrite complex parsers with massive performance gains, shifting the engineer's role from direct coding to crafting validation mechanisms. The approach used an LLM with extensive test case generation as an "oracle" to validate the rewrite, enabling the developer to trust the AI-generated code. One effective technique was instructing Claude to "think really hard about edge cases" in a background agent.

hackernews · robbie-c · Jun 24, 18:05

**Background**: PostHog is an open-source product analytics platform that combines product analytics, session replay, feature flags, A/B testing, and surveys. SQL parsers are critical components that translate user queries into database operations, and their performance directly impacts query response times.

<details><summary>References</summary>
<ul>
<li><a href="https://posthog.com/">PostHog – We make dev tools for product engineers</a></li>
<li><a href="https://github.com/PostHog/posthog">GitHub - PostHog/posthog: PostHog is an all-in-one ... Product OS – PostHog PostHog Product Analytics Platform - GitHub What is PostHog? A Guide to the Analytics Platform | metacto PostHog: The Open Source Alternative to Amplitude PostHog - Open-source product analytics with feature flags ...</a></li>

</ul>
</details>

**Discussion**: Comments were mixed - some praised the clever use of AI with strong validation mechanisms, calling it "vibe-coding" that still requires deep engineering expertise. Others expressed concerns that this approach relies on pre-AI accumulated knowledge and may hinder future knowledge advancement, with one commenter noting it "feels like selling our soul to the devil for short term gains."

**Tags**: `#AI/LLM`, `#performance optimization`, `#SQL parser`, `#PostHog`, `#software engineering`

---

<a id="item-15"></a>
## [Huntington Bank Uses AWS to Redact Sensitive Data from 400M+ Documents](https://aws.amazon.com/blogs/machine-learning/huntington-bank-redacting-sensitive-data-from-400m-documents-with-aws/) ⭐️ 7.0/10

Huntington Bank built an AWS-based solution to detect and redact PII (Personally Identifiable Information) and PCI (Payment Card Industry) data from over 400 million documents, reducing processing time from years to just a few months while achieving over 95% redaction accuracy. This demonstrates how financial institutions can automate data privacy compliance at massive scale using cloud-based AI services. The solution provides a practical enterprise case study showing that processing 400M+ documents in months instead of years is now feasible with measurable accuracy improvements. The solution leverages AWS Comprehend for PII entity detection and redaction, achieving 95%+ accuracy while reducing what would have taken years of manual processing down to just a few months across 400+ million documents.

rss · AWS Machine Learning Blog · Jun 24, 18:24

**Background**: PII (Personally Identifiable Information) includes data like addresses, bank account numbers, and phone numbers that can be used to identify specific individuals. PCI (Payment Card Industry) data refers to payment card information that requires special protection under compliance regulations. AWS Comprehend is a natural language processing service that can detect, locate, and redact PII entities in text documents. Manual redaction at the scale of hundreds of millions of documents would be extremely time-consuming and prone to human error.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.aws.amazon.com/comprehend/latest/dg/pii.html">Personally identifiable information ( PII ) - Amazon Comprehend</a></li>

</ul>
</details>

**Tags**: `#PII detection`, `#AWS`, `#document processing`, `#data privacy`, `#enterprise architecture`, `#machine learning`

---

<a id="item-16"></a>
## [Building Voice Healthcare Agent with Amazon Nova 2 Sonic](https://aws.amazon.com/blogs/machine-learning/build-a-healthcare-appointment-agent-with-amazon-nova-2-sonic/) ⭐️ 7.0/10

AWS发布了技术指南,展示如何使用Amazon Nova 2 Sonic和Amazon Bedrock AgentCore构建语音驱动的医疗预约助手,该助手具备语音认证、预约管理(确认、取消、改期)、诊前健康信息收集和人工转接功能。 此技术教程展示了语音AI在医疗领域的新应用,可帮助医疗机构规模化处理常规来电,降低预约未到率,同时也展示了Nova 2 Sonic在对话式AI和智能体编排方面的能力。 该方案包含浏览器界面用于测试,并设计为可与Amazon Connect等电话服务集成以实现外呼功能。核心功能包括通过语音进行患者身份验证、预约确认/取消/改期、诊前健康信息收集,以及在需要时转接人工客服。

rss · AWS Machine Learning Blog · Jun 24, 18:20

**Background**: Amazon Nova 2 Sonic是亚马逊最新的实时语音到语音模型,提供更智能的AI能力和智能体功能,支持更直观的类人语音交互。Amazon Bedrock AgentCore是AWS的AI智能体运行时服务,支持智能体的部署、管理和工具编排。该教程聚焦于语音对话和工具编排的智能体端问题,展示了如何在医疗场景中构建合规且实用的语音AI应用。

<details><summary>References</summary>
<ul>
<li><a href="https://aws.amazon.com/blogs/aws/introducing-amazon-nova-2-sonic-next-generation-speech-to-speech-model-for-conversational-ai/">Introducing Amazon Nova 2 Sonic: Our new speech-to-speech model for ...</a></li>
<li><a href="https://docs.aws.amazon.com/nova/latest/nova2-userguide/using-conversational-speech.html">Speech-to-Speech (Amazon Nova 2 Sonic) - Amazon Nova</a></li>
<li><a href="https://medium.com/@minehli.a/amazon-bedrocks-agentcore-is-quietly-changing-everything-here-s-what-i-m-betting-on-46ebce77d853">Amazon Bedrock ’s AgentCore Is Quietly Changing... | Medium</a></li>

</ul>
</details>

**Tags**: `#Amazon Nova 2 Sonic`, `#Healthcare AI`, `#Voice Agents`, `#Amazon Bedrock`, `#Conversational AI`

---

<a id="item-17"></a>
## [NVIDIA Accelerates BEV Pooling on GPUs for Physical AI](https://developer.nvidia.com/blog/accelerating-bev-pooling-on-nvidia-gpus-for-physical-ai-applications/) ⭐️ 7.0/10

NVIDIA published a technical blog explaining how to accelerate bird's-eye-view (BEV) pooling on NVIDIA GPUs using TensorRT for autonomous vehicles and robotics perception systems. This optimization enables real-time 3D scene understanding critical for autonomous vehicles and robotics, improving the performance of physical AI applications that require precise environmental perception in dynamic environments. BEV pooling projects multi-camera image features into a shared top-down grid, providing downstream perception and planning modules with a unified spatial representation for decision-making.

rss · NVIDIA Developer Blog · Jun 24, 16:30

**Background**: Bird's-eye-view (BEV) perception is a common design pattern for autonomous vehicles, robotics, and spatial AI systems that project multi-camera image features into a shared top-down grid. Physical AI refers to AI systems that operate in and interact with the physical world, enabling machines to perceive, reason, and act in real-time environments. TensorRT is NVIDIA's deep learning inference optimizer.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/accelerating-bev-pooling-on-nvidia-gpus-for-physical-ai-applications/">Accelerating BEV Pooling on NVIDIA GPUs for Physical AI ...</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/generative-physical-ai/">What is Physical AI? | NVIDIA Glossary</a></li>
<li><a href="https://www.emergentmind.com/topics/efficient-bev-pooling">Efficient BEV Pooling Techniques - emergentmind.com</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#GPU Optimization`, `#BEV Perception`, `#Autonomous Vehicles`, `#Physical AI`, `#Computer Vision`

---

<a id="item-18"></a>
## [AI Researchers Continue Leaving Google for Anthropic](https://techcrunch.com/2026/06/24/ai-researchers-continue-to-leave-google-for-its-rivals/) ⭐️ 7.0/10

Top AI researchers Jonas Adler and Alexander Pritzel are leaving Google for Anthropic, following previous departures of leading scientists Noam Shazeer and John Jumper, continuing a pattern of talent migration from Google to its rivals. This represents a significant talent flight from Google to Anthropic, signaling competitive challenges in Google's AI division. The departure of top researchers indicates potential issues with research culture, compensation, or resource allocation at Google, while Anthropic benefits from acquiring elite AI talent. The specific individuals leaving are Jonas Adler and Alexander Pritzel, both recognized as top AI researchers in the field. This joins a growing list of departures including Noam Shazeer and John Jumper, creating a pattern that suggests systematic challenges within Google's AI research environment.

rss · TechCrunch AI · Jun 24, 21:42

**Background**: Google has long been a leader in AI research, with DeepMind being its primary AI research division. Anthropic, founded by former OpenAI researchers, has emerged as a major competitor in the AI field, particularly focused on AI safety and alignment research. The competition for top AI talent has intensified as companies race to develop advanced AI systems.

**Tags**: `#AI talent`, `#Google`, `#Anthropic`, `#industry news`, `#technology`

---

<a id="item-19"></a>
## [US Memory Chip Company Sees Revenue Quadruple to $41.45B](https://techcrunch.com/2026/06/24/the-memory-chip-crunch-is-paying-off-for-this-u-s-company/) ⭐️ 7.0/10

A US memory chip company reports revenue quadrupling to $41.45 billion and profit surging from $1.88 billion to $28.2 billion year-over-year, suggesting the ongoing memory chip shortage is benefiting domestic manufacturers. This dramatic financial performance demonstrates that US memory chip manufacturers are positioned to capitalize on the global chip shortage crisis. As demand outpaces supply for AI and high-performance computing applications, American companies producing advanced memory like HBM and 3D NAND stand to gain significant market share. The company's profit increase is extraordinary - from $1.88 billion to $28.2 billion represents a 15x surge. This suggests either highly favorable market conditions with extreme supply-demand imbalance, or potentially one-time accounting benefits. The growth is driven by demand for High Bandwidth Memory (HBM) used in AI GPUs and 3D NAND for data centers.

rss · TechCrunch AI · Jun 24, 21:30

**Background**: The global semiconductor industry has been experiencing a severe supply shortage since 2020, particularly for memory chips used in AI, cloud computing, and mobile devices. High Bandwidth Memory (HBM) is a 3D-stacked memory technology developed by Samsung, AMD and SK Hynix that provides high bandwidth for data-intensive applications. 3D NAND stacks memory cells vertically to increase storage density, powering modern SSDs and smartphones.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.techtarget.com/searchstorage/definition/3D-NAND-flash">What is 3D NAND flash? | Definition from TechTarget</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#memory chips`, `#revenue growth`, `#US companies`, `#industry news`

---

<a id="item-20"></a>
## [AI Companies Spend $27M in NY Congressional Race, Bores Loses Narrowly](https://www.theverge.com/ai-artificial-intelligence/956263/alex-bores-new-york-12th-district-congressional-primary-results) ⭐️ 7.0/10

Anthropic and OpenAI spent a combined $27 million in a New York congressional primary, making it the most expensive AI policy proxy war to date. NY Assemblyman Alex Bores narrowly lost the Democratic primary for New York's 12th Congressional district after being targeted by a pro-AI super PAC. This represents a new frontier in AI policy lobbying, showing that major AI companies are directly engaging in US electoral politics with unprecedented sums. The outcome demonstrates that massive spending does not guarantee victory, but signals that the AI industry will continue to exert political influence through campaign financing. The super PAC backing Bores received significant funding from AI companies, making him a target for opposition. The 12th Congressional district covers parts of Manhattan and Queens. This proxy war is part of a broader trend of AI industry involvement in US politics, with reports indicating $150 million in AI lobbying across multiple races.

rss · The Verge AI · Jun 24, 17:25

**Background**: Super PACs are political committees that can raise and spend unlimited money to influence elections, but cannot coordinate directly with candidates. In this race, Anthropic and OpenAI supported opposing candidates through different super PACs, effectively waging a proxy war over future AI governance policy. The outcome of this race reflects the growing political fault lines within the AI industry about how AI should be regulated.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Super_PAC">Super PAC - Wikipedia</a></li>
<li><a href="https://www.forbes.com/sites/paulocarvao/2025/11/28/150-million-ai-lobbying-war-fuels-the-fight-over-preemption/">$150 Million AI Lobbying War Fuels The Fight Over Preemption</a></li>

</ul>
</details>

**Tags**: `#AI industry`, `#politics`, `#Anthropic`, `#OpenAI`, `#lobbying`

---

<a id="item-21"></a>
## [Anthropic Accuses Alibaba of Illegally Accessing Claude Models](https://www.bloomberg.com/news/articles/2026-06-24/anthropic-accuses-alibaba-of-illicitly-accessing-its-ai-models) ⭐️ 7.0/10

Anthropic has publicly accused Alibaba of illegally accessing its Claude AI models, marking a major intellectual property dispute in the AI industry. The company claims Alibaba illicitly extracted model capabilities through systematic queries, potentially using model distillation techniques. This dispute highlights the growing challenge of protecting AI model intellectual property as model extraction techniques become more sophisticated. It could set a precedent for how AI companies protect their models and potentially lead to stricter regulations globally. Model extraction attacks work by querying target models to collect outputs and then training a replica model through knowledge distillation. This technique allows transferring capabilities from large models to smaller ones. Alibaba has not yet responded to the accusations.

rss · Hacker News - AI / LLM / Agent · Jun 25, 00:02

**Background**: Model extraction is an emerging threat in AI security where attackers attempt to replicate AI models by systematically querying them and using the outputs to train clone models. Knowledge distillation, originally a legitimate technique for compressing large models into smaller ones, can also be used for unauthorized model replication. This case represents one of the first high-profile IP disputes involving AI model theft.

<details><summary>References</summary>
<ul>
<li><a href="https://aisecurityandsafety.org/en/guides/model-theft-extraction/">Model Theft & Extraction Attacks: Protecting AI Models (2026)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_distillation">Model distillation</a></li>

</ul>
</details>

**Discussion**: Hacker News comments show skepticism about the practical viability of the accusation, with some noting that it's difficult to prove model extraction occurred. Others discuss the broader implications for AI industry IP protection and whether this signals increased tensions between US and Chinese tech companies.

**Tags**: `#AI`, `#Intellectual Property`, `#Legal`, `#Anthropic`, `#Alibaba`

---

<a id="item-22"></a>
## [OpenAI Codex Causes Millions in SSD Costs](https://www.theregister.com/ai-and-ml/2026/06/23/openai-codex-bombards-ssds-with-needless-write-operations-costing-millions/5260402) ⭐️ 7.0/10

OpenAI Codex CLI is generating excessive unnecessary SSD write operations, causing millions of dollars in unnecessary storage costs according to The Register's investigation. This bug affects AI developers using Codex CLI locally, as unnecessary write operations accelerate SSD wear, reduce performance, and increase cloud infrastructure costs for teams running these agents at scale. The issue stems from Codex CLI's file handling behavior in its local coding agent operations, where it writes far more data to disk than actually needed for the development workflow.

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Jun 24, 21:32

**Background**: OpenAI Codex CLI is an open-source terminal-based coding agent built in Rust. Write amplification is a known SSD issue where more data is written to storage than intended, causing increased wear, reduced performance, and higher costs. Codex CLI can read, edit, and run code on local machines.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.openai.com/codex/cli">CLI – Codex | OpenAI Developers</a></li>

</ul>
</details>

**Discussion**: Only one comment was found on Hacker News, with the user questioning whether this is specifically an OpenAI issue or a broader problem with AI coding agents in general.

**Tags**: `#AI infrastructure`, `#storage efficiency`, `#OpenAI Codex`, `#SSD performance`, `#cloud costs`

---

<a id="item-23"></a>
## [Using Gini Coefficient for Edge Capacity Planning](https://www.fastly.com/blog/using-gini-coefficient-plan-edge-capacity) ⭐️ 7.0/10

Fastly published a technical blog post demonstrating how the Gini Coefficient—a metric traditionally used in economics to measure income inequality—can be applied to model edge traffic inequality and plan CDN infrastructure capacity. This approach provides infrastructure engineers with a novel metric for quantifying traffic distribution across edge nodes, enabling better cache efficiency optimization and capacity planning for CDNs and edge computing networks. The Gini Coefficient measures the degree of inequality in a distribution—ranging from 0 (perfect equality) to 1 (maximum inequality). Fastly applies this concept to analyze how unevenly traffic is distributed across their edge server network, which directly impacts cache hit rates and infrastructure costs.

rss · Lobsters - AI · Jun 24, 17:08

**Background**: The Gini Coefficient is widely used in economics to measure income or wealth inequality within a population, calculated from the Lorenz curve. In this context, Fastly adapts the same mathematical concept to measure traffic inequality across edge computing nodes, helping identify where capacity is underutilized or overloaded.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fastly.com/de/blog/using-gini-coefficient-plan-edge-capacity">Using the Gini Coefficient to Plan Edge Capacity | Fastly</a></li>
<li><a href="https://www.ioriver.io/terms/cdn-capacity">What Is CDN Capacity ? Key Components & Importance</a></li>
<li><a href="https://www.youware.com/guide/future-cdn-edge-computing-web-performance">Edge Computing & CDN in 2026: The Future of Web Performance</a></li>

</ul>
</details>

**Tags**: `#edge computing`, `#capacity planning`, `#gini coefficient`, `#CDN`, `#infrastructure`, `#performance optimization`

---

<a id="item-24"></a>
## [Why Enterprise AI Agents Die at Prototype Stage](https://www.infoq.cn/article/zod9SeNbe75T8YtrIcEC?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Amazon Cloud Technology's Chu Ruisong explains that enterprise AI Agents often fail to progress beyond the prototype stage, and emphasizes Agent engineering as the key solution to move from pilot to production-scale deployment. This issue is significant because many enterprises invest heavily in AI Agent pilots but cannot scale them to production, wasting resources and slowing digital transformation. Agent engineering provides the systematic approach needed to bridge the gap between prototype and production-ready systems. According to Martin Fowler's definition, Agent engineering involves 'constraint mechanisms, feedback loops, workflow control and continuous improvement cycles' around AI Agents. Amazon Bedrock AgentCore, now generally available, is designed to help developers quickly move Agents from pilot to规模化生产 with built-in security and reliability.

rss · InfoQ 中文站 · Jun 24, 17:22

**Background**: AI Agents represent a significant advancement in enterprise automation - their 'autonomy' enables them to proactively execute tasks as 'digital employees' rather than merely assisting in decision-making. The key challenge lies in transitioning experimental prototypes to production systems that can operate reliably at scale. Amazon Bedrock provides the infrastructure to build, deploy, and operate capable agents securely at enterprise scale.

<details><summary>References</summary>
<ul>
<li><a href="https://www.betteryeah.com/blog/harness-engineering-vs-ai-agent-difference-connection-analysis">Harness 工 程 和 Agent 区别联系： 企 业 级智能体控制系统深度解析</a></li>
<li><a href="https://docs.aws.amazon.com/bedrock/latest/userguide/agents-how.html">How Amazon Bedrock Agents works</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1961482189549070102">Agent规模化生产！Amazon Bedrock AgentCore正式可用！</a></li>

</ul>
</details>

**Tags**: `#AI Agents`, `#Enterprise AI`, `#Agent Engineering`, `#Amazon Cloud Technology`, `#AI Production`

---

<a id="item-25"></a>
## [Micron Q3 FY2026: $41.46B Revenue, 346% YoY Growth Driven by AI](https://www.globenewswire.com/news-release/2026/06/24/3317151/14450/en/micron-technology-inc-reports-record-results-for-the-third-quarter-of-fiscal-2026.html) ⭐️ 7.0/10

Micron Technology reported Q3 FY2026 results with revenue of $41.46 billion, a 346% year-over-year increase, driven by massive AI infrastructure demand for high-bandwidth memory. Net income reached $28.24 billion, with non-GAAP gross margin surging to 84.9%. This demonstrates the explosive growth in AI infrastructure demand and the critical role of high-bandwidth memory (HBM) in AI computing. The memory shortage and Micron's dominant position in HBM production are creating significant market leverage, making memory suppliers essential to the AI infrastructure supply chain. All four business segments reported exceptional growth: data center revenue jumped 653% to $11.52 billion, cloud memory grew 306% to $13.77 billion, mobile and client increased 254%, and automotive and embedded doubled. Micron has signed 16 long-term strategic agreements for the next 3-5 years and expects the memory shortage to continue beyond 2027. HBM4 is already in mass production, with HBM4E scheduled for 2027 launch.

telegram · zaihuapd · Jun 24, 22:22

**Background**: High Bandwidth Memory (HBM) is a 3D-stacked memory technology that provides significantly higher bandwidth compared to traditional memory, making it essential for AI accelerators and high-performance computing. The AI infrastructure boom has created unprecedented demand for HBM, with major players like Micron, SK Hynix, and Samsung competing for market share. HBM4 is the fourth generation of this technology, with HBM4E expected to offer even higher performance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://newsroom.lamresearch.com/high-bandwidth-memory-explained-semi-101">High Bandwidth Memory (HBM) Explained</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#financial-results`, `#AI-infrastructure`, `#HBM`, `#memory-market`

---