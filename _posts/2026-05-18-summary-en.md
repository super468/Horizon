---
layout: default
title: "Horizon Summary: 2026-05-18 (EN)"
date: 2026-05-18
lang: en
---

> From 129 items, 11 important content pieces were selected

---

1. [Semble: Code Search Tool Using 98% Fewer Tokens than grep](#item-1) ⭐️ 8.0/10
2. [Native iOS Text Editing: TextKit 2 Performance vs SwiftUI Limitations](#item-2) ⭐️ 8.0/10
3. [Chang Xin Technology Files for STAR Market IPO with 719% Revenue Growth](#item-3) ⭐️ 8.0/10
4. [Maker Runs Debian on $80 RK3562 Budget Tablet](#item-4) ⭐️ 7.0/10
5. [Ibogaine Trials Show Promise for PTSD Treatment in Veterans](#item-5) ⭐️ 7.0/10
6. [Understanding TCP ECONNRESET Connection Resets](#item-6) ⭐️ 7.0/10
7. [AI Is a Technology, Not a Product](#item-7) ⭐️ 7.0/10
8. [GDS Recommends Keeping Public Sector Code Open by Default](#item-8) ⭐️ 7.0/10
9. [arXiv Bans Authors for One Year for Full AI-Written Papers](#item-9) ⭐️ 7.0/10
10. [Zero: Vercel's New Systems Language for AI Agents](#item-10) ⭐️ 7.0/10
11. [Polling Shows Growing Public Backlash Against AI Technology](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Semble: Code Search Tool Using 98% Fewer Tokens than grep](https://github.com/MinishLab/semble) ⭐️ 8.0/10

Stephan and Thomas have open-sourced Semble, a code search tool for AI agents that combines static Model2Vec embeddings (potion-code-16M) with BM25, fused via RRF and reranked with code-aware signals, achieving 98% token savings over grep while running entirely on CPU. This matters because AI coding agents like Claude Code frequently fall back to grep when direct code lookup fails, consuming excessive tokens while often still missing relevant code. Semble provides a token-efficient alternative that maintains near-transformer-level accuracy without needing GPUs or API keys. On a benchmark of ~1250 query/document pairs across 63 repos and 19 languages, Semble achieves 0.854 NDCG@10, reaching 99% of the retrieval quality of a 137M-parameter code-trained transformer while being ~200x faster. It indexes a typical repo in ~250ms and handles queries in ~1.5ms on CPU.

hackernews · Bibabomas · May 17, 15:37

**Background**: Model2Vec is a technique that converts sentence transformers into compact static embedding models by computing fixed token vectors and averaging them for sentence embeddings. BM25 (Best Matching 25) is a ranking function used in information retrieval that estimates document relevance based on term frequency and document length normalization. Reciprocal Rank Fusion (RRF) combines multiple ranked result sets into a unified relevance-optimized list without requiring tuning.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MinishLab/model2vec">GitHub - MinishLab/model2vec: Fast State-of-the-Art Static ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Okapi_BM25">Okapi BM25 - Wikipedia</a></li>
<li><a href="https://www.elastic.co/docs/reference/elasticsearch/rest-apis/reciprocal-rank-fusion">Reciprocal rank fusion</a></li>

</ul>
</details>

**Discussion**: Community members raised important concerns about model trust issues - agents heavily RL'd with grep may not trust alternative tool results and will keep retrying or re-reading, potentially losing token savings. There are also questions comparing Semble to LSPs, colgrep, and RTK, with requests for actual agent benchmarks rather than just retrieval metrics. Some users noted that semantic code search could be useful for human developers too, not just agents.

**Tags**: `#AI-coding-assistants`, `#code-search`, `#open-source`, `#token-optimization`, `#Model2Vec`

---

<a id="item-2"></a>
## [Native iOS Text Editing: TextKit 2 Performance vs SwiftUI Limitations](https://justsitandgrin.im/posts/native-all-the-way-until-you-need-text/) ⭐️ 8.0/10

A technical discussion explores why iOS native development still faces challenges with text editing despite TextKit 2's impressive performance benchmarks, with commenters sharing real-world metrics showing keystrokes processed in under 8ms and 20 rapid keystrokes completed in 150ms. 这很重要，因为开发者在iOS上构建富文本编辑器必须在高性能的原生TextKit 2和已显著成熟的Web技术之间做出选择。讨论显示，与具有GPU加速功能的成熟浏览器渲染引擎相比，SwiftUI在富文本、选择、流式更新和语法高亮方面仍然存在困难。 TextKit 2 enables 25x faster visible-range rendering than full-document styling, with tag and boolean searches completing in under 20ms. However, once developers need features like rich text, selection handling, streaming updates, syntax highlighting, diffing, or smooth scrolling, they end up fighting SwiftUI instead of building the app.

hackernews · dive · May 17, 11:49

**Background**: TextKit is Apple's text rendering framework for iOS and macOS, with TextKit 2 being a complete redesign to meet modern computing demands. SwiftUI is Apple's declarative UI framework, but it wraps underlying UITextView/NSTextView and cannot correctly recognize SwiftUI .Font without conversion. Tree-sitter is a parser tool used for syntax highlighting in code editors.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.apple.com/library/archive/documentation/StringsTextFonts/Conceptual/TextAndWebiPhoneOS/CustomTextProcessing/CustomTextProcessing.html">Using Text Kit to Draw and Manage Text</a></li>
<li><a href="https://fatbobman.com/en/posts/a-deep-dive-into-swiftui-rich-text-layout/">A Deep Dive into SwiftUI Rich Text Layout - Beyond AttributedString...</a></li>
<li><a href="https://cindori.com/developer/building-rich-text-editor">Building a rich text editor for UIKit, AppKit and SwiftUI</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that TextKit 2 delivers excellent performance, with msephton sharing benchmarks from a production text editor handling 5,000-line files. However, pornel argues browser rendering engines have matured with GPU acceleration, while instagary notes that building rich text features in SwiftUI quickly becomes fighting the framework. Wowfunhappy suggests WebKit is appropriate for Markdown views on macOS.

**Tags**: `#ios-development`, `#swiftui`, `#performance`, `#textkit`, `#mobile-engineering`

---

<a id="item-3"></a>
## [Chang Xin Technology Files for STAR Market IPO with 719% Revenue Growth](https://api3.cls.cn/share/article/2373399?os=android&amp;sv=8.7.8&amp;app=cailianpress) ⭐️ 8.0/10

Chang Xin Technology has filed for IPO on the Shanghai STAR Market (科创板), disclosing Q1 2026 results showing 508 billion yuan in revenue, a 719.13% year-over-year increase, and net profit of 330.1 billion yuan. The company forecasts H1 2026 revenue of 1100-1200 billion yuan with 520-580 billion yuan in non-gaap net profit. This represents a major development in China's domestic DRAM industry as Chang Xin Technology becomes one of the country's leading memory chip makers seeking public listing. The extraordinary financial results reflect the ongoing global DRAM supply shortage that has driven prices up 80-90% in Q1 2026 alone, marking a significant shift in the global memory market landscape. The company achieved a complete turnaround from 2025 losses to Q1 2026 non-gaap net profit of 263.4 billion yuan. Parent company net profit reached 247.6 billion yuan. The H1 2026 revenue forecast represents 612-677% year-over-year growth. According to industry analysis, the global DRAM supply gap is expected to extend through Q4 2027, creating a sustained supercycle in the memory market.

telegram · zaihuapd · May 17, 11:05

**Background**: The 科创板 (STAR Market) is China's Nasdaq-style technology board launched in 2019 to support domestic innovation and high-tech manufacturing. DRAM (Dynamic Random Access Memory) is a critical type of volatile memory used in data centers and consumer electronics. The current DRAM shortage stems from AI-driven HBM demand挤占 traditional DDR产能, combined with server replacement cycles and SSD demand growth, creating the most severe supply constraint in three decades.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/上海證券交易所科創板">上海证券交易所科创板 - 维基百科，自由的百科全书</a></li>
<li><a href="https://t.cj.sina.com.cn/articles/view/7746897562/1cdc0469a00101biy0">2025-2026年全球DRAM市场涨价趋势及原因分析__财经头条__新浪财经</a></li>
<li><a href="https://finance.sina.com.cn/money/fund/jjgsgd/2026-05-13/doc-inhxtzpe0720799.shtml">DRAM缺口或延续至27年四季度！芯片存储超级周期如何布局？_新浪财经_新浪网</a></li>

</ul>
</details>

**Tags**: `#IPO`, `#半导体`, `#DRAM`, `#科创板`, `#财报`

---

<a id="item-4"></a>
## [Maker Runs Debian on $80 RK3562 Budget Tablet](https://github.com/tech4bot/rk3562deb) ⭐️ 7.0/10

A maker successfully turned an $80 RK3562 Android tablet into a Debian Linux workstation, demonstrating that budget ARM hardware can run a full Linux desktop environment. This project highlights the potential for repurposing low-cost Android devices into functional Linux workstations, making computing more accessible and enabling hardware hacking education on a budget. The RK3562 is a quad-core ARM processor from Rockchip, and the tablet has 4GB of RAM. Community members note that with only 4GB RAM, users should expect limited web browsing (few tabs) and may benefit from lightweight desktop environments like WezTerm plus tmux.

hackernews · tech4bot · May 17, 13:16

**Background**: The RK3562 is a high-performance, low-power quad-core application processor by Rockchip commonly used in budget Android tablets. Debian is a popular Linux distribution known for stability and broad hardware support. Running Debian on ARM devices enables users to repurpose older or budget hardware for development and computing tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://datasheet4u.com/datasheet/Rockchip/RK3562-1543273">RK3562 - high-performance and low-power quad-core application processor | Rockchip Datasheet</a></li>
<li><a href="https://armbian.com/">Armbian — Optimized Linux for 300+ ARM Boards</a></li>

</ul>
</details>

**Discussion**: Community members discussed practical usability with 4GB RAM, suggesting lightweight solutions like WezTerm + tmux. One commenter asked about using AI for reverse engineering to help port postmarketOS to new devices. Another highlighted concerns about potential price increases if such hacks become popular, noting the Doogee U10 tablet is already becoming scarce.

**Tags**: `#linux`, `#hardware-hacking`, `# ARM`, `#debian`, `#embedded-systems`

---

<a id="item-5"></a>
## [Ibogaine Trials Show Promise for PTSD Treatment in Veterans](https://www.bbc.com/future/article/20260514-how-hallucinogenic-ibogaine-helps-veterans-overcome-ptsd) ⭐️ 7.0/10

Clinical trials on veterans suggest ibogaine, a hallucinogenic compound derived from the African shrub Tabernanthe iboga, could provide a new treatment for PTSD. The drug primarily acts on kappa-opioid receptors (KOR) rather than mu-opioid receptors (MOR). This is significant because PTSD affects approximately 4% of US men and 8% of US women annually, and current treatment options are limited. If proven safe and effective, ibogaine could address an urgent medical need for veterans and others suffering from treatment-resistant PTSD, representing a potential breakthrough in psychedelic medicine. Ibogaine acts as a weak agonist at mu-opioid receptors but primarily activates kappa-opioid receptors, potentially reducing opioid cravings without producing a euphoric high. However, ibogaine has been associated with multiple deaths, including cases in clinical trials under medical supervision, due to its direct interaction with the cardiac system as a side effect.

hackernews · bushwart · May 17, 12:03

**Background**: Ibogaine is a psychoactive alkaloid that exhibits complex pharmacology by interacting with multiple neurotransmitter systems, including opioid, serotonin, sigma, NMDA, and nicotinic acetylcholine receptors. Its metabolite noribogaine primarily acts as a serotonin reuptake inhibitor and kappa-opioid receptor agonist. Ibogaine has been investigated since the 1960s for treating opioid addiction and was once commercially marketed in some countries before being restricted due to safety concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ibogaine">Ibogaine - Wikipedia</a></li>
<li><a href="https://www.mindscaperetreat.com/news/ibogaine-clinical-trials-fda-2026">Ibogaine Clinical Trials & FDA Status in 2026: What Patients ...</a></li>
<li><a href="https://ibogainetreatmentguide.com/how-ibogaine-works/">How Ibogaine Works: Neuroscience, GDNF, & Mechanism of Action ...</a></li>
<li><a href="https://www.roothealing.com/post/unraveling-ibogaines-mechanisms-of-action-a-neuropharmacological-perspective">Unraveling Ibogaine's Mechanisms of Action: A ...</a></li>

</ul>
</details>

**Discussion**: Community comments raise significant safety concerns, with deaths occurring even in clinical trial settings under medical supervision. Critics argue that switching from mu-opioid to kappa-opioid receptor activation may simply substitute one opioid for another rather than truly treating addiction. Some also question the editorial focus on veterans rather than other major PTSD groups like assault survivors, suggesting the treatment could benefit a broader population.

**Tags**: `#PTSD`, `#ibogaine`, `#psychedelic-medicine`, `#veterans`, `#clinical-trials`

---

<a id="item-6"></a>
## [Understanding TCP ECONNRESET Connection Resets](https://movq.de/blog/postings/2026-05-05/1/POSTING-en.html) ⭐️ 7.0/10

A technical blog post investigates TCP ECONNRESET errors, examining the difference between RST and FIN packet behavior, lingering close patterns, and practical debugging tips for connection reuse issues in Go. This matters because TCP connection resets can cause application failures, timeouts, and data loss in networked services. Understanding RST versus FIN behavior helps developers debug connection issues more effectively, especially when connection reuse fails in high-traffic applications. The investigation quotes Linux kernel code referencing RFC 2525 section 2.17, which specifies that RST packets are sent when data is lost rather than using graceful FIN termination. The blog also addresses lingering close patterns and notes that discarding HTTP responses without reading them prevents Go from reusing connections.

hackernews · zdw · May 17, 17:09

**Background**: ECONNRESET is a Unix/Linux error indicating that a TCP connection was forcibly closed by the remote end sending a RST packet. Unlike FIN which performs a graceful 4-way handshake shutdown, RST immediately terminates the connection without acknowledging remaining data. The lingering close pattern involves calling shutdown with SHUT_WR after sending data, then draining incoming data before closing the socket to avoid generating unwanted RST packets.

<details><summary>References</summary>
<ul>
<li><a href="https://www.baeldung.com/cs/tcp-fin-vs-rst">TCP: Differences Between FIN and RST - Baeldung</a></li>
<li><a href="https://ipwithease.com/tcp-fin-vs-rst-packets/">TCP FIN vs RST Packets: Know the Difference - IP With Ease</a></li>

</ul>
</details>

**Discussion**: The community comments highlight that the RST behavior is specified in RFC 2525 section 2.17 to avoid long wait times from graceful FIN closure. One commenter shared a similar Go debugging experience where discarding the HTTP response body prevented connection reuse—likely the same RST behavior occurred under the hood. Another suggested reading Apache's documentation on lingering close for additional context.

**Tags**: `#tcp`, `#networking`, `#socket-programming`, `#debugging`, `#linux-kernel`

---

<a id="item-7"></a>
## [AI Is a Technology, Not a Product](https://daringfireball.net/2026/05/ai_is_technology_not_a_product) ⭐️ 7.0/10

John Gruber argues that AI should be treated as an enabling technology (like Siri made functional) rather than as a standalone product, echoing the 'Dropbox is a feature not a product' logic. This matters because it challenges the prevailing AI industry strategy of building standalone products, and instead suggests that AI companies should integrate their technology into existing ecosystems to avoid becoming disposable. Gruber references Steve Jobs' principle of 'working backwards from the customer experience' to explain why Apple has not prioritized AI as a standalone product in its roadmap, as differentiating technology from products is in Apple's DNA.

hackernews · ch_sm · May 17, 13:11

**Background**: The 'Dropbox is a feature not a product' argument originated from the observation that Dropbox had no ecosystem and survived only because no similar service existed at scale at the time. Similarly, Apple's product philosophy under Steve Jobs differentiated between underlying technologies and end-user products, focusing on customer experience rather than the technology itself.

**Discussion**: The community largely agrees with Gruber's assessment. Commenters note that Apple's ideal AI implementation would be making Siri actually work properly for everyday tasks like setting calendar events or running shortcuts without needing magic words. Others draw parallels to Dropbox's ecosystem challenge, warning that AI companies must build their own ecosystems to become less disposable, much like how all major AI companies are currently attempting to do.

**Tags**: `#AI strategy`, `#product philosophy`, `#Apple`, `#technology vs product`, `#tech industry analysis`

---

<a id="item-8"></a>
## [GDS Recommends Keeping Public Sector Code Open by Default](https://simonwillison.net/2026/May/17/gds-weighs-in/#atom-everything) ⭐️ 7.0/10

The UK Government Digital Service published guidance on May 14th recommending that public sector organizations keep code "open by default," directly countering the NHS's recent decision to close their open source repositories following security vulnerabilities discovered through Project Glasswing. This represents a significant UK government policy development with major implications for the open source debate in public sector technology. The GDS guidance adds substantive authority to the open source community's position and may influence other government agencies' decisions on code sharing. The GDS guidance explicitly states that "making everything private adds additional delivery and policy costs, and can reduce reuse and scrutiny," recommending that openness should remain the default posture with closure used "sparingly and deliberately." While NHS is not mentioned by name, the timing and context make the counter-position clear.

rss · Simon Willison · May 17, 15:59

**Background**: Project Glasswing was a security research initiative that discovered vulnerabilities in NHS systems. In response, NHS decided to close access to their open source code repositories—which the community criticized as a disproportionate reaction. The UK Government Digital Service is the central agency responsible for digital services across the UK government, and their guidance carries significant policy weight.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/May/17/gds-weighs-in/">GDS weighs in on the NHS's decision to retreat from Open Source</a></li>
<li><a href="https://www.periculo.co.uk/cyber-security-blog/project-glasswing-claude-mythos-nhs-cybersecurity">Project Glasswing and Claude Mythos: What AI-Powered ...</a></li>

</ul>
</details>

**Discussion**: Technology blogger Terence Eden interprets the GDS guidance as a "major escalation" in civil service terms, noting that while internal disagreements are common, it is extremely rare for such disputes to spill over into public. The open source community has largely welcomed the GDS position as an authoritative endorsement of open by default.

**Tags**: `#UK Government`, `#NHS`, `#Open Source`, `#Government Digital Service`, `#Cybersecurity`

---

<a id="item-9"></a>
## [arXiv Bans Authors for One Year for Full AI-Written Papers](https://techcrunch.com/2026/05/16/research-repository-arxiv-will-ban-authors-for-a-year-if-they-let-ai-do-all-the-work/) ⭐️ 7.0/10

arXiv announced a new policy that will ban authors for one year if they use AI to do all the work on their research papers. The policy specifically targets cases where AI has been used to completely replace human contribution in research submissions. This is significant because arXiv is one of the most influential research repositories in the academic world, hosting millions of preprints across physics, mathematics, computer science, and other fields. The policy represents a major stance on AI-generated content in scholarly publishing and could set a precedent for other academic platforms and journals. The policy targets papers where AI has been used to do 'all the work,' implying that some human oversight or contribution remains acceptable. The one-year ban is a significant deterrent for researchers who rely on arXiv for rapid dissemination of their work before formal peer review.

rss · Hacker News - AI / LLM / Agent · May 18, 01:27

**Background**: arXiv is a free, open-access preprint repository maintained by Cornell University, where researchers share papers before formal peer review. It has become essential for rapid communication in STEM fields. The rise of large language models (LLMs) like GPT-4 has sparked ongoing debates about AI's role in academic writing and research integrity across the scholarly community.

**Discussion**: There is minimal community engagement on this topic with only 1 point and 0 comments, indicating the news has not yet generated significant discussion within the Hacker News community.

**Tags**: `#academic-publishing`, `#ai-policy`, `#research-integrity`, `#arxiv`, `#plagiarism`

---

<a id="item-10"></a>
## [Zero: Vercel's New Systems Language for AI Agents](https://github.com/vercel-labs/zero) ⭐️ 7.0/10

Vercel Labs has released Zero, a systems programming language specifically designed for building lightweight, native AI agent tools. The language targets the development of small, efficient agent systems. This represents a rare new entrant in the systems programming language space, addressing a specialized need in the rapidly growing AI agent ecosystem. As AI agents become more prevalent, having a purpose-built language could significantly impact how developers build agentic applications. Zero is positioned as a 'systems language' meant for building the infrastructure and tools that power AI agents, rather than for general application development. It focuses on performance, low-level control, and generating small binaries suitable for agent workloads.

rss · Hacker News - AI / LLM / Agent · May 17, 23:45

**Background**: Systems programming languages like C, C++, Rust, and Go are typically used for building operating systems, compilers, and other low-level infrastructure. Vercel, known for Next.js and frontend deployment tools, expanding into AI agent tooling with a dedicated language shows the growing importance of the agent ecosystem in developer tooling.

**Tags**: `#programming-languages`, `#ai-agents`, `#vercel`, `#systems-programming`, `#developer-tools`

---

<a id="item-11"></a>
## [Polling Shows Growing Public Backlash Against AI Technology](https://www.axios.com/2026/05/17/ai-backlash-polling-sentiment) ⭐️ 7.0/10

Recent polling data reveals a significant surge in negative sentiment toward AI technology among the general public, marking a notable shift in public opinion. This growing AI backlash could significantly impact technology adoption rates, investment decisions, and regulatory policies, potentially slowing the deployment of AI systems across industries. The polling indicates a substantial portion of respondents expressing concerns about AI's societal impact, including job displacement, privacy risks, and the unchecked pace of AI development.

rss · Hacker News - AI / LLM / Agent · May 17, 21:23

**Background**: AI backlash refers to the growing public resistance and negative perception toward AI technologies, often driven by fears about automation replacing human jobs, concerns over AI-generated misinformation, and general anxiety about technology's role in society. This phenomenon mirrors historical patterns of technology resistance, such as the Luddite movement in early industrial Britain. Understanding these sentiment trends is crucial for companies developing AI products and policymakers crafting technology regulations.

**Discussion**: The 90 comments on Hacker News reveal engaged debate about AI adoption concerns. Readers discuss the cyclical nature of technology hype and backlash, with many noting that similar negative sentiments eventually gave way to adoption in cases like the internet and smartphones. Others emphasize legitimate concerns about AI safety, job impacts, and the need for thoughtful regulation versus dismissal of the backlash as mere technophobia.

**Tags**: `#AI sentiment`, `#public opinion`, `#AI backlash`, `#polling data`, `#technology adoption`

---