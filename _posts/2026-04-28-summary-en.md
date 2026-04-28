---
layout: default
title: "Horizon Summary: 2026-04-28 (EN)"
date: 2026-04-28
lang: en
---

> From 165 items, 27 important content pieces were selected

---

1. [4TB Voice Data Stolen from 40K Mercor AI Contractors](#item-1) ⭐️ 9.0/10
2. [vLLM v0.20.0 Release: CUDA 13.0 Default, PyTorch 2.11 Upgrade](#item-2) ⭐️ 8.0/10
3. [Microsoft Ends Exclusive Revenue-Sharing Deal with OpenAI](#item-3) ⭐️ 8.0/10
4. [GitHub Copilot Shifts to Usage-Based Pricing](#item-4) ⭐️ 8.0/10
5. [Open-Source Agent Dirac Tops TerminalBench at 65.2%](#item-5) ⭐️ 8.0/10
6. [FDA Approves First Gene Therapy for Genetic Hearing Loss](#item-6) ⭐️ 8.0/10
7. [Why Not Just Use Lean? Proof Assistant Comparison](#item-7) ⭐️ 8.0/10
8. [DeepMind's David Silver Raises $1.1B to Build AI Without Human Data](#item-8) ⭐️ 8.0/10
9. [Google Employees Urge Pichai to Block Pentagon AI Access](#item-9) ⭐️ 8.0/10
10. [Xiaomi Xuanjie O1 Chip Shipments Exceed 1 Million Units](#item-10) ⭐️ 8.0/10
11. [Scientists Achieve Record High-Harmonic Generation Near Schwinger Limit](#item-11) ⭐️ 8.0/10
12. [SVG Sanitization Vulnerabilities: Scratch XSS Case Study](#item-12) ⭐️ 7.0/10
13. [China Blocks Meta's Acquisition of AI Startup Manus](#item-13) ⭐️ 7.0/10
14. [Super ZSNES: GPU-Powered SNES Emulator Project](#item-14) ⭐️ 7.0/10
15. [pgBackRest Maintainer Stops Development After 13 Years](#item-15) ⭐️ 7.0/10
16. [Supreme Court Reviews Police Use of Cell Phone Location Data](#item-16) ⭐️ 7.0/10
17. [OpenAI Achieves FedRAMP Moderate Authorization for Enterprise Products](#item-17) ⭐️ 7.0/10
18. [OpenAI Wins AWS Sales Rights From Microsoft in $50B Deal](#item-18) ⭐️ 7.0/10
19. [Musk vs Altman: OpenAI Mission Trial Begins](#item-19) ⭐️ 7.0/10
20. [Canva Apologizes After AI Tool Replaces 'Palestine' in Designs](#item-20) ⭐️ 7.0/10
21. [Rebuilding the Data Stack for AI](#item-21) ⭐️ 7.0/10
22. [Google Warns Malicious Web Pages Hijacking Enterprise AI Agents](#item-22) ⭐️ 7.0/10
23. [AlphaGo Creator David Silver Launches $1.1B Superlearner AI Company](#item-23) ⭐️ 7.0/10
24. [Developer Shares 3-Month ChatGPT App Review Journey](#item-24) ⭐️ 7.0/10
25. [Moore Threads Reports 86%+ R&D Investment, Deploys 10K-GPU Cluster](#item-25) ⭐️ 7.0/10
26. [When Cloud Regions Fail: HA Architecture for Geopolitical Risks](#item-26) ⭐️ 7.0/10
27. [Xiaomi Open-Sources MiMo-V2.5 Series AI Models Under MIT License](#item-27) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [4TB Voice Data Stolen from 40K Mercor AI Contractors](https://app.oravys.com/blog/mercor-breach-2026) ⭐️ 9.0/10

The Lapsus$ hacking group breached Mercor, an AI contractor platform, stealing 4TB of voice samples from 40,000 contractors paired with their ID documents. This creates a complete 'deepfake-ready kit' enabling identity fraud through banking voiceprint bypass, Arup-style video call impersonation, and insurance fraud. This breach is significant because it combines voice biometric data with ID documents—the two components needed to bypass voice-based banking authentication. Victims face an ironic situation where they may need to submit more voice data to verify if they were compromised, creating a recursive privacy trap. The breach is particularly dangerous because most leaks expose either voice data OR ID documents, not both together. This combination allows attackers to create synthetic voices for bypassing voice biometric systems, conduct video call impersonation, and forge identity for insurance claims. ORAVYS offers free analysis of the first three suspect samples for affected contractors.

hackernews · Oravys · Apr 27, 09:57

**Background**: Voice biometric authentication is increasingly used in banking for 'proof-of-life' verification, identifying over 140 voice features to verify identity. Deepfake technology can now clone voices from samples as short as a few seconds, making voice data extremely valuable for fraud. The German concept of 'Datensparsamkeit' (data frugality) advocates minimizing data collected to reduce breach impact.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gnani.ai/resources/blogs/voice-biometric-security-instantly-reduces-banking-fraud-386b3">Instant Banking Fraud Prevention with Voice Biometric Security</a></li>
<li><a href="https://www.phonexia.com/blog/voice-biometrics-in-the-banking-industry/">Voice Biometrics in the Banking Industry | PHONEXIA</a></li>
<li><a href="https://www.respeecher.com/blog/everything-you-need-know-about-deepfake-voice-its-synthetic-voice-ethical-counterpart">Everything You Need to Know about Deepfake Voice and Its...</a></li>

</ul>
</details>

**Discussion**: The discussion highlights the irony that victims must submit more voice data to verify if their voice was stolen—sending yet another voice sample to an AI company for help. Commenters note that biometrics are essentially 'forever passwords' that cannot be changed once compromised. The German concept of 'Datensparsamkeit' was praised as a solution: the only truly secure data is data that doesn't exist.

**Tags**: `#data-breach`, `#biometric-security`, `#deepfakes`, `#voice-recognition`, `#AI-security`, `#privacy`

---

<a id="item-2"></a>
## [vLLM v0.20.0 Release: CUDA 13.0 Default, PyTorch 2.11 Upgrade](https://github.com/vllm-project/vllm/releases/tag/v0.20.0) ⭐️ 8.0/10

vLLM v0.20.0 was released with 752 commits from 320 contributors, featuring CUDA 13.0 as the default version, a breaking PyTorch 2.11 upgrade, initial DeepSeek V4 support, and Python 3.14 added to the supported versions list. This release is significant because it delivers major infrastructure upgrades including CUDA 13.0 and PyTorch 2.11, which will improve inference performance and compatibility. The addition of DeepSeek V4 support and Python 3.14 compatibility demonstrates vLLM's commitment to staying current with the latest AI model architectures and Python versions. Key breaking change: PyTorch 2.11 is now required (XPU also on 2.11, no longer pinned to 2.10). FlashAttention 4 is re-enabled as the default MLA prefill backend. TurboQuant 2-bit KV cache offers 4× capacity with compression. The release also includes vLLM IR initial skeleton for future kernel work and extensive MoE refactoring.

github · khluu · Apr 27, 21:20

**Background**: vLLM is a high-performance LLM (Large Language Model) inference engine designed to optimize throughput and latency. CUDA is NVIDIA's parallel computing platform, and newer versions like CUDA 13.0 provide better performance. PyTorch 2.11 brings significant changes that may affect existing setups. DeepSeek V4 is a Mixture-of-Experts (MoE) model with 1 trillion parameters and 1M-token context window support.

<details><summary>References</summary>
<ul>
<li><a href="https://build.nvidia.com/deepseek-ai/deepseek-v4-pro/modelcard">deepseek - v 4 -pro Model by Deepseek -ai | NVIDIA NIM</a></li>
<li><a href="https://arxiv.org/html/2512.02556v1">DeepSeek -V3.2: Pushing the Frontier of Open Large Language Models</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#PyTorch`, `#CUDA`, `#deep learning`

---

<a id="item-3"></a>
## [Microsoft Ends Exclusive Revenue-Sharing Deal with OpenAI](https://www.bloomberg.com/news/articles/2026-04-27/microsoft-to-stop-sharing-revenue-with-main-ai-partner-openai) ⭐️ 8.0/10

Microsoft and OpenAI have ended their exclusive revenue-sharing partnership, removing constraints that previously prevented OpenAI from using competing cloud providers like AWS. The deal allowed OpenAI to pursue other cloud infrastructure options, fundamentally shifting the dynamics of their relationship. This termination marks a significant shift in the AI industry power structure. OpenAI can now diversify its cloud infrastructure beyond Azure, potentially weakening Microsoft's leverage while increasing competition among cloud providers. The move signals a new era where even deep partnerships face market pressures. Microsoft previously owned approximately 49% of OpenAI but has reduced its stake to 27%. The exclusive deal originally prevented OpenAI from working with competing cloud providers like AWS, creating a near-monopoly for Azure in the partnership. OpenAI can now freely collaborate with AWS and other providers.

hackernews · helsinkiandrew · Apr 27, 13:22

**Background**: Microsoft invested billions in OpenAI starting in 2019, becoming its exclusive cloud computing partner and the sole provider of infrastructure for training and deploying OpenAI models. The revenue-sharing agreement was unique in the industry, giving Microsoft preferential terms in exchange for its massive compute investments. This partnership was central to Azure's AI positioning against AWS and Google Cloud.

**Discussion**: Commenters suggest Google may be the biggest winner, as virtually all frontier AI labs use TPU and OpenAI now has that option with the Gen 8 TPU launch. Some question why Microsoft accepted terms so favorable to OpenAI, suggesting Azure was 'hanging by a thread' and Microsoft feared risking its investment amid Anthropic competition. Others note Microsoft's ownership stake dropped from 49% to 27%, questioning Microsoft's weakening position.

**Tags**: `#microsoft`, `#openai`, `#ai-industry`, `#cloud-computing`, `#partnership`

---

<a id="item-4"></a>
## [GitHub Copilot Shifts to Usage-Based Pricing](https://github.blog/news-insights/company-news/github-copilot-is-moving-to-usage-based-billing/) ⭐️ 8.0/10

GitHub Copilot is transitioning from fixed monthly subscriptions ($10/month for Pro, $39/month for Pro+) to usage-based billing with AI Credits, marking the end of Microsoft's subsidized AI inference era. 这个计费模式的变化影响了数百万依赖AI辅助编程工具的开发者。重度用户可能面临显著的成本增加，而轻度用户则可能受益于按需付费的模式。这一变化引发了关于与OpenRouter等替代方案价值对比的广泛讨论。 The new model multipliers range from 1x to 6x for newer GPT and Sonnet models, and up to 27x for Opus. Users previously could get over $500 worth of value from the $10/month plan through extensive prompting, making the effective increase potentially 50x or more for heavy users.

hackernews · frizlab · Apr 27, 16:03

**Background**: GitHub Copilot is an AI-powered code completion tool that integrates with popular IDEs. Since its launch, it has operated on fixed subscription plans where users paid a monthly fee regardless of usage. Microsoft's heavy subsidies allowed developers to access advanced AI models like GPT-4 at a fraction of their market cost. The shift to usage-based billing reflects broader industry trends toward metered AI pricing as inference costs remain high.

**Discussion**: 社区对价格上涨表现出强烈担忧，许多用户指出补贴推理时代的结束。评论强调GitHub的定价与直接API提供商相似且没有折扣，导致用户考虑OpenRouter或Deepseek等替代方案。一些用户计算得出，对于以前利用10美元计划无限潜力的重度用户来说，实际增长可能达到50倍。

**Tags**: `#github-copilot`, `#pricing`, `#developer-tools`, `#ai-billing`, `#usage-based-pricing`

---

<a id="item-5"></a>
## [Open-Source Agent Dirac Tops TerminalBench at 65.2%](https://github.com/dirac-run/dirac) ⭐️ 8.0/10

An open-source CLI agent called Dirac achieved 65.2% accuracy on TerminalBench using Gemini-3-flash-preview, significantly outperforming Google's official 47.8% and the existing top closed-source Junie CLI's 64.3%. The agent employs novel techniques including hash-anchored file editing, AST-based context fetching, and operation batching. This demonstrates how significantly the AI harness architecture impacts benchmark performance—a 17.4 percentage point improvement over Google's official results was achieved through better engineering rather than model changes. It highlights that comparing AI agents fairly requires controlling for harness differences, and the open-source nature allows the community to verify and build upon these techniques. Dirac uses hash-anchored edits that compute stable cryptographic hashes for individual lines to anchor changes (remaining valid even when files shift), AST-based context fetching that uses the language's AST to selectively retrieve relevant code sections (avoiding large file reads), and batches all operations to perform multiple reads and edits simultaneously.

hackernews · GodelNumbering · Apr 27, 12:35

**Background**: TerminalBench is a benchmark for testing AI agents on realistic, hard tasks in command line environments. The benchmark evaluates how well AI agents can complete complex terminal operations. Recent reports have highlighted cheating on TerminalBench 2.0, where some agents exploit the benchmark to inflate scores. The hash-anchored file editing technique provides cryptographic verification of changes, while AST-based fetching helps LLMs understand code structure without reading entire files.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2601.11868">[2601.11868] Terminal-Bench: Benchmarking Agents on Hard, Realistic Tasks in Command Line Interfaces</a></li>
<li><a href="https://github.com/laude-institute/terminal-bench">GitHub - harbor-framework/terminal-bench: A benchmark for LLMs on complicated tasks in the terminal · GitHub</a></li>
<li><a href="https://www.aitoolnet.com/dirac">Dirac - Open-Source Coding Agent with Hash - Anchored ... - Aitoolnet</a></li>

</ul>
</details>

**Discussion**: 评论者赞赏技术创新的同时提出了重要担忧：一人指出基准测试应测试不同模型系列的泛化能力（不仅仅是Gemini），并指出登录页面未提及Gemini 3 Flash。另一人强调harness差异可能比模型差异更重要，询问是否有比较harness的排行榜。一位用户还注意到向dirac.run发送了遥测数据，询问收集了什么内容。

**Tags**: `#open-source`, `#ai-agents`, `#benchmarking`, `#gemini`, `#terminal-bench`, `#llm-harnesses`

---

<a id="item-6"></a>
## [FDA Approves First Gene Therapy for Genetic Hearing Loss](https://www.fda.gov/news-events/press-announcements/fda-approves-first-ever-gene-therapy-treatment-genetic-hearing-loss-under-national-priority-voucher) ⭐️ 8.0/10

FDA has approved Otarmeni (lunsotogene parvec-cwha), the first-ever gene therapy for treating genetic hearing loss caused by OTOF gene mutations. The therapy is indicated for pediatric and adult patients with severe-to-profound sensorineural hearing loss associated with biallelic OTOF variants. This approval marks a historic milestone as the first FDA-approved gene therapy for genetic hearing loss, opening new possibilities for treating previously incurable forms of hereditary deafness. The therapy uses AAV vectors to deliver a functional copy of the OTOF gene, potentially restoring hearing function in patients who would otherwise face lifelong deafness. Otarmeni is an adeno-associated virus (AAV) vector-based gene therapy that delivers a functional OTOF gene to restore otoferlin protein production, which is essential for auditory synapse function. The FDA approved it under the National Priority Voucher Program, and Regeneron will provide the therapy for free in the U.S. It applies only to hearing loss caused by OTOF mutations, representing a small subset of genetic deafness cases.

hackernews · JeanKage · Apr 27, 10:15

**Background**: OTOF gene mutations cause auditory neuropathy spectrum disorder, where sound enters the inner ear normally but transmission from the inner ear to the brain is impaired due to defective otoferlin protein. Otoferlin is crucial for synaptic vesicle exocytosis at the inner hair cell ribbon synapse. This therapy represents years of research from Decibel Therapeutics, which was acquired by Regeneron, and builds on clinical trials showing safety and efficacy followed up to 2.5 years.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fda.gov/news-events/press-announcements/fda-approves-first-ever-gene-therapy-treatment-genetic-hearing-loss-under-national-priority-voucher">FDA Approves First-Ever Gene Therapy for Treatment of Genetic Hearing Loss Under National Priority Voucher Program | FDA</a></li>
<li><a href="https://www.nature.com/articles/s41586-026-10393-y">Multicentre gene therapy for OTOF-related deafness followed up to 2.5 years | Nature</a></li>
<li><a href="https://investor.regeneron.com/news-releases/news-release-details/otarmenitm-lunsotogene-parvec-cwha-approved-fda-first-and-only">Otarmeni™ (lunsotogene parvec-cwha) Approved by FDA as First and Only Gene Therapy for Genetic Hearing Loss; Regeneron to Provide Otarmeni for Free in the U.S. | Regeneron Pharmaceuticals Inc.</a></li>

</ul>
</details>

**Discussion**: The community response is overwhelmingly positive, with many celebrating this breakthrough for children and families affected by OTOF-related deafness. Some commenters share personal stories of living with hearing loss and express hope for future treatments covering other genetic causes like GJB2. Others note the limitation that this therapy doesn't help those with acquired hearing loss from conditions like mumps.

**Tags**: `#gene-therapy`, `#FDA`, `#medical-breakthrough`, `#biotechnology`, `#hearing-loss`

---

<a id="item-7"></a>
## [Why Not Just Use Lean? Proof Assistant Comparison](https://lawrencecpaulson.github.io//2026/04/23/Why_not_Lean.html) ⭐️ 8.0/10

A Hacker News discussion (248 points, 177 comments) compared Lean's approach to functional programming and theorem proving against Agda, Coq, and Isabelle/HOL, with practitioners sharing nuanced perspectives on the tradeoffs between these proof assistants. This discussion matters because choosing a proof assistant is a long-term commitment, and the real-world insights from practitioners help developers make informed decisions based on actual usability rather than theoretical claims. One commenter clarified that Lean does not actually retain proof objects in the final proof—contrary to the original author's claim. Community members from Agda, Coq, and Isabelle backgrounds shared that Lean's main strength is being decent at everything with a huge community, rather than being the best at any single aspect.

hackernews · ibobev · Apr 27, 14:24

**Background**: Proof assistants are formal verification tools used to prove mathematical theorems using computer assistance. Lean combines functional programming with theorem proving in a single framework. Agda is a dependently typed programming language based on Martin-Löf type theory. Coq is known for its powerful tactic-based proof development. Isabelle/HOL uses higher-order logic for proof construction. Each tool makes different tradeoffs between programming expressivity and proof verification capability.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Isabelle_(proof_assistant)">Isabelle (proof assistant) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agda_(programming_language)">Agda (programming language) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The discussion revealed mixed opinions: some found Lean a 'clunky downgrade' from Agda in terms of dependent types, while others appreciated its balanced approach. Isabelle users noted different tradeoffs rather than clear superiority. A key correction was that Lean doesn't actually retain large proof objects as the original post suggested.

**Tags**: `#formal methods`, `#lean`, `#proof assistants`, `#theorem proving`, `#functional programming`

---

<a id="item-8"></a>
## [DeepMind's David Silver Raises $1.1B to Build AI Without Human Data](https://techcrunch.com/2026/04/27/deepminds-david-silver-just-raised-1-1b-to-build-an-ai-that-learns-without-human-data/) ⭐️ 8.0/10

Ineffable Intelligence, a British AI lab founded a few months ago by former DeepMind researcher David Silver, has raised $1.1 billion in funding at a valuation of $5.1 billion. The company aims to develop AI systems that can learn without human data, a research direction known as self-supervised or zero-data learning. This funding represents one of the largest investments in a single AI research lab focused on alternative learning paradigms beyond traditional supervised learning. If successful, such systems could dramatically reduce dependency on expensive human-annotated datasets and potentially discover solutions humans have not considered. David Silver previously led DeepMind's AlphaZero project, which achieved superhuman performance in chess, shogi, and Go using tabula rasa reinforcement learning through self-play. The new lab will build on this foundation to develop more general AI systems capable of autonomous learning without human intervention or external supervision.

rss · TechCrunch AI · Apr 27, 17:24

**Background**: Traditional AI models typically require massive amounts of human-labeled data for training, which is expensive and time-consuming to produce. Self-supervised learning is a machine learning technique that uses unsupervised methods to accomplish tasks typical of supervised learning, eliminating the need for labeled data. David Silver's AlphaZero demonstrated that systems can learn complex tasks purely through self-play and reinforcement learning, starting from scratch without any human knowledge.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/self-supervised-learning">What Is Self-Supervised Learning? | IBM</a></li>
<li><a href="https://arxiv.org/html/2406.00606v2">LLMs Could Autonomously Learn Without External Supervision</a></li>
<li><a href="https://en.wikipedia.org/wiki/AlphaZero">AlphaZero - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI_Research`, `#Funding`, `#DeepMind`, `#Machine_Learning`, `#David_Silver`

---

<a id="item-9"></a>
## [Google Employees Urge Pichai to Block Pentagon AI Access](https://www.theverge.com/ai-artificial-intelligence/919326/google-ai-pentagon-classified-letter) ⭐️ 8.0/10

Over 600 Google employees, including staff from the DeepMind AI lab and more than 20 senior leaders (principals, directors, and vice presidents), signed a letter to CEO Sundar Pichai demanding that Google block the Pentagon from accessing its AI models for classified military purposes. This protest represents a significant escalation in tech employee activism, as it involves senior leadership beyond individual contributors, signaling deep institutional concerns about the ethical implications of military AI applications. The organizers specifically claim that DeepMind staff are heavily represented among the signatories, indicating that Google's premier AI research division has serious reservations about the classified military use of its technology.

rss · The Verge AI · Apr 27, 18:17

**Background**: This letter echoes earlier controversies at Google, notably the 2018 Project Maven protest where employees successfully pushed back against a Pentagon AI contract for drone footage analysis. Following that backlash, Google established AI ethics principles and declined to renew the contract. DeepMind was formed as a separate AI research unit with explicit commitments to responsible AI development, making their staff involvement in this protest particularly notable.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/">Google DeepMind</a></li>
<li><a href="https://www.youtube.com/watch?v=1XF-NG_35NE">What's next for AI at DeepMind , Google 's artificial intelligence lab</a></li>

</ul>
</details>

**Discussion**: No community comments were provided in the source material.

**Tags**: `#ai-ethics`, `#corporate-responsibility`, `#employee-activism`, `#google-deepmind`, `#military-ai`

---

<a id="item-10"></a>
## [Xiaomi Xuanjie O1 Chip Shipments Exceed 1 Million Units](https://weibo.com/1997509257/5292279283585125) ⭐️ 8.0/10

At Xiaomi Investor Day on April 27, Lei Jun announced that the company's self-developed 3nm Xuanjie O1 chip has shipped over 1 million units, with plans to expand self-developed chips to Xiaomi's automotive business. This marks a significant milestone for China's semiconductor industry, demonstrating that Xiaomi has become one of the few Chinese companies capable of designing and manufacturing advanced 3nm chips. The over $2 billion R&D investment and 10-year, $7 billion commitment signal serious long-term strategic intent in competing with global chip giants. The Xuanjie O1 uses TSMC's second-generation 3nm (N3E) process with 19 billion transistors, the same process used in Qualcomm Snapdragon 8 Elite, MediaTek Dimensity 9400, and Apple A18 Pro. The chip debuted in Xiaomi 15S Pro and high-end tablets. R&D investment reached 13.5 billion yuan by April 2025, with a planned 10-year investment of at least 50 billion yuan.

telegram · zaihuapd · Apr 27, 05:50

**Background**: The 3nm process represents the most advanced semiconductor manufacturing node currently in mass production for smartphone chips. Xuanjie O1 is the first system-on-chip designed by a Chinese company using second-generation 3nm technology, marking a breakthrough in China's ability to develop high-end mobile processors. Prior to this, Chinese smartphone chips lagged behind global leaders in advanced process technology.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/玄戒">玄戒 - 维基百科，自由的百科全书</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1913543324637329084">破而后立，一鸣惊人！——小米玄戒O1芯片（小米15S Pro）详细评测 - 知乎</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#China tech`, `#Xiaomi`, `#3nm chip`, `#EV chips`

---

<a id="item-11"></a>
## [Scientists Achieve Record High-Harmonic Generation Near Schwinger Limit](https://www.nature.com/articles/s41586-026-10400-2) ⭐️ 8.0/10

Physicists used the Gemini laser system with dual plasma mirrors to achieve record high-harmonic conversion efficiency, reducing the rise time to approximately 351 femtoseconds and generating over 9 mJ of energy in the 12th to 47th order harmonics. This breakthrough creates the strongest coherent light in a laboratory setting and brings light intensity close to the Schwinger limit (10²⁹ W/cm²), enabling new research into quantum vacuum behavior and strong-field quantum electrodynamics that was previously impossible. The experiment achieved high-harmonic conversion efficiency that closely matches theoretical predictions by precisely controlling the contrast of femtosecond laser pulses at the sub-picosecond scale. This confirms that the essential elements for Coherent Harmonic Focusing (CHF) are now complete.

telegram · zaihuapd · Apr 27, 16:00

**Background**: High-harmonic generation (HHG) is a nonlinear optical process where materials exposed to intense laser pulses emit high-order harmonics of the driving laser light. The Schwinger limit (施温格极限) is a theoretical threshold in quantum electrodynamics above which electromagnetic fields become nonlinear, causing the vacuum to exhibit nonlinear properties. This limit represents one of the most extreme conditions in physics and has never been reached in laboratory experiments until now.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Schwinger_limit">Schwinger limit - Wikipedia</a></li>
<li><a href="https://zh.wikipedia.org/zh-cn/高次諧波產生">高次谐波产生 - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**Tags**: `#laser_physics`, `#quantum_electrodynamics`, `#high_harmonic_generation`, `#extreme_light`, `#Schwinger_limit`

---

<a id="item-12"></a>
## [SVG Sanitization Vulnerabilities: Scratch XSS Case Study](https://muffin.ink/blog/scratch-svg-sanitization/) ⭐️ 7.0/10

A security researcher published a deep-dive analysis documenting an XSS vulnerability in Scratch's SVG sanitization and demonstrating why regex-based fixes are fundamentally inadequate for preventing malicious SVG exploits. This case demonstrates a common pitfall in web security: using regex to sanitize complex markup like SVG is prone to bypasses. The discussion highlights that proper solutions like Content Security Policy (CSP) are essential, and raises ethical questions about responsible disclosure practices. The Scratch vulnerability involved XSS through SVG uploads that could execute arbitrary JavaScript in users' browsers. While Scratch attempted a regex-based fix, researchers demonstrated it could be bypassed. DOMPurify and similar dedicated sanitization libraries represent proper solutions, but CSP provides the most robust defense.

hackernews · varun_ch · Apr 27, 15:31

**Background**: SVG (Scalable Vector Graphics) is an XML-based image format that supports embedded JavaScript and event handlers, making it a potential vector for cross-site scripting (XSS) attacks when uploaded to web applications. XSS attacks allow attackers to execute malicious scripts in victims' browsers, potentially stealing session cookies or performing actions on behalf of users. Content Security Policy (CSP) is an HTTP header that tells browsers which resources a page can load, providing defense-in-depth against XSS.

<details><summary>References</summary>
<ul>
<li><a href="https://dompurify.com/">DOMPurify – Fast & Secure XSS Sanitizer for HTML</a></li>
<li><a href="https://portswigger.net/web-security/cross-site-scripting/contexts/lab-some-svg-markup-allowed">Lab: Reflected XSS with some SVG markup allowed | Web Security Academy</a></li>
<li><a href="https://rietta.com/blog/svg-xss-injection-attacks/">Cross-site Scripting Injection Attacks Using SVG Images</a></li>

</ul>
</details>

**Discussion**: Commenters praised CSP as the proper solution, with simonw noting CSP can be set directly in HTML via meta tags. andybak suggested supporting only a safe subset of SVG. nmilo criticized Scratch for using regex sanitization and questioned whether proper responsible disclosure was followed. Others discussed the need for sandbox attributes to isolate SVG content.

**Tags**: `#security`, `#svg`, `#xss`, `#web-security`, `#sanitization`

---

<a id="item-13"></a>
## [China Blocks Meta's Acquisition of AI Startup Manus](https://www.cnbc.com/2026/04/27/meta-manus-china-blocks-acquisition-ai-startup.html) ⭐️ 7.0/10

China blocked Meta's planned acquisition of AI startup Manus, invoking export control laws to prevent the deal involving the Singapore-based company. The acquisition, announced in December 2025, was valued at approximately $2-3 billion according to media reports. This decision signals China's willingness to enforce strict controls over AI technology originating within its borders, even when companies relocate to jurisdictions like Singapore to avoid regulations. It establishes a precedent that echoes the TikTok regulatory saga, potentially affecting how international AI acquisitions involving Chinese-origin technology are structured. Manus had relocated to Singapore after closing a $75 million fundraising round led by US venture firm Benchmark in May 2025, shutting down its China operations and laying off dozens of employees. China reportedly cited Article 12 (catch-all provisions) of its Export Control Law and offshore affiliate rules to justify blocking the acquisition, with Manus's co-founders reportedly under investigation for allegedly violating export control and national security laws.

hackernews · yakkomajuri · Apr 27, 11:43

**Background**: China's Export Control Law, enacted in 2020 and expanded since then, grants authorities broad authority to regulate the export of sensitive technologies, including certain AI-related intellectual property. A key provision known as the "catch-all clause" allows regulators to control exports not explicitly listed if they determine the technology could threaten national security. Singapore has become a popular jurisdiction for Chinese tech companies seeking a neutral base for international operations, but China's updated regulations have sought to close what some call the "Singapore loophole."

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Manus_(AI_agent)">Manus (AI agent) - Wikipedia</a></li>
<li><a href="https://www.kingandwood.com/us/en/insights/latest-thinking/chinas-technology-import-export-control-a-crucial-compliance-landscape.html">China’s Technology Import/Export Control: A Crucial ...</a></li>
<li><a href="https://fdichina.com/blog/blog-china-export-restrictions-12-rules-2025/">China Export Restrictions: 12 Essential Rules & 5 Costly ...</a></li>

</ul>
</details>

**Discussion**: Community members noted the irony that much of the world's AI advancement owes a debt to Meta and Google's open-source releases, including Llama. Commenters observed that China is essentially applying the same logic as US export controls—asserting the right to control domestically-originated algorithms. There was discussion about how breaking Singapore's status as a regulatory fig leaf could create problematic precedents, and skepticism about how China would actually unwind a completed transaction.

**Tags**: `#AI regulation`, `#China-US tech relations`, `#Meta`, `#export controls`, `#geopolitics`

---

<a id="item-14"></a>
## [Super ZSNES: GPU-Powered SNES Emulator Project](https://zsnes.com/) ⭐️ 7.0/10

Super ZSNES is a newly announced GPU-accelerated SNES emulator project that offloads rendering tasks to the GPU, using parallel processing to handle what the original SNES Picture Processing Unit (PPU) did on specialized hardware. This represents a significant shift in emulation methodology, potentially offering faster performance and new rendering capabilities for retro gaming. The project has sparked genuine technical debate about the tradeoffs between accuracy and GPU-based parallel rendering approaches. Community discussions reveal the implementation renders tile-by-tile for backgrounds and OBJ rather than per-pixel state capture. A contributor noted that Mathew Valente (TSSF) spent considerable effort tracking down original synthesizer samples used by Nobuo Uematsu for Final Fantasy music.

hackernews · haunter · Apr 27, 17:50

**Background**: The original SNES console contained two Picture Processing Unit (PPU) chips responsible for generating video output, handling backgrounds, sprites, and color effects. ZSNES was a popular SNES emulator in the late 1990s and early 2000s that helped popularize emulation. GPU-accelerated emulation uses graphics card parallel processing to handle computational tasks that would traditionally run on CPU.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fabiensanglard.net/snes_ppus_how/">How the SNES Graphics System works</a></li>
<li><a href="https://sneslab.net/wiki/PPU_Registers">PPU Registers - SnesLab</a></li>

</ul>
</details>

**Discussion**: Comments show a mix of nostalgia and technical interest, with users discussing childhood memories of ZSNES and debating PPU implementation approaches. One user raised concerns about legally obtaining games, while another praised the audio sample recovery efforts by Mathew Valente. The overall sentiment is positive with genuine technical engagement.

**Tags**: `#emulator`, `#SNES`, `#GPU`, `#retro-gaming`, `#open-source`

---

<a id="item-15"></a>
## [pgBackRest Maintainer Stops Development After 13 Years](https://github.com/pgbackrest/pgbackrest) ⭐️ 7.0/10

The lead maintainer of pgBackRest, a widely-used open-source PostgreSQL backup and restore tool, announced on LinkedIn that they are stopping development after 13 years of work, citing the need for a change after sustained effort. This discontinuation affects many organizations relying on pgBackRest for PostgreSQL backups, raising concerns about the long-term sustainability of critical open-source infrastructure and who will maintain widely-used community projects. pgBackRest supports full, differential, and incremental backups with asynchronous archiving and restore, designed to scale to the largest databases and workloads. The project was partially sponsored by corporate support for much of its 13-year history.

hackernews · c0l0 · Apr 27, 10:56

**Background**: pgBackRest is an open-source backup and restore solution for PostgreSQL that offers reliable backup, restore, and archive functions. It is widely used in production environments and known for handling large databases efficiently. PostgreSQL is one of the most popular open-source relational databases in the world.

<details><summary>References</summary>
<ul>
<li><a href="https://pgbackrest.org/">pgBackRest - Reliable PostgreSQL Backup & Restore</a></li>
<li><a href="https://medium.com/@yaseminbsra.sergen/setting-up-and-using-pgbackrest-with-patroni-7161024cc898">Setting Up and Using pgBackRest with Patroni | by Yasemin... | Medium</a></li>

</ul>
</details>

**Discussion**: The community expressed gratitude for the developer's 13 years of dedication, with some sharing their own guides and positive experiences using pgBackRest. Discussion also focused on open-source sustainability, with suggestions that a for-profit company could potentially take over maintenance of such a widely-used tool.

**Tags**: `#open-source`, `#postgresql`, `#pgbackrest`, `#devops`, `#database`

---

<a id="item-16"></a>
## [Supreme Court Reviews Police Use of Cell Phone Location Data](https://www.nytimes.com/2026/04/27/us/politics/supreme-court-cell-data-geofence.html) ⭐️ 7.0/10

The US Supreme Court is hearing a case on geofence warrants that allow police to obtain cell phone location data from tech companies. Google stopped responding to such warrants last year because it no longer stores user location data centrally—instead keeping it on each user's device. This case could establish critical precedent for Fourth Amendment protections in the digital age. The ruling may determine whether mass location data collection through geofence warrants violates constitutional privacy rights, affecting how law enforcement can track citizens using technology. Google previously stored location data in a database called Sensorvault, which law enforcement used to identify all devices within a specific geographic area during a particular time frame. Beyond Google, law enforcement has also sought geofence data from Apple, Lyft, Snapchat, Uber, Microsoft, and Yahoo.

hackernews · unethical_ban · Apr 27, 15:29

**Background**: A geofence warrant is a reverse location warrant that allows police to request all mobile devices within a specific geographic area during a specific time period. The Fourth Amendment protects against unreasonable searches and seizures, but the third-party doctrine has historically allowed less privacy protection for information shared with third parties. The Supreme Court previously ruled in Carpenter v. United States (2018) that police need a warrant to access historic cell phone location data, but this case may clarify extends to real-time geofence requests.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Geofence_warrant">Geofence warrant</a></li>
<li><a href="https://thehill.com/regulation/court-battles/5848192-geofence-warrants-fourth-amendment-supreme-court/">Geofence warrants case tests Fourth Amendment at Supreme Court</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions—some praise Google's privacy-protective changes, while others criticize the third-party doctrine that allows any shared data to be potentially accessed by government. There's skepticism about judicial impartiality, with concerns that some justices have already made up their minds. Commenters also debate the ethics of comparing digital geofencing to physical surveillance methods.

**Tags**: `#privacy`, `#law`, `#supreme-court`, `#surveillance`, `#geofencing`

---

<a id="item-17"></a>
## [OpenAI Achieves FedRAMP Moderate Authorization for Enterprise Products](https://openai.com/index/openai-available-at-fedramp-moderate) ⭐️ 7.0/10

OpenAI has obtained FedRAMP Moderate authorization for ChatGPT Enterprise and the OpenAI API, enabling secure AI adoption for U.S. federal agencies. This authorization allows federal agencies to legally use OpenAI's enterprise AI tools for sensitive government work, opening a massive market opportunity and setting a precedent for AI governance in the public sector. FedRAMP Moderate requires 325 security controls based on FIPS 199, protecting controlled unclassified information (CUI) with moderate confidentiality, integrity, and availability requirements.

rss · OpenAI News · Apr 27, 14:00

**Background**: FedRAMP (Federal Risk and Authorization Management Program) is a U.S. government program that provides a standardized approach to security assessment and authorization for cloud products. It defines three impact levels (Low, Moderate, High) based on FIPS 199, which categorizes the severity of potential adverse effects if information systems were compromised. Moderate is the most common authorization level for government cloud deployments, requiring significantly more controls than Low.

<details><summary>References</summary>
<ul>
<li><a href="https://www.vanta.com/collection/fedramp/fedramp-moderate">FedRAMP Moderate : Who’s in scope and how to prepare | Vanta</a></li>
<li><a href="https://secureframe.com/hub/fedramp/impact-levels">FedRAMP Levels & Baselines, Explained</a></li>
<li><a href="https://secureframe.com/hub/fedramp/moderate">FedRAMP Moderate : Requirements & How to Prepare</a></li>

</ul>
</details>

**Tags**: `#AI compliance`, `#enterprise AI`, `#government AI`, `#OpenAI`, `#FedRAMP`

---

<a id="item-18"></a>
## [OpenAI Wins AWS Sales Rights From Microsoft in $50B Deal](https://techcrunch.com/2026/04/27/openai-ends-microsoft-legal-peril-over-its-50b-amazon-deal/) ⭐️ 7.0/10

OpenAI has secured concessions from Microsoft that will allow it to sell its products on AWS (Amazon's cloud platform), while Microsoft receives more favorable revenue-sharing terms in a complex three-way deal involving Amazon as well. This deal reshapes competitive dynamics in the AI and cloud services markets. By gaining direct access to AWS's massive customer base, OpenAI can now compete more effectively with other AI providers, while Microsoft secures better financial returns from its significant investment in OpenAI. The deal is valued at approximately $50 billion and represents a significant shift in the AI cloud computing landscape. Microsoft, OpenAI's largest shareholder, had previously restricted the company from directly selling through competing cloud platforms.

rss · TechCrunch AI · Apr 27, 17:40

**Background**: Microsoft has invested approximately $13 billion in OpenAI and has been its exclusive cloud infrastructure partner, providing Azure for running OpenAI's models. The original partnership gave Microsoft exclusive rights to commercialize GPT models through Azure, which created certain restrictions on OpenAI's ability to distribute its products independently.

**Tags**: `#OpenAI`, `#Microsoft`, `#Amazon AWS`, `#AI business`, `#cloud computing`

---

<a id="item-19"></a>
## [Musk vs Altman: OpenAI Mission Trial Begins](https://www.theverge.com/tech/917225/sam-altman-elon-musk-openai-lawsuit) ⭐️ 7.0/10

Elon Musk and Sam Altman are set for a high-stakes trial starting April 27th where Musk's 2024 lawsuit accuses OpenAI of abandoning its founding mission to develop AI for humanity's benefit, with jury selection beginning this week in Northern California. The trial outcome could determine whether OpenAI is allowed to exist as a for-profit enterprise and may even affect leadership, potentially impacting the company's highly anticipated IPO and the future direction of one of the world's most influential AI companies. Musk's lawsuit challenges OpenAI's evolution under Sam Altman, particularly the company's transition from a non-profit research lab to a commercial venture with Microsoft investment. During jury selection, several potential jurors voiced negative views of Musk himself.

rss · The Verge AI · Apr 27, 15:50

**Background**: OpenAI was founded in 2015 as a non-profit AI research company with the mission to ensure artificial intelligence benefits humanity. Musk was an early co-founder but left in 2018. The company later created a for-profit subsidiary and received massive investment from Microsoft, leading to significant changes in its structure and direction.

**Tags**: `#OpenAI`, `#AI Industry`, `#Legal Battle`, `#Elon Musk`, `#Sam Altman`

---

<a id="item-20"></a>
## [Canva Apologizes After AI Tool Replaces 'Palestine' in Designs](https://www.theverge.com/ai-artificial-intelligence/919028/canva-magic-layers-ai-replacing-palestine) ⭐️ 7.0/10

Canva's AI feature Magic Layers was discovered automatically replacing the word 'Palestine' in user designs, making unauthorized content alterations. The company subsequently issued a public apology for the issue. This incident raises serious concerns about AI content manipulation and corporate accountability. Users expect their designs to remain unchanged when using AI tools, but silent content modification based on unknown criteria undermines trust in design platforms. Magic Layers is designed to break flat images into separate editable components, not to alter visible text content. The issue was first discovered and reported by X user @ros_ie9.

rss · The Verge AI · Apr 27, 14:29

**Background**: This case represents a significant AI ethics incident where automated content modification occurred without user consent. Canva marketed Magic Layers as a tool to make designs more editable while maintaining original visual integrity. The silent replacement of specific words raises questions about AI bias and content filtering in design tools.

**Discussion**: The incident sparked discussions about AI content manipulation and corporate responsibility. Many users expressed concern about AI tools making unauthorized changes to their creative work, with some questioning what other words or content might be silently altered.

**Tags**: `#AI ethics`, `#content moderation`, `#Canva`, `#AI bias`, `#technology controversy`

---

<a id="item-21"></a>
## [Rebuilding the Data Stack for AI](https://www.technologyreview.com/2026/04/27/1136322/rebuilding-the-data-stack-for-ai/) ⭐️ 7.0/10

MIT Technology Review Insights reports that enterprises are realizing the biggest obstacle to meaningful AI adoption at scale is their data infrastructure, not the AI models themselves, prompting a widespread rebuild of data stacks. This matters because most enterprises have invested heavily in AI models but neglected the foundational data layer, leaving them unable to deploy AI at scale despite having boardroom buy-in and budget. The technical components of modern AI data infrastructure include data lakehouse architectures (combining data warehouse and data lake capabilities), feature stores for managing ML features, and MLOps pipelines for model deployment and maintenance.

rss · MIT Technology Review · Apr 27, 13:00

**Background**: A data lakehouse is a new architecture that combines the best of data warehouses (structured, optimized for analytics) and data lakes (flexible, for raw data). A feature store is a centralized repository for storing curated features used in machine learning pipelines. MLOps (Machine Learning Operations) refers to practices for deploying and maintaining ML models in production reliably and efficiently. Traditional enterprise data systems were not designed for the demands of AI at scale.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data_warehouse_architectures">Data warehouse architectures</a></li>
<li><a href="https://www.featurestore.org/">Feature Store For ML</a></li>
<li><a href="https://en.wikipedia.org/wiki/MLOps">MLOps - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#enterprise AI`, `#data infrastructure`, `#AI adoption`, `#digital transformation`, `#data stack`

---

<a id="item-22"></a>
## [Google Warns Malicious Web Pages Hijacking Enterprise AI Agents](https://www.artificialintelligence-news.com/news/google-warns-malicious-web-pages-poisoning-ai-agents/) ⭐️ 7.0/10

Google researchers discovered that malicious actors are embedding hidden instructions within standard HTML on public web pages to hijack enterprise AI agents through indirect prompt injection attacks. Security teams scanning the Common Crawl repository—a massive database containing billions of public web pages—uncovered a growing trend of these digital booby traps. This attack vector represents a critical security threat to enterprises deploying AI agents in production environments, as it exploits the inherent behavior of AI agents to browse websites and process web content. Organizations relying on AI agents for automation face risks of data exfiltration, unauthorized code execution, and complete system compromise. The hidden instructions are embedded in HTML in ways that are invisible to human users but can be parsed by AI agents processing web content. According to security researchers, this attack technique has transitioned from theoretical to confirmed exploits over the past twelve months, with documented CVEs showing zero-click remote code execution capabilities through AI coding assistants.

rss · Artificial Intelligence News · Apr 27, 11:12

**Background**: Indirect Prompt Injection (IPI) attacks are a class of threats where adversarial instructions embedded in external content hijack LLM behavior by blending malicious instructions with trusted content. AI agents often rely on web browsing and content retrieval to gather information, making them particularly vulnerable to this attack vector. Common Crawl is a 501(c)(3) non-profit organization that maintains a free, open repository of web crawl data widely used for AI training and research.

<details><summary>References</summary>
<ul>
<li><a href="https://commoncrawl.org/">Common Crawl - Open Repository of Web Crawl Data</a></li>
<li><a href="https://www.emergentmind.com/topics/indirect-prompt-injection-ipi-attacks">Indirect Prompt Injection Attacks</a></li>
<li><a href="https://www.sentinelone.com/cybersecurity-101/cybersecurity/indirect-prompt-injection-attacks/">What is Indirect Prompt Injection ? Risks & Prevention</a></li>

</ul>
</details>

**Discussion**: Security researchers and AI practitioners have expressed significant concern about this attack vector, with many noting that traditional web security measures designed for human users do not adequately protect AI agents. The community is actively discussing potential mitigation strategies, including content sanitization, sandboxing, and implementing stricter trust boundaries for AI agent operations.

**Tags**: `#AI security`, `#prompt injection`, `#enterprise AI`, `#cybersecurity`, `#AI agents`

---

<a id="item-23"></a>
## [AlphaGo Creator David Silver Launches $1.1B Superlearner AI Company](https://www.wired.com/story/david-silver-ai-ineffable-intelligence-reinforcement-learning/) ⭐️ 7.0/10

David Silver, the lead researcher behind AlphaGo, has founded Ineffable Intelligence, a new British AI lab that has raised $1.1 billion in funding at a $5.1 billion valuation. He publicly criticizes the current trajectory of AI development and aims to build AI 'superlearners' that learn through interaction with environments rather than relying on vast datasets of human-annotated examples. This represents a significant challenge to the prevailing approach in AI development, coming from one of the most accomplished researchers in the field. Silver's $1.1 billion funding and his critique suggest there may be fundamental limitations in current AI paradigms that rely heavily on human data and reinforcement learning from human feedback. Ineffable Intelligence's approach centers on self-supervised learning techniques, where AI systems develop capabilities through environmental interaction rather than learning from vast collections of human-annotated examples. This represents a fundamentally different paradigm from the data-intensive approaches currently dominating the AI industry.

rss · Hacker News - AI / LLM / Agent · Apr 28, 00:35

**Background**: David Silver led the DeepMind team that created AlphaGo, the first AI to defeat a professional human player in Go. AlphaGo's breakthrough used deep reinforcement learning combined with tree search. Self-supervised learning differs from traditional supervised learning by allowing AI to learn from raw data without human-labeled annotations, potentially reducing the massive human effort currently required for training large language models.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/04/27/deepminds-david-silver-just-raised-1-1b-to-build-an-ai-that-learns-without-human-data/">DeepMind's David Silver just raised $1.1B to build an AI that ...</a></li>
<li><a href="https://www.aibusinessreview.org/2026/04/27/david-silver-raises-1-1-billion-self-learning-ai/">David Silver Raises $1.1B for Self-Learning AI</a></li>

</ul>
</details>

**Tags**: `#AI Research`, `#DeepMind`, `#Reinforcement Learning`, `#AlphaGo`, `#AI Industry`

---

<a id="item-24"></a>
## [Developer Shares 3-Month ChatGPT App Review Journey](https://news.ycombinator.com/item?id=47923382) ⭐️ 7.0/10

A developer built a ChatGPT fitness app called Tredict in just 2 weeks of coding, but spent 3 months going through OpenAI's review process before it was approved and listed in the ChatGPT App Directory. This case provides rare insight into the actual OpenAI app submission timeline and compliance requirements. The 3-month review duration and the need to remove certain features to stay within OpenAI's fitness/health guidelines are valuable learnings for other developers planning to submit ChatGPT apps. The app uses MCP UI Apps with interactive widgets rather than just tools, rendering actual activity data and workout plans inside the chat. Getting user-authenticated content into sandboxed iframes was the hardest technical challenge, as the iframe has no access to OAuth tokens. ChatGPT also has a more limited context window compared to Claude for multi-week training plan creation.

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Apr 27, 16:05

**Background**: OpenAI launched the ChatGPT App Directory in December, allowing third-party developers to submit apps. The directory works similar to an app store, letting users browse and install ChatGPT-integrated applications. OpenAI maintains fitness/health guidelines that apps must follow, and the review process ensures compliance. MCP (Model Context Protocol) is an open protocol enabling AI models to connect with external tools and services.

<details><summary>References</summary>
<ul>
<li><a href="https://help.openai.com/en/articles/11487775-connectors-in-chatgpt">Apps in ChatGPT | OpenAI Help Center</a></li>
<li><a href="https://indianexpress.com/article/technology/artificial-intelligence/chatgpt-app-store-directory-third-party-services-how-to-use-10428147/">ChatGPT gets an app store-style directory , bringing third - party apps ...</a></li>

</ul>
</details>

**Tags**: `#ChatGPT`, `#OpenAI`, `#App Development`, `#Fitness Tech`, `#Developer Experience`

---

<a id="item-25"></a>
## [Moore Threads Reports 86%+ R&D Investment, Deploys 10K-GPU Cluster](https://www.infoq.cn/article/GitNHq2Sa7K34WjiqmNq?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Moore Threads released its latest financial report showing that over 86% of its investment is allocated to R&D, and announced the successful deployment of a 万卡 (ten thousand GPU) scale AI computing cluster, marking a significant milestone in China's domestic AI infrastructure. This development represents significant progress in China's push for AI chip self-sufficiency amid US technology restrictions. The successful deployment of a 10,000-GPU cluster demonstrates Moore Threads' capability to build large-scale AI computing infrastructure domestically, reducing reliance on foreign chips and competing with global leaders like Nvidia. According to the financial report, Moore Threads continues to prioritize R&D with over 86% investment ratio. The deployed ten-thousand-GPU cluster is the first physically realized domestically-produced 'ten thousand card' AI cluster system in China, representing a monumental leap in AI infrastructure capabilities.

rss · InfoQ 中文站 · Apr 27, 15:32

**Background**: Moore Threads Technology Co. Ltd was founded in October 2020, specializing in graphics processing unit (GPU) design. The company is dedicated to providing advanced infrastructure and one-stop solutions for accelerated computing, enabling digital transformation across various industries. The '万卡' (ten thousand GPU) cluster concept represents a new generation of AI infrastructure in China, marking the industry's transition from traditional computing to AI-powered digital transformation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Moore_Threads">Moore Threads - Wikipedia</a></li>
<li><a href="https://freshfromchina.com/chinas-ai-supercluster-scalex-ten-thousand-card-system-redefines-ai-computing-power/">China’s AI Supercluster: ScaleX “Ten Thousand Card” System ...</a></li>
<li><a href="https://en.mthreads.com/about">About Us | Moore Threads</a></li>

</ul>
</details>

**Tags**: `#AI基础设施`, `#GPU计算`, `#中国芯片`, `#摩尔线程`, `#智算集群`

---

<a id="item-26"></a>
## [When Cloud Regions Fail: HA Architecture for Geopolitical Risks](https://www.infoq.cn/article/5qXyqHdrXhaT7iEr24l6?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

InfoQ published an article discussing high-availability architecture strategies when cloud regions become unavailable due to geopolitical instability, addressing critical infrastructure planning for multi-region cloud deployments. This topic matters because geopolitical tensions can suddenly make cloud regions inaccessible or force data sovereignty compliance, directly impacting business continuity for organizations with global cloud deployments. The article explores strategies including Active-Active and Active-Passive architectures, geo-redundancy deployment across politically diverse regions, and disaster recovery planning to maintain service availability when entire cloud regions fail.

rss · InfoQ 中文站 · Apr 27, 13:00

**Background**: Cloud providers organize services into geographic regions, each with independent infrastructure. When geopolitical events cause region-level failures—such as sanctions, regulations, or infrastructure seizures—engineering teams need pre-planned strategies. Geo-redundancy distributes workloads across regions in different political jurisdictions to mitigate single-point failures.

<details><summary>References</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/azure/well-architected/reliability/redundancy">Architecture Strategies for Designing for Redundancy ...</a></li>
<li><a href="https://www.cisco.com/c/en/us/td/docs/wireless/ucc/cpc/cnaaa/2026-02/geo-redundancy/cpc-geo-redundancy-guide-2026-02-0/m-pre-requisites-and-ip-allocation.html">UCC CPC AAA Geo Redundancy Guide, Release 2026.02.0</a></li>

</ul>
</details>

**Tags**: `#cloud-infrastructure`, `#high-availability`, `#disaster-recovery`, `#geopolitical-risk`, `#cloud-architecture`

---

<a id="item-27"></a>
## [Xiaomi Open-Sources MiMo-V2.5 Series AI Models Under MIT License](https://x.com/XiaomiMiMo/status/2048821516079661561) ⭐️ 7.0/10

Xiaomi has officially open-sourced its MiMo-V2.5 series models under the MIT license, enabling royalty-free commercial deployment, continued training, and fine-tuning. The series includes two models: MiMo-V2.5-Pro, optimized for complex Agent and code tasks, and MiMo-V2.5, a native full-modal model with strong Agent capabilities. The release positions Xiaomi competitively against other open-source AI providers, with MiMo-V2.5-Pro achieving first-place rankings on GDPVal-AA and ClawEval benchmarks among open-source models. This commercial-friendly licensing could accelerate enterprise AI adoption and foster broader ecosystem innovation. Both models support up to 1 million token context windows, enabling long-document processing and extended conversations. MiMo-V2.5-Pro specializes in complex agentic workflows and coding tasks, while MiMo-V2.5 provides balanced native full-modal capabilities for diverse applications.

telegram · zaihuapd · Apr 28, 00:27

**Background**: GDPVal-AA is an evaluation framework by Artificial Analysis that tests AI models on economically valuable knowledge work across 44 occupations and 9 major industries, using Elo scoring derived from blind pairwise comparisons. ClawEval is an end-to-end benchmark for real-world agent workflows, assessing capabilities in tool use, planning, execution, and recovery. Both benchmarks are independent evaluations that provide rigorous assessments of AI model performance in practical applications.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/evaluations/gdpval-aa">GDPval-AA Leaderboard | Artificial Analysis</a></li>
<li><a href="https://claw-eval.github.io/">Claw-Eval: A Transparent Benchmark for Real-World Agents</a></li>
<li><a href="https://llm-stats.com/benchmarks/gdpval-aa">GDPval-AA Leaderboard</a></li>

</ul>
</details>

**Tags**: `#Xiaomi`, `#MiMo`, `#open-source AI`, `#multi-modal models`, `#LLM release`

---