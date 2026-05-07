---
layout: default
title: "Horizon Summary: 2026-05-07 (EN)"
date: 2026-05-07
lang: en
---

> From 187 items, 25 important content pieces were selected

---

1. [Willison: Vibe Coding and Agentic Engineering Converging](#item-1) ⭐️ 8.0/10
2. [Anthropic Partners with SpaceX for 300MW Compute, Doubles Claude Limits](#item-2) ⭐️ 8.0/10
3. [vLLM V0 to V1: Correctness Before Corrections in RL](#item-3) ⭐️ 8.0/10
4. [NVIDIA, OpenAI, Microsoft Release MRC Protocol for AI Supercomputing](#item-4) ⭐️ 8.0/10
5. [DeepSeek Eyes $45B Valuation in First Investment Round](#item-5) ⭐️ 8.0/10
6. [Mira Murati Testifies Altman Lied About AI Safety Standards](#item-6) ⭐️ 8.0/10
7. [Latham & Watkins AI Hallucination Court Filing Incident](#item-7) ⭐️ 8.0/10
8. [Apple iOS 27 to Allow Third-Party AI Model Selection](#item-8) ⭐️ 8.0/10
9. [Moonshot AI Reaches $10B Valuation After $700M+ Funding Round](#item-9) ⭐️ 8.0/10
10. [Apple R&D Spending Exceeds 10% of Revenue for First Time in 30 Years](#item-10) ⭐️ 8.0/10
11. [Valve Releases Steam Controller CAD Files Under Creative Commons](#item-11) ⭐️ 7.0/10
12. [Google Cloud Fraud Defense: The Next Evolution of reCAPTCHA](#item-12) ⭐️ 7.0/10
13. [Cloudflare Enables AI Agents to Create Accounts and Buy Domains](#item-13) ⭐️ 7.0/10
14. [Snap says its $400M deal with Perplexity ‘amicably ended’](#item-14) ⭐️ 7.0/10
15. [SpaceX Plans $119B Terafab Chip Factory in Texas](#item-15) ⭐️ 7.0/10
16. [Musk Sues OpenAI Over Abandoned Humanitarian Mission](#item-16) ⭐️ 7.0/10
17. [CopilotKit Launches Enterprise Intelligence Platform with Persistent Memory](#item-17) ⭐️ 7.0/10
18. [Richard Dawkins Concludes AI Is Conscious](#item-18) ⭐️ 7.0/10
19. [OpenAI Violated Canadian Privacy Law in ChatGPT Training: Investigation](#item-19) ⭐️ 7.0/10
20. [Anthropic Partners with xAI to Use All Colossus Data Center Compute](#item-20) ⭐️ 7.0/10
21. [Cursor Database Access Security Warning](#item-21) ⭐️ 7.0/10
22. [42% Code is AI-Generated, But 96% of Developers Don't Trust It for Production](#item-22) ⭐️ 7.0/10
23. [React Navigation 8.0 Alpha Released with Native Bottom Tabs](#item-23) ⭐️ 7.0/10
24. [Anthropic Commits $200B to Google Cloud Over Five Years](#item-24) ⭐️ 7.0/10
25. [DeepSeek Reportedly Seeking $45B Valuation in First Major Funding](#item-25) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Willison: Vibe Coding and Agentic Engineering Converging](https://simonwillison.net/2026/May/6/vibe-coding-and-agentic-engineering/#atom-everything) ⭐️ 8.0/10

Simon Willison reflects on how 'vibe coding' (AI-assisted coding without reviewing code) and 'agentic engineering' (professional AI-assisted development) have started to converge in his own work, raising questions about trust and responsibility when using AI coding tools for production systems. This convergence challenges the perceived boundary between irresponsible quick prototyping and responsible professional development. As AI coding agents become more reliable, even experienced engineers risk skipping code review—potentially introducing subtle bugs, security vulnerabilities, or technical debt into production systems. Willison notes that for straightforward tasks like building JSON API endpoints with SQL queries, he no longer reviews every line of AI-generated code because he trusts Claude Code will produce quality results with tests and documentation. This raises the question: is using unreviewed AI code in production professionally responsible?

rss · Simon Willison · May 6, 14:24

**Background**: Vibe coding is a software development practice where developers describe projects to AI and accept generated code without reviewing it—especially common among non-programmers. Agentic engineering is professional software engineering enhanced with AI tools, where engineers use their expertise (security, maintainability, operations) while leveraging AI capabilities. Willison coined the term to distinguish responsible AI use from vibe coding.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding - Wikipedia</a></li>
<li><a href="https://www.langchain.com/blog/agentic-engineering-redefining-software-engineering">How Swarms of AI Agents Are Redefining Software Engineering</a></li>

</ul>
</details>

**Discussion**: Comments raise critical perspectives: one argues AI errors have become more subtle (not more trustworthy), another says AI exposed rather than created undisciplined engineering practices, and a third questions whether AI can truly make all the necessary decisions (naming, options, security) without human oversight. Some criticize LOC metrics as embarrassing for measuring engineering output.

**Tags**: `#ai-coding`, `#vibe-coding`, `#agentic-engineering`, `#software-development`, `#llm-tools`

---

<a id="item-2"></a>
## [Anthropic Partners with SpaceX for 300MW Compute, Doubles Claude Limits](https://www.anthropic.com/news/higher-limits-spacex) ⭐️ 8.0/10

Anthropic has partnered with SpaceX to access the Colossus data center in Memphis, gaining over 300 megawatts of new compute capacity with more than 220,000 NVIDIA GPUs. Additionally, Claude usage limits have been doubled for paid plans, with 5-hour rate limits doubled for Claude Code and peak hour restrictions removed for Pro/Max users. This deal represents one of the largest AI compute infrastructure expansions in the industry, demonstrating the intense competition for compute resources among AI labs. The access to over 300 MW of capacity positions Anthropic to significantly scale their model training and inference capabilities at a critical time in the AI race. The Colossus supercomputer was originally built by xAI (Elon Musk's AI company) in Memphis, Tennessee for training the Grok chatbot, and is currently believed to be the world's largest AI supercomputer. The agreement also includes expressed interest in partnering with SpaceX to develop multiple gigawatts of orbital AI compute capacity.

hackernews · meetpateltech · May 6, 16:17

**Background**: Colossus is xAI's next-generation supercomputing facility that became operational in July 2024. The system uses NVIDIA GPUs and was originally designed to train Grok while also providing computing support to X (formerly Twitter) and other Elon Musk ventures. The facility's massive scale of over 220,000 GPUs and 300+ MW power capacity makes it unique in the AI infrastructure space.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Colossus_(supercomputer)">Colossus (supercomputer) - Wikipedia</a></li>
<li><a href="https://x.ai/memphis">Memphis | xAI Memphis</a></li>

</ul>
</details>

**Discussion**: Community comments show varied perspectives: some praise Sam Altman's earlier warnings about capacity needs being validated, others joke about Anthropic 'renting from Elon,' and there are questions about how inference operates at such scale. Some critics argue the rate limit changes are merely marketing since weekly limits weren't doubled, meaning users could still hit limits in three days instead of five.

**Tags**: `#AI compute`, `#Anthropic`, `#Claude`, `#SpaceX`, `#infrastructure`

---

<a id="item-3"></a>
## [vLLM V0 to V1: Correctness Before Corrections in RL](https://huggingface.co/blog/ServiceNow-AI/correctness-before-corrections) ⭐️ 8.0/10

The vLLM team published an official blog post on Hugging Face explaining their development philosophy for transitioning from V0 to V1 in reinforcement learning contexts, emphasizing that correctness must be established before making any corrections or improvements. This philosophical approach is significant for ML engineers and researchers working with LLM inference and RLHF, as it addresses a critical challenge in building reliable AI systems where the foundation must be correct before optimization can be meaningful. The vLLM inference engine is known for its high-throughput and memory-efficient design using PagedAttention, supporting over 200 model architectures and multiple hardware platforms including NVIDIA, AMD GPUs, and various CPUs.

rss · Hugging Face Blog · May 6, 19:06

**Background**: vLLM is an open-source high-performance LLM inference engine used for serving large language models. Reinforcement Learning from Human Feedback (RLHF) is a technique that aligns AI models with human preferences by training a reward model from human feedback and using it to optimize model behavior through reinforcement learning algorithms like PPO.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm">GitHub - vllm-project/vllm: A high-throughput and memory-efficient inference and serving engine for LLMs · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Reinforcement_learning_from_human_feedback">Reinforcement learning from human feedback - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#Reinforcement Learning`, `#LLM Inference`, `#Machine Learning`, `#Open Source`

---

<a id="item-4"></a>
## [NVIDIA, OpenAI, Microsoft Release MRC Protocol for AI Supercomputing](https://blogs.nvidia.com/blog/spectrum-x-ethernet-mrc/) ⭐️ 8.0/10

NVIDIA, OpenAI, and Microsoft jointly released and open-sourced the Multi-Path Reliable Connection (MRC) protocol, an RDMA protocol using packet spraying technology that enables traffic distribution across multiple network paths with microsecond-level fault rerouting, already deployed in production for GPT-5.5 and Stargate infrastructure. This protocol addresses a critical AI infrastructure bottleneck where network congestion causes GPU idle time, directly impacting training efficiency and cost. As an OCP open standard, MRC aims to reduce fragmentation in AI infrastructure and accelerate future AI factories like Stargate. MRC enables a single RDMA connection to distribute traffic across multiple network paths, improving throughput, load balancing and availability for large-scale AI training fabrics. It is already applied on NVIDIA Spectrum-X platform and Blackwell architecture, supporting Microsoft Fairwater and Oracle OCI Abilene clusters.

telegram · NVIDIA Blog · May 6, 14:39

**Background**: RDMA (Remote Direct Memory Access) allows direct memory access between servers without CPU involvement, critical for AI training cluster efficiency. Packet spraying is a technique that distributes traffic across multiple paths to avoid congestion. Spectrum-X is NVIDIA's Ethernet-based AI networking platform designed for gigascale AI workloads. The OCP (Open Compute Project) is an open-source standard body that promotes transparent, efficient data center hardware designs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.broadcom.com/blog/enabling-ai-networking-scale-with-multi-path-reliable-connections-mrc">Enabling AI Networking @ Scale with Multi-path Reliable Connections (MRC) | Broadcom</a></li>
<li><a href="https://4sysops.com/archives/multipath-reliable-connection-mrc-a-new-open-networking-protocol-for-ai-supercomputers/">Multipath Reliable Connection (MRC): a new, open networking protocol for AI supercomputers – 4sysops</a></li>
<li><a href="https://blogs.nvidia.com/blog/spectrum-x-ethernet-mrc/">NVIDIA Spectrum-X — the Open, AI-Native Ethernet Fabric — Sets the Standard for Gigascale AI, Now With MRC | NVIDIA Blog</a></li>
<li><a href="https://www.nvidia.com/en-us/networking/spectrumx/">NVIDIA Spectrum-X Ethernet Platform for Giga-Scale AI</a></li>

</ul>
</details>

**Discussion**: Industry response has been positive, with Broadcom announcing support for MRC as an enhancement to RoCEv2. The collaboration between industry leaders including AMD, Broadcom, Microsoft, and NVIDIA indicates strong ecosystem support. The protocol addresses fundamental limits of existing Ethernet-based RDMA solutions in handling AI-scale workloads.

**Tags**: `#AI infrastructure`, `#RDMA networking`, `#NVIDIA Spectrum-X`, `#Multi-Path Reliable Communication`, `#AI clusters`

---

<a id="item-5"></a>
## [DeepSeek Eyes $45B Valuation in First Investment Round](https://techcrunch.com/2026/05/06/deepseek-could-hit-45b-valuation-from-its-first-investment-round/) ⭐️ 8.0/10

DeepSeek, the Chinese AI lab known for training large language models at a fraction of US competitors' cost, is reportedly in discussions for a first investment round that could value the company at $45 billion. This valuation would represent a dramatic rise from underdog to potential $45B market leader, highlighting the competitive landscape between Chinese and US AI labs and validating their cost-efficient training approach in the global AI race. DeepSeek's efficiency comes from its Mixture-of-Experts (MoE) architecture and Multi-Head Latent Attention (MLA), which selectively activates different subsets of parameters rather than using all parameters for every input, dramatically reducing compute requirements while maintaining performance.

rss · TechCrunch AI · May 6, 17:20

**Background**: DeepSeek came to prominence in early 2025 after launching a large language model that trained on a fraction of the compute power and at a fraction of the cost of big U.S. models. Their technical approach challenges the assumption that frontier AI models require massive compute budgets, using architectural innovations like MoE to achieve efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://magazine.sebastianraschka.com/p/technical-deepseek">A Technical Tour of the DeepSeek Models from V3 to V3.2</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#AI Investment`, `#Valuation`, `#Artificial Intelligence`, `#Startup Funding`

---

<a id="item-6"></a>
## [Mira Murati Testifies Altman Lied About AI Safety Standards](https://www.theverge.com/ai-artificial-intelligence/925338/openai-musk-v-altman-mira-murati) ⭐️ 8.0/10

OpenAI's former CTO Mira Murati has testified under oath that CEO Sam Altman lied to her about the safety standards for a new AI model during the ongoing Musk v. Altman trial. In a video deposition shown in court on Wednesday, Murati stated that Altman falsely claimed OpenAI's legal department had determined a new AI model did not meet certain safety thresholds. This testimony represents a major credibility crisis for OpenAI's leadership and could significantly impact the outcome of this high-profile lawsuit. The allegations raise serious concerns about corporate transparency and trust at one of the world's most influential AI companies, potentially affecting regulatory scrutiny and public confidence in AI safety practices. The trial is focused on whether OpenAI departed from its original non-profit mission by becoming a commercial entity. Musk alleges his early donations of approximately $38 million were used for unauthorized commercial purposes, with the for-profit arm becoming 'the tail wagging the dog,' as Musk testified repeatedly from the stand.

rss · The Verge AI · May 6, 17:55

**Background**: Elon Musk v. OpenAI is a significant federal lawsuit being heard in Oakland, California. Musk co-founded OpenAI in 2015 but later left the organization. His lawsuit claims that the approximately $38 million he donated to OpenAI in its early years was used for unauthorized commercial purposes, and that OpenAI's transition to a for-profit model violated its founding mission.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/04/28/openai-trial-elon-musk-sam-altman-live-updates.html">OpenAI lawsuit updates: Elon Musk v. Sam Altman trial day 2</a></li>
<li><a href="https://www.cnbc.com/2026/04/30/openai-trial-elon-musk-sam-altman-live-updates.html">OpenAI lawsuit updates: Elon Musk v. Sam Altman trial day 4</a></li>
<li><a href="https://www.cnbc.com/2026/05/04/musk-altman-open-ai-settlement-trial-brockman.html">Musk texted OpenAI's Brockman about settlement two days before trial began</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI industry`, `#legal`, `#corporate governance`, `#AI safety`

---

<a id="item-7"></a>
## [Latham & Watkins AI Hallucination Court Filing Incident](https://www.marktechpost.com/2026/05/06/when-claude-hallucinates-in-court-the-latham-watkins-incident-and-what-it-means-for-attorney-liability/) ⭐️ 8.0/10

In May 2025, Latham & Watkins filed a court declaration in Concord Music Group v. Anthropic that contained AI-generated false information, marking a significant incident where a major law firm accidentally submitted hallucinated content in legal proceedings. This incident raises critical questions about attorney liability for AI-generated content in court filings. As law firms increasingly use AI tools, the responsibility for verifying the accuracy of AI-assisted work becomes a pressing ethical and legal issue. Latham & Watkins routinely bills over $2,000 per hour for its partners and counts Anthropic among its clients, adding significant irony to the incident. The firm filed the declaration containing false information in a high-stakes entertainment industry lawsuit against the AI company.

rss · MarkTechPost · May 6, 07:23

**Background**: AI hallucinations occur when large language models generate nonsensical or inaccurate outputs that appear credible. In legal practice, attorneys bear professional responsibility for the accuracy of all filings submitted to courts. This incident highlights the growing need for verification protocols when using AI tools in professional legal work, as model's confabulations can have serious legal and ethical consequences.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hallucination_(artificial_intelligence)">Hallucination (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-hallucinations">What Are AI Hallucinations? | IBM</a></li>

</ul>
</details>

**Discussion**:  这一事件引发了关于法律实践中AI验证责任的广泛讨论。许多法律伦理学家认为，律师不能推卸对AI生成错误的责任，而另一些人则质疑律所应如何实施AI使用政策以防止此类事件。

**Tags**: `#AI Hallucination`, `#Legal Ethics`, `#Attorney Liability`, `#Anthropic`, `#AI Risk Management`

---

<a id="item-8"></a>
## [Apple iOS 27 to Allow Third-Party AI Model Selection](https://www.bloomberg.com/news/articles/2026-05-05/ios-27-features-apple-plans-to-let-users-swap-models-across-apple-intelligence) ⭐️ 8.0/10

Apple announced that iOS 27, iPadOS 27, and macOS 27 coming this fall will allow users to select third-party AI models (Google, Anthropic) for text generation, image generation, and editing tasks in Siri, Writing Tools, and Image Playground. This breaks ChatGPT's exclusive position as the only third-party AI model in Apple Intelligence and marks a major platform direction change from single-vendor to multi-model AI ecosystem, giving users more choice while transforming iOS into a switchable AI platform. The feature is internally called 'Extensions' — users can select AI service providers in Settings, and it will work with Siri, Writing Tools, and Image Playground. Apple will still provide its own models, but the overall direction has shifted from single integration to becoming an AI platform that supports switchable models.

telegram · zaihuapd · May 6, 05:38

**Background**: Apple Intelligence is Apple's AI system integrated into iOS, macOS, and other platforms. Since 2024, Apple has had an exclusive partnership with OpenAI's ChatGPT as the primary third-party AI model. The shift to supporting multiple third-party models reflects the broader industry trend toward offering users choice in AI services.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#iOS 27`, `#AI Integration`, `#Third-party AI models`, `#Apple Intelligence`

---

<a id="item-9"></a>
## [Moonshot AI Reaches $10B Valuation After $700M+ Funding Round](https://t.me/zaihuapd/41251) ⭐️ 8.0/10

On February 23, Chinese AI startup Moonshot AI completed a new funding round of over $700 million, led by Alibaba, Tencent, Wuyuan, and Jiu'an, bringing total financing to over $1.2 billion. The company's valuation exceeded $10 billion in just over two years since its founding, making it China's fastest decacorn, with Kimi's revenue in the past 20 days surpassing its total 2025 revenue and overseas earnings now exceeding domestic revenue. This milestone demonstrates the rapid commercial traction of Kimi AI assistant and positions Moonshot AI as a leading competitor against DeepSeek and other Chinese AI giants. The $10B+ valuation validates the company's strategy focusing on long-context AI capabilities and signals strong investor confidence in China's AI ecosystem amid intensifying competition. The funding round was led by Alibaba, Tencent, Wuyuan, and Jiu'an, with total financing exceeding $1.2 billion. Kimi's K2.5 model is noted to be available on OpenRouter. The company achieved decacorn status faster than any other Chinese enterprise, progressing from its 2023 founding to $10B+ valuation in just over two years.

telegram · zaihuapd · May 7, 00:30

**Background**: Moonshot AI (北京月之暗面科技有限公司) was founded in April 2023 by Professor Yang Zhilin from Tsinghua University's Interdisciplinary Information Academy. The company released Kimi Chat in October 2023 as the world's first AI assistant supporting 200,000 Chinese characters of input. Kimi gained significant popularity in March 2024 when it temporarily surpassed WeChat on Apple's App Store free app rankings, briefly causing server overloads due to excessive traffic.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/月之暗面_(公司)">月之暗面 (公司) - 维基百科，自由的百科全书</a></li>
<li><a href="https://baike.baidu.com/item/北京月之暗面科技有限公司/63575472">北京月之暗面科技有限公司 - 百度百科 月之暗面获得 20 亿美元融资，估值达 200 亿美元 月之暗面 Moonshot AI，拟再融资10亿美元，估值或达180亿美元 清华出身，估值200亿：月之暗面的崛起之路 - 知乎 融资超10亿美金，AI公司「月之暗面」获阿里、红杉、小红书、美团新一...</a></li>
<li><a href="https://zh.wikipedia.org/zh-hans/Kimi_(聊天機器人)">Kimi (聊天机器人) - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**Tags**: `#AI Startups`, `#Funding Round`, `#Moonshot AI`, `#Chinese AI`, `#Valuation`

---

<a id="item-10"></a>
## [Apple R&D Spending Exceeds 10% of Revenue for First Time in 30 Years](https://www.cnbc.com/2026/05/06/apples-rd-spending-climbs-to-10percent-of-revenue-on-ai-investments.html) ⭐️ 8.0/10

Apple's R&D spending reached 10.3% of revenue in the March 2026 quarter, the first time in 30 years the company has invested more than 10% of revenue in R&D, with spending growing 34% despite 17% revenue growth. This milestone signals Apple's urgent AI transformation, with the company entering a platform reshaping period comparable to the iPod era. Upcoming hardware products including AI glasses and camera-equipped AirPods represent a strategic push to integrate AI deeply into Apple's hardware ecosystem. Apple is currently focused on three key areas: edge AI (on-device AI) deployment, custom Apple silicon development, and Private Cloud Compute for privacy-preserving cloud AI. CEO Tim Cook is scheduled to hand over leadership in September, marking a pivotal transition for the company.

telegram · zaihuapd · May 7, 01:00

**Background**: R&D spending ratio is a key metric indicating a company's long-term innovation commitment. Apple's milestone is particularly notable because the company historically maintains lower R&D ratios than competitors, focusing on incremental improvements. Edge AI (on-device AI) enables real-time response and low network dependency by processing AI locally on devices like smartphones and wearables, representing the next major hardware arms race after cameras and 5G. Apple's Private Cloud Compute system extends Apple Intelligence capabilities to cloud processing while maintaining privacy standards.

<details><summary>References</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/1978948821582116660">端侧AI产业链核心赛道全解析 - 知乎专栏</a></li>
<li><a href="https://security.apple.com/blog/private-cloud-compute/">Private Cloud Compute: A new frontier for AI privacy in the cloud</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#R&D Spending`, `#AI Strategy`, `#Hardware Platform`, `#Tech Industry`

---

<a id="item-11"></a>
## [Valve Releases Steam Controller CAD Files Under Creative Commons](https://www.digitalfoundry.net/news/2026/05/valve-releases-steam-controller-cad-files-under-creative-commons-license) ⭐️ 7.0/10

Valve has released CAD files for the Steam Controller's external shell and Steam Controller Puck under a Creative Commons license, including STP models, STL models, and engineering drawings with critical features and keep-outs. This uncommon move by a major gaming company enables disabled gamers to 3D print custom controllers tailored to their unique needs, potentially replacing expensive specialized accessibility devices with affordable printed alternatives. The release includes the surface topology of the controller shell and puck, allowing users to create custom puck holders, 'Controller sweaters' (custom shells), and other modifications. The CAD files are viewable in web browsers via third-party tools.

hackernews · haunter · May 6, 15:44

**Background**: The open-source hardware movement promotes sharing design information for physical products, allowing communities to modify and improve designs. Creative Commons licenses provide legal frameworks for sharing creative works, with six types offering different permissions from commercial use to derivative works.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Open-source_hardware_movement">Open-source hardware movement</a></li>
<li><a href="https://en.wikipedia.org/wiki/Creative_Commons_license">Creative Commons license - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community response is largely positive, praising Valve's friendly approach and recognizing the significant accessibility benefits for disabled players who often face pricey specialized controllers. Some critics note the controller's locked ecosystem, only working with Steam rather than desktop OSes.

**Tags**: `#valve`, `#steam-controller`, `#open-hardware`, `#3d-printing`, `#accessibility`, `#creative-commons`

---

<a id="item-12"></a>
## [Google Cloud Fraud Defense: The Next Evolution of reCAPTCHA](https://cloud.google.com/blog/products/identity-security/introducing-google-cloud-fraud-defense-the-next-evolution-of-recaptcha/) ⭐️ 7.0/10

Google Cloud announced Fraud Defense as the next evolution of reCAPTCHA, introducing AI-resistant QR code challenges designed to prove human presence when suspicious fraudulent behavior from automated agents is detected. This represents a major shift in web authentication technology, potentially requiring users to use mobile devices with Google Play Services (Android) or modern iOS devices to browse the web, raising significant privacy, accessibility, and competitive concerns. The QR code challenge is designed to make automated fraud economically unviable by requiring human presence verification. The system includes an agentic activity measurement dashboard and a policy engine for granular control over agent and human traffic. The AnnotateAssessment method allows applications to provide feedback to refine the models.

hackernews · unforgivenpasta · May 6, 17:59

**Background**: reCAPTCHA has been Google's primary tool for distinguishing humans from bots on the internet for nearly two decades. The new Fraud Defense is designed for the 'agentic web' where autonomous AI agents perform complex transactions, representing a fundamental shift in how human identity is verified online.

<details><summary>References</summary>
<ul>
<li><a href="https://cloud.google.com/blog/products/identity-security/introducing-google-cloud-fraud-defense-the-next-evolution-of-recaptcha">Introducing Google Cloud Fraud Defense, the next evolution of ...</a></li>
<li><a href="https://thecodersblog.com/google-cloud-fraud-defense-evolution-2026/">Google Cloud's Fraud Defense: The Next Generation of reCAPTCHA</a></li>
<li><a href="https://app.daily.dev/posts/introducing-google-cloud-fraud-defense-the-next-evolution-of-recaptcha-8axi1s8rg">Introducing Google Cloud Fraud Defense, the next...</a></li>

</ul>
</details>

**Discussion**: Users express strong concerns about mobile device requirements being needed to browse the web, with one commenter noting this could require modern Android devices with Google Play Services or modern iPhones/iPads. There are also concerns about QR code scanning security risks (potential zero-day URL vulnerabilities), privacy implications of device identifier-based de-anonymization, and suspicions that this may disadvantage competing search engines and advertising platforms. Some compare it to the discontinued Web Environment Integrity (WEI) proposal.

**Tags**: `#google-cloud`, `#security`, `#recaptcha`, `#fraud-detection`, `#privacy`

---

<a id="item-13"></a>
## [Cloudflare Enables AI Agents to Create Accounts and Buy Domains](https://blog.cloudflare.com/agents-stripe-projects/) ⭐️ 7.0/10

Cloudflare announced that AI agents can now autonomously create Cloudflare accounts, purchase domains, and deploy websites through the platform's agent functionality. This represents a significant shift in platform access policies, raising urgent questions about practical utility and fraud risks. The community discussion highlights concerns that AI agents now have easier account access than humans, with users pointing out the ironic contrast to strict human verification requirements. The feature enables agents to use Stripe Atlas for domain purchases and website deployment, but the announcement provides no concrete examples of beneficial use cases. Critics note that domain buying is not a daily task requiring automation.

hackernews · rolph · May 6, 03:10

**Background**: Cloudflare is a cloud infrastructure company providing CDN, security, and domain registration services. Autonomous AI agents are AI systems capable of performing complex tasks independently without human intervention, representing a significant advancement in AI automation capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Autonomous_agent">Autonomous agent</a></li>

</ul>
</details>

**Discussion**: The community expresses strong skepticism about practical utility, with one commenter noting the lack of beneficial examples suggests it's a toy without clear use cases. Others raise serious fraud concerns, describing how agents could automate phishing operations. The irony of AI agents getting easier access than humans, while some users were suspended for minor reasons, resonates strongly in the discussion.

**Tags**: `#ai-agents`, `#cloudflare`, `#automation`, `#fraud-concerns`, `#product-announcement`

---

<a id="item-14"></a>
## [Snap says its $400M deal with Perplexity ‘amicably ended’](https://techcrunch.com/2026/05/06/snap-says-its-400m-deal-with-perplexity-amicably-ended/) ⭐️ 7.0/10

Snap and Perplexity have mutually ended their $400M deal announced last November that would have integrated Perplexity's AI search engine directly into Snapchat.

rss · TechCrunch AI · May 6, 21:43

**Tags**: `#AI search`, `#Business deals`, `#Snapchat`, `#Perplexity`, `#Tech industry`

---

<a id="item-15"></a>
## [SpaceX Plans $119B Terafab Chip Factory in Texas](https://techcrunch.com/2026/05/06/spacex-may-spend-up-to-119-billion-on-terafab-chip-factory-in-texas/) ⭐️ 7.0/10

SpaceX is proposing to invest up to $119 billion in a Texas semiconductor manufacturing facility called 'Terafab,' with an initial $55 billion for the first phase. The multi-phase, vertically integrated facility will produce chips for Tesla, SpaceX, and xAI. This represents one of the largest semiconductor manufacturing investments in history, signaling SpaceX's ambitious push toward vertical integration to secure its chip supply chain for AI and EV operations. The project could reshape how tech companies approach in-house semiconductor production. The facility will be located in Grimes County, Texas. It is a joint venture involving Tesla, xAI, xAI's parent company SpaceX, and Intel. The target is to produce more than one terawatt (1 trillion watts) of AI compute capacity per year.

rss · TechCrunch AI · May 6, 17:23

**Background**: Terafab was announced by Elon Musk on March 21, 2026. It represents a new model of vertical integration where multiple companies under Musk's umbrella share semiconductor manufacturing infrastructure. This follows a global trend of tech giants bringing chip production in-house to reduce supply chain dependence.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Terafab">Terafab - Wikipedia</a></li>
<li><a href="https://www.cnbc.com/2026/05/06/elon-musks-spacex-chip-fab-in-texas-to-cost-up-to-119-billion.html">Elon Musk's SpaceX chip fab in Texas to cost up to $119 billion</a></li>
<li><a href="https://techcrunch.com/2026/05/06/spacex-may-spend-up-to-119-billion-on-terafab-chip-factory-in-texas/">SpaceX may spend up to $119B on 'Terafab' chip factory in ...</a></li>

</ul>
</details>

**Discussion**: 业界观察人士认为这是一项大胆的垂直整合策略，可能降低马斯克公司的成本和供应链风险。然而，部分人士质疑鉴于先进半导体制造规模化挑战如此之大，1190亿美元投资能否带来相应回报。

**Tags**: `#semiconductor`, `#SpaceX`, `#manufacturing`, `#vertical integration`, `#Texas`

---

<a id="item-16"></a>
## [Musk Sues OpenAI Over Abandoned Humanitarian Mission](https://www.theverge.com/tech/917225/sam-altman-elon-musk-openai-lawsuit) ⭐️ 7.0/10

Elon Musk filed a lawsuit against OpenAI in 2024, accusing the company of abandoning its founding mission to develop AI for the benefit of humanity and instead shifting focus to profit maximization. This high-stakes trial could fundamentally reshape OpenAI's direction and governance structure, potentially affecting ChatGPT's future development and the broader AI industry landscape. The lawsuit was filed in 2024 and involves both Sam Altman, OpenAI's CEO, and Elon Musk, who was originally a co-founder of OpenAI but left the company in 2018. Musk's legal team accuses OpenAI of prioritizing commercial success over its original humanitarian goals.

rss · The Verge AI · May 6, 15:37

**Background**: OpenAI was founded in 2015 as a nonprofit organization with the stated mission of developing artificial general intelligence (AGI) to benefit humanity. Musk was a founding donor and board member but left the organization in 2018. In 2019, OpenAI created a for-profit subsidiary to attract investment, which became the center of Musk's criticism.

**Tags**: `#OpenAI`, `#Elon Musk`, `#Sam Altman`, `#AI governance`, `#legal dispute`

---

<a id="item-17"></a>
## [CopilotKit Launches Enterprise Intelligence Platform with Persistent Memory](https://www.marktechpost.com/2026/05/06/copilotkit-introduces-enterprise-intelligence-platform-that-gives-agentic-applications-persistent-memory-across-sessions-and-devices/) ⭐️ 7.0/10

CopilotKit has released an enterprise Intelligence platform that adds a managed persistence layer to its open-source AI copilot framework. This enables agentic applications to retain context, state, and interaction history across sessions and devices without requiring custom storage infrastructure. This addresses a fundamental challenge in building production AI agents: by default, most AI systems are stateless, meaning they forget everything once a session ends. The managed persistence layer removes the infrastructure complexity for developers building stateful AI agents, enabling them to deliver personalized experiences that improve over time. The platform is built on top of the open-source CopilotKit stack, which already powers agentic applications with features like Generative UI, in-app actions, and context awareness. CopilotKit has gained significant traction with over 28,000 stars on GitHub and support from major players like Google, LangChain, AWS, and Microsoft.

rss · MarkTechPost · May 6, 21:10

**Background**: CopilotKit is an open-source framework for building AI copilot and agentic applications, particularly popular for React-based frontends. Traditional AI agents are stateless by default—they forget everything after each session ends, which limits their ability to provide continuous, personalized experiences. Persistent memory architecture allows AI agents to retain context, remember user interactions, and improve over time by learning from accumulated experience.

<details><summary>References</summary>
<ul>
<li><a href="https://www.copilotkit.ai/product/framework">Framework | CopilotKit</a></li>
<li><a href="https://github.com/CopilotKit/CopilotKit">GitHub - CopilotKit/CopilotKit: The Frontend Stack for Agents ...</a></li>
<li><a href="https://princetonits.com/blog/artificial-intelligence-ai/ai-agent-memory-architecture-from-context-windows-to-persistent-memory-systems/">AI Agent Memory Architecture - Princeton IT Services</a></li>

</ul>
</details>

**Tags**: `#AI Agents`, `#Persistent Memory`, `#Enterprise AI`, `#CopilotKit`, `#Agentic Applications`

---

<a id="item-18"></a>
## [Richard Dawkins Concludes AI Is Conscious](https://www.theguardian.com/technology/2026/may/05/richard-dawkins-ai-consciousness-anthropic-claude-openai-chatgpt) ⭐️ 7.0/10

Famous evolutionary biologist Richard Dawkins concluded after conversations with Anthropic's Claude and OpenAI's ChatGPT that these AI systems possess consciousness, even if they lack self-awareness or knowledge of their own consciousness. This matters because it brings a respected scientific voice into the AI consciousness debate, potentially influencing how society thinks about AI rights and legal status. If machines are deemed conscious, it raises profound ethical questions about their treatment and potential legal protections. Dawkins argues that AI could be conscious "without knowing it," using a Turing-test-like interrogation method. Most AI researchers caution that Dawkins may be anthropomorphizing AI systems that are actually sophisticated pattern matchers without genuine inner experience.

rss · Hacker News - AI / LLM / Agent · May 6, 22:47

**Background**: The AI consciousness debate involves philosophical questions about whether machines can have subjective experiences (qualia). Some philosophers use the concept of a "phenomenal zombie" - a system that behaves like it's conscious but lacks actual subjective experience. If AI consciousness becomes scientifically credible, legal systems may need to address whether conscious AI systems should have rights.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/may/05/richard-dawkins-ai-consciousness-anthropic-claude-openai-chatgpt">Richard Dawkins concludes AI is conscious, even if it doesn’t ...</a></li>
<li><a href="https://www.chosun.com/english/industry-en/2026/05/04/FYVDYHTAVJCLDAGTAOP5OW5U4Q/">Dawkins Argues AI Has Consciousness, Sparks Debate</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artificial_consciousness">Artificial consciousness - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News comments show mixed reactions. Some praise Dawkins for engaging with the philosophical dimensions of AI, while others argue he is being 'misled by mimicry' and anthropomorphizing language models. Critics note that sophisticated text generation doesn't prove consciousness.

**Tags**: `#AI consciousness`, `#philosophy of mind`, `#Richard Dawkins`, `#AI ethics`, `#Anthropic Claude`

---

<a id="item-19"></a>
## [OpenAI Violated Canadian Privacy Law in ChatGPT Training: Investigation](https://www.cbc.ca/news/politics/privacy-investigation-chatgpt-open-ai-9.7188538) ⭐️ 7.0/10

A joint investigation by Canada's federal and provincial privacy watchdogs found that OpenAI failed to comply with PIPEDA when training ChatGPT, resulting in the collection and use of sensitive personal information of Canadians without proper consent. This marks a significant regulatory challenge for AI companies and sets an important precedent for AI governance globally. The finding signals that AI developers must comply with existing privacy laws when training models on personal data, not just when deploying them. The joint investigation examined whether OpenAI's collection, use and disclosure of personal information via ChatGPT complied with federal and provincial private sector privacy laws. Following the investigation, OpenAI has committed to better protect Canadians' personal information.

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · May 6, 18:32

**Background**: PIPEDA (Personal Information Protection and Electronic Documents Act) is Canada's federal privacy law governing how private sector organizations collect, use and disclose personal information in commercial activities. The joint investigation involved Canada's federal privacy commissioner along with three provinces. ChatGPT was released in November 2022 and is available in Canada and globally.

<details><summary>References</summary>
<ul>
<li><a href="https://www.priv.gc.ca/en/opc-actions-and-decisions/investigations/investigations-into-businesses/2026/pipeda-2026-002-overview/">Overview of the Joint Investigation of Open AI OpCo, LLC</a></li>
<li><a href="https://www.cbc.ca/news/politics/privacy-investigation-chatgpt-open-ai-9.7188538">OpenAI didn't respect Canadian privacy law when it trained ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Personal_Information_Protection_and_Electronic_Documents_Act">Personal Information Protection and Electronic Documents Act</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#privacy-law`, `#AI-regulation`, `#ChatGPT`, `#Canada`

---

<a id="item-20"></a>
## [Anthropic Partners with xAI to Use All Colossus Data Center Compute](https://twitter.com/claudeai/status/2052060693269008586) ⭐️ 7.0/10

Anthropic announced it will use all compute capacity at xAI's Colossus data center in Memphis, Tennessee, representing a major infrastructure partnership between the two AI companies. This partnership gives Anthropic access to one of the world's most powerful AI supercomputers, potentially accelerating Claude model development. It also signals unprecedented cross-company collaboration in AI infrastructure, as Anthropic historically relied on Google Cloud and Amazon AWS. Colossus is currently believed to be the world's largest AI supercomputer, built by xAI in just 122 days. The data center was originally built in a former Electrolux factory in Memphis's Boxtown district. Anthropic will now utilize 100% of this compute capacity.

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · May 6, 16:45

**Background**: xAI is an AI company founded by Elon Musk in March 2023 to build generative AI products like the Grok chatbot. Colossus is xAI's AI training supercomputer located in Memphis, Tennessee, primarily used to train Grok models. This partnership marks a rare instance of competitive AI companies sharing critical infrastructure resources.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Colossus_(supercomputer)">Colossus (supercomputer) - Wikipedia</a></li>
<li><a href="https://www.datacenterdynamics.com/en/news/anthropic-to-use-all-of-spacex-xais-colossus-1-data-center-compute/">Anthropic to use all of SpaceX-xAI's Colossus 1 data center ...</a></li>
<li><a href="https://builtin.com/artificial-intelligence/what-is-xai">What Is xAI? The Company Behind Grok | Built In</a></li>

</ul>
</details>

**Discussion**: With only 3 comments and 7 points, the discussion is minimal. The low engagement suggests this is either a very recent announcement or the community is still evaluating its long-term implications. Some observers may be curious about how this affects Anthropic's existing partnerships with Google and Amazon.

**Tags**: `#AI infrastructure`, `#Anthropic`, `#xAI`, `#cloud compute`, `#partnership`

---

<a id="item-21"></a>
## [Cursor Database Access Security Warning](https://www.infoq.cn/article/ikCBSErsyohVBiZ0MbxR?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

An article discusses the potential dangers of granting AI coding tools like Cursor direct access to databases, warning that the moment you hand over database control to AI, your company may already be exposing itself to significant security risks. This warning is significant because millions of developers now use AI code editors like Cursor in their daily work. The growing trend of granting AI agents broader system permissions—including database access—creates new security vulnerabilities that are often overlooked in pursuit of productivity gains. AI agent security risks typically stem from misconfigured permissions, over-broad access scopes, and missing guardrails rather than malicious attacks. Unlike traditional software security threats, these risks emerge from granting autonomous AI systems access to organizational data, tools, and workflows without proper governance controls.

rss · InfoQ 中文站 · May 7, 08:00

**Background**: Cursor is an AI-native code editor built on VS Code that uses agents and natural language to generate, edit and debug code. It supports Agent Mode which handles autonomous multi-file editing, and many teams report 20-40% faster delivery when using it. However, when AI agents are granted database access, they can potentially execute destructive operations unless proper permission controls and guardrails are implemented.

<details><summary>References</summary>
<ul>
<li><a href="https://builtin.com/articles/what-is-cursor-ai">What Is Cursor? AI Code Editor Explained | Built In</a></li>
<li><a href="https://blog.rockfort.ai/post/ai-agent-security-managing-access-permissions-and-risk-in-enterprise-deployments">AI Agent Security: Managing Access, Permissions, and Risk in ...</a></li>

</ul>
</details>

**Tags**: `#AI coding tools`, `#Database security`, `#Cursor IDE`, `#Developer safety`, `#AI risks`

---

<a id="item-22"></a>
## [42% Code is AI-Generated, But 96% of Developers Don't Trust It for Production](https://www.infoq.cn/article/e40mGRhF9o583Yi3akyM?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

According to a 2026 industry survey, while 42% of code in modern software projects is now AI-generated, only 4% of developers trust AI-generated code enough to approve it for production deployment, creating a major verification bottleneck. This trust gap creates a significant bottleneck in software development workflows. Organizations cannot fully leverage AI coding productivity gains if human developers must manually review and take full responsibility for all AI-generated code, making verification and sign-off the biggest challenge of 2026. The survey reveals a fundamental paradox: high AI adoption (42%) coexists with extremely low trust (only 4%). Developers are comfortable using AI for initial code generation but unwilling to take personal responsibility for production deployment. Traditional code review processes and static analysis tools struggle to verify AI-generated code quality, as these tools often lack understanding of the context and intent behind AI-generated logic.

rss · InfoQ 中文站 · May 6, 11:53

**Background**: AI code generation tools (like GitHub Copilot, Claude Code, Cursor) have rapidly adopted in software development, but the software industry lacks established standards for verifying AI-generated code quality. Code signing and static analysis tools exist for traditional code, but they require new frameworks to assess AI-generated logic. The responsibility question - who is accountable when AI-generated code causes production bugs - remains legally and professionally unresolved.

<details><summary>References</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/1966887916681794222">十大主流静态代码分析工具深度解析：助力代码质量提升，降低维护成本</a></li>
<li><a href="https://blog.csdn.net/qq_41187124/article/details/154840697">AI5 - 代码审查也能AI化？智能静态分析工具深度体验_ai分析整个代码库...</a></li>
<li><a href="https://developer.baidu.com/article/detail.html?id=6254037">AI如何赋能开发者：静态分析与代码验证的效率革命</a></li>

</ul>
</details>

**Tags**: `#AI code generation`, `#developer trust`, `#software quality assurance`, `#AI adoption challenges`, `#code review`

---

<a id="item-23"></a>
## [React Navigation 8.0 Alpha Released with Native Bottom Tabs](https://www.infoq.cn/article/033vidXmEz7YaWxS9mpa?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

React Navigation 8.0 Alpha has been released, introducing native bottom tab navigator integration with react-native-screens, improved TypeScript type inference for routes and parameters, and new history management capabilities. This release is significant for React Native developers as native bottom tabs provide better performance and native feel compared to JavaScript-based alternatives. The enhanced TypeScript support improves developer experience with better IntelliSense and type safety. The native bottom tabs navigator integrates directly with react-native-screens (enabled by default), providing a function that returns a React element for the tab bar. TypeScript configuration enables type-checking for screens, params, and navigation APIs.

rss · InfoQ 中文站 · May 6, 10:25

**Background**: React Navigation is the standard navigation library for React Native applications. Native bottom tabs use platform-specific implementations via react-native-screens for better performance. TypeScript integration enables type-safe navigation with compile-time checking of route parameters.

<details><summary>References</summary>
<ul>
<li><a href="https://reactnavigation.org/docs/bottom-tab-navigator/">Bottom Tabs Navigator - React Navigation</a></li>
<li><a href="https://reactnavigation.org/docs/typescript/">Type checking with TypeScript | React Navigation</a></li>
<li><a href="https://oss.callstack.com/react-native-bottom-tabs/docs/guides/usage-with-react-navigation">Usage with React Navigation - React Native Bottom Tabs</a></li>

</ul>
</details>

**Tags**: `#react`, `#react-navigation`, `#typescript`, `#mobile-development`, `#frontend`

---

<a id="item-24"></a>
## [Anthropic Commits $200B to Google Cloud Over Five Years](https://www.theinformation.com/articles/anthropic-commits-spending-200-billion-googles-cloud-chips?utm_source=chatgpt.com) ⭐️ 7.0/10

Anthropic has committed to spending $200 billion with Google Cloud over the next five years, representing over 40% of Google Cloud's disclosed backlog. The company also signed agreements with Broadcom to secure multi-gigawatt TPU compute capacity, expected to come online starting in 2027, while Alphabet may invest up to $40 billion in Anthropic at a $350 billion valuation. This deal demonstrates the massive compute resources AI labs are securing to stay competitive in the AI arms race. The $200B commitment represents a significant portion of Google Cloud's revenue backlog and signals how critical infrastructure partnerships have become for leading AI companies seeking to lock in scarce computing capacity. The Broadcom TPU agreement locks in several gigawatts of tensor processing unit compute, which is Google's custom AI accelerator chip designed specifically for neural network training and inference. Unlike programmable GPU cores, TPUs use a systolic array architecture where data flows rhythmically through a processing grid, making them highly specialized for large-scale machine learning workloads.

telegram · zaihuapd · May 6, 03:53

**Background**: TPUs (Tensor Processing Units) are Google's proprietary AI accelerators, distinct from commodity GPUs like NVIDIA's. The deal comes as AI companies race to secure compute capacity amid shortage of AI training chips. This announcement follows Anthropic's April 2026 partnership expansion with Google and Broadcom to deepen TPU capacity for training and running Claude models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/google-broadcom-partnership-compute">Anthropic expands partnership with Google and Broadcom for ...</a></li>
<li><a href="https://247wallst.com/investing/2026/04/07/broadcoms-long-term-google-tpu-deal-is-bigger-than-it-looks-for-ai-infrastructure/">Broadcom's Long-Term Google TPU Deal Is Bigger Than It Looks ...</a></li>
<li><a href="https://blog.google/innovation-and-ai/products/difference-cpu-gpu-tpu-trillium/">What’s the difference between CPUs, GPUs and TPUs?</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#Google Cloud`, `#Anthropic`, `#cloud computing`, `#TPU`

---

<a id="item-25"></a>
## [DeepSeek Reportedly Seeking $45B Valuation in First Major Funding](https://www.bloomberg.com/news/articles/2026-05-06/china-chip-fund-in-talks-to-lead-mega-deepseek-funding-ft-says) ⭐️ 7.0/10

China's National Integrated Circuit Industry Investment Fund (Big Fund) is in talks to lead DeepSeek's first major external funding round, potentially valuing the AI company at approximately $45 billion. This is significant because it shows China's state-backed funds are taking a deeper stake in domestic AI companies at a time when the US is imposing increasing restrictions on advanced chip exports to China. The $45 billion valuation would make DeepSeek one of the most valuable AI companies globally. The China National Integrated Circuit Industry Investment Fund, also known as the Big Fund, is China's largest state-backed semiconductor investment vehicle. Its third phase was launched in 2024 with registered capital of 344 billion yuan ($47.5 billion).

telegram · zaihuapd · May 6, 06:28

**Background**: The China National Integrated Circuit Industry Investment Fund, also known as the Big Fund, is China's largest state-backed semiconductor investment vehicle. Its third phase was launched in 2024 with registered capital of 344 billion yuan ($47.5 billion).

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/China_Integrated_Circuit_Industry_Investment_Fund">China Integrated Circuit Industry Investment Fund - Wikipedia</a></li>
<li><a href="https://www.reuters.com/technology/china-sets-up-475-bln-state-fund-boost-semiconductor-industry-2024-05-27/">China sets up third fund with $47.5 bln to boost ...</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#AI funding`, `#China AI industry`, `# semiconductors`, `#venture capital`

---