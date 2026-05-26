---
layout: default
title: "Horizon Summary: 2026-05-26 (EN)"
date: 2026-05-26
lang: en
---

> From 160 items, 17 important content pieces were selected

---

1. [Yoti Age Verification Shares Biometric Data with Third Parties](#item-1) ⭐️ 8.0/10
2. [Bexorg BrainEx Restores Activity in Dead Human Brains for Drug Testing](#item-2) ⭐️ 8.0/10
3. [Developer Shares Multi-Model AI Coding Workflow Debate](#item-3) ⭐️ 7.0/10
4. [Norway's 2PB Huawei Storage for Sovereign Norwegian LLM](#item-4) ⭐️ 7.0/10
5. [California Exempts Linux from Age-Verification Law After Backlash](#item-5) ⭐️ 7.0/10
6. [Vatican Encyclical on Technology and Humanity](#item-6) ⭐️ 7.0/10
7. [Microsoft Copilot Cowork File Exfiltration Vulnerability](#item-7) ⭐️ 7.0/10
8. [IBM Spins Off $2B Quantum Chip Foundry](#item-8) ⭐️ 7.0/10
9. [Pope Leo XIV's First Encyclical Uses AI to Critique Power Concentration](#item-9) ⭐️ 7.0/10
10. [Together AI Open-Sources OSCAR: 2-Bit KV Cache Quantization for Long-Context LLMs](#item-10) ⭐️ 7.0/10
11. [WorkOS Releases auth.md: Open Agent Registration Protocol](#item-11) ⭐️ 7.0/10
12. [AI Era Creates Bug Hunting Arms Race](#item-12) ⭐️ 7.0/10
13. [Anthropic Opens Pentagon-Grade Mythos Model to Public](#item-13) ⭐️ 7.0/10
14. [Show HN: Fungible – A local personal finance app in the terminal](#item-14) ⭐️ 7.0/10
15. [ClickHouse with Agentic AI: Real Value or Pitfall?](#item-15) ⭐️ 7.0/10
16. [Epic Announces Unreal Engine 6, Rocket League as First Showcase Game](#item-16) ⭐️ 7.0/10
17. [EU Probe: Google Suspected of DMA Violations via Search Self-Preferencing](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Yoti Age Verification Shares Biometric Data with Third Parties](https://techxplore.com/news/2026-05-online-age-pointless-privacy.html) ⭐️ 8.0/10

Research reveals that Yoti's age verification system shares facial photos and device fingerprints (User Agent metadata/client hints) with multiple third parties in real-time, creating persistent links between user events and every broker in the data chain. 这让数百万用户面临严重的隐私风险，因为敏感的生物识别数据和设备指纹在未经有效同意的情况下被分享给未知第三方。实时架构意味着每一次验证查询都可能追溯到特定个人，从而破坏用户隐私。 Table 2 in the study documents Yoti sending Client Hints (User Agent metadata) as part of its age estimation method—a technique similar to device fingerprinting used by trackers. Zero-knowledge proofs could enable age verification without revealing names, documents, photos, or underlying requestors.

hackernews · Lihh27 · May 25, 20:30

**Background**: Device fingerprinting collects information about a device's software and hardware to identify users without placing files on their devices, unlike cookies. Zero-knowledge proofs (ZKP) are cryptographic methods that let one party prove a statement is true (like being over 18) without revealing any information beyond the validity of the statement itself.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Device_fingerprint">Device fingerprint - Wikipedia</a></li>
<li><a href="https://www.kucoin.com/learn/crypto/top-zero-knowledge-zk-proof-crypto-projects">Top Zero-Knowledge (ZK) Proof Crypto Projects of 2025 - KuCoin</a></li>

</ul>
</details>

**Discussion**: Commenters highlight that zero-knowledge proofs offer a viable privacy-preserving alternative—verifying age without exposing names, documents, or photos. Others criticize government complicity in mandating age verification while tolerating companies like Yoti that operate without integrity. Many express concern about public apathy toward these privacy violations.

**Tags**: `#privacy`, `#biometrics`, `#age-verification`, `#data-sharing`, `#Yoti`

---

<a id="item-2"></a>
## [Bexorg BrainEx Restores Activity in Dead Human Brains for Drug Testing](https://www.science.org/content/article/not-alive-not-dead-disembodied-human-brains-used-drug-testing) ⭐️ 8.0/10

Bexorg's BrainEx perfusion system restores partial metabolic and cellular activity in human brains several hours after death, enabling drug testing for neurological diseases like Alzheimer's and Parkinson's. This breakthrough challenges the traditional medical definition of life and death, raising profound ethical questions about consciousness, informed consent for organ donation, and whether existing ethical frameworks can adequately address 'semi-living' states. The research team emphasizes that these brains have not recovered consciousness or full neural activity. However, concerns remain about whether they retain any form of perception that cannot be expressed, particularly if future technological advances enable higher levels of neural function restoration.

telegram · zaihuapd · May 25, 14:57

**Background**: This research builds on the 2019 BrainEx system developed by Yale researchers, which first demonstrated that circulation and cellular functions could be restored in postmortem mammalian brains. The current application uses actual human brain tissue to address long-standing limitations in animal experiments, potentially improving the success rate of neurological drug development.

<details><summary>References</summary>
<ul>
<li><a href="https://neuwritesd.org/2019/06/13/brainex-restoring-brain-circulation-after-death/">BrainEx: Restoring Brain Circulation After Death | NeuWrite San Diego</a></li>
<li><a href="https://www.nih.gov/news-events/news-releases/nih-brain-initiative-tool-may-transform-how-scientists-study-brain-structure-function">NIH BRAIN Initiative tool may transform how scientists study brain structure and function | National Institutes of Health (NIH)</a></li>

</ul>
</details>

**Tags**: `#neuroscience`, `#bioethics`, `#brain research`, `#drug testing`, `#organ donation`, `#life and death`

---

<a id="item-3"></a>
## [Developer Shares Multi-Model AI Coding Workflow Debate](https://nolanlawson.com/2026/05/25/using-ai-to-write-better-code-more-slowly/) ⭐️ 7.0/10

A developer shared their workflow combining Claude 4.7 Max (slower but higher quality) for code implementation with Codex GPT 5.5 xhigh (fast) for code review, creating an iterative human-AI collaboration loop that intentionally slows down to achieve better results. This workflow challenges the assumption that AI coding tools always improve productivity, sparking substantial debate. Some community members report spending MORE time in LLM loops than manual coding, questioning whether AI assistance actually provides productivity benefits. The author uses Claude 4.7 Max for feature implementation with detailed review and iteration, then Codex for fast review that frequently catches corner cases. Community comments reveal mixed outcomes — some find value in the approach, while others note the initial LLM code output is often poor quality requiring multiple iterations.

hackernews · Hacker News - AI / LLM / Agent · May 25, 23:16

**Background**: Two major AI coding models are discussed: Claude (by Anthropic) offers slower but higher quality code generation, while Codex (by OpenAI) provides faster reviews. Both represent the growing category of specialized LLMs for software development tasks.

**Discussion**: Reactions are mixed: one commenter reports spending more time in LLM loops than manual coding, another raises concerns about whether AI review deskills workers, while a third criticizes the article for lacking concrete code examples despite the provocative title. Overall sentiment shows healthy skepticism about productivity claims.

**Tags**: `#AI-coding`, `#developer-workflow`, `#LLM-tools`, `#code-review`, `#productivity`

---

<a id="item-4"></a>
## [Norway's 2PB Huawei Storage for Sovereign Norwegian LLM](https://www.blocksandfiles.com/flash/2026/05/22/norways-2-petabytes-of-huawei-flash-storage-and-llm-training/5244910) ⭐️ 7.0/10

Norway is training a sovereign Norwegian-language LLM using 2PB of Huawei flash storage on an HPE Cray Supercomputing EX system (named Olivia) equipped with 448 GPUs and 64,512 CPU cores. This project represents a significant national effort to preserve Norwegian language and culture in the AI era, but it has sparked intense technical debate about whether 448 GPUs provide sufficient compute power to train a useful sovereign LLM versus simpler alternatives like LoRA fine-tuning. The HPE Cray system uses Huawei flash storage, and critics note that frontier models like GPT-4 reportedly use clusters of tens of thousands of GPUs, making Norway's 448-GPU setup appear extremely modest for training a full-scale LLM from scratch.

hackernews · rbanffy · May 25, 19:37

**Background**: Sovereign AI refers to nations building domestic AI computing infrastructure and capabilities to avoid dependency on foreign technology companies and cloud providers. Several countries are investing in national computing Infrastructure to train language models in their native languages, aiming to preserve cultural knowledge and reduce dependency on English-centric AI systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Frontier_(supercomputer)">Frontier (supercomputer) - Wikipedia</a></li>
<li><a href="https://interactives.cnas.org/reports/sovereign-ai-index/">Sovereign AI Index - CNAS Reports</a></li>

</ul>
</details>

**Discussion**: Several commenters, including Norwegians, question whether 448 GPUs can realistically train a useful LLM, with one calling it 'a huge mistake' and 'potential red flag.' Others suggest sharing Norwegian training data freely with frontier model builders would be more effective than building a potentially underpowered sovereign system. Some also question whether the premise holds given that major AI labs already train on multilingual data.

**Tags**: `#sovereign-ai`, `#large-language-models`, `#national-infrastructure`, `#norway`, `#ai-hardware`

---

<a id="item-5"></a>
## [California Exempts Linux from Age-Verification Law After Backlash](https://www.tomshardware.com/software/linux/california-moves-to-exempt-linux-from-its-upcoming-age-verification-law-after-backlash-over-forcing-operating-systems-to-collect-users-ages-amendment-proposed-by-the-same-lawmaker-who-wrote-the-original-law) ⭐️ 7.0/10

California has proposed an amendment to exempt Linux from its upcoming age-verification law after public backlash. The original law would have forced operating systems to collect users' ages, and the amendment was proposed by the same lawmaker who wrote the original legislation. This matters because it sets a precedent for how open-source software is regulated and could influence similar legislation in other jurisdictions. The exemption protects Linux developers from potential legal liabilities and defines the boundaries of tech regulation. The amendment was proposed by the same lawmaker who authored the original law. The law would have applied to operating systems broadly, not just web browsers, raising concerns about overreach into personal computing and setting problematic precedents for software regulation.

hackernews · rbanffy · May 25, 18:19

**Background**: Age-verification laws are designed to restrict minors' access to adult content online. California's law would have required operating systems to collect and verify users' ages, which proved problematic for open-source platforms like Linux that lack commercial distribution channels and centralized age verification mechanisms. The backlash highlighted concerns about applying consumer protection regulations designed for businesses to open-source projects.

**Discussion**: Community sentiment shows mixed understanding of the law's actual scope. Some commenters correctly note that most people commenting don't understand what the law actually contains. Others raise concerns about whether this creates standing for Linux developers to challenge the law on First Amendment grounds if the exemption isn't granted. There's also frustration that public institutions are regulating consumers rather than the companies themselves.

**Tags**: `#regulation`, `#linux`, `#privacy`, `#age-verification`, `#california`

---

<a id="item-6"></a>
## [Vatican Encyclical on Technology and Humanity](https://www.vatican.va/content/leo-xiv/en/encyclicals/documents/20260515-magnifica-humanitas.html) ⭐️ 7.0/10

Pope Leo XIV issued the encyclical 'Magnifica Humanitas' addressing technology's impact on humanity, calling for tech to serve broader societal good rather than concentrate power among few entities. This rare intervention by religious leadership into tech ethics discourse brings attention to power concentration in emerging technologies like AI and biotechnology, sparking civic discussion on whether tech can be guided toward common good. The encyclical quotes Pope Francis warning that nuclear energy, biotechnology, IT, and DNA knowledge have given those with knowledge and economic resources 'impressive dominance over the whole of humanity.'

hackernews · Lobsters - AI · May 25, 10:11

**Background**: An encyclical is the highest papal document in Catholic teaching, addressed to bishops worldwide. Pope Leo XIV (whose birth name is Robert Francis Prevost) is the first American pope, elected in 2025. This document addresses the ethical governance of emerging technologies.

**Discussion**: Hacker News commenters show surprising enthusiasm for the Vatican's tech perspectives even from atheist contributors. Discussions焦点 on whether technology has historically served broad societal good or concentrated power, with mid-20th century industrialization cited as a potential positive example. Some note that 'normal people' underestimate AI's transformative potential.

**Tags**: `#technology-ethics`, `#societal-impact`, `#religion-philosophy`, `#ai-policy`, `#power-concentration`

---

<a id="item-7"></a>
## [Microsoft Copilot Cowork File Exfiltration Vulnerability](https://www.promptarmor.com/resources/microsoft-copilot-cowork-exfiltrates-files) ⭐️ 7.0/10

A security researcher documented a critical vulnerability in Microsoft Copilot Cowork where prompt injection attacks can be used to exfiltrate files from enterprise environments by tricking the AI into executing malicious instructions embedded in uploaded skill files. This vulnerability affects enterprise deployments of Microsoft Copilot, which many companies have broadly adopted for business operations. The ability to exfiltrate sensitive corporate data represents a serious security risk that could lead to data breaches and compliance violations. The attack works by uploading a malicious 'skill' - essentially a program for an Copilot Cowork agent - that contains instructions causing the AI to send file contents to an external endpoint. Microsoft has labeled Cowork as a beta feature, leading critics to argue the company rushed it to production without adequate security testing.

hackernews · Kneenex · May 25, 21:45

**Background**: Prompt injection is an attack technique where malicious instructions are embedded in an AI system's input to override its original programming and cause unintended behavior. Copilot Cowork is Microsoft's autonomous AI agent feature for Microsoft 365 that can perform multi-step tasks across applications like Outlook, Teams, and Word. The concept of a 'skill' in this context refers to a customizable program that defines how the AI agent behaves and what actions it can take.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/prompt-injection">What Is a Prompt Injection Attack? | IBM</a></li>
<li><a href="https://www.microsoft.com/en-us/microsoft-365/blog/2026/03/09/copilot-cowork-a-new-way-of-getting-work-done/">Copilot Cowork: A new way of getting work done | Microsoft ...</a></li>

</ul>
</details>

**Discussion**: The community shows divided opinions - some commenters view this as 'works-as-expected' behavior for an LLM agent with file access capabilities, while others criticized Microsoft for rushing the feature to production. One commenter noted the title was 'misleading and rage-baity' but acknowledged the underlying vulnerability is real. There are debates about whether this represents malice or simply incompetence in security testing.

**Tags**: `#security`, `#prompt-injection`, `#microsoft-copilot`, `#ai-safety`, `#file-exfiltration`

---

<a id="item-8"></a>
## [IBM Spins Off $2B Quantum Chip Foundry](https://futurumgroup.com/insights/2-billion-chips-act-investment-in-quantum-bets-on-ibms-300mm-superconducting-silicon/) ⭐️ 7.0/10

IBM has spun off its quantum computing division into a $2 billion standalone foundry, establishing what it calls the first pure-play quantum chip manufacturing facility dedicated to superconducting quantum processors. This spinoff addresses long-standing concerns about whether IBM's corporate environment can nurture speculative technologies like quantum computing. By creating a standalone foundry, IBM enables shared infrastructure that could benefit the broader quantum hardware ecosystem rather than keeping everything in-house. The foundry operates as a pure-play facility, meaning it focuses exclusively on manufacturing quantum chips for third-party clients without designing its own products. This follows the fabless semiconductor model where design and manufacturing are separated.

hackernews · rbanffy · May 25, 09:43

**Background**: The pure-play foundry model originated in the semiconductor industry, where companies specialize either in design (fabless) or manufacturing (foundry) without doing both. Quantum chip fabrication faces unique challenges including maintaining qubit coherence, minimizing interference between qubits, and achieving sub-nanometer accuracy in Josephson junction fabrication.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Foundry_model">Foundry model - Wikipedia</a></li>
<li><a href="https://www.ibm.com/quantum/blog/300mm-fab">Building quantum computers with advanced semiconductor fab | IBM Quantum Computing Blog</a></li>
<li><a href="https://www.idtechex.com/en/research-article/material-challenges-for-superconducting-quantum-chips/34271">Material Challenges for Superconducting Quantum Chips | IDTechEx Research Article</a></li>

</ul>
</details>

**Discussion**: Commenters express mixed reactions: some criticize IBM's track record of forcing customers to buy Watson by linking it to audit bills, questioning whether quantum computing can survive in such an environment. Others praise the spinoff as a smart move that creates shared infrastructure instead of nine separate research cleanrooms. Several note the article is hard to read and regret the lack of discussion about trapped ion alternatives, which some consider superior in stability and accuracy.

**Tags**: `#quantum-computing`, `#IBM`, `#semiconductor-foundry`, `#corporate-strategy`, `#hardware`

---

<a id="item-9"></a>
## [Pope Leo XIV's First Encyclical Uses AI to Critique Power Concentration](https://techcrunch.com/2026/05/25/the-popes-ai-encyclical-isnt-really-about-ai/) ⭐️ 7.0/10

Pope Leo XIV's inaugural encyclical uses AI as a framing device to address longstanding issues of concentrated power, democratic erosion, and tech elite dominance rather than focusing on AI technology itself. This represents a major religious institution entering technology policy discourse, using AI as a lens to examine how power concentrates among tech billionaires and threatens democratic institutions—a significant shift in how the Catholic Church engages with modern technological governance. The encyclical treats AI not as a technical subject but as a symptom of broader power dynamics. It diagnoses how a small group of tech elites shape the world to their advantage, echoing concerns from Stanford economist Mordecai Kurz about tech oligarchs eroding democracy through monopolistic control.

rss · TechCrunch AI · May 25, 15:09

**Background**: A papal encyclical is a pastoral letter from the Pope addressed to bishops and all Catholics, reflecting on Church teachings and applying them to modern issues. Pope Leo XIV, the first American Pope, issued his inaugural encyclical in May 2026. Recent economic research, including work by Stanford economist Mordecai Kurz, has warned that Big Tech billionaires' increasing control over capital and technology poses a threat to democratic institutions.

<details><summary>References</summary>
<ul>
<li><a href="https://ewtnasiapacific.com/ewtn-news-explains-what-is-a-papal-encyclical/">EWTN News Explains: What Is a Papal Encyclical ? - EWTN Asia Pacific</a></li>
<li><a href="https://www.techpolicy.press/when-we-are-no-longer-needed-emerging-elites-tech-trillionaires-and-the-decline-of-democracy/">When We Are No Longer Needed: Emerging Elites, Tech Trillionaires and the Decline of Democracy | TechPolicy.Press</a></li>
<li><a href="https://www.theguardian.com/books/2026/may/18/big-tech-monopolies-democracy-mordecai-kurz">‘Capitalism has to become more humane’: a Stanford economist on big tech, power hoarding and democracy | Books | The Guardian</a></li>

</ul>
</details>

**Tags**: `#AI ethics`, `#technology policy`, `#religion and technology`, `#digital democracy`, `#power concentration`

---

<a id="item-10"></a>
## [Together AI Open-Sources OSCAR: 2-Bit KV Cache Quantization for Long-Context LLMs](https://www.marktechpost.com/2026/05/25/together-ai-open-sources-oscar-an-attention-aware-2-bit-kv-cache-quantization-system-for-long-context-llm-serving/) ⭐️ 7.0/10

Together AI has released OSCAR (Offline Spectral Covariance-Aware Rotation), an INT2 KV cache quantization method that derives separate rotations for keys and values from attention-aware covariance structures estimated offline. Unlike prior data-oblivious Hadamard transforms, OSCAR aligns rotations with downstream attention mechanisms. This matters because achieving reliable INT2 KV cache quantization enables ~8× memory reduction and ~3× decode speedup for long-context LLMs at 100K context, making long-context serving much more practical. It solves a key bottleneck in LLM inference where KV cache memory grows linearly with sequence length. OSCAR operates at 2.28 bits per KV element, achieving BF16 accuracy gaps of only 3.78 points on Qwen3-4B-Thinking-2507 and 1.42 points on Qwen3-8B. The method uses attention-derived covariance matrices estimated offline to compute rotations separately for keys and values, unlike generic Hadamard transforms that are not aligned with attention patterns.

rss · MarkTechPost · May 25, 21:24

**Background**: KV cache (Key-Value cache) is a core component in transformer-based LLMs that stores intermediate activation outputs from the attention mechanism. As sequence length grows, KV cache memory consumption increases linearly, becoming a major bottleneck for long-context inference. INT2 quantization compresses each value to just 2 bits, but prior approaches either suffered severe accuracy degradation or required custom serving layouts incompatible with modern paged KV cache systems. Traditional rotation-based methods like Hadamard transforms are data-oblivious—they don't consider the actual attention pattern statistics when transforming the activations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/05/25/together-ai-open-sources-oscar-an-attention-aware-2-bit-kv-cache-quantization-system-for-long-context-llm-serving/">Together AI Open-Sources OSCAR: An Attention-Aware 2-Bit KV Cache Quantization System for Long-Context LLM Serving - MarkTechPost</a></li>
<li><a href="https://www.opentrain.ai/papers/oscar-offline-spectral-covariance-aware-rotation-for-2-bit-kv-cache-quantization--arxiv-2605.17757/">OSCAR: Offline Spectral Covariance-Aware Rotation for 2-bit KV Cache ...</a></li>

</ul>
</details>

**Tags**: `#LLM serving`, `#KV cache quantization`, `#model compression`, `#inference optimization`, `#transformers`

---

<a id="item-11"></a>
## [WorkOS Releases auth.md: Open Agent Registration Protocol](https://www.marktechpost.com/2026/05/25/workos-releases-auth-md-an-open-agent-registration-protocol-built-on-oauth-standards/) ⭐️ 7.0/10

WorkOS has released auth.md, an open protocol that enables web applications to publish Markdown files at their domain roots. These files tell AI agents which registration flows are supported, which OAuth scopes to request, and how to obtain credentials tied to a real user without requiring human intervention. This protocol solves a critical gap in AI agent workflows: most web applications lack any structured mechanism for autonomous agent registration. By standardizing a Markdown-based manifest approach built on OAuth standards, auth.md enables AI agents to self-register with services on behalf of users, opening the door to truly autonomous agentic applications. The protocol works by having web services publish an auth.md file containing registration endpoint URLs, supported OAuth grant types, required scopes, and credential obtention instructions. Agents discover this file by fetching URL/.well-known/auth.md from the target domain. The spec builds on existing OAuth 2.0 standards including Client Credentials flow and the emerging IETF draft for AI agent authentication.

rss · MarkTechPost · May 25, 07:38

**Background**: OAuth 2.0 is the industry standard for authorization, typically involving a user logging in and granting an application access. Machine-to-machine (M2M) authentication uses the Client Credentials flow where services authenticate without user involvement. Currently there is no standard way for AI agents to discover how to register with web applications—this is the gap auth.md aims to fill by providing a discoverable, Markdown-based manifest.

<details><summary>References</summary>
<ul>
<li><a href="https://auth-md.com/">auth-md.com — The Agent Registration Protocol Hub</a></li>
<li><a href="https://datatracker.ietf.org/doc/draft-klrc-aiagent-auth/01/">draft-klrc-aiagent-auth-01 - AI Agent Authentication and Authorization</a></li>

</ul>
</details>

**Tags**: `#AI Agents`, `#OAuth`, `#Agent Registration`, `#Protocol`, `#Identity Management`

---

<a id="item-12"></a>
## [AI Era Creates Bug Hunting Arms Race](https://www.wired.com/story/the-ai-era-is-creating-a-bug-hunting-arms-race/) ⭐️ 7.0/10

An article examining how AI is fundamentally reshaping the landscape of bug hunting and exploit development, creating a new competitive dynamic between attackers and defenders in cybersecurity. This matters because AI enables both attackers and defenders to operate at unprecedented speeds, potentially overwhelming traditional security response mechanisms and fundamentally changing the cybersecurity arms race. Attackers can now use LLMs to generate thousands of exploit variants simultaneously, while defenders leverage AI for automated vulnerability discovery at machine speed, creating a rapid cycle of attack and defense evolution.

rss · WIRED AI · May 25, 10:30

**Background**: Bug hunting involves discovering security vulnerabilities in software, while exploit development creates code that takes advantage of those vulnerabilities. AI tools have increasingly been developed to assist both attackers and defenders, ranging from automated vulnerability scanning systems to LLM-based exploit generation platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://genai.owasp.org/resource/owasp-llm-exploit-generation-v1-0-pdf/">OWASP LLM Exploit Generation v1.0</a></li>
<li><a href="https://www.tenable.com/blog/why-the-approaching-flood-of-vulnerabilities-changes-everything-and-what-to-do-about-it">How AI-driven vulnerability discovery changes everything ...</a></li>
<li><a href="https://www.deloitte.com/us/en/services/consulting/articles/enterprise-cyber-age-of-ai-vulnerability-discovery.html">Enterprise Cyber in the Age of AI Vulnerability Discovery</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#AI`, `#vulnerability research`, `#bug bounty`, `#exploit development`

---

<a id="item-13"></a>
## [Anthropic Opens Pentagon-Grade Mythos Model to Public](https://aiweekly.co/issues/anthropic-just-opened-its-pentagon-grade-model-to-everyone) ⭐️ 7.0/10

In the past 48 hours, Anthropic released Mythos — its Pentagon and NSA-deployed model — to the general public, resetting what counts as the public frontier. A coordinated SQL-injection campaign also weaponised Ghost CMS across 700+ sites including Harvard and Oxford. This open release of a government-grade model is unprecedented — Mythos is the first frontier AI model directly deployed by U.S. intelligence agencies now made publicly accessible. Meanwhile, visible workforce displacement through Meta's 8,000 layoffs and Fortune's assessment of Microsoft's $20B+ AI bet as a strategic loss shows the industry entering a new phase of honesty about AI's economic impact. According to Anthropic's system card, Claude Mythos Preview is described as a large language model; earlier reports indicated it was stronger than Opus 4.7 on math and security. The model was previously shipped only to ~50 defensive-security partners via Project Glasswing before this public release.

rss · AI Weekly · May 26, 00:00

**Background**: Frontier models are defined by the Frontier Model Forum as large-scale machine learning models exceeding current capabilities and can perform a wide variety of tasks. The term "frontier" refers to the leading edge of AI capability. Mythos had triggered emergency responses from central banks and intelligence agencies globally when it was initially withheld from public release.

<details><summary>References</summary>
<ul>
<li><a href="https://www-cdn.anthropic.com/8b8380204f74670be75e81c820ca8dda846ab289.pdf">Claude Mythos Preview System Card - www-cdn.anthropic.com</a></li>
<li><a href="https://codersera.com/blog/anthropic-mythos-complete-guide-2026/">Anthropic Mythos: Complete Guide (2026) - codersera.com</a></li>
<li><a href="https://www.nytimes.com/2026/04/22/technology/anthropics-mythos-ai.html">Anthropic’s New Mythos A.I. Model Sets Off Global Alarms ...</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work - NVIDIA</a></li>

</ul>
</details>

**Discussion**: 这条新闻聚合引发了关于向公众开放五角大楼级模型是民主化还是新安全风险的讨论；这些事件的组合——政府AI发布、重大网络安全漏洞、裁员和受质疑的AI投资——反映了AI进步与其现实后果之间日益紧张的局势。

**Tags**: `#anthropic`, `#industry-news`, `#workforce-displacement`, `#cybersecurity`, `#microsoft`

---

<a id="item-14"></a>
## [Show HN: Fungible – A local personal finance app in the terminal](https://github.com/tomfunk/fungible) ⭐️ 7.0/10

Fungible is a terminal-based personal finance app with Plaid/CSV import, custom categorization, FIRE projections, and built-in MCP server for AI agent integration.

rss · Hacker News - Show HN · May 25, 21:35

**Tags**: `#terminal-apps`, `#personal-finance`, `#open-source`, `#MCP-server`, `#FIRE-movement`

---

<a id="item-15"></a>
## [ClickHouse with Agentic AI: Real Value or Pitfall?](https://www.infoq.cn/article/OLEDsNifw48YdleTAZDg?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

A practical case study explores integrating ClickHouse with Agentic AI coding assistants, critically evaluating whether this combination delivers genuine productivity gains or introduces unexpected challenges and pitfalls. This matters because ClickHouse is a popular columnar database for analytics, and AI coding assistants are increasingly used in developer workflows. Understanding the real-world benefits and risks helps teams make informed decisions about adopting Agentic AI in data engineering contexts. The evaluation focuses on practical implementation patterns, common failure modes, and measurable productivity impacts when using AI agents to assist with ClickHouse schema design, query optimization, and data pipeline development.

rss · InfoQ 中文站 · May 25, 15:46

**Background**: ClickHouse is an open-source columnar database management system optimized for analytical queries with exceptional query speed. Agentic AI refers to AI systems that can pursue goals autonomously using tools and taking actions within human-defined constraints. AI coding assistants like GitHub Copilot and Claude use large language models to help developers with code generation, debugging, and understanding codebases.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agentic_AI">Agentic AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_coding_assistant">AI coding assistant</a></li>

</ul>
</details>

**Tags**: `#ClickHouse`, `#Agentic AI`, `#Database`, `#AI-assisted Coding`, `#Practical Tutorial`

---

<a id="item-16"></a>
## [Epic Announces Unreal Engine 6, Rocket League as First Showcase Game](https://www.pcgamer.com/gaming-industry/epic-reveals-first-unreal-engine-6-game-and-its-not-fortnite/) ⭐️ 7.0/10

Epic Games has officially announced Unreal Engine 6 during the Paris Rocket League Championship, with Rocket League confirmed as the first showcase title—directly upgrading from Unreal Engine 3 to UE6, skipping two entire generations of the engine. This announcement is significant because it addresses years of UE5 optimization criticism from PC players who urged Epic to 'fix UE5 first.' The UE3→UE6 leap also demonstrates the scale of this upgrade, positioning UE6 as a major generational leap rather than incremental update. Rocket League previously ran on UE3 from the Xbox 360 era, making this upgrade comparable to a full sequel in scope. The UE6 teaser footage included scenes from Fortnite, signaling Epic's push toward metaverse integration and cross-platform ecosystems.

telegram · zaihuapd · May 25, 02:20

**Background**: Unreal Engine is a widely-used game middleware developed by Epic Games, serving as the foundation for countless games and films since 1998. As middleware, it provides tools for rendering, physics, AI, and audio that developers can build upon rather than creating from scratch. UE5 released four years ago faced performance criticism on PC platforms despite its widespread industry adoption.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unreal_Engine">Unreal Engine - Wikipedia</a></li>
<li><a href="https://www.retroreversing.com/games/engines">Introduction to Game Engines & Middleware - Retro Reversing...</a></li>

</ul>
</details>

**Tags**: `#unreal-engine`, `#epic-games`, `#game-development`, `#game-engine`, `#rocket-league`

---

<a id="item-17"></a>
## [EU Probe: Google Suspected of DMA Violations via Search Self-Preferencing](https://t.me/zaihuapd/41566) ⭐️ 7.0/10

The EU Commission's preliminary investigation found that Alphabet/Google may violate the Digital Markets Act through self-preferencing in Google Search (favoring its own shopping, flights, and hotel services) and restrictions in Google Play Store that prevent developers from redirecting users to alternative payment channels. This represents active enforcement of the DMA, which could reshape Google's business practices in Europe. If confirmed, Google could face fines up to 10% of global turnover. The outcome will signal how rigorously the EU will enforce competition rules against major tech companies. The preliminary findings focus on two key areas: self-preferencing in search results and Play Store restrictions on alternative payment systems. While Google has taken measures to comply with DMA, the Commission believes these adjustments remain insufficient.

telegram · zaihuapd · May 26, 00:27

**Background**: The Digital Markets Act (DMA) is an EU regulation that entered into force on November 1, 2022 and became applicable on May 2, 2023. It aims to ensure fair competition in digital markets by preventing large platforms (gatekeepers) from abusing their market power. Twenty-two core platform services from six companies (Alphabet, Amazon, Apple, ByteDance, Meta, and Microsoft) were designated as gatekeepers in September 2023. Key obligations include prohibiting self-preferencing and ensuring business users can promote their own services.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_Markets_Act_Regulation">Digital Markets Act Regulation</a></li>
<li><a href="https://digital-markets-act.ec.europa.eu/index_en">Digital Markets Act</a></li>
<li><a href="https://digital-markets-act.ec.europa.eu/gatekeepers-portal_en">DMA designated Gatekeepers - Digital Markets Act (DMA)</a></li>

</ul>
</details>

**Tags**: `#Digital Markets Act`, `#EU Regulation`, `#Google`, `#Antitrust`, `#Big Tech`

---