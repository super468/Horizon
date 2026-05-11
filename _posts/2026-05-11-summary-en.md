---
layout: default
title: "Horizon Summary: 2026-05-11 (EN)"
date: 2026-05-11
lang: en
---

> From 131 items, 17 important content pieces were selected

---

1. [NVIDIA Releases cuda-oxide: Experimental Rust-to-CUDA Compiler](#item-1) ⭐️ 8.0/10
2. [llama.cpp b9095 Adds NCCL-Free Internal AllReduce for Tensor Parallelism](#item-2) ⭐️ 7.0/10
3. [Open WebUI v0.9.5 Adds SSRF Protection and iframe CSP](#item-3) ⭐️ 7.0/10
4. [Hardware Attestation as EU Digital Monopoly](#item-4) ⭐️ 7.0/10
5. [Local AI on Consumer Devices Will Become the Norm](#item-5) ⭐️ 7.0/10
6. [1e4.ai: Human-like Chess Engine via Neural Networks](#item-6) ⭐️ 7.0/10
7. [Rossmann Pledges $10K for OrcaSlicer Developer Amid Bambu Lab Lawsuit Threat](#item-7) ⭐️ 7.0/10
8. [Task Paralysis and AI in Software Development](#item-8) ⭐️ 7.0/10
9. [MachinaCheck: Multi-Agent CNC AI on AMD MI300X](#item-9) ⭐️ 7.0/10
10. [2026 Vector Database Comparison: Pricing, Scale, and Architecture Guide](#item-10) ⭐️ 7.0/10
11. [Hermes Agent Overtakes OpenClaw as Top AI Agent on OpenRouter](#item-11) ⭐️ 7.0/10
12. [NY Times Publishes Fake AI Quotation in Political Article](#item-12) ⭐️ 7.0/10
13. [Gemini API File Search Now Multimodal](#item-13) ⭐️ 7.0/10
14. [Optimizing Swift Matrix Multiplication for LLM Training](#item-14) ⭐️ 7.0/10
15. [GitHub Uses eBPF to Prevent Deployment Risks and Cascading Failures](#item-15) ⭐️ 7.0/10
16. [Report Exposes Chinese Claude API Grey Market: Fraud Behind 90% Discount](#item-16) ⭐️ 7.0/10
17. [xAI Grok Build Tool Leaked, Plans 10T Parameter Model to Rival Claude Code](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [NVIDIA Releases cuda-oxide: Experimental Rust-to-CUDA Compiler](https://www.marktechpost.com/2026/05/09/nvidia-ai-just-released-cuda-oxide-an-experimental-rust-to-cuda-compiler-backend-that-compiles-simt-gpu-kernels-directly-to-ptx/) ⭐️ 8.0/10

NVlabs has released cuda-oxide v0.1.0, a custom rustc code generation backend that compiles #[kernel]-annotated Rust functions directly to PTX (Parallel Thread Execution) through a multi-stage pipeline: Rust → Stable MIR → Pliron IR → LLVM IR → PTX, enabling single-source host+device compilation via a single cargo oxide build command. 这代表了Rust高性能GPU计算发展的重要一步。作为NVIDIA官方的实验性编译器工具，cuda-oxide允许开发者使用Rust编写GPU内核，同时利用内存安全保证，有可能取代容易出错的CUDA C++代码用于性能关键的GPU工作负载。 The compiler uses Pliron IR, an extensible compiler intermediate representation framework written in Rust and inspired by MLIR. The compilation pipeline first transforms Rust to Stable MIR, then to Pliron IR, followed by LLVM IR, and finally to PTX for SIMT (Single Instruction Multiple Threads) GPU execution.

rss · MarkTechPost · May 10, 06:01

**Background**: PTX (Parallel Thread Execution) is NVIDIA's intermediate representation that serves as the assembly language for CUDA-capable GPUs, similar to how assembly works for CPUs. SIMT is the execution model used in CUDA where multiple threads execute the same instruction simultaneously but can take different paths based on conditional logic. The GPU Ocelot project previously provided PTX module registration capabilities but is no longer actively maintained.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Parallel_Thread_Execution">Parallel Thread Execution - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Single_instruction,_multiple_threads">Single instruction, multiple threads - Wikipedia</a></li>
<li><a href="https://github.com/vaivaswatha/pliron">GitHub - vaivaswatha/pliron: An Extensible Compiler IR ...</a></li>

</ul>
</details>

**Tags**: `#GPU computing`, `#Rust`, `#CUDA`, `#compiler`, `#PTX`

---

<a id="item-2"></a>
## [llama.cpp b9095 Adds NCCL-Free Internal AllReduce for Tensor Parallelism](https://github.com/ggml-org/llama.cpp/releases/tag/b9095) ⭐️ 7.0/10

The b9095 release of llama.cpp introduces an internal NCCL-free AllReduce implementation for tensor parallelism using a single-phase CUDA kernel that pipelines D2H (device-to-host) copy, cross-GPU handshake via pinned-memory volatile flags, and the reduction in one kernel launch per GPU. 该实现消除了张量并行对外部NCCL库的依赖，简化了部署流程，并可能提高在NCCL不可用或存在问题的系统上的兼容性。它为需要在多GPU上运行大型语言模型的开发者提供了一种更简单、无依赖的解决方案。 The current implementation scope is limited to 2 GPUs, FP32 precision, and tensors up to 256 KB. Provider selection is configurable via the GGML_CUDA_ALLREDUCE environment variable ("nccl" or "internal"). The implementation falls back to the meta-backend CPU reduce for unsupported sizes or GPU counts exceeding 2.

github · github-actions[bot] · May 10, 09:43

**Background**: llama.cpp is a C++ library for efficient inference of large language models (LLMs) based on the GGML tensor library. AllReduce is a collective operation that combines data from multiple GPUs and distributes the result back to all participants, essential for tensor parallelism in distributed model training/inference. NCCL (NVIDIA Collective Communications Library) is NVIDIA's proprietary library for GPU-to-GPU communication. This internal implementation uses pinned memory (page-locked memory) for fast cross-GPU data exchange without NCCL.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ggml-org/ggml">GitHub - ggml-org/ggml: Tensor library for machine learning</a></li>
<li><a href="https://ggml.ai/">ggml.ai</a></li>

</ul>
</details>

**Tags**: `#llama.cpp`, `#CUDA`, `#GPU`, `#tensor-parallelism`, `#AllReduce`

---

<a id="item-3"></a>
## [Open WebUI v0.9.5 Adds SSRF Protection and iframe CSP](https://github.com/open-webui/open-webui/releases/tag/v0.9.5) ⭐️ 7.0/10

Open WebUI v0.9.5 introduces redirect-based SSRF protection that blocks all 3xx redirects by default via the new AIOHTTP_CLIENT_ALLOW_REDIRECTS environment variable, and adds configurable iframe Content-Security-Policy controls through the IFRAME_CSP environment variable. This release addresses critical SSRF vulnerabilities that could allow attackers to access internal services, cloud metadata endpoints, and private networks through malicious redirects. The iframe CSP controls also prevent LLM-generated or user-uploaded HTML from executing potentially malicious code in previews. The SSRF protection covers multiple call sites including web fetch, image loading, OAuth discovery, tool server execution, and code interpreter login. Redirects to RFC 1918 addresses, loopback addresses, and cloud metadata endpoints are blocked. Users can disable redirects by setting AIOHTTP_CLIENT_ALLOW_REDIRECTS=true if needed for specific deployments.

github · github-actions[bot] · May 10, 18:14

**Background**: SSRF (Server-Side Request Forgery) is a web security vulnerability that allows attackers to make the server execute unintended network requests, potentially accessing internal services, databases, or cloud metadata endpoints. RFC 1918 addresses (10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16) and cloud metadata services (169.254.169.254) are common SSRF targets. Content-Security-Policy (CSP) is a browser security header that controls what resources can be loaded and executed.

<details><summary>References</summary>
<ul>
<li><a href="https://portswigger.net/web-security/ssrf">What is SSRF (Server-side request forgery)? Tutorial ... The use of an Open Redirect in Server Side Request Forgery (SSRF) Server-Side Request Forgery Prevention Cheat Sheet - OWASP Server Side Request Forgery (SSRF) - Security | MDN Server-Side Request Forgery (SSRF) Explained: Attack ...</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/Security/Attacks/SSRF">Server Side Request Forgery (SSRF) - Security | MDN</a></li>
<li><a href="https://docs.cloud.google.com/compute/docs/metadata/overview">About VM metadata | Compute Engine | Google Cloud Documentation</a></li>

</ul>
</details>

**Tags**: `#security`, `#ssrf`, `#open-webui`, `#server-security`, `#release-update`

---

<a id="item-4"></a>
## [Hardware Attestation as EU Digital Monopoly](https://grapheneos.social/@GrapheneOS/116550899908879585) ⭐️ 7.0/10

The EU Digital Identity Wallet (EUDI) now requires hardware attestation from Google or Apple to function, effectively forcing all EU citizens to use devices from only two approved American suppliers for digital identity verification. This policy creates a digital monopoly lock-in that ties EU digital sovereignty to US tech giants, while also introduction privacy risks through device-linked attestation packets that can track user behavior across services. The EUDI does not use zero-knowledge proofs or blind signatures, meaning every attestation leaves a traceable packet that links the action to the specific device. Hardware attestation relies on TPM (Trusted Platform Module) chips that contain unique, unchangeable cryptographic keys embedded during manufacturing.

hackernews · ChuckMcM · May 10, 17:54

**Background**: Trusted Computing is a technology standard developed by the TCG (Trusted Computing Group) that uses a dedicated TPM chip to provide cryptographic attestation of device state. Hardware attestation creates a cryptographically verifiable fingerprint of the device's boot process and configuration. The technology has historical controversy, dating back to Intel's 1999 CPU serial number proposal which faced massive opposition and was abandoned, followed by continued pushing for TPM and related technologies that enabled mobile walled gardens.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Trusted_Computing">Trusted Computing - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Trusted_Platform_Module">Trusted Platform Module - Wikipedia</a></li>
<li><a href="https://aembit.io/blog/attestation-based-identity-hardware-cloud-security/">Attestation-Based Identity: How It Works and Why It Matters</a></li>

</ul>
</details>

**Discussion**: Comments highlight the irony of EU digital identity being tied to American duopoly, with users noting the lack of privacy-preserving technologies like zero-knowledge proofs. One commenter traces the history of Trusted Computing from Intel's abandoned serial number to Windows 11 TPM requirements as a 'continuing push toward walled gardens'. Another warns that this approach treats 'protecting the children > sovereignty' as a priority.

**Tags**: `#digital-sovereignty`, `#hardware-attestation`, `#privacy`, `#monopoly`, `#trusted-computing`

---

<a id="item-5"></a>
## [Local AI on Consumer Devices Will Become the Norm](https://unix.foo/posts/local-ai-needs-to-be-norm/) ⭐️ 7.0/10

An article argues that local AI running on consumer devices will become the norm as hardware improves, following a progression from large data centers with performant LLMs to servers with H100 GPUs, and eventually to consumer devices like MacBook Pro with 128GB VRAM or Strix Halo. This shift could fundamentally change how companies use AI, moving from the pattern of expensive remote LLMs for planning to local slow-but-faster-than-human LLMs for execution, potentially reducing costs and improving privacy and data control. The hardware progression timeline suggests this pattern will become mainstream within the next year. Currently, models like Phi-3, Gemma, or quantized LLaMA can run on edge devices using INT4 quantization for 2.5-4X model size reduction, while dual RTX 5090s can match H100 performance for 70B models at 25% of the cost.

hackernews · cylo · May 10, 17:19

**Background**: Local AI refers to running large language models directly on personal devices rather than sending data to remote cloud servers. This approach offers privacy benefits since data stays on the device. Open-weight models (like LLaMA) can be run locally thanks to model compression techniques such as quantization, which reduces model size by using lower precision weights. Consumer GPUs have historically been too limited for large models, but hardware improvements are changing this equation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sitepoint.com/definitive-guide-local-llms-2026-privacy-tools-hardware/">Guide to Local LLMs in 2026: Privacy, Tools & Hardware</a></li>
<li><a href="https://zenvanriel.com/ai-engineer-blog/how-to-deploy-ai-on-edge-devices-with-small-language-models/">How to Deploy AI on Edge Devices with Small Language Models ?</a></li>

</ul>
</details>

**Discussion**: Community sentiment strongly supports the prediction, with commenters providing concrete use cases for local models (text-to-speech, RAG document search, code execution) and a hardware progression timeline. Some draw parallels to open source software history, noting that initial skepticism toward open source eventually gave way to mainstream adoption. Others distinguish between private AI and local AI, arguing that self-hosted solutions with good tenant isolation could address privacy concerns without requiring local-only deployment.

**Tags**: `#local-ai`, `#edge-ai`, `#llm`, `#hardware-trends`, `#ai-infrastructure`

---

<a id="item-6"></a>
## [1e4.ai: Human-like Chess Engine via Neural Networks](https://news.ycombinator.com/item?id=48088819) ⭐️ 7.0/10

A developer released 1e4.ai, a chess web app featuring transformer-based neural networks trained on nearly 1 billion Lichess games to play like human players at specific Elo ratings (800-2200+), including realistic clock time management and blunder patterns. This represents a novel approach in game AI by prioritizing human-like behavior over pure strength. The system demonstrates that small neural networks (~9M parameters) can effectively simulate human decision-making patterns, potentially useful for training tools, testing, and studying how humans think about chess. The network takes board state, move history, player rating, and remaining clock time as inputs. It uses three separate models per rating bucket: move prediction, clock usage, and win probability. The architecture runs entirely on CPU without GPU. Performance benchmarks show 56.7% top-1 move prediction vs Maia-2's 52.7%, though it weakens above 1700 Elo due to the small model size.

rss · Hacker News - Show HN · May 10, 22:31

**Background**: The project builds on Maia-2 (a human-behavior modeling chess AI) and DeepMind's "Grandmaster-Level Chess Without Search" research. Lichess is a popular free open-source chess platform that stores millions of rated games with Elo ratings, making it ideal for training human-like AI. Transformer networks in chess have largely replaced traditional CNNs due to superior position evaluation capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Transformer_(deep_learning)">Transformer (deep learning) - Wikipedia</a></li>
<li><a href="https://www.kaggle.com/datasets/datasnaek/chess">Chess Game Dataset ( Lichess ) | Kaggle</a></li>

</ul>
</details>

**Tags**: `#chess`, `#machine-learning`, `#transformers`, `#neural-networks`, `#game-ai`

---

<a id="item-7"></a>
## [Rossmann Pledges $10K for OrcaSlicer Developer Amid Bambu Lab Lawsuit Threat](https://www.tomshardware.com/3d-printing/louis-rossmann-tells-3d-printer-maker-bambu-lab-to-go-bleep-yourself-over-its-lawsuit-against-enthusiast-right-to-repair-advocate-offers-to-pay-the-legal-fees-for-a-threatened-orcaslicer-developer) ⭐️ 7.0/10

Louis Rossmann, a prominent right-to-repair advocate and YouTuber, has pledged $10,000 to cover legal fees for an independent OrcaSlicer developer threatened with a cease and desist letter by Bambu Lab, escalating a conflict over 3D printer firmware access and user control. This represents a significant escalation in the ongoing right-to-repair battle in the 3D printing community, potentially setting precedent for how open-source software interacts with proprietary printer ecosystems and cloud services. The dispute centers on an OrcaSlicer fork that allegedly connected to Bambu Lab's private cloud APIs to impersonate Bambu Studio. The original OrcaSlicer supports Bambu printers through direct printer communication, but the threatened fork reportedly accessed non-public cloud interfaces.

hackernews · iancmceachern · May 10, 14:47

**Background**: OrcaSlicer is an open-source G-code generator and slicing software for 3D printers, supporting multiple brands including Bambu Lab, Prusa, and Voron systems. A slicer converts 3D models into printer-readable code (G-code) that controls print movements. Bambu Lab has faced criticism for requiring cloud authentication and limiting offline functionality, prompting community backlash over perceived restrictions on user ownership.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/3d-printing/louis-rossmann-tells-3d-printer-maker-bambu-lab-to-go-bleep-yourself-over-its-lawsuit-against-enthusiast-right-to-repair-advocate-offers-to-pay-the-legal-fees-for-a-threatened-orcaslicer-developer">Louis Rossmann tells 3D printer maker Bambu Lab to ‘Go (Bleep ...</a></li>
<li><a href="https://github.com/OrcaSlicer/OrcaSlicer">GitHub - OrcaSlicer/OrcaSlicer: G-code generator for 3D printers (Bambu, Prusa, Voron, VzBot, RatRig, Creality, etc.) · GitHub</a></li>
<li><a href="https://www.orcaslicer.com/download/">Download OrcaSlicer — Free 3D Printing Slicer Software for Windows, macOS, Linux</a></li>

</ul>
</details>

**Discussion**: Commenters express strong support for Louis Rossmann's funding pledge, with many criticizing Bambu Lab for limiting user control and feeling 'betrayed' as customers. Some users note the distinction between connecting to the printer directly versus accessing private cloud APIs. Users highlight that Bambu Lab previously attempted to eliminate offline access entirely before public outcry.

**Tags**: `#right-to-repair`, `#3d-printing`, `#open-source`, `#legal`, `#community`

---

<a id="item-8"></a>
## [Task Paralysis and AI in Software Development](https://g5t.de/articles/20260510-task-paralysis-and-ai/index.html) ⭐️ 7.0/10

developers report that AI coding assistants have caused 'task paralysis,' making it harder to start work and draining the enjoyment of programming. Instead of hands-on coding, developers now mainly review AI-generated outputs and manage AI agents. This matters because it affects developer wellbeing and the nature of software development work. As AI tools become more prevalent, developers risk losing the deep technical engagement they enjoy, potentially leading to burnout and profession-wide changes in what it means to be a programmer. Developers describe the shift from 'bottom to top' (owning the full process from understanding to implementation) to 'top to bottom' (receiving agent output and just reviewing it). Some report subscribing to higher AI tiers (Max 5 to Max 20) quickly, burning through limits and fearing AI addiction, especially those with ADHD who struggle with quick dopamine sources.

hackernews · MrGilbert · May 10, 06:20

**Background**: Task paralysis refers to a state where the abundance of AI assistance options makes it harder to begin tasks, as developers wait for AI to generate solutions rather than starting themselves. AI coding assistants like Claude Code have become popular tools that can generate entire codebases from natural language, shifting developer work from writing code to managing agents and reviewing outputs.

**Discussion**: The 108 comments show strong agreement with the article's thesis. Developers share personal stories of losing programming joy, describing the transition from deep technical work to agent management as 'boring' and 'frustrating.' Key concerns include AI addiction, skill atrophy, and whether developers will become unnecessary 'monkeys' who merely feed context to AI and review outputs. Some worry especially about those with ADHD who are prone to quick dopamine addiction.

**Tags**: `#AI`, `#software development`, `#task paralysis`, `#developer experience`, `#productivity`, `#addiction`

---

<a id="item-9"></a>
## [MachinaCheck: Multi-Agent CNC AI on AMD MI300X](https://huggingface.co/blog/lablab-ai-amd-developer-hackathon/machinacheck) ⭐️ 7.0/10

MachinaCheck is a multi-agent AI system developed at the AMD Developer Hackathon that automates CNC manufacturability analysis. It takes STEP CAD files along with material, tolerance, and thread specifications, then runs a four-agent pipeline to determine if a design can be manufactured. This project demonstrates the practical application of multi-agent AI frameworks in specialized manufacturing sectors. By automating manufacturability checks, companies can significantly reduce the time and cost associated with design errors, potentially transforming how machine shops evaluate production feasibility. The system runs on AMD's MI300X accelerator featuring 304 GPU compute units and 192 GB of HBM3 memory with 5.3 TB/s bandwidth. The four-agent pipeline includes STEP geometry parsing via cadquery, operations classification, and tool inventory matching. The system can generate a detailed feasibility report in just 30 seconds.

rss · Hugging Face Blog · May 10, 18:44

**Background**: CNC (Computer Numerical Control) manufacturing involves creating custom parts from materials like metal and plastic using computer-controlled cutting tools. A key challenge is determining whether a designed part can actually be manufactured without expensive trial-and-error. Multi-agent AI systems use multiple AI agents working collaboratively to solve complex tasks more effectively than single AI models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html">AMD Instinct™ MI300X Accelerators</a></li>
<li><a href="https://tensorwave.com/blog/mi300x-2">AMD MI300X Accelerator Unpacked: Specs, Performance, & More - TensorWave</a></li>
<li><a href="https://aitoolly.com/ai-news/article/2026-05-11-machinacheck-building-a-multi-agent-cnc-manufacturability-system-on-amd-mi300x">MachinaCheck: CNC AI System on AMD MI300X Hardware | AIToolly</a></li>

</ul>
</details>

**Tags**: `#multi-agent-systems`, `#CNC-manufacturing`, `#AMD-MI300X`, `#AI-accelerators`, `#hardware-hackathon`

---

<a id="item-10"></a>
## [2026 Vector Database Comparison: Pricing, Scale, and Architecture Guide](https://www.marktechpost.com/2026/05/10/best-vector-databases-in-2026-pricing-scale-limits-and-architecture-tradeoffs-across-nine-leading-systems/) ⭐️ 7.0/10

A comparative guide evaluates nine production vector databases across their architecture approaches, pricing models, and scale limits, providing practical insights for developers building RAG and agentic AI applications. Vector databases have become core retrieval infrastructure for RAG and agentic AI systems. This guide helps practitioners make informed decisions when selecting a vector database by understanding the tradeoffs between cost, performance, and scalability. The comparison covers architecture approaches, pricing models, and scale limits across nine leading systems, with specific attention to how each system handles vector storage, indexing, and retrieval at scale.

rss · MarkTechPost · May 10, 23:56

**Background**: Vector databases store data embeddings and enable approximate nearest neighbor search, which is essential for semantic retrieval in AI applications. RAG (Retrieval-Augmented Generation) combines information retrieval with text generation to enhance LLM outputs. Agentic AI involves multiple AI agents orchestrating tasks together, requiring scalable and reliable retrieval infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vector_database">Vector database - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval-augmented generation - Wikipedia</a></li>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/agentic-ai-explained">Agentic AI, explained | MIT Sloan</a></li>
<li><a href="https://www.pinecone.io/learn/vector-database/">What is a Vector Database & How Does it Work? | Pinecone</a></li>

</ul>
</details>

**Tags**: `#vector-databases`, `#AI-infrastructure`, `#RAG`, `#database-comparison`, `#2026-trends`

---

<a id="item-11"></a>
## [Hermes Agent Overtakes OpenClaw as Top AI Agent on OpenRouter](https://www.marktechpost.com/2026/05/10/openclaw-vs-hermes-agent-why-nous-researchs-self-improving-agent-now-leads-openrouters-global-rankings/) ⭐️ 7.0/10

Hermes Agent, the open-source self-improving AI agent from Nous Research, has overtaken OpenClaw to claim the #1 position on OpenRouter's global daily token rankings as of May 10, 2026 — generating 224 billion daily tokens versus OpenClaw's 186 billion. This milestone places a Nous Research project ahead of an OpenAI-sponsored platform in real-world daily inference volume, demonstrating rapid adoption of self-improving AI agents just three months after launch. Hermes Agent is the only agent with a built-in learning loop — it creates skills from experience, improves during use, persists knowledge, searches past conversations, and builds a deepening model of who you are across sessions.

rss · MarkTechPost · May 10, 16:20

**Background**: OpenRouter is a unified gateway platform that allows developers to access multiple AI models through a single API and unified credit system. Self-improving AI agents represent a shift in AI architecture, employing internal learning loops to reflect on actions, identify successes and failures, and dynamically adapt strategies without retraining. Nous Research is an AI safety and capabilities research organization that created Hermes Agent as a production-ready autonomous agent.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/">OpenRouter</a></li>
<li><a href="https://hermes-agent.nousresearch.com/">Hermes Agent — The Agent That Grows With You | Nous Research</a></li>
<li><a href="https://www.agntable.com/blog/what-is-hermes-agent">What is Hermes Agent ? Features, Memory & Skills</a></li>

</ul>
</details>

**Tags**: `#AI Agents`, `#Nous Research`, `#OpenRouter`, `#OpenClaw`, `#Self-Improving AI`

---

<a id="item-12"></a>
## [NY Times Publishes Fake AI Quotation in Political Article](https://simonwillison.net/2026/May/10/new-york-times-editors-note/#atom-everything) ⭐️ 7.0/10

The New York Times issued an Editor's Note acknowledging that a quotation attributed to Conservative leader Pierre Poilievre was actually an AI-generated summary presented as a direct quote. The article originally claimed Mr. Poilievre referred to politicians who changed allegiances as 'turncoats', but this was fabricated by the AI tool and never said in his actual April speech. This incident represents a significant real-world case of AI hallucination being published in major journalism, demonstrating the concrete risks of trusting AI-generated content without verification. It highlights the critical need for journalism standards to evolve when using AI tools in reporting, as even trusted AI outputs can produce convincing fabrications. The Times noted that the reporter should have checked the accuracy of what the AI tool returned before publishing. The corrected article now accurately quotes from a speech delivered by Mr. Poilievre in April 2026. This case involves the Canadian federal election with Mark Carney and the Liberal Party.

rss · Simon Willison · May 10, 23:58

**Background**: AI hallucination refers to when large language models generate fabricated information that appears authentic but is factually incorrect. This is a well-known limitation of generative AI systems, where models can produce coherent-sounding but entirely false statements. Journalism has increasingly adopted AI tools for assistance, but this case demonstrates the danger of treating AI outputs as verified facts without human cross-checking.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hallucination_(artificial_intelligence)">Hallucination (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-hallucinations">What Are AI Hallucinations? - IBM</a></li>

</ul>
</details>

**Tags**: `#ai-ethics`, `#hallucinations`, `#journalism`, `#generative-ai`, `#new-york-times`

---

<a id="item-13"></a>
## [Gemini API File Search Now Multimodal](https://blog.google/innovation-and-ai/technology/developers-tools/expanded-gemini-api-file-search-multimodal-rag/) ⭐️ 7.0/10

Google announced that the Gemini API now supports multimodal file search for RAG applications. Using the gemini-embedding-2 model, developers can now process and retrieve information across different file types including images without relying on traditional OCR. This capability enables TRUE visual retrieval, making it significantly easier to build efficient multimodal file retrieval systems. Developers can now create RAG applications that search across diverse document types including images, PDFs, and text files - valuable for enterprise knowledge management and document search. The gemini-embedding-2 model embeds images directly rather than relying on OCR, enabling native image search. For multimodal stores, citations also include downloadable image references. This represents a significant expansion from text-only file search capabilities.

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · May 10, 03:22

**Background**: RAG (Retrieval Augmented Generation) is a technique that enhances AI model accuracy by retrieving relevant information from external sources before generating responses. Multimodal file search allows processing different file types (images, documents, PDFs) within a single search system. Previously, file search often relied on OCR to extract text from images - this update enables direct image embedding and retrieval.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/expanded-gemini-api-file-search-multimodal-rag/">Gemini API File Search is now multimodal - The Keyword</a></li>
<li><a href="https://dev.to/googleai/multimodal-rag-with-the-gemini-api-file-search-tool-a-developer-guide-5878">Multimodal RAG with the Gemini API File Search Tool: A ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval-augmented generation - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News discussion shows moderate interest with 145 points and 39 comments. Developers are curious about practical applications and performance. Some questions remain about how this compares to other multimodal search solutions and the cost/performance tradeoffs of the new embedding model.

**Tags**: `#Google Gemini`, `#Multimodal AI`, `#RAG`, `#API Development`, `#Retrieval Augmented Generation`

---

<a id="item-14"></a>
## [Optimizing Swift Matrix Multiplication for LLM Training](https://www.cocoawithlove.com/blog/matrix-multiplications-swift.html) ⭐️ 7.0/10

A practical guide demonstrates achieving 1000x performance improvement in Swift matrix multiplication for LLM training, taking performance from Gflop/s to Tflop/s through low-level optimization techniques. This optimization is significant for developers building LLMs on Apple Silicon, as matrix multiplication is a fundamental operation in neural network training and achieving Tflop/s-level performance enables practical in-device LLM training. The author's iterative optimization approach builds progressively from basic Swift implementations through BLAS in Accelerate framework to direct AMX (Apple Matrix Coprocessor) usage, leveraging Apple Silicon's dedicated matrix accelerator for Tflop/s-level throughput.

rss · Lobsters - AI · May 10, 15:49

**Background**: Apple Silicon integrates a dedicated Apple Matrix Coprocessor (AMX) that executes matrix operations with high throughput, though its programming model is largely hidden behind the Accelerate framework. The BLAS (Basic Linear Algebra Subprograms) library in Accelerate provides a Swift-friendly API for common linear algebra operations like matrix multiplication. Performance is measured in FLOPS (Floating-point Operations Per Second), with Gflop/s representing billions and Tflop/s representing trillions of operations per second.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/frosnerd/comparing-openblas-and-accelerate-on-apple-silicon-for-blas-routines-2pb9">Comparing OpenBLAS and Accelerate on Apple Silicon for BLAS ...</a></li>
<li><a href="https://developer.apple.com/documentation/accelerate/blas">BLAS | Apple Developer Documentation</a></li>

</ul>
</details>

**Discussion**:  Discussion on Lobsters focuses on the practical value of this optimization guide for Swift developers working on ML on Apple Silicon, with appreciation for the author's deep expertise in Swift performance tuning.

**Tags**: `#swift`, `#matrix-multiplication`, `#llm-training`, `#performance-optimization`, `#apple-silicon`

---

<a id="item-15"></a>
## [GitHub Uses eBPF to Prevent Deployment Risks and Cascading Failures](https://www.infoq.cn/article/duka4AFM1UaEmx23F2ZB?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

GitHub has implemented eBPF technology in production environments to eliminate deployment risks and prevent cascading failures caused by circular dependencies between services. This represents a practical application of eBPF at scale in a major tech company, addressing real-world DevOps challenges. Circular dependencies in deployment pipelines can cause system-wide outages if not detected early, making this approach highly valuable for maintaining infrastructure reliability. eBPF (extended Berkeley Packet Filter) allows running custom programs in the Linux kernel with minimal overhead and sandboxed safety. GitHub's implementation likely uses eBPF to monitor service interactions and deployment sequences in real-time, detecting problematic dependency graphs before they cause cascading failures.

rss · InfoQ 中文站 · May 10, 15:11

**Background**: eBPF originated from the classic Berkeley Packet Filter but has evolved into a powerful framework for running безопасные programs in kernel space without modifying the kernel itself. Circular dependencies occur when service A depends on service B, which depends on service A, creating a deadlock that can trigger cascading failures during deployments. This is a common challenge in large microservice architectures.

<details><summary>References</summary>
<ul>
<li><a href="https://ebpf.io/zh-hans/what-is-ebpf/">什 么 是 eBPF ? An Introduction and Deep Dive into the eBPF Technology</a></li>
<li><a href="https://www.ibm.com/cn-zh/think/topics/ebpf">什 么 是 eBPF ？| IBM</a></li>
<li><a href="https://cloud.tencent.com/developer/article/1970118">一文看懂 eBPF ｜ eBPF 的简单使用-腾讯云开发者社区-腾讯云</a></li>

</ul>
</details>

**Tags**: `#eBPF`, `#DevOps`, `#系统 reliability`, `#部署风险控制`, `#GitHub`, `#故障预防`

---

<a id="item-16"></a>
## [Report Exposes Chinese Claude API Grey Market: Fraud Behind 90% Discount](https://www.tomshardware.com/tech-industry/artificial-intelligence/chinese-grey-market-sells-claude-api-access-at-90-percent-off-through-proxy-networks-that-harvest-user-data) ⭐️ 7.0/10

A security report reveals that Chinese grey market services are selling Claude API access at up to 90% discount through proxy networks. These services obtain access using stolen credit cards, abused free trial accounts, or hired identity verification, while also substituting cheaper models and harvesting user prompts for model distillation. This affects developers who think they're getting a deal but are actually having their code and business secrets stolen. The model substitution fraud also means user's may not be using the intended AI model, potentially introducing security vulnerabilities and reliability issues into their applications. The main fraud methods include using stolen credit cards to pay for API access, creating multiple free trial accounts, splitting subscription plans to share access, and hiring people in low-income countries to bypass identity verification. Service providers also commonly substitute cheaper domestic models when users request Claude Opus, and collect user prompts and outputs to sell for model distillation training.

telegram · zaihuapd · May 10, 01:48

**Background**: API proxy services (中转站) act as intermediaries that route user requests to official AI providers. Model distillation is a technique where a smaller model learns to mimic a larger model's behavior using the larger model's outputs. Anthropic's Claude is one of the leading proprietary LLMs, and in China, direct access to foreign AI APIs often faces network restrictions and high costs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.rfa.org/mandarin/shangye/2025/01/30/deepseek-debates/">DeepSeek靠“ 蒸 馏 ”火出圈：创新还是剽 窃 ？ – 普通话主页</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/2020215397866033689">最近用的几个Claude API中转站价格和体验对比 - 知乎</a></li>
<li><a href="https://developer.aliyun.com/article/1728443">我对比了8个Claude API中转站，踩了不少坑，总结给你</a></li>

</ul>
</details>

**Discussion**: There is significant discussion on Chinese developer forums about identifying reliable API proxies, with some users sharing experiences of being charged for premium models but receiving inferior results. The broader AI community has also raised concerns about model distillation as a form of intellectual property theft, with companies like Anthropic and OpenAI actively pursuing legal action.

**Tags**: `#AI安全`, `#API欺诈`, `#数据隐私`, `#Claude`, `#灰色产业`

---

<a id="item-17"></a>
## [xAI Grok Build Tool Leaked, Plans 10T Parameter Model to Rival Claude Code](https://tech.ifeng.com/c/8t0yrbeeuwt) ⭐️ 7.0/10

xAI's desktop programming tool 'Grok Build' was leaked, revealing a cross-platform AI Agent workflow application that can autonomously execute multi-step development tasks, defaulting to Grok 4.3 Early Access with support for local files, Git permissions, MCP, official skills and plugins. This leak directly challenges Anthropic's Claude Code in the AI coding tools space. The leaked documents reveal xAI is training massive models up to 10 trillion parameters, signaling Musk's ambition to compete with Claude Code's Opus-level coding capabilities. To match Claude Code's Opus tier would require at least 6 trillion parameters according to the leaked materials. The documents also reveal plans for 1T, 1.5T, and 10T parameter models, plus an image/video model called Imagine V2.

telegram · zaihuapd · May 10, 13:34

**Background**: Claude Code is Anthropic's AI coding assistant, with Opus being its most capable tier. MCP (Model Context Protocol) is an open standard introduced by Anthropic in November 2024 to standardize how AI systems integrate with external tools. Elon Musk previously stated xAI would release a new model in June with coding capabilities surpassing Claude.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model ) - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/news/model-context-protocol">Introducing the Model Context Protocol \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#xAI`, `#Grok`, `#AI coding tools`, `#Claude Code`, `#large language models`

---