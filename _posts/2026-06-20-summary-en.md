---
layout: default
title: "Horizon Summary: 2026-06-20 (EN)"
date: 2026-06-20
lang: en
---

> From 161 items, 13 important content pieces were selected

---

1. [Nobel-Winner John Jumper Leaves DeepMind for Anthropic](#item-1) ⭐️ 9.0/10
2. [Norway Imposes Near-Ban on AI in Elementary Schools](#item-2) ⭐️ 8.0/10
3. [Project Valhalla Arrives in JDK 28 After Decade of Development](#item-3) ⭐️ 8.0/10
4. [There Are No Instances in ATProto](#item-4) ⭐️ 7.0/10
5. [AWS Launches Web Search for Amazon Bedrock AgentCore](#item-5) ⭐️ 7.0/10
6. [US Government Ban on Anthropic Models Sparks Debate](#item-6) ⭐️ 7.0/10
7. [US Bans Anthropic's Fable 5 and Mythos 5 Models](#item-7) ⭐️ 7.0/10
8. [Subquadratic Claims Breakthrough in LLM Computational Bottleneck](#item-8) ⭐️ 7.0/10
9. [First Long-Term BCI Power User After Three Years](#item-9) ⭐️ 7.0/10
10. [AlphaFold Creator John Jumper Joins Anthropic](#item-10) ⭐️ 7.0/10
11. [Anthropic Pauses Token-Based Billing for Claude Agent SDK](#item-11) ⭐️ 7.0/10
12. [US Pressures ASML Over Alleged EUV Machine Flow to China](#item-12) ⭐️ 7.0/10
13. [SpaceX Pre-IPO Chinese Investor Sales Revealed](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Nobel-Winner John Jumper Leaves DeepMind for Anthropic](https://www.businessinsider.com/alphafold-john-jumper-leaves-google-deepmind-anthropic-demis-hassabis-nobel-2026-6) ⭐️ 9.0/10

John Jumper, the lead scientist behind AlphaFold who won a Nobel Prize, has departed from Google DeepMind to join Anthropic, marking a significant talent move in the AI industry. This represents a major talent acquisition as Jumper is one of the most accomplished AI researchers in protein structure prediction. His departure highlights the intense competition for top AI talent among leading AI labs and signals Anthropic's ambitions in scientific AI applications. Jumper led the team that developed AlphaFold, which solved the decades-old protein folding problem using deep learning. AlphaFold can predict protein structures in minutes with remarkable accuracy, a breakthrough that has transformed computational biology.

rss · Hacker News - AI / LLM / Agent · Jun 20, 01:45

**Background**: The protein folding problem refers to the challenge of predicting a protein's 3D structure from its amino acid sequence. This has been a grand challenge in biology for 50 years. AlphaFold solved this problem in 2020 using attention-based deep learning networks trained on massive protein sequence databases. The breakthrough earned Jumper and Demis Hassabis the Nobel Prize in Chemistry in 2024.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Protein_folding">Protein folding - Wikipedia</a></li>
<li><a href="https://www.ebi.ac.uk/training/online/courses/alphafold/an-introductory-guide-to-its-strengths-and-limitations/what-is-the-protein-folding-problem/">What is the protein folding problem? | AlphaFold</a></li>
<li><a href="https://en.wikipedia.org/wiki/AlphaFold">AlphaFold - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI`, `#DeepMind`, `#Anthropic`, `#AlphaFold`, `#Talent Movement`, `#Nobel Prize`

---

<a id="item-2"></a>
## [Norway Imposes Near-Ban on AI in Elementary Schools](https://www.reuters.com/technology/norway-imposes-near-ban-ai-elementary-school-2026-06-19/) ⭐️ 8.0/10

Norway's government announced that students in first through seventh grade, aged 6 to 13, should generally not use AI tools, while students aged 14 to 16 in lower secondary school can cautiously adopt AI under teacher supervision. This represents a significant government policy decision that could set a precedent for other countries grappling with how to regulate AI in education. It directly affects millions of young students and their learning development during critical formative years. The policy distinguishes between elementary school students (ages 6-13) who should avoid AI entirely, and lower secondary students (ages 14-16) who may use AI tools with teacher oversight. The government cited concerns that generative AI does not help younger children develop fundamental reading, writing, and comprehension skills.

hackernews · ilreb · Jun 19, 16:03

**Background**: AI in education has become a globally contentious issue. Many educators report that AI has negatively impacted student learning outcomes and educator performance. Critics argue that AI acts as a 'shortcut' that produces finished-looking work without genuine understanding, similar to giving calculators to children before they learn arithmetic.

**Discussion**: The overall sentiment in the discussion is supportive of the policy. Commenters agree that children under 13 need to learn fundamental skills before using AI tools, comparing it to not giving calculators before understanding arithmetic. Some expressed concerns about enforcement challenges and implementation difficulties in practice.

**Tags**: `#AI policy`, `#education`, `#government regulation`, `#children and technology`, `#edtech`

---

<a id="item-3"></a>
## [Project Valhalla Arrives in JDK 28 After Decade of Development](https://www.jvm-weekly.com/p/project-valhalla-explained-how-a) ⭐️ 8.0/10

Project Valhalla, Java's decade-long value types initiative, is finally arriving in JDK 28. The feature enables memory optimization through flattened arrays and inline types, allowing values to be stored directly in arrays without object headers or pointers. 这代表了 Java 处理数据结构的根本性转变，可实现显著的内存节省和性能提升。对于使用大量小对象的应用程序，差异可能很大，因为 JVM 现在可以将值密集地存储在连续内存中，无需每个元素的头部。 Value types (formerly inline classes) give up the ability to have identity, enabling the JVM to store values directly in arrays without object headers. The flattened array layout stores values contiguously—8 bytes per point (plus potential null flag)—with no headers per element and no pointers, allowing dense memory layout.

hackernews · philonoist · Jun 19, 06:35

**Background**: Project Valhalla began around 2014 as an effort to bring value types to Java. Unlike regular reference types, value types are compared by their bit patterns rather than identity, allowing the JVM to optimize memory layout. Brian Goetz, the engineer behind Project Valhalla, suggested operator overloading could be added after value types. The project addresses the fundamental overhead of object headers in Java's heap-based memory model.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Project_Valhalla_(Java_language)">Project Valhalla ( Java language) - Wikipedia</a></li>
<li><a href="https://www.infoq.com/articles/inline-classes-java/">A First Look at Java Inline Classes - InfoQ</a></li>
<li><a href="https://stackoverflow.com/questions/29591897/what-are-value-types-from-project-valhalla">java - What are Value Types from Project Valhalla ? - Stack Overflow</a></li>

</ul>
</details>

**Discussion**: Comments show appreciation for the hard work, but also debates about memory layout accuracy—one commenter noted the Point example in the article appears to be at least 65 bits (two 32-bit ints), questioning how heap flattening works for objects exceeding 64-bit representations. Others defend Java's evolution, arguing the language has made significant progress since JDK 8 and the work represents great progress.

**Tags**: `#Project Valhalla`, `#Java JVM`, `#Value Types`, `#Memory Optimization`, `#JDK 28`

---

<a id="item-4"></a>
## [There Are No Instances in ATProto](https://overreacted.io/there-are-no-instances-in-atproto/) ⭐️ 7.0/10

Dan Abramov explains that the concept of 'instances' is a category error when applied to ATProto (Bluesky's decentralized protocol), as it uses a fundamentally different architecture based on Relays, AppViews, and PDSes rather than the server-centric model of Mastodon's ActivityPub. This matters because many people mistakenly ask 'where are all the Bluesky instances?' - treating ATProto like Mastodon. Understanding this architectural difference is crucial for properly comparing decentralized social network protocols and making informed decisions about which ecosystem to participate in. ATProto breaks down into three distinct services: PDSes (Personal Data Servers) store user data, Relays shuttle data between services for performance, and AppViews aggregate content for consumption. Each service has independent scaling demands - unlike Mastodon where each instance handles everything. In practice, Bluesky (the corporation) runs the main AppView and hosts almost all user data, making the system more centralized in practice than the protocol design might suggest.

hackernews · danabramov · Jun 19, 15:10

**Background**: AT Protocol (ATProto) is a decentralized social networking protocol developed by Bluesky, distinct from ActivityPub used by Mastodon. While ActivityPub uses a server-centric federation model where each instance hosts its own users and communicates with other instances, ATProto uses a relay-based distribution model where content is published to relays for distribution rather than direct server-to-server communication. This architectural difference fundamentally changes how 'decentralization' works in each system.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AT_Protocol">AT Protocol - Wikipedia</a></li>
<li><a href="https://atproto.com/guides/overview">Protocol Overview - AT Protocol</a></li>
<li><a href="https://en.wikipedia.org/wiki/ActivityPub">ActivityPub - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News上的讨论（194条评论）显示出真诚的技术分歧。批评者认为RSS类比不成立，因为RSS博客是自给自足的，而ATProto的AppView严重依赖Relay。其他人则称赞这种架构是"美丽的解决方案"，但指出实际上Bluesky控制着大部分基础设施。总体情绪是，虽然协议在技术上是去中心化的，但生态系统仍然围绕Bluesky的服务集中化。

**Tags**: `#ATProto`, `#Bluesky`, `#Decentralized Social Networks`, `#Protocol Architecture`, `#ActivityPub`

---

<a id="item-5"></a>
## [AWS Launches Web Search for Amazon Bedrock AgentCore](https://aws.amazon.com/blogs/machine-learning/introducing-web-search-on-amazon-bedrock-agentcore/) ⭐️ 7.0/10

Web Search on Amazon Bedrock AgentCore is now generally available. This new capability enables AI agents to conduct web searches as part of their agentic workflows, allowing them to access real-time information from the internet. This feature significantly enhances AI agents' ability to retrieve current information from the web, making them more useful for tasks requiring real-time data, research, or external knowledge. Developers building AI applications on AWS can now create more capable and versatile agents with just a few lines of code. The Web Search capability can be wired into AgentCore with a few lines of code, making integration straightforward. This feature is part of Amazon Bedrock AgentCore's broader platform for building, deploying, and operating production-ready AI agents at scale.

rss · AWS Machine Learning Blog · Jun 19, 14:15

**Background**: Amazon Bedrock AgentCore is an agentic platform for building, deploying, and operating highly effective AI agents securely at scale using any framework and foundation model. It enables agents to take actions across tools and data with the right permissions and governance. The platform supports various use cases and provides deterministic controls to actively block unauthorized agent actions.

<details><summary>References</summary>
<ul>
<li><a href="https://aws.amazon.com/bedrock/agentcore/">Amazon Bedrock AgentCore - AWS</a></li>
<li><a href="https://docs.aws.amazon.com/bedrock-agentcore/latest/devguide/what-is-bedrock-agentcore.html">Overview - Amazon Bedrock AgentCore</a></li>

</ul>
</details>

**Tags**: `#Amazon Bedrock`, `#AWS`, `#AI Agents`, `#Machine Learning`, `#Cloud Computing`

---

<a id="item-6"></a>
## [US Government Ban on Anthropic Models Sparks Debate](https://techcrunch.com/video/is-the-us-governments-anthropic-ban-accidentally-helping-the-brand/) ⭐️ 7.0/10

The US government forced Anthropic to pull its two newest models, Fable 5 and Mythos 5, citing national security concerns after Amazon researchers allegedly discovered a way to bypass Fable 5's guardrails. This ban raises critical questions about government authority over AI model releases and whether regulatory actions paradoxically boost brand visibility for the affected company, as the incident has generated significant media attention. Cybersecurity researchers have signed an open letter calling the ban dangerous, noting that the same jailbreak methods discovered by Amazon researchers also work on other AI models from different providers.

rss · TechCrunch AI · Jun 19, 16:08

**Background**: AI guardrails are technical mechanisms that control LLM outputs by filtering or constraining responses to prevent harmful content. Red teaming in AI safety refers to adversarial testing where researchers intentionally try to bypass safety measures to identify vulnerabilities before deployment. The practice helps developers understand what their AI systems can do, including unintended capabilities they may not have intended to enable.

<details><summary>References</summary>
<ul>
<li><a href="https://www.actionai.co/posts/llm-guardrails-technical-guide">LLM Guardrails : Technical Guide to Controlling LLM Outputs | ActionAI</a></li>
<li><a href="https://ea-crux-project.vercel.app/knowledge-base/responses/red-teaming/">Red Teaming | LongtermWiki</a></li>

</ul>
</details>

**Discussion**: The cybersecurity research community has expressed concern that government-mandated model removals could set a dangerous precedent for regulatory overreach, while also questioning whether such bans actually improve safety or merely create performative security theater.

**Tags**: `#AI regulation`, `#Anthropic`, `#US government`, `#national security`, `#tech policy`

---

<a id="item-7"></a>
## [US Bans Anthropic's Fable 5 and Mythos 5 Models](https://techcrunch.com/podcast/the-us-banned-anthropics-fable-5-release-but-the-numbers-dont-seem-to-care/) ⭐️ 7.0/10

The US government forced Anthropic to withdraw its two newest models, Fable 5 and Mythos 5, citing national security concerns after Amazon researchers allegedly found a way to bypass Fable 5's guardrails. This represents a significant regulatory development in the AI industry, as it's one of the few times the US government has directly banned a specific AI model. This could set a precedent for future AI safety regulations. The ban came after Amazon researchers discovered a method to bypass Fable 5's safety guardrails. Cybersecurity researchers have signed an open letter calling the move dangerous, and Anthropic noted that similar jailbreaks exist in other models across the industry.

rss · TechCrunch AI · Jun 19, 16:01

**Background**: Anthropic is an AI safety company focused on building helpful, harmless, and honest AI systems. Their models include safety guardrails designed to prevent harmful outputs. 'Jailbreaking' refers to techniques that bypass these safety measures. The US government has increasingly scrutinized AI models for potential national security risks.

**Discussion**: Cybersecurity researchers have signed an open letter calling the government ban dangerous, arguing that similar jailbreaks exist across other AI models. This raises questions about whether the ban was proportionate or if it sets a concerning precedent for government intervention in AI development.

**Tags**: `#AI regulation`, `#Anthropic`, `#government policy`, `#AI safety`, `#model bans`

---

<a id="item-8"></a>
## [Subquadratic Claims Breakthrough in LLM Computational Bottleneck](https://www.technologyreview.com/2026/06/19/1139313/a-startup-claims-it-broke-through-a-bottleneck-thats-holding-back-llms/) ⭐️ 7.0/10

Miami-based AI startup Subquadratic emerged from stealth mode in June 2026, claiming to have solved a mathematical bottleneck that has constrained large language models for nearly a decade. The company has begun sharing technical details to substantiate its claims, though significant skepticism remains in the AI community. If verified, this breakthrough could dramatically accelerate LLM training and inference speeds while reducing computational costs. The O(n²) complexity of self-attention has been a fundamental scalability limitation in transformer architectures since their 2017 introduction, affecting all modern LLMs including GPT-4 and Claude. The bottleneck being addressed is the quadratic computational complexity O(n²) of the self-attention mechanism in Transformers, where processing cost scales with the square of input sequence length. Subquadratic claims to have developed subquadratic-time algorithms that could reduce this complexity, though specific technical details remain thin and unverified.

rss · MIT Technology Review · Jun 19, 10:40

**Background**: The Transformer architecture, introduced in the landmark 2017 paper 'Attention Is All You Need', relies on self-attention as its core processing mechanism. This mechanism computes relationships between all token pairs in a sequence, resulting in O(n²) computational complexity that becomes a severe bottleneck for long sequences. Researchers have explored linear attention mechanisms and other optimizations to address this issue, making it one of the most active areas of AI infrastructure research.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Time_complexity">Time complexity - Wikipedia</a></li>
<li><a href="https://zenn.dev/sennsann99/articles/b30952ce102933">How Linear Attention Solves the $ O ( N ^2)$ Bottleneck</a></li>
<li><a href="https://mbrenndoerfer.com/writing/quadratic-attention-bottleneck-transformers-long-sequences">Quadratic Attention Bottleneck : Why Transformers Struggle with...</a></li>

</ul>
</details>

**Discussion**: AI界对迄今为止分享的薄弱技术细节普遍持怀疑态度。许多研究人员指出，突破基本计算复杂度壁垒的主张需要非凡的证据，而Subquadratic的早期披露尚未提供足够的数学严谨性来说服专家。讨论强调了雄心勃勃的初创公司说法与缓慢而严谨的学术验证之间的张力。

**Tags**: `#LLM optimization`, `#AI startup`, `#machine learning bottlenecks`, `#Subquadratic`, `#AI infrastructure`

---

<a id="item-9"></a>
## [First Long-Term BCI Power User After Three Years](https://www.technologyreview.com/2026/06/19/1139270/brain-computer-interface-trials-are-taking-off/) ⭐️ 7.0/10

Casey Harrell, a man with ALS who is paralyzed and unable to speak, has become the first long-term 'power user' of a brain-computer interface implant. He has now spent nearly three years using a BCI that enables him to communicate despite his paralysis. This milestone demonstrates the practical viability of brain implants for restoring communication in paralysis patients. It shows that BCI technology can work reliably over long periods in real-world settings, potentially helping thousands of patients with similar conditions. The intracortical BCI works by surgically implanting a microelectrode array into the motor cortex, where it records neural activity related to movement. Computer algorithms then decode these signals to translate the patient's intended speech into text or voice output.

rss · MIT Technology Review · Jun 19, 09:00

**Background**: Brain-computer interfaces (BCIs) are systems that create a direct communication pathway between the brain and external devices. Intracortical BCIs use surgically implanted electrodes to record neural signals from the motor cortex, which can then be decoded to control computers or communication devices. ALS (amyotrophic lateral sclerosis) is a progressive neurodegenerative disease that leads to paralysis and loss of speech, making BCIs potentially life-changing for patients who lose the ability to communicate.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Brain–computer_interface">Brain–computer interface - Wikipedia</a></li>
<li><a href="https://www.rnel.pitt.edu/research/neuroprosthetics/intracortical-brain-computer-interfaces">Intracortical Brain-Computer Interfaces | Rehabilitation and Neural Engineering Laboratory | University of Pittsburgh</a></li>

</ul>
</details>

**Tags**: `#brain-computer interface`, `#ALS`, `#medical technology`, `#neural implants`, `#assistive technology`

---

<a id="item-10"></a>
## [AlphaFold Creator John Jumper Joins Anthropic](https://twitter.com/JohnJumperSci/status/2068001285173834106) ⭐️ 7.0/10

John Jumper, the lead author of AlphaFold at Google DeepMind, has announced he is joining Anthropic, the AI safety company known for developing Claude. This marks a significant talent move from one of the most celebrated AI research teams to a leading AI safety organization. This recruitment represents a major win for Anthropic in the competitive AI talent landscape. As the creator of AlphaFold, Jumper brings unparalleled expertise in deep learning and scientific computing, potentially strengthening Anthropic's research capabilities in AI safety and alignment. AlphaFold revolutionized protein structure prediction by accurately predicting 3D protein structures from amino acid sequences, solving a 50-year-old grand challenge in biology. AlphaFold 2 won the 2020 CASP14 competition with unprecedented accuracy, and the team published their methods in Nature.

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Jun 19, 17:53

**Background**: AlphaFold is a deep learning system developed by Google DeepMind that predicts protein 3D structures from amino acid sequences. It uses an attention-based architecture called Evoformer to integrate evolutionary information. The system solved what was known as the 'protein folding problem' - one of the biggest challenges in computational biology. Anthropic is an AI safety company focused on developing beneficial AI systems and has been competing with OpenAI and Google for top AI talent.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Protein_folding">Protein folding - Wikipedia</a></li>
<li><a href="https://deepmind.google/science/alphafold/">AlphaFold — Google DeepMind</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion shows mixed reactions. Many commenters praised Jumper's incredible achievement with AlphaFold and viewed this as a positive move for AI safety research. Some expressed curiosity about what Jumper will work on at Anthropic, noting that this reflects the ongoing competition for top AI researchers between leading labs. A few comments questioned whether the AI safety focus at Anthropic was genuine or marketing.

**Tags**: `#AI industry`, `#Anthropic`, `#talent acquisition`, `#DeepMind`, `#personnel news`

---

<a id="item-11"></a>
## [Anthropic Pauses Token-Based Billing for Claude Agent SDK](https://arstechnica.com/ai/2026/06/anthropic-pauses-token-based-billing-for-its-claude-agent-sdk/) ⭐️ 7.0/10

Anthropic has temporarily paused token-based billing for its Claude Agent SDK, providing users a reprieve from the standard per-token pricing model that charges for both input and output tokens. This represents a potential major shift in AI API pricing models and could influence industry standards. The pause signals that Anthropic recognizes its existing subscriptions weren't designed for the usage patterns of AI agents, which consume significantly more tokens than traditional API usage. The pause is temporary—users should expect to bear the full costs of their extensive agent usage before long. In April, Anthropic's Head of Claude Code Boris Chen stated that their subscriptions weren't built for the usage patterns of these agentic tools, which typically make far more API calls than standard integrations.

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Jun 19, 16:59

**Background**: Token-based billing is the dominant pricing model in the AI API industry, measuring both input tokens (text sent to the model) and output tokens (text generated) for each API call, with separate rates applied to each. This model has been criticized for being difficult to predict and manage, especially for agents that make many continuous calls. Claude Agent SDK is the same infrastructure that powers Claude Code, Anthropic's agentic coding tool for developers.

<details><summary>References</summary>
<ul>
<li><a href="https://arstechnica.com/ai/2026/06/anthropic-pauses-token-based-billing-for-its-claude-agent-sdk/">Anthropic "pauses" token-based billing for its Claude Agent SDK</a></li>
<li><a href="https://www.anthropic.com/news/claude-sonnet-4-5">Introducing Claude Sonnet 4.5 \ Anthropic</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent , Terminal, IDE</a></li>

</ul>
</details>

**Tags**: `#anthropic`, `#claude`, `#pricing`, `#ai-business`, `#api-billing`

---

<a id="item-12"></a>
## [US Pressures ASML Over Alleged EUV Machine Flow to China](https://www.bloomberg.com/news/articles/2026-06-19/us-tells-asml-it-s-concerned-china-may-have-top-chip-tool) ⭐️ 7.0/10

US Commerce Secretary Lutnick expressed concern to ASML that a top-tier extreme ultraviolet (EUV) lithography machine may have reached China in violation of export controls. ASML denies this, stating it has never exported any EUV machines to China, and that none of the 314 EUV machines operating globally are in China. This represents a significant escalation in US-China tech tensions, as EUV lithography machines are critical for manufacturing advanced chips at 7nm and below. If confirmed, it would undermine US-led export control efforts and potentially accelerate China's semiconductor self-sufficiency drive. The dispute could also influence pending US legislation for stricter chip equipment restrictions. US高级官员声称掌握ASML未善意行事的证据，包括对华出口EUV相关运输设备，但拒绝出示证据。ASML已散发文件自证清白，强调从未出口任何EUV专用组件。此事加剧了美欧在芯片管制上的紧张关系。

telegram · zaihuapd · Jun 19, 03:09

**Background**: EUV lithography is the most advanced chip manufacturing technology, using 13.5nm extreme ultraviolet light to create intricate patterns on semiconductor wafers. ASML holds a monopoly on EUV systems, which are essential for producing chips at 7nm and below. The US has imposed export controls on EUV technology citing national security concerns, pressuring the Netherlands to restrict ASML's sales to China.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Extreme_ultraviolet_lithography">Extreme ultraviolet lithography - Wikipedia</a></li>
<li><a href="https://www.asml.com/en/products/euv-lithography-systems">EUV lithography systems – Products | ASML</a></li>

</ul>
</details>

**Tags**: `#ASML`, `#semiconductor`, `#EUV lithography`, `#US-China relations`, `#export controls`

---

<a id="item-13"></a>
## [SpaceX Pre-IPO Chinese Investor Sales Revealed](https://www.propublica.org/article/spacex-elon-musk-ipo-foreign-investors-china) ⭐️ 7.0/10

Court documents reveal SpaceX sold shares to Chinese, Hong Kong, and Russian investors through US intermediary Tomales Bay Capital before its recent IPO, with individual investments ranging from $800,000 to $40 million between 2018 and 2021. This matters because SpaceX later banned Chinese and Hong Kong investors from its IPO citing 'regulatory and compliance risks,' creating a stark contradiction with its earlier actions. The revelation raises serious questions about regulatory hypocrisy and potential securities law violations. The investors included individuals with ties to Chinese military contractors and Qatari royal family entities. Tomales Bay Capital promised investors special access including quarterly business updates, facility tours, and interviews with the CFO. SpaceX's valuation surged from $33.3 billion in 2019 to $2.7 trillion.

telegram · zaihuapd · Jun 19, 12:00

**Background**: SpaceX handles sensitive US military projects and operates under strict export control regulations. SEC Regulation D allows companies to raise capital from accredited investors without full public registration. The US has imposed various investment restrictions on China and Hong Kong citing national security concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fool.com/investing/how-to-invest/stocks/how-to-invest-in-spacex-stock/">Learn how to invest in SpaceX stock. | The Motley Fool</a></li>
<li><a href="https://raizer.app/investor/tomales-bay-capital">Tomales Bay Capital – VC Investor Profile & Insights</a></li>

</ul>
</details>

**Tags**: `#spacex`, `#ipo`, `#investor-regulation`, `#elon-musk`, `#securities-law`

---