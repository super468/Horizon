---
layout: default
title: "Horizon Summary: 2026-04-04 (EN)"
date: 2026-04-04
lang: en
---

> From 160 items, 24 important content pieces were selected

---

1. [vLLM v0.19.0 Released with Gemma 4 Support and Zero-Bubble Decoding](#item-1) ⭐️ 8.0/10
2. [Anthropic Blocks OpenClaw, Forces Extra Pay for Third-Party Harnesses](#item-2) ⭐️ 8.0/10
3. [Utah Allows AI to Prescribe Psychiatric Drugs Without Doctors](#item-3) ⭐️ 8.0/10
4. [AI Coding Agents Will Automate Zero-Day Discovery](#item-4) ⭐️ 8.0/10
5. [What Makes Open AI Models Succeed: Beyond Benchmarks](#item-5) ⭐️ 8.0/10
6. [KubeVirt v1.8 Brings Multi-Hypervisor and Confidential Computing to Kubernetes](#item-6) ⭐️ 8.0/10
7. [Google Open-Sources Gemma 4 with Mobile Offline Agent Support](#item-7) ⭐️ 8.0/10
8. [China CAC Draft Rules on Digital Virtual Humans, Bans Minor Virtual Companions](#item-8) ⭐️ 8.0/10
9. [Anthropic Launches New PAC Ahead of Midterms](#item-9) ⭐️ 7.0/10
10. [Meta Pauses Work With Mercor After Data Breach](#item-10) ⭐️ 7.0/10
11. [AI-Generated Kernel Security Reports Surge 10x](#item-11) ⭐️ 7.0/10
12. [Linux Kernel Maintainer Reports AI Security Reports Now Genuinely Useful](#item-12) ⭐️ 7.0/10
13. [CSP Meta Tag in Iframe Cannot Be Bypassed by JavaScript](#item-13) ⭐️ 7.0/10
14. [Axios Supply Chain Attack Used Targeted Social Engineering](#item-14) ⭐️ 7.0/10
15. [PyPI Supply Chain Attack Compromises LiteLLM, Steals Sensitive Data](#item-15) ⭐️ 7.0/10
16. [Discord Open-Sources Osprey Security Rules Engine](#item-16) ⭐️ 7.0/10
17. [Cloudflare Deploys Edge-Based API Vulnerability Scanning](#item-17) ⭐️ 7.0/10
18. [Cursor 3: AI Agent-First Unified Development Workspace](#item-18) ⭐️ 7.0/10
19. [Google Vids Integrates Veo 3.1, Free AI Video for All Users](#item-19) ⭐️ 7.0/10
20. [US Humanoid Robots Depend on Chinese Suppliers for Key Components](#item-20) ⭐️ 7.0/10
21. [Adobe Help Desk Breach Exposes 13M Tickets](#item-21) ⭐️ 7.0/10
22. [MIIT Warns of Critical Apple Vulnerabilities Affecting iOS 17.2.1 and Below](#item-22) ⭐️ 7.0/10
23. [LinkedIn Allegedly Scans Browser Extensions, Shares Data with Third Parties](#item-23) ⭐️ 7.0/10
24. [Reverse Engineering Claude Code Signatures Bypasses Bun Dependency](#item-24) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.19.0 Released with Gemma 4 Support and Zero-Bubble Decoding](https://github.com/vllm-project/vllm/releases/tag/v0.19.0) ⭐️ 8.0/10

vLLM v0.19.0 was released with 448 commits from 197 contributors, introducing full Google Gemma 4 architecture support (requires transformers>=5.5.0), zero-bubble async scheduling for speculative decoding, mature Model Runner V2 with piecewise CUDA graphs for pipeline parallelism, ViT full CUDA graph capture, and general CPU KV cache offloading with pluggable cache policy. This release is significant for LLM inference practitioners as it delivers major performance improvements through zero-bubble speculative decoding and piecewise CUDA graphs, while expanding model support to cutting-edge architectures like Gemma 4. The CPU KV cache offloading and DBO generalization provide more flexible deployment options and broader hardware compatibility. Key features include: zero-bubble async scheduling with speculative decoding (#32951), Model Runner V2 gains PP CUDA graphs (#35162) and spec decode rejection sampler (#37238, #37237), ViT full CUDA graph capture (#35963), general CPU KV cache offloading with block-level preemption (#37160, #37874, #34805), DBO generalized to general models (#37926), and NVIDIA B300/GB300 (SM 10.3) support with allreduce fusion enabled by default.

github · khluu · Apr 3, 02:19

**Background**: vLLM is a high-performance inference engine for large language models. Speculative decoding uses a smaller draft model to predict tokens that are verified by a larger model, improving throughput. Piecewise CUDA graphs split model computation into pieces to reduce compilation overhead while maintaining CUDA graph benefits. CPU KV cache offloading allows moving KV cache to CPU memory to support longer sequences or larger models within limited GPU memory. EPLB (Expert Parallel Load Balancer) redistributes expert mappings in MoE models to balance load across expert parallel ranks.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.sglang.io/advanced_features/piecewise_cuda_graph.html">Piecewise CUDA Graph — SGLang</a></li>
<li><a href="https://docs.vllm.ai/en/stable/design/cuda_graphs/">CUDA Graphs - vLLM</a></li>
<li><a href="https://docs.vllm.ai/en/latest/serving/expert_parallel_deployment/">Expert Parallel Deployment - vLLM</a></li>

</ul>
</details>

**Tags**: `#llm-inference`, `#vllm`, `#machine-learning`, `#cuda`, `#speculative-decoding`

---

<a id="item-2"></a>
## [Anthropic Blocks OpenClaw, Forces Extra Pay for Third-Party Harnesses](https://www.theverge.com/ai-artificial-intelligence/907074/anthropic-openclaw-claude-subscription-ban) ⭐️ 8.0/10

Anthropic announced that starting April 4th at 3PM ET, users will no longer be able to use their Claude subscription limits for third-party harnesses like OpenClaw. Instead, users must pay additional pay-as-you-go costs billed separately from their subscription. This policy change significantly impacts developers who rely on third-party harnesses like OpenClaw to automate Claude AI. It represents a notable shift in Anthropic's pricing strategy, potentially affecting the broader AI agent ecosystem and forcing developers to absorb higher costs or seek alternatives. Anthropic is offering a one-time credit equal to the monthly subscription price (redeemable by April 17) and discounts of up to 30% for pre-purchasing usage bundles. The company cites 'outsized strain on our systems' as the reason, stating capacity must be prioritized for core product customers.

rss · The Verge AI · Apr 3, 23:52

**Background**: OpenClaw is an open-source autonomous AI agent framework that acts as a 'harness' — a framework enabling AI models like Claude to operate autonomously for tasks like coding. The term 'harness' in AI refers to tools that structure the environment around AI agents so they can work reliably. Anthropic also released Claude Code Channels, a competing product that lets users message Claude Code directly through Discord or Telegram.

<details><summary>References</summary>
<ul>
<li><a href="https://venturebeat.com/orchestration/anthropic-just-shipped-an-openclaw-killer-called-claude-code-channels">Anthropic just shipped an OpenClaw killer called Claude Code Channels, letting you message it over Telegram and Discord | VentureBeat</a></li>
<li><a href="https://docs.openclaw.ai/tools/acp-agents">ACP Agents - OpenClaw</a></li>
<li><a href="https://github.com/walkinglabs/awesome-harness-engineering">GitHub - walkinglabs/awesome- harness -engineering: Awesome...</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed. Some users understand the economic reasoning — power users of autonomous agents like OpenClaw effectively subsidize their usage through subscription plans. Others see this as a 'structural mismatch' between subscription models designed for human usage versus autonomous agent infrastructure load. Some users are considering switching to alternative AI models due to the increased costs.

**Tags**: `#Anthropic`, `#Claude AI`, `#OpenClaw`, `#AI pricing`, `#AI policy`

---

<a id="item-3"></a>
## [Utah Allows AI to Prescribe Psychiatric Drugs Without Doctors](https://www.theverge.com/ai-artificial-intelligence/906525/ai-chatbot-prescribe-refill-psychiatric-drugs) ⭐️ 8.0/10

Utah has become the second US state to allow an AI system called Doctronic to prescribe and refill psychiatric drugs without direct doctor oversight, marking only the second time in the country that AI has been granted such clinical prescribing authority. This represents a significant regulatory milestone that could set a precedent for AI in healthcare nationwide. While state officials praise it for reducing costs and easing mental health care shortages, physicians are concerned about transparency, patient safety, and the lack of oversight in AI-driven medical decisions. The AI handles prescription renewals only, not initial prescriptions - a human doctor must have originally prescribed the medication. It covers up to 190 commonly prescribed medications but cannot handle drugs requiring blood-test monitoring. In data shared with Utah regulators, Doctronic compared its AI system with human clinicians across 500 urgent care cases.

rss · The Verge AI · Apr 3, 11:43

**Background**: This is only the second instance of AI receiving clinical prescribing authority in the US, following California's earlier approval. The system represents a major shift in how medical authority is delegated, raising questions about AI accountability in high-stakes healthcare decisions. Utah officials argue the pilot could help address the shortage of psychiatric care providers in rural areas.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theverge.com/ai-artificial-intelligence/906525/ai-chatbot-prescribe-refill-psychiatric-drugs">Chatbots are now prescribing psychiatric drugs | The Verge</a></li>
<li><a href="https://www.thewellnesslondon.com/ai-doctor/blog/ai-prescribing-is-here-what-utah-s-doctronic-pilot-means-for-healthcare">AI Prescribing Is Here: What Utah's Doctronic Pilot Means for...</a></li>

</ul>
</details>

**Discussion**: Physicians have expressed significant concerns about the system's opacity, warning that AI-driven prescribing lacks the transparency needed for patient safety. Critics argue that without clear oversight mechanisms, patients could be at risk from algorithmic errors or inappropriate prescriptions. Supporters counter that the system could significantly reduce healthcare costs and improve access to mental health services.

**Tags**: `#AI regulation`, `#healthcare AI`, `#medical AI`, `#AI policy`, `#psychiatric care`

---

<a id="item-4"></a>
## [AI Coding Agents Will Automate Zero-Day Discovery](https://simonwillison.net/2026/Apr/3/vulnerability-research-is-cooked/#atom-everything) ⭐️ 8.0/10

Thomas Ptacek argues that AI coding agents will soon enable automated zero-day discovery by simply pointing agents at source code and typing 'find me zero days', fundamentally changing vulnerability research economics and practice within the next few months. This represents a fundamental paradigm shift in cybersecurity. LLMs can potentially automate most high-impact vulnerability research, making zero-day discovery accessible to anyone with access to frontier AI models and dramatically lowering the barrier to entry for exploit development. LLMs are uniquely suited for vulnerability research because they encode vast knowledge of source code correlations and documented bug classes (stale pointers, integer mishandling, type confusion, allocator grooming) in their weights. They excel at pattern-matching bug classes and constraint-solving for reachability and exploitability, and can run infinite success/failure trials without getting bored.

rss · Simon Willison · Apr 3, 23:59

**Background**: Vulnerability research is the practice of finding security flaws in software that can be exploited. Zero-day vulnerabilities are unknown flaws that have not yet been patched. Traditionally, this required highly skilled security researchers to manually analyze source code. Frontier AI models refer to the latest generation of large language models. The article was inspired by a podcast interview with Nicholas Carlini from Anthropic.

**Discussion**: The original article was discussed on the Security Cryptography Whatever podcast and has been tagged with ai-security-research on Simon Willison's blog, which already contains 11 posts.

**Tags**: `#AI`, `#cybersecurity`, `#vulnerability-research`, `#LLMs`, `#exploit-development`, `#AI-agents`

---

<a id="item-5"></a>
## [What Makes Open AI Models Succeed: Beyond Benchmarks](https://www.interconnects.ai/p/gemma-4-and-what-makes-an-open-model) ⭐️ 8.0/10

AI commentator Nathan Lambert published an analysis arguing that Google Gemma 4's success depends not on benchmark scores but on factors like accessibility, fine-tuning flexibility, and ecosystem support that drive actual model adoption. This analysis matters because it shifts focus from pure performance metrics to the practical elements that determine whether open-weight models achieve real-world impact and developer adoption in an increasingly crowded AI landscape. Gemma 4 was released under a permissive Apache 2.0 license, making it available on Hugging Face, Kaggle, and Ollama for customization on platforms like Google Colab, Vertex AI, or consumer GPUs—features Lambert identifies as key differentiators beyond raw capability.

rss · Interconnects · Apr 3, 16:57

**Background**: The debate between 'open weights' versus 'fully open source' models is central to AI ecosystem discussions. Open weights models like Gemma provide model parameters for inference and fine-tuning but do not disclose training code or datasets, unlike truly open-source alternatives. Google's recent Gemma 4 launch emphasized agentic AI and coding capabilities, positioning the models against Chinese open-weights competitors.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/gemma-4/">Gemma 4: Byte for byte, the most capable open models</a></li>
<li><a href="https://www.theregister.com/2026/04/02/googles_gemma_4_open_weights/">Google battles Chinese open weights models with Gemma 4 • The Register</a></li>
<li><a href="https://ai.google.dev/gemma/docs/core">Gemma 3 model overview | Google AI for Developers</a></li>

</ul>
</details>

**Tags**: `#open-source AI`, `#Gemma`, `#Google AI`, `#model ecosystem`, `#AI strategy`

---

<a id="item-6"></a>
## [KubeVirt v1.8 Brings Multi-Hypervisor and Confidential Computing to Kubernetes](https://www.infoq.cn/article/kwmoqShV5lx0TslYbo3j?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

KubeVirt has released version 1.8, introducing multi-hypervisor support and confidential computing capabilities to the Kubernetes platform. This release significantly expands Kubernetes' virtualization and security capabilities, enabling users to manage virtual machines with different hypervisors while protecting sensitive data during processing. Multi-hypervisor support allows organizations to leverage different virtualization technologies within Kubernetes, while confidential computing protects data-in-use by isolating sensitive information in protected CPU enclaves.

rss · InfoQ 中文站 · Apr 3, 15:00

**Background**: KubeVirt is a virtual machine management add-on for Kubernetes that extends the platform to run and manage VMs alongside containers using the same APIs, tools, and workflows. Confidential computing is a security technology that protects data during processing by encrypting it in memory using CPU enclaves, addressing a gap in traditional data protection which typically only covers data in transit and at rest.

<details><summary>References</summary>
<ul>
<li><a href="https://kubevirt.io/">KubeVirt.io</a></li>
<li><a href="https://cloud.google.com/security/products/confidential-computing">Confidential Computing | Google Cloud</a></li>
<li><a href="https://www.ibm.com/think/topics/confidential-computing">What Is Confidential Computing? | IBM</a></li>

</ul>
</details>

**Tags**: `#Kubernetes`, `#KubeVirt`, `#Virtualization`, `#Confidential Computing`, `#Cloud Native`

---

<a id="item-7"></a>
## [Google Open-Sources Gemma 4 with Mobile Offline Agent Support](https://www.infoq.cn/article/X1c6ZllztrQhGEIoYrBR?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

Google officially released Gemma 4, an open-source AI model optimized for edge devices, featuring mobile offline AI Agent capability and significantly reduced memory footprint, enabling deployment on mainstream smartphones without network connectivity. This release positions Gemma 4 as a direct competitor to Alibaba's Qwen in the open-source model race, marking Google's continued push into the on-device AI frontier. It enables offline, low-latency, high-privacy intelligent interactions on mobile devices. Gemma 4 is developed by Google DeepMind and undergoes strict safety evaluations similar to the proprietary Gemini model. The model is designed for edge computing scenarios, maintaining reasoning capabilities while significantly compressing parameter scale and operational overhead.

rss · InfoQ 中文站 · Apr 3, 14:40

**Background**: Gemma is Google's series of open-source lightweight AI models. The earlier Gemma 3 emphasized efficiency, running on a single GPU or TPU, even on phones. Mobile-Agent refers to AI agents capable of autonomously operating smartphone apps through visual perception, planning, executing and reflecting on operational steps. Qwen (通义千问) is Alibaba's open-source large language model series.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.google.dev/gemma/docs/core/model_card_4?hl=zh-cn">Gemma 4 模 型 卡片 | Google AI for Developers</a></li>
<li><a href="https://www.winandmac.com/2025/03/google-gemma-3-open-source-model/">Google 發佈開 源 Gemma ... - winandmac.com 視麥媒體</a></li>
<li><a href="https://github.com/QwenLM/Qwen">GitHub - QwenLM/ Qwen : The official repo of Qwen (通义千问) chat...</a></li>

</ul>
</details>

**Tags**: `#Google Gemma`, `#Open Source AI`, `#Mobile AI`, `#Large Language Models`, `#AI Model Competition`

---

<a id="item-8"></a>
## [China CAC Draft Rules on Digital Virtual Humans, Bans Minor Virtual Companions](https://mp.weixin.qq.com/s/EHpjg2sfth0W7OE-v6hq9g) ⭐️ 8.0/10

China's Cyberspace Administration released a draft regulation on April 3, 2026, requiring digital virtual human services to display prominent 'digital human' identification marks throughout their service area, obtain explicit consent for using personal data to create models, and ban virtual companion services for minors, with penalties up to 200,000 yuan for violations. 这是中国首次对数字虚拟人服务建立正式监管框架，直接影响提供AI虚拟伴侣和数字形象服务的公司。禁止未成年人使用虚拟伴侣服务符合全球监管趋势，旨在应对AI伴侣产品带来的情感操控和成瘾风险担忧。 Services with public opinion or social mobilization capabilities must complete algorithm filing and security assessments. Users retain the right to withdraw consent and request deletion of their digital virtual human. The draft is open for public feedback until May 6, 2026.

telegram · zaihuapd · Apr 3, 09:39

**Background**: Digital virtual humans are AI-generated digital avatars that can interact with users online. The regulation comes amid growing global scrutiny of AI companion products - from the EU AI Act classifying emotion-recognition AI as high-risk to the US FTC investigating AI companion services. China's approach aims to distinguish between utility AI (like customer service bots) and companion AI involving emotional interaction, applying stricter rules to the latter.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cac.gov.cn/2025-12/28/c_1768662848000498.htm">专家解读｜规范人工智能前沿业态健康发展的新探索：解读《人工智能拟...</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1994117858939135385">剑悬“虚拟恋人”：中国AI伴侣新规深度解析 - 知乎</a></li>
<li><a href="https://beian.cac.gov.cn/">互联网信息服务算法备案系统</a></li>

</ul>
</details>

**Discussion**: Industry experts view the draft as a positive step balancing innovation and risk prevention, providing clear guidance for emerging sectors like AI companions and virtual idols. However, some concerns remain about the definition boundaries between utility and companion AI, with discussions on how mixed-type products should handle compliance.

**Tags**: `#AI regulation`, `#virtual companions`, `#China tech policy`, `#minor protection`, `#digital virtual humans`

---

<a id="item-9"></a>
## [Anthropic Launches New PAC Ahead of Midterms](https://techcrunch.com/2026/04/03/anthropic-ramps-up-its-political-activities-with-a-new-pac/) ⭐️ 7.0/10

Anthropic has established a new Political Action Committee to support candidates favorable to its AI policy agenda ahead of the upcoming midterm elections. This development signals Anthropic's direct entry into electoral politics, marking a significant escalation in corporate political engagement within the AI industry and potentially influencing future tech policy and regulation. The PAC is positioned to back candidates who support Anthropic's policy positions on AI regulation, safety standards, and industry governance, though specific financial details and target candidates have not been disclosed.

rss · TechCrunch AI · Apr 3, 20:22

**Background**: A Political Action Committee (PAC) is a type of organization that raises and spends money to elect or defeat political candidates. In the US, corporations are prohibited from directly contributing to candidates but can form PACs to collect voluntary donations from employees and shareholders for electoral purposes. The AI industry has seen increased political engagement as companies seek to shape emerging regulations around AI safety, governance, and competitive positioning.

**Tags**: `#AI policy`, `#corporate politics`, `#Anthropic`, `#lobbying`, `#tech industry`

---

<a id="item-10"></a>
## [Meta Pauses Work With Mercor After Data Breach](https://www.wired.com/story/meta-pauses-work-with-mercor-after-data-breach-puts-ai-industry-secrets-at-risk/) ⭐️ 7.0/10

Meta has paused its partnership with Mercor, a major AI data vendor, following a security breach that may have exposed proprietary AI training data and methodologies from multiple leading AI laboratories. This incident highlights the security risks in AI supply chains and could have far-reaching implications for the entire AI industry, as the exposed data may include sensitive training methodologies that companies spend years developing. The breach occurred at Mercor, which provides data labeling and processing services for AI model training. Multiple major AI labs are currently investigating the extent of the data exposure. The specific nature of the exposed data and the timeline of the incident remain unclear.

rss · WIRED AI · Apr 3, 21:28

**Background**: Mercor is a data vendor that provides training data services to AI companies, including data labeling, curation, and processing essential for developing large language models and other AI systems. Data vendors like Mercor handle vast amounts of potentially sensitive information used to train AI models, making them attractive targets for security breaches.

**Tags**: `#AI security`, `#data breach`, `#Meta`, `#AI industry`, `#Mercor`, `#corporate news`

---

<a id="item-11"></a>
## [AI-Generated Kernel Security Reports Surge 10x](https://simonwillison.net/2026/Apr/3/willy-tarreau/#atom-everything) ⭐️ 7.0/10

Willy Tarreau reports kernel security vulnerability submissions have increased from 2-3 per week two years ago to 5-10 per day since early 2026, attributing the surge to AI-generated reports that are mostly valid, necessitating additional maintainers. This represents a significant shift in open-source security maintenance, as AI tools are now finding real vulnerabilities at scale. The Linux kernel maintainers face unprecedented workload increases while managing duplicate reports from different AI tools. Most AI-generated reports are valid, and maintainers are now seeing daily duplicates - the same bug found by different people using possibly different AI tools. The worst days are Fridays and Tuesdays.

rss · Simon Willison · Apr 3, 21:48

**Background**: Willy Tarreau is the Lead Software Developer of HAProxy, a popular open-source load balancer and proxy server. He is also active on the Linux kernel security mailing list. The Linux kernel is the core of the Android and Linux operating systems, and its security maintenance relies on volunteer maintainers.

**Tags**: `#security`, `#linux-kernel`, `#AI`, `#vulnerability-reports`, `#open-source-maintenance`

---

<a id="item-12"></a>
## [Linux Kernel Maintainer Reports AI Security Reports Now Genuinely Useful](https://simonwillison.net/2026/Apr/3/greg-kroah-hartman/#atom-everything) ⭐️ 7.0/10

Linux kernel maintainer Greg Kroah-Hartman reports that AI-generated security reports have transitioned from obviously wrong 'AI slop' to genuinely useful real reports in the past month, marking a significant qualitative shift. This represents a notable milestone in AI's practical utility for security work, coming from a highly respected authoritative source. It suggests AI tools are becoming viable for real-world security vulnerability detection in open source projects. Kroah-Hartman noted that 'something happened a month ago' that caused this shift. Previously, AI-generated reports were 'obviously wrong or low quality' and 'kind of funny,' but now all open source projects are receiving good, real security reports generated with AI.

rss · Simon Willison · Apr 3, 21:44

**Background**: Greg Kroah-Hartman is a highly respected Linux kernel maintainer known for maintaining the stable kernel releases and his direct, technical approach. He has previously been critical of low-quality contributions to the kernel. The Linux kernel project is one of the largest and most important open source projects globally, making its security processes significant for the entire software ecosystem.

**Tags**: `#linux`, `#ai`, `#security`, `#open-source`, `#kernel`

---

<a id="item-13"></a>
## [CSP Meta Tag in Iframe Cannot Be Bypassed by JavaScript](https://simonwillison.net/2026/Apr/3/test-csp-iframe-escape/#atom-everything) ⭐️ 7.0/10

Security researcher Simon Willison discovered that CSP meta tags injected at the top of iframe content are enforced even when subsequent untrusted JavaScript attempts to manipulate them, enabling secure sandboxing without separate domains. This finding enables developers to build artifact/sandboxed code execution environments (similar to Claude Artifacts) with CSP protection without needing separate domains, simplifying security architecture for interactive web applications. The research demonstrates that meta http-equiv="Content-Security-Policy" tags placed at the beginning of iframe srcdoc content are obeyed by the browser, and JavaScript cannot modify or remove them after the page loads.

rss · Simon Willison · Apr 3, 16:05

**Background**: Content Security Policy (CSP) is a security header that helps prevent XSS and data injection attacks by controlling which resources a page can load. Iframes are commonly used to isolate untrusted content, but traditionally required separate domains for effective isolation. The srcdoc attribute allows embedding HTML directly in an iframe without an external URL.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/bhaveshk90/Content-Security-Policy-CSP-Bypass-Techniques">GitHub - bhaveshk90/Content-Security-Policy-CSP-Bypass-Techniques: Content-Security-Policy (CSP) Bypass Techniques · GitHub</a></li>
<li><a href="https://www.browserstack.com/guide/csp-bypass">Learn & bypass Content Security Policy HTTP Response Header | BrowserStack</a></li>

</ul>
</details>

**Tags**: `#iframes`, `#security`, `#javascript`, `#content-security-policy`, `#sandboxing`

---

<a id="item-14"></a>
## [Axios Supply Chain Attack Used Targeted Social Engineering](https://simonwillison.net/2026/Apr/3/supply-chain-social-engineering/#atom-everything) ⭐️ 7.0/10

The Axios team published a postmortem revealing that their supply chain attack was carried out through sophisticated social engineering targeting a specific maintainer, mimicking techniques from the UNC1069 North Korean threat actor documented by Google Threat Intelligence. This attack demonstrates that supply chain threats are evolving beyond automated exploits to include highly targeted, human-focused social engineering campaigns. Every open source maintainer of widely-used packages needs to be aware of this attack strategy. The attackers cloned a company and its founder's likeness, created a branded Slack workspace with fake profiles of OSS maintainers, scheduled a Microsoft Teams meeting, and convinced the maintainer to install what appeared to be a system update—which was actually a Remote Access Trojan (RAT) that stole credentials to publish a malicious npm package.

rss · Simon Willison · Apr 3, 13:54

**Background**: UNC1069 is a financially motivated North Korean threat actor active since at least 2018, linked to BlueNoroff, a Lazarus Group subunit specializing in cryptocurrency theft. The attack deployed WAVESHAPER.V2, an updated version of a cross-platform backdoor. This incident marks one of the most sophisticated supply chain attacks targeting open source maintainers through direct social engineering.

<details><summary>References</summary>
<ul>
<li><a href="https://cloud.google.com/blog/topics/threat-intelligence/unc1069-targets-cryptocurrency-ai-social-engineering">UNC1069 Targets Cryptocurrency Sector with New ... - Google Cloud</a></li>
<li><a href="https://thehackernews.com/2026/04/google-attributes-axios-npm-supply.html">Google Attributes Axios npm Supply Chain Attack to North ...</a></li>
<li><a href="https://cybersecsentinel.com/axios-npm-backdoored-unc1069-deploys-cross-platform-rat-via-supply-chain-attack/">Axios npm Backdoored: UNC1069 Deploys Cross-Platform RAT via ...</a></li>

</ul>
</details>

**Discussion**: The discussion emphasizes that developers frequently need to install meeting software under time pressure and often click through prompts quickly, making this a highly effective attack vector. Many comment that maintainers of popular packages are prime targets for such targeted attacks.

**Tags**: `#supply-chain-security`, `#social-engineering`, `#axios`, `#security-incident`, `#malware`

---

<a id="item-15"></a>
## [PyPI Supply Chain Attack Compromises LiteLLM, Steals Sensitive Data](https://www.infoq.cn/article/YqWdW6lF74rlqXkJ5AMJ?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

A supply chain attack on PyPI compromised the LiteLLM library, leading to the exfiltration of sensitive data. Over 40,000 downloads occurred of the tampered version. This incident highlights the vulnerability of open-source package repositories and the risks developers face when using third-party libraries. Compromised dependencies can expose millions of applications to data breaches and further attacks. The attack was discovered by FutureSearch researcher Callum McMahon. LiteLLM simplifies access to 100+ LLMs with standardized API compatibility. This is not an isolated incident—PyPI has seen multiple supply chain attacks recently.

rss · InfoQ 中文站 · Apr 3, 15:00

**Background**: Supply chain attacks target software distribution channels to inject malicious code into legitimate packages. PyPI (Python Package Index) is the official repository for Python packages, serving millions of developers daily. When attackers compromise popular libraries, all downstream users become vulnerable.

<details><summary>References</summary>
<ul>
<li><a href="https://www.litellm.ai/">LiteLLM</a></li>
<li><a href="https://blog.eimoon.com/p/litellm-pypi-supply-chain-attack-analysis/">LiteLLM PyPI 供 应 链 攻 击 复盘：受影响版本、 攻 击 方式与止损建议</a></li>
<li><a href="https://www.infoq.cn/article/YqWdW6lF74rlqXkJ5AMJ">PyPI 供 应 链 攻 击 导致 LiteLLM 遭入侵，致使敏感信息被窃取 - InfoQ</a></li>

</ul>
</details>

**Discussion**: Andrej Karpathy alerted developers to this attack, and it quickly spread through the AI and Python communities. The incident has raised concerns about the security of package repositories and the need for better verification mechanisms.

**Tags**: `#供应链攻击`, `#PyPI`, `#安全`, `#LiteLLM`, `#数据泄露`

---

<a id="item-16"></a>
## [Discord Open-Sources Osprey Security Rules Engine](https://www.infoq.cn/article/Wz12mUPtcy79cyTsIOwV?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Discord has open-sourced Osprey, its internal security rules engine developed by the ROOST team, capable of processing 2.3 million rules per second across 400 million daily actions. This release provides the broader security community with a production-grade rules engine that has proven capability at Discord's scale of 150M+ users. It enables other platforms to build trust and safety tools without starting from scratch. Osprey is built with a Rust coordinator for high performance and low latency. It serves as an event stream decisions engine designed to detect and remove harmful content at scale.

rss · InfoQ 中文站 · Apr 3, 11:00

**Background**: A rules engine is a software system that evaluates incoming events or data against a set of predefined rules to make automated decisions. Discord processes billions of daily user actions, making fast rule evaluation critical for content moderation and user safety. The ROOST team at Discord focuses on platform trust and safety infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/roostorg/osprey">GitHub - roostorg/ osprey : Automate the obvious and investigate the...</a></li>
<li><a href="https://www.live-feeds.com/2026/03/31/discord-open-sources-osprey-safety-rules-engine-processing-2-3-million-rules-per-second/">Discord Open Sources Osprey Safety Rules Engine ... - Live Feeds</a></li>
<li><a href="https://discord.com/press-releases/roost-announces-coop-and-osprey-free-open-source-trust-and-safety-infrastructure-for-the-ai-era">ROOST Announces “Coop” and “ Osprey ”: Free, Open-Source Trust...</a></li>

</ul>
</details>

**Tags**: `#security`, `#open-source`, `#rules-engine`, `#performance`, `#Discord`

---

<a id="item-17"></a>
## [Cloudflare Deploys Edge-Based API Vulnerability Scanning](https://www.infoq.cn/article/8LBRc9hODxYmCvKU85fy?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Cloudflare has deployed proactive API vulnerability scanning capabilities directly at its edge network, enabling users to detect and remediate API security issues without deploying additional agents or infrastructure. This represents a significant shift toward edge-based security, allowing organizations to identify API vulnerabilities at the network edge before malicious actors can exploit them. It addresses the growing concern around API security as APIs become the primary attack vector for modern applications. The scanning occurs at the edge, meaning it can analyze API traffic in real-time without introducing latency. Cloudflare's approach allows for continuous monitoring and can identify common vulnerabilities such as broken authentication, excessive data exposure, and lack of rate limiting.

rss · InfoQ 中文站 · Apr 3, 10:30

**Background**: API security has become a critical concern as organizations increasingly rely on APIs to connect services and expose data. Traditional API security solutions often require agents or API gateways, which add complexity and potential points of failure. Edge-based scanning offers a alternative approach by leveraging the existing Cloudflare network infrastructure.

**Tags**: `#cloud-security`, `#api-security`, `#edge-computing`, `#vulnerability-scanning`, `#cloudflare`

---

<a id="item-18"></a>
## [Cursor 3: AI Agent-First Unified Development Workspace](https://cursor.com/blog/cursor-3) ⭐️ 7.0/10

Cursor released version 3, repositioning itself as an AI agent-oriented unified development workspace with a completely redesigned agent-centric UI, multi-repository workspace support, and cross-platform access via mobile, web, desktop, and integrations like Slack, GitHub, and Linear. This represents a major shift from managing code to managing AI agents, enabling developers to run multiple agents in parallel and seamlessly switch between local (for fast iteration) and cloud (for continuous operation when offline or switching tasks). Cursor 3 supports cloud-local hybrid sessions where local agents handle modifications and testing while cloud agents continue running when offline or switching tasks. The new integrated diff view enables faster editing and reviewing of changes, with continued support for staging, committing, and managing pull requests. Composer 2 scores 61.7% on Terminal-Bench 2.0.

telegram · zaihuapd · Apr 3, 02:00

**Background**: Cursor is an AI-first code editor built on VS Code, widely used for AI-assisted software development. The shift to agent-centric workflows reflects the broader trend of AI agents moving from conversational tools to practical production helpers. Cloud-local hybrid development environments have become a key capability for maintaining continuous AI agent operations across different work contexts.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/ai-software-engineer/cursor-3-has-arrived-and-just-went-agent-first-b8a078d87c93">Cursor 3 Has Arrived — And Just Went Agent-First... | Medium</a></li>
<li><a href="https://railsdrop.com/2026/01/03/engineers-guide-to-cursor-ai-mastering-the-ai-first-ide-in-2026/">Engineer’s Guide to Cursor AI : Mastering the AI -First IDE in 2026</a></li>
<li><a href="https://blog.eimoon.com/p/claude-code-remote-control-guide/">Claude Code 远程控制指南：随时随地掌控你的本地开发环境</a></li>

</ul>
</details>

**Discussion**: The developer community sees this as a significant evolution from a code editor to an AI agent management platform. Users particularly value the parallel agent execution capability and the seamless cloud-local handoff, though some note the traditional IDE remains available when needed. The change is viewed as a practical step toward managing AI agents rather than just writing code.

**Tags**: `#AI code editor`, `#Cursor`, `#software development tools`, `#AI agents`, `#developer productivity`

---

<a id="item-19"></a>
## [Google Vids Integrates Veo 3.1, Free AI Video for All Users](https://www.techradar.com/ai-platforms-assistants/google-is-pushing-ai-video-into-ordinary-life-just-as-openai-pulls-sora-back) ⭐️ 7.0/10

Google has updated its browser-based AI video creation tool Google Vids with the Veo 3.1 model, making it free for all Google account users with 10 video generations per month. The update also integrates Lyria 3 music generation for 30-second to 3-minute soundtracks, though this feature is exclusive to Google AI Pro and Ultra subscribers. This represents a significant democratization of AI video creation, making advanced video generation accessible to everyday users while maintaining premium features for paying customers. The move contrasts sharply with OpenAI's more restrictive approach to Sora, highlighting Google's strategy of embedding AI capabilities into widely-used platforms for mass adoption. The update includes customizable digital avatars with adjustable appearance, voice, and props, while AI Ultra subscribers receive up to 1,000 video generations monthly. Veo 3.1 supports 4K output with both 16:9 landscape and 9:16 portrait aspect ratios and generates native audio alongside video content.

telegram · zaihuapd · Apr 3, 05:23

**Background**: Google Vids is a browser-based AI video production tool within Google's creative suite, enabling users to generate professional-quality videos from text prompts. Veo 3.1, released in October 2025, is Google's state-of-the-art video generation model capable of producing 8-second clips at up to 4K resolution with integrated audio. This integration positions Google to compete directly with OpenAI's Sora in the rapidly growing AI video generation market.

<details><summary>References</summary>
<ul>
<li><a href="https://aistudio.google.com/models/veo-3">Veo 3 | Google AI Studio</a></li>
<li><a href="https://deepmind.google/models/veo/">Veo — Google DeepMind</a></li>
<li><a href="https://deepmind.google/models/lyria/">Lyria 3 — Google DeepMind</a></li>

</ul>
</details>

**Tags**: `#AI Video Generation`, `#Google Vids`, `#Veo 3.1`, `#Consumer AI Tools`, `#Google AI Strategy`

---

<a id="item-20"></a>
## [US Humanoid Robots Depend on Chinese Suppliers for Key Components](https://www.wsj.com/tech/under-the-skin-of-americas-humanoid-robots-chinese-technology-27dd4fdf) ⭐️ 7.0/10

The Wall Street Journal reports that US humanoid robots are increasingly relying on Chinese suppliers for critical components including motors, joints, magnets, and sensors. Disney's Olaf robot uses parts from China's Unitree Robotics, and Tesla is working with Chinese suppliers to advance Optimus mass production. This dependency raises significant supply chain security concerns, especially as China launches 28 humanoid robots in 2025—nearly three times the number from US companies. Morgan Stanley estimates Chinese supply chains could reduce manufacturing costs by up to two-thirds, making it difficult for US firms to decouple. US bipartisan legislators proposed legislation in February 2025 to assess US robotics competitiveness and supply chain risks. The bill reflects growing concerns about technological dependency in a strategic industry that could reshape manufacturing and logistics.

telegram · zaihuapd · Apr 3, 08:55

**Background**: Unitree Robotics (宇树科技) is a Hangzhou-based Chinese robotics company founded in 2016, initially specializing in quadruped robots for the consumer market. Morgan Stanley has published multiple reports on the humanoid robot industry, projecting potential market sizes and cost structures. The robots mentioned in the WSJ article represent the intersection of entertainment (Disney) and industrial (Tesla) applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unitree_Robotics">Unitree Robotics - Wikipedia</a></li>
<li><a href="https://www.unitree.com/">Unitree Robotics | Robot Dog_Quadruped_Humanoid Robotics ...</a></li>
<li><a href="https://news.qq.com/rain/a/20240628A07LSS00">解读摩根士丹利最新人形机器人报告：30万亿美金市场规模与特斯拉Optim...</a></li>

</ul>
</details>

**Tags**: `#humanoid_robots`, `#supply_chain`, `#us_china_tech`, `#manufacturing`, `#tesla_optimus`

---

<a id="item-21"></a>
## [Adobe Help Desk Breach Exposes 13M Tickets](https://cybernews.com/security/threat-actor-claims-adobe-data-theft/?utm_source=flipboard&amp;utm_content=CyberNews_com%2Fmagazine%2FLatest+cybersecurity+news) ⭐️ 7.0/10

A threat actor nicknamed 'Mr. Raccoon' claims to have breached Adobe's help desk system, potentially exposing approximately 13 million support tickets, 15,000 employee records, HackerOne bug bounty submissions, and some internal files. Adobe has not yet responded to these claims. This incident highlights the vulnerability of help desk systems and the potential risks associated with third-party vendor access, as researchers note the breach scope appears limited to the help desk rather than Adobe's core internal network. The potential exposure of employee records and internal communications could still pose significant security and privacy concerns. The claimed attack vector may involve compromised accounts of outsourced employees through malware or subsequent phishing attacks, and researchers consider the claims plausible given screenshots showing Adobe's internal OneDrive/SharePoint and employee webcam feeds.

telegram · zaihuapd · Apr 3, 10:40

**Background**: HackerOne is a crowdsourced security platform that organizations use to run bug bounty programs, allowing security researchers to report vulnerabilities in exchange for rewards. Help desk systems typically contain customer support tickets, employee information, and internal communications, making them valuable targets for threat actors even if they don't contain core network access.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HackerOne">HackerOne - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The news item carries a '茶馆讨论' (tea house discussion) tag indicating community engagement, however no specific discussion content was visible at the time of reporting.

**Tags**: `#data-breach`, `#adobe`, `#cybersecurity`, `#threat-actor`, `#corporate-security`

---

<a id="item-22"></a>
## [MIIT Warns of Critical Apple Vulnerabilities Affecting iOS 17.2.1 and Below](https://www.nvdb.org.cn/publicAnnouncement/2040008892420247553) ⭐️ 7.0/10

China's Ministry of Industry and Information Technology (MIIT) through the NVDB platform has warned that attackers are actively exploiting Apple device vulnerabilities to carry out network attacks, potentially leading to data theft and system control. The affected range covers iOS 13.0 to 17.2.1 on iPhone and iPad devices. This advisory affects millions of iPhone and iPad users in China who have not updated to iOS 17.3 or later. Attackers can gain root privileges through social engineering, enabling complete device compromise including data exfiltration and unauthorized system control. The attack vector involves attackers sending malicious SMS messages, emails, or linking users to poisoned webpages that install remote control trojans, granting attackers the highest privileges on affected devices. NVDB recommends users upgrade their systems immediately and avoid clicking on links from unknown sources.

telegram · zaihuapd · Apr 3, 11:23

**Background**: NVDB (网络安全威胁和漏洞信息共享平台) is the cybersecurity threat and vulnerability information sharing platform operated by China's Ministry of Industry and Information Technology. This is a routine security advisory from the Chinese government. iOS 17.2.1 was released in December 2023, and subsequent iOS versions have already patched these vulnerabilities.

**Tags**: `#cybersecurity`, `#apple`, `#ios`, `#vulnerability`, `#government-advisory`

---

<a id="item-23"></a>
## [LinkedIn Allegedly Scans Browser Extensions, Shares Data with Third Parties](https://cybernews.com/privacy/linkedin-surveillance-browsergate/?utm_source=flipboard&amp;utm_content=CyberNews_com%2Fmagazine%2FLatest+cybersecurity+news) ⭐️ 7.0/10

An investigation alleged that LinkedIn deployed code to scan users' installed browser extensions, collecting data on over 6,000 extensions and 200+ competitor tools, then encrypting and transmitting this data back to their servers, potentially affecting 405 million users. This privacy violation is significant because it involves sensitive user data including religious beliefs, political views, health status, and job-seeking behavior, shared with third parties without user consent, potentially violating GDPR requirements. The scanned data was shared with third-party companies including HUMAN Security, and under EU GDPR, such data processing typically requires explicit user consent which LinkedIn did not obtain nor disclose.

telegram · zaihuapd · Apr 3, 12:09

**Background**: Browser fingerprinting is a technique that collects details from a user's browser and device to create a unique identifier. LinkedIn allegedly scanned extensions to detect sensitive information about users such as their religious beliefs, political affiliations, health conditions, and employment status, potentially building detailed profiles without consent.

<details><summary>References</summary>
<ul>
<li><a href="https://cybernews.com/privacy/linkedin-surveillance-browsergate/">LinkedIn secretly injects code to spy on your browser | Cybernews</a></li>
<li><a href="https://www.gadgetreview.com/linkedin-allegedly-scans-your-browser-and-sends-the-data-to-third-parties">LinkedIn Allegedly Scans Your Browser - and Sends... - Gadget Review</a></li>
<li><a href="https://fingerprint.com/blog/browser-fingerprinting-techniques/">Browser Fingerprinting Techniques : 6 Top Methods Explained</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#LinkedIn`, `#data-collection`, `#GDPR`, `#cybersecurity`

---

<a id="item-24"></a>
## [Reverse Engineering Claude Code Signatures Bypasses Bun Dependency](https://a10k.co/b/reverse-engineering-claude-code-cch.html) ⭐️ 7.0/10

Researchers discovered how to forge Claude Code's proprietary `cch` request signing header without the Bun runtime, using xxHash64 and SHA-256 algorithms to calculate the signature components. This enables a Python proof-of-concept that can bypass the Bun dependency requirement, potentially allowing unauthorized access to Claude Code's API features like fast mode, though the signature appears to be primarily for billing attribution and feature gating rather than strong access control. The `cch` header uses xxHash64 to hash the complete JSON request body when a placeholder `cch=00000` is present, while the last 3 digits of `cc_version` are derived from a specific character in the first user message combined with a built-in salt and version number via SHA-256.

telegram · zaihuapd · Apr 3, 15:00

**Background**: Claude Code is Anthropic's CLI tool for AI-assisted coding that sends requests to the Anthropic API with proprietary headers. The `cch` header serves as a request integrity check - requests with incorrect signatures are rejected. The Bun runtime was previously required to compute these signatures, as they were not calculated in JavaScript but in the native fetch implementation within Claude Code's private Bun runtime.

<details><summary>References</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/fast-mode">Speed up responses with fast mode - Claude Code Docs</a></li>
<li><a href="https://github.com/Cyan4973/xxHash">xxHash - Extremely fast hash algorithm - GitHub xxHash: xxHash XXHash Algorithm Implementation | ceph/xxHash | DeepWiki xxHash - Extremely fast hash algorithm - Google Open Source xxhash64 - Azure Databricks | Microsoft Learn xxHash: xxHash XxHash64 Class (System.IO.Hashing) | Microsoft Learn xxhash64 - Azure Databricks | Microsoft Learn XXHash Algorithm Implementation | ceph/xxHash | DeepWiki xxHash in C# | SSOJet</a></li>
<li><a href="https://xxhash.com/doc/v0.8.2/index.html">xxHash: xxHash</a></li>

</ul>
</details>

**Discussion**: The research was discussed in a Chinese-language tech community (花频道茶馆), suggesting interest in the reverse engineering community. The ability to replicate the signature in Python demonstrates that the mechanism is not a strong security boundary but rather a functional gating and attribution system.

**Tags**: `#reverse-engineering`, `#claude-code`, `#anthropic`, `#bun-runtime`, `#api-security`, `#xxhash`

---