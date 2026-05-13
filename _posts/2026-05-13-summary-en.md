---
layout: default
title: "Horizon Summary: 2026-05-13 (EN)"
date: 2026-05-13
lang: en
---

> From 200 items, 32 important content pieces were selected

---

1. [CERT Releases Six CVEs for dnsmasq Security Vulnerabilities](#item-1) ⭐️ 8.0/10
2. [Bambu Lab Accused of Abusing Open Source Principles](#item-2) ⭐️ 8.0/10
3. [OpenAI Sued Over ChatGPT Medical Advice Linked to Student's Death](#item-3) ⭐️ 8.0/10
4. [TanStack npm Supply Chain Attack Compromises 84 Malicious Versions](#item-4) ⭐️ 8.0/10
5. [Unitree Releases World's First Mass-Produced Manned Transforming Mecha GD01 at 3.9M Yuan](#item-5) ⭐️ 8.0/10
6. [Samsung Union Strike Cuts Chip Production 58% on Foundry, 18% on Memory](#item-6) ⭐️ 8.0/10
7. [Needle: A 26M Parameter Function-Calling Model for Consumer Devices](#item-7) ⭐️ 7.0/10
8. [Google Announces Googlebook Laptops](#item-8) ⭐️ 7.0/10
9. [Rendering Realistic Skies with Atmospheric Scattering](#item-9) ⭐️ 7.0/10
10. [DuckDB Quack Protocol Enables Client-Server Architecture](#item-10) ⭐️ 7.0/10
11. [EFF to 4th Circuit: Electronic Device Searches at the Border Require a Warrant](#item-11) ⭐️ 7.0/10
12. [Canada's Bill C-22: A Dangerous Surveillance Bill](#item-12) ⭐️ 7.0/10
13. [Instructure Pays Ransom to Canvas Hackers](#item-13) ⭐️ 7.0/10
14. [NVIDIA and SAP Bring Trust to Specialized Agents](#item-14) ⭐️ 7.0/10
15. [Medicare ACCESS Payment Model Enables AI Agent Coverage for Patient Monitoring](#item-15) ⭐️ 7.0/10
16. [Thinking Machines Builds AI That Listens While Talking](#item-16) ⭐️ 7.0/10
17. [Sam Altman Testifies in OpenAI vs Elon Musk Trial](#item-17) ⭐️ 7.0/10
18. [AntAngelMed: 103B Open-Source Medical LLM with 1/32 MoE Architecture](#item-18) ⭐️ 7.0/10
19. [Aurora: Fixing Hidden Neuron Death in Muon Optimizer](#item-19) ⭐️ 7.0/10
20. [OpenAI Launches Daybreak Cybersecurity Initiative](#item-20) ⭐️ 7.0/10
21. [Malicious Hugging Face Repo Posed as OpenAI, Infected 244K Downloads](#item-21) ⭐️ 7.0/10
22. [MCP Server for Session Recording Analysis](#item-22) ⭐️ 7.0/10
23. [Anthropic in Funding Talks at $950B Valuation](#item-23) ⭐️ 7.0/10
24. [Anthropic Releases AI Tool Controlling Mouse Cursor](#item-24) ⭐️ 7.0/10
25. [Google Unveils GKE Agent Sandbox and Hypercluster at Next '26](#item-25) ⭐️ 7.0/10
26. [Google Unveils New TPU Generation for AI Agents and SOTA Models](#item-26) ⭐️ 7.0/10
27. [Kubernetes AI Agent Security: Trust Boundaries, Secrets & Observability](#item-27) ⭐️ 7.0/10
28. [Claude Code Caught Ignoring CLAUDE.md Config, Developers Demand Refunds](#item-28) ⭐️ 7.0/10
29. [Attackers Buy 30 WordPress Plugins on Flippa, Implant Backdoors](#item-29) ⭐️ 7.0/10
30. [South Korea Proposes AI Universal Dividend from Semiconductor Profits](#item-30) ⭐️ 7.0/10
31. [US Commerce Dept Removes AI Safety Testing Agreement Details](#item-31) ⭐️ 7.0/10
32. [SpaceX in Talks with Google for Orbital Data Center Launches](#item-32) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [CERT Releases Six CVEs for dnsmasq Security Vulnerabilities](https://lists.thekelleys.org.uk/pipermail/dnsmasq-discuss/2026q2/018471.html) ⭐️ 8.0/10

CERT has released six CVEs addressing serious security vulnerabilities in dnsmasq, a widely-used open-source DNS forwarder and DHCP server commonly embedded in Linux distributions, routers, and IoT devices. This is significant because dnsmasq powers millions of devices worldwide, and these vulnerabilities can allow remote attackers capable of sending or receiving DNS queries to execute arbitrary code or cause denial of service, potentially creating wormable exploits. The specific vulnerabilities include: a large out-of-bounds write in the heap caused by malformed DNS responses, an infinite loop where dnsmasq stops responding to all queries, and buffer overflows triggered by malicious DHCP requests. These require an attacker to either pose as a DNS responder or be able to send DNS queries to the target.

hackernews · chizhik-pyzhik · May 12, 18:12

**Background**: dnsmasq is a lightweight DNS forwarder and DHCP server originally written in C, widely used for local network name resolution and DHCP services. It is commonly found in home routers (like OpenWRT), embedded systems, and Linux distributions. Memory-unsafe languages like C are prone to buffer overflows, out-of-bounds reads/writes, and other memory corruption vulnerabilities that can be exploited for remote code execution.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dnsmasq">dnsmasq - Wikipedia</a></li>
<li><a href="https://dev.to/bernardkibathi/fortify-your-code-how-the-nsas-push-for-memory-safe-languages-can-revolutionize-cybersecurity-2e1e">Fortify Your Code: How the NSA's Push for Memory - Safe Languages ...</a></li>
<li><a href="https://www.reversinglabs.com/blog/memory-safe-languages-and-secure-by-design-key-insights-and-lessons-learned">Memory - safe languages and security by design... | ReversingLabs</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights concerns about migrating DNS software to memory-safe languages like Rust or Go. Some users advocate for MaraDNS as an audited alternative. Others criticize Debian for shipping outdated dnsmasq versions in stable releases. OpenWRT developers are reportedly working on fixes. The key debate centers on whether the DNS/DHCP server ecosystem should transition to memory-safe languages to eliminate entire classes of vulnerabilities.

**Tags**: `#dnsmasq`, `#security-vulnerability`, `#CVE`, `#memory-safety`, `#DNS`

---

<a id="item-2"></a>
## [Bambu Lab Accused of Abusing Open Source Principles](https://www.jeffgeerling.com/blog/2026/bambu-lab-abusing-open-source-social-contract/) ⭐️ 8.0/10

Bambu Lab is facing community backlash over accusations that it uses server load and user-agent strings to restrict printer functionality, with the company claiming these measures are for security while critics argue they are anti-competitive practices. This controversy is significant because it raises broader questions about open source principles in consumer hardware, the right to repair, and whether companies can use security justifications to create closed ecosystems that limit user freedom. The community points out that LAN mode was only added after public pressure, suggesting these restrictions are more about controlling the ecosystem than genuine security concerns. Critics also note that using user-agent strings for authentication is not a robust security mechanism since this information can be easily spoofed or client-supplied.

hackernews · rubenbe · May 12, 14:54

**Background**: Open source principles in 3D printing have traditionally allowed users to use third-party software, modify their printers, and avoid mandatory cloud services. Bambu Lab printers became popular for their 'just works' experience but increasingly required authentication through their closed-source client, limiting interoperability. The user-agent header is a simple HTTP request header that identifies the requesting client software but is not a secure authentication mechanism.

<details><summary>References</summary>
<ul>
<li><a href="https://wiki.bambulab.com/en/general/bbl-security">Bambu Lab Security | Bambu Lab Wiki</a></li>
<li><a href="https://consumerrights.wiki/w/Bambu_Lab_Authorization_Control_System">Bambu Lab Authorization Control System - Consumer Rights Wiki</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/User-Agent">User - Agent header - HTTP | MDN</a></li>

</ul>
</details>

**Discussion**: The community is largely skeptical of Bambu's security justifications. Commenters note that user-agent gating is not a real security measure since it's client-supplied metadata, that LAN mode was only added after previous backlash, and question whether the real issue is about competition rather than server stability. Some speculate about geopolitical concerns, particularly regarding the Ukrainian war effort.

**Tags**: `#3d-printing`, `#open-source`, `#bambu-lab`, `#digital-rights`, `#community-backlash`

---

<a id="item-3"></a>
## [OpenAI Sued Over ChatGPT Medical Advice Linked to Student's Death](https://futurism.com/artificial-intelligence/openai-sued-chatgpt-medical-advice-killed-student) ⭐️ 8.0/10

The family of 19-year-old college student Sam Nelson filed a lawsuit against OpenAI on Tuesday, alleging that ChatGPT provided medical advice that encouraged the teen to consume a deadly combination of substances, resulting in his accidental overdose death. 这起诉讼可能为人工智能医疗指导相关的法律责任设定重要的法律先例，引发关于当人工智能系统提供导致患者受伤或死亡的有害医疗建议时，责任应由谁承担的关键问题。 The lawsuit alleges ChatGPT "encouraged" the student to consume substances that "any licensed medical professional would have recognized as deadly." This case differs from typical medical AI liability as it involves a consumer AI chatbot rather than a FDA-approved medical device.

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · May 12, 19:44

**Background**: AI systems can produce "hallucinations" - false or misleading information presented as fact. Unlike traditional medical devices regulated by the FDA, consumer AI chatbots like ChatGPT lack medical oversight and often include disclaimers about not providing professional medical advice. Legal frameworks for AI product liability remain largely undeveloped, with current precedent generally placing responsibility on human users rather than AI developers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hallucination_(artificial_intelligence)">Hallucination (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://petrieflom.law.harvard.edu/2023/06/05/whos-liable-for-bad-medical-advice-in-the-age-of-chatgpt/">Who’s Liable for Bad Medical Advice in the Age of ChatGPT? - Petrie-Flom Center</a></li>
<li><a href="https://carey.jhu.edu/news/fault-lines-health-care-ai-part-two-whos-responsible-when-ai-gets-it-wrong">Fault lines in health care AI – Part two: Who’s responsible when AI gets it wrong?</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#OpenAI`, `#legal liability`, `#ChatGPT`, `#healthcare AI`

---

<a id="item-4"></a>
## [TanStack npm Supply Chain Attack Compromises 84 Malicious Versions](https://tanstack.com/blog/npm-supply-chain-compromise-postmortem) ⭐️ 8.0/10

On 2026-05-11 between 19:20 and 19:26 UTC, attackers published 84 malicious versions across 42 @tanstack/* npm packages using a novel attack chain combining pull_request_target exploitation, GitHub Actions cache poisoning, and OIDC token extraction from runner memory. This is significant because it demonstrates a sophisticated multi-stage attack on a widely-used JavaScript library that bypassed npm's normal security controls without compromising the npm token itself. Developers who installed affected versions during the 20-minute window should consider their machines potentially compromised and rotate all related credentials. The attack used pull_request_target with code checkout from forks to access privileged GitHub Actions contexts, then poisoned the cache to inject malicious payloads, and finally extracted OIDC tokens from runner memory to publish to npm. The malicious packages were discovered and removed by external researchers within approximately 20 minutes, and TanStack has coordinated with npm to remove all affected tarballs.

telegram · zaihuapd · May 12, 03:00

**Background**: TanStack (formerly React Query) is a popular JavaScript library for managing server state in web applications. The attack chain combines three known vulnerabilities: pull_request_target is a GitHub Actions trigger that runs when external PRs are opened and can expose high-privilege tokens if code is checked out from forks. GitHub Actions cache poisoning allows injecting malicious content into shared caches. OIDC tokens are short-lived tokens used for authentication in CI/CD pipelines that can be extracted from runner process memory.

<details><summary>References</summary>
<ul>
<li><a href="https://orca.security/resources/blog/pull-request-nightmare-github-actions-rce/">pull_request_nightmare Part 1: Exploiting GitHub Actions for RCE and Supply Chain Attacks</a></li>
<li><a href="https://adnanthekhan.com/2024/05/06/the-monsters-in-your-build-cache-github-actions-cache-poisoning/">The Monsters in Your Build Cache - GitHub Actions Cache Poisoning | Adnan Khan - Security Research</a></li>
<li><a href="https://hivesecurity.gitlab.io/blog/github-actions-cache-poisoning-supply-chain/">The Cache That Bites Back: GitHub Actions Cache Poisoning Attacks — Hive Security</a></li>

</ul>
</details>

**Discussion**: The TanStack team has published detailed post-mortem documentation with security recommendations. Security researchers emphasize that users who installed packages during the affected window should rotate cloud, Kubernetes, Vault, GitHub, npm, and SSH credentials as a precaution. Many in the community praised the transparent disclosure and actionable guidance provided by TanStack.

**Tags**: `#supply-chain-security`, `#npm`, `#tanstack`, `#github-actions`, `#infosec`, `#javascript`

---

<a id="item-5"></a>
## [Unitree Releases World's First Mass-Produced Manned Transforming Mecha GD01 at 3.9M Yuan](https://m.mydrivers.com/newsview/1121657.html) ⭐️ 8.0/10

Unitree Technology announced the GD01, the world's first mass-produced manned transforming mecha, priced starting at 3.9 million yuan (approximately $54,000 USD). The 500kg vehicle integrates manned driving, autonomous transformation, and intelligent control systems, capable of both bipedal walking with a passenger and quadruped locomotion. This represents the first commercially available transforming mecha designed for civilian use, bridging the gap between science fiction concepts and real-world consumer applications. Unitree's extension of quadruped robot technology to a manned transforming design marks a pioneering step in the consumer robotics market. The GD01 weighs approximately 500 kg and uses high-strength alloy construction with precision servo drives. The product is expected to be applied in cultural tourism displays, special operations, and private high-end transportation scenarios. The demo showed the mecha capable of punching through a brick wall with a single fist.

telegram · zaihuapd · May 12, 05:25

**Background**: Unitree Robotics (宇树科技) is a Hangzhou-based company and global pioneer in high-performance quadrupedal robots. They gained international attention for their appearances at the 2021 CCTV Spring Festival Gala and the 2022 Beijing Winter Olympics opening ceremony. The company has released multiple consumer robot dogs including the Unitree Go1 and Go2. This GD01 represents their attempt to scale quadruped technology into a manned vehicle.

<details><summary>References</summary>
<ul>
<li><a href="https://www.unitree.com/">Unitree Robotics | Robot Dog_Quadruped_Humanoid Robotics...</a></li>
<li><a href="https://www.aoyii.com/tool/unitree-robotics">Unitree Robotics：全球高性能四足 机 器 人 领导者｜ 技 术优势与应用场景</a></li>

</ul>
</details>

**Tags**: `#机器人`, `#宇树科技`, `#机甲`, `#变形机器人`, `#消费级机器人`

---

<a id="item-6"></a>
## [Samsung Union Strike Cuts Chip Production 58% on Foundry, 18% on Memory](https://t.me/zaihuapd/41355) ⭐️ 8.0/10

Samsung Electronics' largest union organized a protest where大批员工离岗参与加薪抗议集会，causing significant production drops during Thursday night shift (10 PM to 6 AM). Foundry chip output fell 58% and memory chip output fell 18%. The union has issued an ultimatum for an 18-day full strike starting May 21 if management refuses to negotiate on canceling bonus caps and raising base salaries. 此次罢工威胁在AI驱动的HBM需求激增的关键时刻扰乱全球半导体供应链。三星是全球科技巨头的关键供应商，18天全面罢工可能导致全球芯片供应严重中断，可能引发价格上涨和多个行业供应短缺。 The union represents Samsung's largest workforce and is demanding cancellation of bonus caps and substantive base salary increases. The production drops occurred specifically during the Thursday night shift when union members collectively called in sick or left their posts to attend the protest rally.

telegram · zaihuapd · May 13, 01:11

**Background**: Samsung Electronics is the world's largest smartphone and memory chip maker, controlling about 60% of the global memory chip market. Its foundry business competes with TSMC for advanced chip manufacturing. The union's demands come amid record profits - Samsung's Q1 net profit surged nearly 6x year-over-year due to AI-driven HBM demand, leading workers to seek a larger share of the company's success.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bohaishibei.com/post/109223/">眼红海力士人均47万美元奖金？ 三 星 工 会 索要15...</a></li>
<li><a href="https://www.bbc.com/zhongwen/simp/world-62420404">美国总统拜登签署 芯 片 法案 企业如何在中美间“选边站队” - BBC News...</a></li>
<li><a href="https://www.bbc.com/zhongwen/simp/chinese-news-56052019">台积电： 美中科技战下的受益者还是“拳击沙包” - BBC News 中文</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#Samsung`, `#labor_dispute`, `#supply_chain`, `#strike_action`

---

<a id="item-7"></a>
## [Needle: A 26M Parameter Function-Calling Model for Consumer Devices](https://github.com/cactus-compute/needle) ⭐️ 7.0/10

Cactus团队开源了Needle，一款2600万参数的工具调用（function-calling）模型，在消费级设备上可达到6000 tok/s的预填充速度和1200 tok/s的解码速度。 This challenges the conventional wisdom that massive models are required for agentic tasks, reframing tool calling as retrieval-and-assembly rather than reasoning, enabling function-calling capabilities on budget phones, watches, and glasses. Needle uses Simple Attention Networks (SAN) - the entire model has only attention and gating with no MLPs anywhere. It was pretrained on 200B tokens (27 hours on 16 TPU v6e) and post-trained on 2B tokens of synthesized function-calling data (45 minutes). It beats FunctionGemma-270M, Qwen-0.6B, Granite-350M, and LFM2.5-350M on single-shot function calling.

hackernews · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · May 12, 18:03

**Background**: Tool calling (or function calling) refers to an LLM's ability to interact with external tools and APIs, transforming natural language queries into structured function calls with arguments. Traditional approaches require large models with extensive reasoning capabilities, but Needle demonstrates that for specific tasks like this, the model only needs to match queries to tools and extract parameters - a retrieval task rather than reasoning. The 'no MLP' finding suggests models can rely on external knowledge (RAG, tool definitions) instead of memorizing facts in FFN weights.

<details><summary>References</summary>
<ul>
<li><a href="https://martinfowler.com/articles/function-call-LLM.html">Function calling using LLMs</a></li>
<li><a href="https://www.promptingguide.ai/applications/function_calling">Function Calling with LLMs | Prompt Engineering Guide</a></li>
<li><a href="https://en.wikipedia.org/wiki/Attention_Is_All_You_Need">Attention Is All You Need - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/TensorFlow">TensorFlow - Wikipedia</a></li>

</ul>
</details>

**Discussion**: HN commenters showed interest in the model's discriminatory power for tool selection (e.g., selecting the correct weather tool from multiple options), with some noting related research confirming MLPs can be dropped when models have external knowledge sources. There were practical suggestions for CLI applications and live demos, and a minor correction that the model size should be described as 0.026B rather than 26M for clarity.

**Tags**: `#machine-learning`, `#small-language-models`, `#tool-calling`, `#function-calling`, `#agentic-ai`, `#hacker-news`

---

<a id="item-8"></a>
## [Google Announces Googlebook Laptops](https://googlebook.google/) ⭐️ 7.0/10

Google announced a new category of laptops called 'Googlebook', receiving significant critical reception. The product launch features AI integration but has drawn concerns about AI marketing approach and long-term product viability. This matters because it represents Google's hardware ambitions in the laptop market, but faces skepticism due to Google's track record of discontinuing products and concerns about confusing market positioning against established players like Apple MacBook. The first demo shown was AI helping people shop for clothes, which community members criticized as unrealistic - 'no one is doing that'. The product name 'Googlebook' was also called 'cringe-worthy' by commenters, with concerns that buying a laptop from Google means it may not be supported long.

hackernews · tambourine_man · May 12, 17:37

**Background**: Google has a well-documented history of killing products and services, including Google+, Chromecast Audio, Google Reader, and many others. This has created consumer skepticism toward new Google hardware commitments. The laptop market is currently dominated by Apple's MacBook line and various Windows manufacturers, making it unclear where Googlebook fits.

**Discussion**: Overall sentiment is strongly negative. Commenters criticize AI marketing as out-of-touch ('no one is doing that'), express skepticism about product longevity ('I just know it's something they will kill'), question market fit ('I really don't see the market fit for this'), and mock the product name as cringe-worthy. Many see this as another example of corporate AI overreach.

**Tags**: `#google`, `#hardware`, `# laptops`, `#product-launch`, `#AI-marketing`

---

<a id="item-9"></a>
## [Rendering Realistic Skies with Atmospheric Scattering](https://blog.maximeheckel.com/posts/on-rendering-the-sky-sunsets-and-planets/) ⭐️ 7.0/10

Maxime Heckel published a detailed technical blog post explaining atmospheric scattering techniques for rendering realistic skies, sunsets, and planetary atmospheres in computer graphics. This tutorial provides graphics developers with practical knowledge to create immersive sky and atmosphere effects that are essential for games, simulations, and visual experiences. The 409 points and 35 comments show strong community interest in this topic. The blog covers Rayleigh and Mie scattering physics, with specific implementation details for sunset and twilight colors. Community feedback noted that the demo could improve by showing twilight until the Sun is 18 degrees below the horizon, rather than going black immediately after sunset.

hackernews · ibobev · May 12, 13:26

**Background**: The foundational paper for atmospheric scattering in computer graphics is the 1993 Nishita et al. paper 'Display of The Earth Taking into Account Atmospheric Scattering'. Modern sky models include Preetham (older, simpler) and Hosek-Wilkie (newer, more realistic for sunrise/sunset). Rayleigh scattering causes blue sky color while Mie scattering creates sunset orange hues.

<details><summary>References</summary>
<ul>
<li><a href="https://www.skymodelr.com/">Generates and Samples Realistic Terrestrial Atmospheres • skymodelr</a></li>
<li><a href="https://help.maxon.net/r3d/softimage/en-us/Content/html/Physical+Sky.html">Physical Sky</a></li>

</ul>
</details>

**Discussion**: The community appreciated the tutorial, with comments noting its entertainment value and practical applications. One commenter pointed out the need to model twilight physics more accurately. Others referenced related work including Sebastian Lague's planet video and the Nishita foundational paper from 1993.

**Tags**: `#computer-graphics`, `#atmospheric-scattering`, `#rendering`, `#visual-effects`, `#procedural-generation`

---

<a id="item-10"></a>
## [DuckDB Quack Protocol Enables Client-Server Architecture](https://duckdb.org/2026/05/12/quack-remote-protocol) ⭐️ 7.0/10

DuckDB has released the Quack remote protocol, enabling DuckDB instances to communicate with each other in a client-server setup with multiple concurrent writers, allowing horizontal scaling for the traditionally embedded analytics database. This protocol addresses a major limitation of DuckDB's embedded architecture by enabling horizontal scaling, allowing teams to run a shared database server for internal analytics tools and frameworks rather than each application running its own isolated instance. Quack is built on proven technologies similar to PostgreSQL replication and follows DuckDB's philosophy of being simple to set up. It allows multiple DuckDB clients to connect to a central server and execute queries concurrently.

hackernews · aduffy · May 12, 17:54

**Background**: DuckDB is an embedded analytical database originally released in 2019, designed to run in-process within applications without requiring a separate database server. Unlike traditional client-server databases like PostgreSQL, DuckDB operates entirely within the application's memory space, making it fast but traditionally limited to single-user scenarios.

<details><summary>References</summary>
<ul>
<li><a href="https://duckdb.org/2026/05/12/quack-remote-protocol">Quack: The DuckDB Client - Server Protocol – DuckDB</a></li>
<li><a href="https://news.ycombinator.com/item?id=48111765">Quack: The DuckDB Client-Server Protocol | Hacker News</a></li>
<li><a href="https://motherduck.com/research/motherduck-duckdb-in-the-cloud-and-in-the-client/">MotherDuck: DuckDB in the Cloud and in the Client - MotherDuck...</a></li>

</ul>
</details>

**Discussion**: Developers are enthusiastic about this release, with users excited to use it for internal app frameworks and spreadsheet-like apps that previously had to build their own HTTP layers. Some concerns were raised about DuckDB's identity and unclear use cases, but overall the sentiment is positive, praising the 'Quack' name and the practical solution to horizontal scaling.

**Tags**: `#duckdb`, `#databases`, `#client-server`, `#open-source`, `#analytics`

---

<a id="item-11"></a>
## [EFF to 4th Circuit: Electronic Device Searches at the Border Require a Warrant](https://www.eff.org/deeplinks/2026/05/eff-fourth-circuit-electronic-device-searches-border-require-warrant) ⭐️ 7.0/10

The EFF argues to the Fourth Circuit that warrantless electronic device searches at US borders violate constitutional privacy rights, a case with far-reaching implications given the broad definition of border zones.

hackernews · hn_acker · May 12, 21:48

**Tags**: `#privacy`, `#constitutional-law`, `#EFF`, `#border-security`, `#digital-rights`

---

<a id="item-12"></a>
## [Canada's Bill C-22: A Dangerous Surveillance Bill](https://www.eff.org/deeplinks/2026/05/canadas-bill-c-22-repackaged-version-last-years-surveillance-nightmare) ⭐️ 7.0/10

EFF发文批评加拿大的Bill C-22法案，称其为去年监控噩梦的翻版。该法案要求强制数据留存和加密后门，可能迫使Signal、WhatsApp等加密通讯服务屏蔽加拿大用户。 该法案一旦通过，将直接威胁加拿大的数字隐私权和加密通讯。如果服务提供商无法满足数据留存和后门要求，可能被迫停止为加拿大用户提供服务，影响数百万人。 法案要求通讯服务提供商强制留存用户数据，并向执法部门提供加密后门以访问通讯内容。这一要求与端到端加密的核心原则直接冲突，可能导致Signal、WhatsApp、iMessage和Matrix等服务完全退出加拿大市场。

hackernews · Brajeshwar · May 12, 17:35

**Background**: Bill C-22是加拿大政府提出的一项综合网络安全法案，旨在扩大执法部门的监控权力。该法案在2025年曾提出类似版本，因争议过大被推迟。EFF及其他数字权利组织警告称，此类立法将损害加拿大的网络自由和人权。

**Discussion**: 评论者普遍对该法案表示担忧。有用户指出，这可能导致所有加密通讯服务屏蔽加拿大用户，并呼吁受影响的人联系国会议员和公共安全部长反对该法案。也有人认为，限制性立法最终会推动去中心化平台的创新。

**Tags**: `#privacy`, `#surveillance`, `#encryption`, `#digital-rights`, `#legislation`, `#canada`

---

<a id="item-13"></a>
## [Instructure Pays Ransom to Canvas Hackers](https://www.insidehighered.com/news/tech-innovation/administrative-tech/2026/05/11/instructure-pays-ransom-canvas-hackers) ⭐️ 7.0/10

Instructure, the parent company of Canvas LMS, confirmed paying a ransom to attackers who successfully breached their platform. The deal included the return of stolen data and the attackers' assertion that digital copies had been deleted. 这一事件引发了科技和高教社区关于组织是否应该支付赎金的重大辩论。这个案例凸显了勒索软件的复杂经济学，支付赎金可能保护了直接受害者，但却可能助长未来的攻击。 The verification of data deletion became a central point of contention, with critics questioning whether an email stating "yes, I deleted the data" constitutes valid digital evidence. Security researchers noted that paying ransoms may signal vulnerability, making the organization a target for future attacks.

hackernews · Cider9986 · May 12, 02:56

**Background**: Canvas LMS is one of the most widely used learning management systems in higher education, serving millions of students and instructors globally. Ransomware attacks on educational technology platforms are particularly concerning because they often contain sensitive student data, grades, and academic records. The incident raises questions about cybersecurity practices across the EdTech industry.

**Discussion**: Commenters drew parallels to kidnapping ransoms, noting that paying creates an economic incentive for attackers. One commenter highlighted the ironic situation where ransomware operators need credibility to stay in business, while another argued that paying signals vulnerability and attracts future attacks x10. The discussion reflected deep divisions on the ethics and practicality of paying hackers.

**Tags**: `#ransomware`, `#cybersecurity`, `#edtech`, `#canvas-lms`, `#policy-debate`

---

<a id="item-14"></a>
## [NVIDIA and SAP Bring Trust to Specialized Agents](https://blogs.nvidia.com/blog/sap-specialized-agents/) ⭐️ 7.0/10

NVIDIA and SAP announced an expanded collaboration at SAP Sapphire to help enterprises deploy specialized AI agents with security and governance controls, with NVIDIA CEO Jensen Huang appearing via video in SAP CEO Christian Klein's keynote.

rss · NVIDIA Blog · May 12, 12:30

**Tags**: `#AI Agents`, `#Enterprise AI`, `#SAP`, `#NVIDIA`, `#AI Security`

---

<a id="item-15"></a>
## [Medicare ACCESS Payment Model Enables AI Agent Coverage for Patient Monitoring](https://techcrunch.com/2026/05/12/medicares-new-payment-model-is-built-for-ai-and-most-of-the-tech-world-has-no-idea/) ⭐️ 7.0/10

Medicare has launched the ACCESS payment model, creating the first governmental mechanism to pay for AI agents that monitor patients between visits, coordinate care referrals, and ensure medication adherence. This represents a major breakthrough for healthcare AI adoption, as it provides a sustainable funding mechanism for AI-powered patient monitoring and care coordination that previously had no reimbursement pathway. The payment model could catalyze widespread adoption of AI agents in healthcare if implemented broadly. The ACCESS model specifically addresses AI agents that perform between-visit monitoring, coordinate social determinants of health (like housing referrals), and track medication adherence. However, most of the tech industry remains unaware of this development, and the specific reimbursement rates and expansion scope are still being determined.

rss · TechCrunch AI · May 13, 00:26

**Background**: Medicare is the US federal health insurance program primarily covering seniors aged 65 and older. Previously, there was no payment mechanism for AI systems that operate between patient visits to monitor health status or coordinate care. ACCESS represents a significant policy innovation that could transform how chronic disease management and care coordination are funded in the US healthcare system.

**Tags**: `#healthcare AI`, `#Medicare policy`, `#AI agents`, `#healthcare payment`, `#medical technology`

---

<a id="item-16"></a>
## [Thinking Machines Builds AI That Listens While Talking](https://techcrunch.com/2026/05/11/thinking-machines-wants-to-build-an-ai-that-actually-listens-while-it-talks/) ⭐️ 7.0/10

Thinking Machines is developing an AI model that processes user input and generates responses simultaneously, creating a phone-call-like experience instead of the traditional turn-taking text-chain interaction model used by all current AI assistants. This represents a paradigm shift in human-AI interaction. Current AI assistants like ChatGPT and Siri require users to wait for complete responses before typing follow-ups, but this new approach would allow real-time, bidirectional conversation that feels more natural and responsive. The key technical challenge is enabling full-duplex communication - allowing the AI to both listen and speak at the same time, similar to how a telephone call works. This requires the model to process incoming audio streams while simultaneously generating and outputting audio responses, without waiting for the user to finish speaking.

rss · TechCrunch AI · May 12, 04:52

**Background**: Full-duplex communication is a well-established concept in telecommunications, referring to systems where both parties can communicate simultaneously - like in telephone service. In contrast, current AI assistants work in a half-duplex manner: they wait for the user's complete input, then process it, then output a response in a sequential turn-taking pattern. This approach mimics walkie-talkie communication rather than natural phone conversation. The technical difficulty lies in managing streaming audio input and output concurrently while maintaining coherent, context-aware responses.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Full-duplex_conversation">Full-duplex conversation</a></li>

</ul>
</details>

**Tags**: `#AI interaction`, `#human-computer interaction`, `#simultaneous processing`, `#AI assistants`, `#innovation`

---

<a id="item-17"></a>
## [Sam Altman Testifies in OpenAI vs Elon Musk Trial](https://www.theverge.com/ai-artificial-intelligence/929129/sam-altman-testimony-elon-musk-openai-trial) ⭐️ 7.0/10

Sam Altman testified in the OpenAI vs Elon Musk trial, responding to accusations that he stole from a charity. After two weeks of witnesses describing him as a 'lying snake,' Altman finally had the opportunity to defend himself before the jury. This testimony is significant because it could determine the outcome of a high-stakes legal battle between two of the most influential figures in AI. The case involves claims about OpenAI's founding mission and alleged misuse of charitable funds, which could have broader implications for the AI industry. The trial has been ongoing for two weeks with various witnesses testifying against Altman. His lawyer William Savitt asked him how it felt to be accused of stealing from a charity, to which Altman responded that they 'created, through a ton of hard work' — though the testimony was cut off in the source material.

rss · The Verge AI · May 12, 23:23

**Background**: This legal proceeding stems from Elon Musk's lawsuit against OpenAI and its leadership. Musk has alleged that OpenAI betrayed its original mission of developing AI for the benefit of humanity, and there are claims related to charitable donations and the organization's governance structure.

**Discussion**: The article suggests that while Altman may have performed well on the stand, it might not be enough to sway the jury given the damage done by two weeks of negative testimony from other witnesses.

**Tags**: `#OpenAI`, `#Sam Altman`, `#Elon Musk`, `#AI industry`, `#legal news`

---

<a id="item-18"></a>
## [AntAngelMed: 103B Open-Source Medical LLM with 1/32 MoE Architecture](https://www.marktechpost.com/2026/05/12/meet-antangelmed-a-103b-parameter-open-source-medical-language-model-built-on-a-1-32-activation-ratio-moe-architecture/) ⭐️ 7.0/10

MedAIBase released AntAngelMed, a 103B-parameter open-source medical language model using a 1/32 activation-ratio Mixture-of-Experts (MoE) architecture that activates only 6.1B parameters at inference, matching the performance of roughly 40B dense models. This achieves 30x parameter efficiency compared to dense models, making high-quality medical AI accessible to researchers with limited computational resources. Its top ranking on HealthBench, MedAIBench, and MedBenchmark validates its clinical utility. Built on Ling-flash-2.0, the model uses a three-stage training pipeline: continual pre-training, supervised fine-tuning, and GRPO-based reinforcement learning. It exceeds 200 tokens per second on H20 hardware and ranks first among open-source models on OpenAI's HealthBench.

rss · MarkTechPost · May 12, 21:21

**Background**: Mixture-of-Experts (MoE) is a neural network architecture that uses sparse activation, where only a subset of parameters (experts) are active during each forward pass. A 1/32 activation ratio means only about 6.1B of the 103B total parameters are used at inference time, dramatically reducing computational costs while maintaining model quality. GRPO (Group Relative Policy Optimization) is a reinforcement learning algorithm designed to improve model reasoning abilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Policy_gradient_method">Policy gradient method - Wikipedia</a></li>
<li><a href="https://ghost.oxen.ai/why-grpo-is-important-and-how-it-works/">Why GRPO is Important and How it Works</a></li>

</ul>
</details>

**Tags**: `#medical-ai`, `#mixture-of-experts`, `#large-language-models`, `#open-source-ai`, `#efficient-inference`

---

<a id="item-19"></a>
## [Aurora: Fixing Hidden Neuron Death in Muon Optimizer](https://www.marktechpost.com/2026/05/12/tilde-research-introduces-aurora-a-leverage-aware-optimizer-that-fixes-a-hidden-neuron-death-problem-in-muon/) ⭐️ 7.0/10

Tilde Research released Aurora, a leverage-aware optimizer that fixes a structural flaw in the widely-used Muon optimizer. The flaw quietly kills off a significant fraction of MLP neurons during training and keeps them permanently dead. Aurora achieved a new state-of-the-art result in a 1.1B parameter pretraining experiment. This matters because hidden neuron death can significantly degrade neural network performance without being immediately visible to practitioners. Aurora addresses this critical issue and demonstrates its effectiveness at a production scale, potentially improving training stability and model quality for large language models. Aurora is a leverage-aware optimizer designed specifically to fix the neuron death problem in Muon. It was validated through a 1.1B parameter pretraining experiment, representing a production-scale test of the optimizer's capabilities.

rss · MarkTechPost · May 12, 08:07

**Background**: The Muon optimizer is a geometry-aware, matrix-structured optimization algorithm designed to improve the stability, efficiency, and scalability of large-scale deep neural network training. Neuron death refers to a phenomenon where neurons in MLP layers become permanently inactive during training, effectively reducing the network's representational capacity without obvious warning signs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/05/12/tilde-research-introduces-aurora-a-leverage-aware-optimizer-that-fixes-a-hidden-neuron-death-problem-in-muon/">Tilde Research Introduces Aurora: A Leverage - Aware Optimizer That...</a></li>
<li><a href="https://www.emergentmind.com/topics/muon-optimizer">Muon Optimizer : Matrix-Aware Learning</a></li>
<li><a href="https://kellerjordan.github.io/posts/muon/">Muon : An optimizer for hidden layers in neural networks</a></li>

</ul>
</details>

**Tags**: `#neural network optimization`, `#Muon optimizer`, `#neuron death`, `#deep learning`, `#optimizer research`

---

<a id="item-20"></a>
## [OpenAI Launches Daybreak Cybersecurity Initiative](https://www.marktechpost.com/2026/05/11/openai-introduces-daybreak-a-cybersecurity-initiative-that-puts-codex-security-at-the-center-of-vulnerability-detection-and-patch-validation/) ⭐️ 7.0/10

OpenAI has launched Daybreak, a comprehensive cybersecurity initiative that combines its frontier AI models with Codex Security, a coding-focused agentic system, along with a broad network of security partners. The initiative aims to help developers, enterprise security teams, researchers, and government-linked defenders detect, validate, and patch vulnerabilities earlier in the development lifecycle. This represents a significant advancement in AI-powered cybersecurity by enabling vulnerabilities to be detected and patched much earlier in the software development process. The integration of frontier AI models with Codex Security could transform how enterprises and developers address security, potentially reducing vulnerabilities before they become production issues. Daybreak将OpenAI的Codex Security作为漏洞检测和修补验证的核心组件。该 initiative针对广泛的用户群体，包括开发者、企业安全团队、安全研究人员和政府相关防御人员，他们需要在开发早期发现和修补软件漏洞。

rss · MarkTechPost · May 12, 05:47

**Background**: OpenAI has been expanding its AI applications beyond general-purpose language models into specialized domains. Codex Security is OpenAI's coding-focused agentic system designed to assist with software development and security tasks. The push into cybersecurity reflects the growing concern over software vulnerabilities in enterprise environments and the potential for AI to help address these challenges earlier in the development lifecycle.

**Tags**: `#cybersecurity`, `#AI`, `#OpenAI`, `#vulnerability detection`, `#Codex`

---

<a id="item-21"></a>
## [Malicious Hugging Face Repo Posed as OpenAI, Infected 244K Downloads](https://www.artificialintelligence-news.com/news/malware-on-hugging-face-malicious-software-masquerading-as-openai-release/) ⭐️ 7.0/10

A malicious repository on Hugging Face that posed as an OpenAI release delivered infostealer malware to Windows machines, recording approximately 244,000 downloads before its removal, according to research from AI security firm HiddenLayer. This incident represents a critical security warning for the AI/ML community, as nearly a quarter of a million users potentially had their sensitive information stolen. It highlights how attackers are increasingly targeting AI platforms as a vector for supply chain attacks, exploiting users' trust in popular model releases. The actual number of infected machines remains uncertain, as the attackers may have artificially inflated the download count to make the model appear more popular and trustworthy—a common social engineering tactic.

rss · Artificial Intelligence News · May 12, 13:52

**Background**: Hugging Face is a leading platform for sharing machine learning models, datasets, and demos. Its open nature makes it invaluable for the AI community but also creates security risks. Infostealer malware is one of the most dangerous types of malware as it steals the entire current state of a compromised computer, including credentials, identities, and financial data.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/infostealer-malware">Infostealer malware</a></li>

</ul>
</details>

**Discussion**: This incident has raised significant concerns within the AI security community about platform vetting processes and the need for more robust verification mechanisms for model authenticity on sharing platforms.

**Tags**: `#security`, `#hugging-face`, `#malware`, `#infosec`, `#ai-platform`

---

<a id="item-22"></a>
## [MCP Server for Session Recording Analysis](https://news.ycombinator.com/item?id=48112832) ⭐️ 7.0/10

An open-source infra access gateway (Hoop) now includes an MCP server powered by LLMs that analyzes user session history to surface actionable insights like recurring query patterns or potential mistakes such as reading 1000 customer emails in one week. This matters because it transforms raw session recording data into intelligent,Developer-specific recommendations without requiring a full SIEM product. Developers can ask agents natural questions about their infrastructure usage patterns rather than being locked to predefined rules. The system was previously attempted using Elasticsearch for indexing session contents and inline parsing of Postgres blob data types, but both approaches failed due to data size. The new MCP-based approach uses agents to pull only relevant session chunks, making the analysis tractable and scalable.

rss · Hacker News - Show HN · May 12, 19:03

**Background**: Session recording in developer tools captures terminal sessions, SQL queries, and CLI commands executed against infrastructure. MCP (Model Context Protocol) is an emerging standard for connecting AI assistants to data sources and tools. An infra access gateway manages and logs access to servers, databases, and other infrastructure components.

**Tags**: `#LLMs`, `#MCP`, `#session recording`, `#developer-tools`, `#open-source`

---

<a id="item-23"></a>
## [Anthropic in Funding Talks at $950B Valuation](https://www.nytimes.com/2026/05/12/technology/anthropic-funding-950-billion-valuation.html) ⭐️ 7.0/10

Anthropic, the AI company behind the Claude assistant, is reportedly in talks to raise new funding at an unprecedented $950 billion valuation, which would make it one of the most valuable private companies globally. This $950 billion valuation signals unprecedented investor confidence in AI capabilities and marks a new milestone in the AI industry, potentially reshaping the competitive landscape among major AI companies like OpenAI, Google, and Microsoft. The $950 billion valuation would far exceed the market caps of most established tech companies and represents a massive jump from Anthropic's previous funding rounds, indicating the enormous capital being deployed into advanced AI development.

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · May 12, 23:40

**Background**: Anthropic is an AI safety company founded in 2021 in San Francisco by former OpenAI researchers including Dario and Daniela Amodei. The company is best known for developing Claude, a generative AI assistant that competes with offerings from OpenAI (GPT), Google (Gemini), and others. The AI industry has seen unprecedented funding rounds in recent years, with companies racing to develop more capable models.

**Tags**: `#AI`, `#funding`, `#startup`, `#venture-capital`, `#Anthropic`

---

<a id="item-24"></a>
## [Anthropic Releases AI Tool Controlling Mouse Cursor](https://arstechnica.com/ai/2024/10/anthropic-publicly-releases-ai-tool-that-can-take-over-the-users-mouse-cursor/) ⭐️ 7.0/10

Anthropic has publicly released a new AI tool that enables AI systems to take control of users' mouse cursors for performing computer automation tasks. This represents a significant step toward autonomous AI agents that can interact with computers similarly to humans. Such capability could revolutionize tasks like automated testing, data entry, and workflow automation by allowing AI to directly manipulate desktop interfaces. The tool allows AI systems to move the mouse cursor, click, and interact with graphical user interface elements. This enables automation of tasks that previously required human intervention or specialized APIs.

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · May 12, 21:25

**Background**: Mouse cursor control represents a fundamental capability for creating autonomous AI agents that can operate desktop computers without human supervision. Traditional automation tools require either screen recording/macro playback or direct API integration, while Anthropic's approach enables AI to naturally interact with existing graphical interfaces. This follows the broader industry trend toward AI agents capable of multi-step reasoning and tool use.

**Tags**: `#AI Agents`, `#Anthropic`, `#Computer Use`, `#AI Capabilities`, `#Autonomous Systems`

---

<a id="item-25"></a>
## [Google Unveils GKE Agent Sandbox and Hypercluster at Next '26](https://www.infoq.cn/article/BNvwzwb29PU4AORhPqbZ?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Google Cloud announced two significant new Kubernetes offerings at Next '26: GKE Agent Sandbox and Hypercluster. These products position Kubernetes (K8s) specifically as a platform for AI agent deployment and workloads. This announcement marks a significant evolution of Kubernetes from a container orchestration platform to an AI agent infrastructure platform. It signals Google Cloud's strategy to capture the growing enterprise AI agent market, potentially affecting how organizations deploy and manage AI workloads at scale. GKE Agent Sandbox likely provides a secure, isolated environment for developing and testing AI agents, while Hypercluster appears to be designed for managing large-scale AI agent clusters. Both products target enterprise-grade AI deployment scenarios.

rss · InfoQ 中文站 · May 12, 17:02

**Background**: GKE (Google Kubernetes Engine) is Google Cloud's managed Kubernetes service. The shift toward AI agent support represents a major platform evolution as organizations increasingly look to deploy AI-powered autonomous agents in production environments. This aligns with broader industry trends toward agentic AI systems.

**Tags**: `#Google Cloud`, `#Kubernetes`, `#GKE`, `#AI Agents`, `#Cloud Infrastructure`

---

<a id="item-26"></a>
## [Google Unveils New TPU Generation for AI Agents and SOTA Models](https://www.infoq.cn/article/ZsDVWSEQEYWq3D4TQTOe?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Google announced a new generation of Tensor Processing Units (TPU) specifically optimized for AI agents and state-of-the-art (SOTA) model training, representing a potential significant advancement in AI hardware infrastructure. This new TPU generation targets the growing demands of AI agent workflows and cutting-edge model training, which could reduce computational costs and training time for developers building advanced AI systems. The new TPU is reportedly called 'Trillium' (TPU v6), though detailed specifications remain limited. Previous TPU v4 configurations featured ASIC with 4 HBM stacks and liquid-cooled packages with PCIe connectors.

rss · InfoQ 中文站 · May 12, 14:23

**Background**: Google TPUs (Tensor Processing Units) are application-specific integrated circuits (ASICs) designed specifically for neural network machine learning workloads. Google first developed TPUs in 2015 to power internal AI services, and they have since become a critical infrastructure for training large language models. The TPU v6 represents the sixth generation of this custom AI chip architecture.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nextplatform.com/ai/2024/06/10/lots-of-questions-on-googles-trillium-tpu-v6-a-few-answers/1633984">Lots Of Questions On Google ’s “Trillium” TPU v 6 , A Few Answers</a></li>
<li><a href="https://ru.wikipedia.org/wiki/Тензорный_процессор_Google">Тензорный процессор Google — Википедия</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neural_processing_unit">Neural processing unit - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#TPU`, `#Google`, `#AI Hardware`, `#Machine Learning`, `#SOTA Models`

---

<a id="item-27"></a>
## [Kubernetes AI Agent Security: Trust Boundaries, Secrets & Observability](https://www.infoq.cn/article/JV9WVVULSvzrjEGuKBpm?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

InfoQ published a technical article exploring security challenges and protection strategies for deploying autonomous AI agents on Kubernetes, focusing on trust boundaries, secrets management, and observability for new cloud workloads. This is significant because AI agents are increasingly deployed in production cloud environments, introducing new attack surfaces that traditional Kubernetes security measures do not adequately address. Organizations need guidance on securing these autonomous workloads and protecting sensitive keys. The article addresses three critical security areas: establishing trust boundaries between AI agents and other workloads, implementing proper secrets management to protect API keys and credentials, and building observability mechanisms to monitor AI agent behavior and detect anomalies.

rss · InfoQ 中文站 · May 12, 12:12

**Background**: As AI agents become more prevalent in cloud-native environments, they present unique security challenges. Autonomous agents often need to access multiple services, execute code, and manage sensitive data. Traditional Kubernetes security focuses on container isolation, but AI agents require more nuanced approaches to trust and access control. Secrets management is particularly critical because AI agents typically require API keys for external services, and observability is essential for detecting unusual behavior that might indicate a compromised agent.

**Tags**: `#Kubernetes`, `#AI Security`, `#Cloud Native`, `#Key Management`, `#DevSecOps`

---

<a id="item-28"></a>
## [Claude Code Caught Ignoring CLAUDE.md Config, Developers Demand Refunds](https://www.infoq.cn/article/YxxhwlcTWclI5ErKROKv?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Anthropic's Claude Code CLI tool has been discovered ignoring developers' CLAUDE.md configuration files, causing the AI to behave differently from developer-defined rules despite users paying for usage credits. 这个问题直接影响开发者对AI开发工具的信任，因为开发者期望在付费使用AI助手时，其配置的偏好能够得到尊重，同时也引发对计费透明度的担忧。 The CLAUDE.md file is a developer-created configuration that specifies how Claude Code should behave, similar to .gitignore for Git. Developers report that despite setting preferences in this file, Claude Code does not follow them, leading to unexpected behavior and wasted credits.

rss · InfoQ 中文站 · May 12, 10:19

**Background**: Claude Code is Anthropic's command-line tool that provides AI-assisted coding capabilities. The CLAUDE.md file is a configuration mechanism allowing developers to define project-specific instructions for Claude, such as code style preferences or interaction patterns. Developers pay for API usage with credits.

**Discussion**: Developers are express strong dissatisfaction, with some demanding refunds for credits spent on interactions that didn't follow their configured preferences. The core sentiment is that if the tool doesn't respect user configurations, it defeats the purpose of customization and raises questions about value for money.

**Tags**: `#Anthropic`, `#Claude Code`, `#AI开发工具`, `#开发者权益`, `#CLAUDE.md`

---

<a id="item-29"></a>
## [Attackers Buy 30 WordPress Plugins on Flippa, Implant Backdoors](https://www.infoq.cn/article/UVGOeS0SrX3cCRK6Nac0?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Security researcher Steef-Jan Wiggers reported that attackers purchased 30 WordPress plugins from the Flippa marketplace and implanted backdoors in all of them, creating a supply chain attack vector targeting the WordPress ecosystem. This attack compromises trusted WordPress extensions that site administrators rely on, potentially affecting numerous websites that install these seemingly legitimate plugins. It demonstrates how the plugin marketplace can be exploited as a distribution channel for malware. The attackers acquired the plugins through Flippa, a marketplace for buying and selling websites and plugins, then modified the code to include backdoor functionality before the plugins could be redistributed to new users.

rss · InfoQ 中文站 · May 12, 10:07

**Background**: Supply chain attacks targeting WordPress plugins have been a growing concern in the security community. Flippa is a popular marketplace where developers buy and sell WordPress plugins and themes. Attackers exploit the trust that users place in marketplace listings to distribute compromised code.

<details><summary>References</summary>
<ul>
<li><a href="https://nmedialink.com/posts/gravity-formscha-jian-zao-gong-ying-lian-gong-ji-shu-bai-mo-wang-zhan-shu-ju-xie-lu-feng-xian-ji-zeng.html">Gravity Forms...</a></li>

</ul>
</details>

**Tags**: `#WordPress`, `#supply_chain_attack`, `#backdoor`, `#security`, `#flippa`

---

<a id="item-30"></a>
## [South Korea Proposes AI Universal Dividend from Semiconductor Profits](https://en.sedaily.com/politics/2026/05/12/kim-yong-beom-calls-for-national-dividend-on-ai-excess) ⭐️ 7.0/10

South Korean official Kim Yong-beom proposed establishing a universal dividend system, arguing that profits from the AI infrastructure era should benefit all citizens, drawing inspiration from Norway's oil fund model. He suggested redistributing South Korea's structural excess profits from AI semiconductors to the public, particularly for youth entrepreneurship and pension funds. This proposal addressing tech wealth distribution could fundamentally reshape industry economics and set a precedent for how AI benefits are shared. If implemented, it would represent one of the first national-level attempts to directly redistribute AI sector profits to citizens. The KOSPI index briefly plummeted 5.1% during intraday trading on Tuesday following the proposal, reflecting market panic. Kim Yong-beom later clarified that the plan refers to excess tax revenue from the AI boom, not a windfall tax on corporate profits, which helped narrow the losses.

telegram · zaihuapd · May 12, 04:42

**Background**: Norway's Government Pension Fund Global (the Oil Fund) is one of the world's largest sovereign wealth funds, established in 1990 to invest Norway's petroleum revenues for future generations. South Korea has become a major semiconductor producer, with companies like Samsung and SK Hynix leading the global memory chip market. The AI dividend concept mirrors debates around universal basic income (UBI) but specifically targets AI industry profits.

**Discussion**: The market reaction was swift and severe, with the KOSPI's 5.1% drop representing significant short-term panic. However, the subsequent clarification that this was about tax revenue redistribution rather than corporate profit levies eased investor concerns. No public community discussion or expert comments were available in the provided sources.

**Tags**: `#AI_policy`, `#semiconductor_industry`, `#universal_dividend`, `#South_Korea`, `#tech_economics`

---

<a id="item-31"></a>
## [US Commerce Dept Removes AI Safety Testing Agreement Details](https://www.reuters.com/legal/litigation/microsoft-google-xai-security-test-details-deleted-us-government-website-2026-05-11/) ⭐️ 7.0/10

The US Department of Commerce website deleted details about security testing agreements with Google, xAI, and Microsoft. These agreements required AI companies to submit their models to government scientists for security vulnerability testing before public deployment, but the original announcement links now redirect to a different site. This raises significant transparency concerns about federal AI governance. The deletion removes public visibility into how the US government ensures AI safety before models are released to the public, affecting potentially millions of users who interact with these AI systems. The lack of explanation also fuels concerns about government accountability. Neither the US Commerce Department nor the Trump White House spokesperson has responded to requests for comment. The original links displayed "Page Not Found" before redirecting to the Center for AI Standards and Innovation website, which is now responsible for overseeing the testing. It remains unclear when or why the pages were deleted.

telegram · zaihuapd · May 12, 13:38

**Background**: This news addresses a gap in public knowledge about how advanced AI models are vetted before public release. Pre-deployment security testing is a key part of President Biden's 2023 executive order on AI, which required leading AI companies to share safety test results with the US government before releasing models that could pose national security risks. The Center for AI Standards and Innovation was established to coordinate these testing efforts.

**Tags**: `#AI regulation`, `#AI safety`, `#US government`, `#tech policy`, `#government transparency`

---

<a id="item-32"></a>
## [SpaceX in Talks with Google for Orbital Data Center Launches](https://www.wsj.com/tech/spacex-google-in-talks-to-explore-data-centers-in-orbit-7b7799e2) ⭐️ 7.0/10

Google is in talks with SpaceX to use SpaceX rockets to launch satellites for Project Suncatcher, Google's orbital data center initiative planned for launch by 2027. Google has also partnered with Planet Labs to develop these satellites. This partnership represents a significant convergence of space technology, cloud computing, and AI infrastructure, potentially opening a new computing paradigm for AI and cloud services. SpaceX is positioning orbital data centers as a key pitch for its upcoming summer IPO, making this deal strategically important for both companies. Project Suncatcher was announced by Google last year with plans to launch prototype satellites by 2027. SpaceX recently signed a deal with Anthropic to provide 300 MW of compute power and over 220,000 Nvidia GPUs by the end of May, demonstrating the massive infrastructure requirements for AI training.

telegram · zaihuapd · May 12, 16:28

**Background**: Orbital data centers are computing facilities placed in space, typically in low Earth orbit, that could offer advantages like reduced latency for global coverage and access to solar energy. SpaceX has been expanding beyond rocket launches into satellite internet (Starlink) and broader space infrastructure services. This represents a convergence of the space industry with cloud computing and AI infrastructure.

**Tags**: `#space-technology`, `#orbital-data-center`, `#spacex`, `#google-cloud`, `#ai-infrastructure`

---