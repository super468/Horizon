---
layout: default
title: "Horizon Summary: 2026-05-03 (EN)"
date: 2026-05-03
lang: en
---

> From 120 items, 11 important content pieces were selected

---

1. [VS Code Auto-Inserting Copilot Co-Author Into Commits Without Consent](#item-1) ⭐️ 8.0/10
2. [Dav2d](#item-2) ⭐️ 8.0/10
3. [NetHack 5.0.0 Released After 37 Years](#item-3) ⭐️ 7.0/10
4. [California to Begin Ticketing Driverless Cars for Traffic Violations](#item-4) ⭐️ 7.0/10
5. [Roblox Stock Plummets 18% as Child Safety Measures Impact Bookings](#item-5) ⭐️ 7.0/10
6. [Refusal in Language Models Is Mediated by a Single Direction](#item-6) ⭐️ 7.0/10
7. [Academy Bars AI-Generated Actors and Scripts from Oscar Eligibility](#item-7) ⭐️ 7.0/10
8. [CISA, NSA & Five Eyes Publish Joint Security Guide for AI Agent Deployment](#item-8) ⭐️ 7.0/10
9. [OpenAI o1 Outperforms Doctors in ER Triage Diagnosis Trial](#item-9) ⭐️ 7.0/10
10. [White House Opposes Anthropic Expanding Mythos AI Access](#item-10) ⭐️ 7.0/10
11. [Super PAC Pays TikTok Influencers to Spread China AI Threat Narrative](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [VS Code Auto-Inserting Copilot Co-Author Into Commits Without Consent](https://github.com/microsoft/vscode/pull/310226) ⭐️ 8.0/10

VS Code automatically adds 'Co-Authored-by Copilot' footer to git commits even when developers have not used Copilot AI assistance. This was caused by a configuration schema change that set the default to 'all', but the runtime fallback in repository.ts still calls config.get('addAICoAuthor', 'off'), creating an inconsistent behavior where the feature triggers regardless of actual usage. 这很重要，因为git提交是代码作者身份的法律和技术记录。未经同意自动插入AI合著信息会伪造提交历史，侵蚀开发者信任，并可能为需要开发者来源证书(DCO)签名的项目带来责任问题。社区将此视为微软将AI品牌置于开发者诚信之上。 The technical inconsistency lies in the schema default being changed to 'all' while the runtime fallback still returns 'off', causing unexpected behavior. Notably, Copilot's own AI analysis on the PR recommended reverting the change, stating it creates inconsistency without behavioral benefit - a recommendation that was apparently ignored.

hackernews · indrora · May 2, 19:57

**Background**: Git commits can contain multiple authors through the 'Co-Authored-By' trailer format, which GitHub recognizes and displays in commit history. The Developer Certificate of Origin (DCO) is a per-commit sign-off requirement used by many open source projects stating contributors have the right to submit their contribution. Falsifying authorship without consent undermines both these standards.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/creating-a-commit-with-multiple-authors">Creating a commit with multiple authors - GitHub Docs</a></li>
<li><a href="https://developercertificate.org/">Developer Certificate of Origin</a></li>
<li><a href="https://wiki.linuxfoundation.org/dco">Developer Certificate of Origin (DCO) - Linux Foundation</a></li>

</ul>
</details>

**Discussion**: The community discussion shows strong backlash, with developers comparing this to the invasive 'Sent from my iPhone' phenomenon but worse since commits are legal records. Critics condemn Microsoft for prioritizing AI branding over developer trust after spending decades rebuilding its reputation. One commenter who approved the PR has publicly apologized. The sentiment is overwhelmingly negative, with many seeing this as a betrayal of the developer-friendly VS Code legacy.

**Tags**: `#vscode`, `#copilot`, `#git`, `#developer-trust`, `#ai-ethics`

---

<a id="item-2"></a>
## [Dav2d](https://code.videolan.org/videolan/dav2d) ⭐️ 8.0/10

dav2d is a new open-source AV2 video decoder from VideoLAN claiming to be the fastest implementation across all platforms, released as the upcoming AV2 codec promises 30% better compression than AV1

hackernews · dabinat · May 2, 17:32

**Tags**: `#video-codec`, `#AV2`, `#open-source`, `#performance-optimization`, `#video-streaming`

---

<a id="item-3"></a>
## [NetHack 5.0.0 Released After 37 Years](https://nethack.org/v500/release.html) ⭐️ 7.0/10

NetHack 5.0.0 has been released as a major version update, replacing the legacy yacc and lex-based build tools (including the level compiler, dungeon compiler, and makedefs utility) with Lua-based alternatives that are loaded and processed by the game during play. This represents a fundamental architectural shift for a game that has existed since 1987, moving from traditional compiler tools to an embedded scripting language. The change enables more flexible modding and tooling, but breaks compatibility with saved games from previous versions, affecting long-time players who have invested years in completing the game. Saved games and bones files from earlier versions will not work with NetHack 5.0.0. NetHack predates Lua (which has been around since 1993), making this replacement truly the end of an era. The new Lua API also exposes map generation logic and other data for third-party tooling and forks.

hackernews · rsaarelm · May 2, 18:03

**Background**: NetHack is a classic roguelike game first released in 1987, known for its extreme difficulty and procedural dungeon generation. Roguelike games are turn-based RPGs featuring tile-based exploration, permadeath, and procedurally generated levels. The Berlin Interpretation in 2008 codified roguelike elements using games like Rogue, NetHack, and Angband as reference points.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Roguelike">Roguelike - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/List_of_roguelikes">List of roguelikes - Wikipedia</a></li>
<li><a href="https://libregamewiki.org/Roguelike_games">Roguelike games - Libregamewiki</a></li>

</ul>
</details>

**Discussion**: Community reactions mix nostalgia with technical appreciation. Long-time players express excitement about finishing their decade-old save files, but frustration that these saves won't work with 5.0.0. Developers and modders welcome the Lua transition as enabling new tooling and forks, with one calling it 'truly the end of an era' for the ancient yacc/lex build system.

**Tags**: `#NetHack`, `#roguelike`, `#game-development`, `#Lua`, `#legacy-software`

---

<a id="item-4"></a>
## [California to Begin Ticketing Driverless Cars for Traffic Violations](https://www.bbc.com/news/articles/clypjx3rg2go) ⭐️ 7.0/10

California will begin issuing traffic tickets to autonomous vehicles that violate traffic laws, marking a new regulatory approach to hold AVs accountable like human drivers. This is significant because it establishes clear accountability for autonomous vehicle companies, preventing them from using 'no driver' as a shield to escape responsibility for violations. It sets a precedent that could influence AV regulation globally and addresses public concerns about AVs blocking traffic lanes and violating traffic courtesies. The ticketing system will likely use the same traffic violation categories applied to human drivers, providing concrete data on specific AV behavioral issues. For example, Waymo vehicles have been observed blocking full lanes of traffic on busy streets rather than using quieter side streets—behaviors not captured by safety or crash statistics.

hackernews · geox · May 2, 17:59

**Background**: Autonomous vehicles (AVs) have been testing on California roads for years, but regulators have struggled with how to enforce traffic laws when there's no human driver to ticket. This new approach treats AV companies as responsible entities, similar to how corporations are held liable for other violations. California is a key testing ground for AV technology due to the presence of major companies like Waymo and Cruise.

**Discussion**: The discussion shows mixed sentiments—some commenters like the idea of tickets as improvement signals, while others are surprised this wasn't already implemented. Key concerns include holding AV executives criminally accountable for serious violations like vehicular manslaughter, preventing companies from treating fines as 'a cost of doing business,' and addressing practical issues like AVs blocking traffic lanes. One user questions why ticketing wasn't already happening when AVs were allowed on roads.

**Tags**: `#autonomous-vehicles`, `#regulation`, `#self-driving-cars`, `#california`, `#policy`

---

<a id="item-5"></a>
## [Roblox Stock Plummets 18% as Child Safety Measures Impact Bookings](https://www.cnbc.com/2026/05/01/roblox-rblx-stock-child-safety-earnings.html) ⭐️ 7.0/10

Roblox shares dropped 18% after the company introduced age-based communication restrictions and mandatory face verification for chat, measures designed to protect younger users but which investors fear will negatively impact bookings. This stock drop highlights the tension between short-term quarterly pressure and long-term product viability. Investors are concerned that restricting social interactions core to the platform could drive users away, while the company argues safety improvements are essential for sustainable growth. Under the new system, players are divided into six age groups (under 9, 9–12, 13–15, 16–17, 18–20, 21+), with users only able to communicate with others within ±1 age group. According to Roblox, 73% of age-checked daily active users were under 18, with 35% under 13 as of January 31.

hackernews · 1vuio0pswjnm7 · May 2, 17:10

**Background**: Bookings is Roblox's key financial metric representing total user spending on Robux (virtual currency) during a period, regardless of when revenue is recognized. For FY2025, Roblox reported $6.8 billion in bookings. The company takes a 30% cut of each Robux purchase, making bookings a critical indicator of platform health.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fool.com/investing/2026/02/11/roblox-sees-huge-bookings-growth-but-this-metric/">Roblox Sees Huge Revenue and Bookings Growth, But This Metric ...</a></li>
<li><a href="https://ir.roblox.com/news/news-details/2025/Roblox-Reports-Fourth-Quarter-and-Full-Year-2024-Financial-Results/default.aspx">Roblox Reports Fourth Quarter and Full Year 2024 Financial ...</a></li>
<li><a href="https://www.metricduck.com/blog/roblox-10k-analysis-bookings-losses-deferred-revenue">Roblox 10-K Analysis: $6.8 Billion in Bookings, $1.1 Billion ...</a></li>

</ul>
</details>

**Discussion**: Commenters broadly support the safety measures but critique the implementation. One user argues mandatory face verification is 'a solid technical solution that completely misses the human problems it creates.' Others note that nearly every game on Roblox is social, and the matchmaking system isn't mature enough to ensure all players in a lobby can communicate. Some defend investors, stating safety measures are necessary for long-term viability—without them, parents would stop allowing children on the platform.

**Tags**: `#roblox`, `#child-safety`, `#stock-market`, `#gaming-industry`, `#product-strategy`

---

<a id="item-6"></a>
## [Refusal in Language Models Is Mediated by a Single Direction](https://arxiv.org/abs/2406.11717) ⭐️ 7.0/10

Research finding that LLM refusal behavior is controlled by a single direction in the model's latent space, discussed on HN with additional context about later work and practical implications.

hackernews · fagnerbrack · May 2, 13:15

**Tags**: `#language-models`, `#model-alignment`, `#refusal-mechanisms`, `#abliteration`, `#ai-safety`

---

<a id="item-7"></a>
## [Academy Bars AI-Generated Actors and Scripts from Oscar Eligibility](https://techcrunch.com/2026/05/02/ai-generated-actors-and-scripts-are-now-ineligible-for-oscars/) ⭐️ 7.0/10

The Academy of Motion Picture Arts and Sciences has officially updated its eligibility rules to exclude AI-generated actors and scripts from Oscar consideration, marking a definitive stance on AI-created content in feature films. This policy change represents a watershed moment for the film industry, establishing a clear boundary that distinguishes human creative authorship from AI generation at the highest levels of cinematic recognition. It sends a strong signal to studios and creators about the Academy's commitment to preserving human artistic contribution. The specific criteria defining AI-generated content and the enforcement mechanism remain unclear. The brief reference to Tilly Norwood in the article suggests this may relate to a specific AI-generated film project or character that prompted this policy response.

rss · TechCrunch AI · May 2, 21:54

**Background**: The Academy of Motion Picture Arts and Sciences organizes the Oscars, the most prestigious film awards in the entertainment industry. Eligibility rules determine which films and creative contributions qualify for nomination and consideration. This new policy follows growing debates in Hollywood about the role of AI in filmmaking.

**Discussion**: 行业反应尚在形成中，但这一政策可能会在电影制作人、AI研究人员和制片厂之间引发关于什么是真正的创意 authorship 以及电影行业应如何适应不断发展的AI技术的重大争论。

**Tags**: `#AI in entertainment`, `#Oscars`, `#film industry`, `#AI policy`, `#Academy Awards`

---

<a id="item-8"></a>
## [CISA, NSA & Five Eyes Publish Joint Security Guide for AI Agent Deployment](https://cyberscoop.com/cisa-nsa-five-eyes-guidance-secure-deployment-ai-agents/) ⭐️ 7.0/10

The US CISA and NSA, along with the Five Eyes intelligence alliance countries (US, UK, Canada, Australia, New Zealand), have published a joint security guidance document for safely deploying AI agents in enterprise environments. This is significant because it represents the first authoritative government-level guidance specifically addressing AI agent security in enterprise settings. As AI agents become more autonomous and capable of taking actions on behalf of organizations, having clear security frameworks from trusted intelligence agencies becomes crucial for enterprise adoption. The guide provides best practices for securing AI agent workflows, managing RAG (Retrieval-Augmented Generation) security boundaries, and implementing governance frameworks for autonomous systems. It aims to help CTOs and enterprise security teams establish secure multi-agent workflows.

rss · Hacker News - AI / LLM / Agent · May 2, 21:10

**Background**: Five Eyes (FVEY) is an Anglosphere intelligence alliance comprising Australia, Canada, New Zealand, the United Kingdom, and the United States, formed under the multilateral UKUSA Agreement for joint signals intelligence cooperation. AI agents are autonomous software systems that can use AI models to reason, plan, and take actions on behalf of users, with enterprise deployments requiring careful security governance due to their ability to access sensitive data and execute tasks autonomously.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Five_Eyes">Five Eyes - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ai-agents/governance-security-across-organization">Governance and security for AI agents across the organization</a></li>

</ul>
</details>

**Tags**: `#ai-security`, `#government-guidance`, `#cisa`, `#five-eyes`, `#ai-agents`

---

<a id="item-9"></a>
## [OpenAI o1 Outperforms Doctors in ER Triage Diagnosis Trial](https://www.theguardian.com/technology/2026/apr/30/ai-outperforms-doctors-in-harvard-trial-of-emergency-triage-diagnoses) ⭐️ 7.0/10

OpenAI's o1 reasoning model correctly diagnosed 67% of ER patients in a Harvard trial, significantly beating triage doctors who achieved only 50-55% accuracy in the same conditions. This represents a major breakthrough in AI-assisted healthcare, potentially transforming emergency room operations by improving diagnostic accuracy and reducing misdiagnosis-related deaths. The findings suggest AI could serve as a powerful tool to support medical professionals in high-stakes triage decisions. The trial was conducted by Harvard Medical School researchers and used the o1 model's chain-of-thought reasoning capabilities to analyze patient symptoms and medical histories. The model processed information similarly to how doctors approach diagnostic reasoning, breaking down complex cases step by step.

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · May 3, 00:30

**Background**: Emergency room triage is the process of prioritizing patients based on the severity of their conditions when resources are limited. Triage nurses and doctors typically achieve 50-55% diagnostic accuracy due to time pressures and complex symptom presentations. OpenAI o1 is a reasoning-focused model that uses chain-of-thought prompting to improve accuracy on complex tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Triage">Triage - Wikipedia</a></li>
<li><a href="https://www.datacamp.com/blog/open-ai-o1">OpenAI o1 Guide: How It Works, Use Cases, API & More</a></li>

</ul>
</details>

**Tags**: `#AI in healthcare`, `#medical diagnosis`, `#emergency triage`, `#OpenAI o1`, `#AI benchmarking`

---

<a id="item-10"></a>
## [White House Opposes Anthropic Expanding Mythos AI Access](https://t.me/zaihuapd/41172) ⭐️ 7.0/10

The White House opposes Anthropic's proposal to expand access to the Mythos AI model from approximately 50 entities to about 120 entities, citing national security concerns and worries that the company's computing resources may not be able to meet the needs of both new entities and government users. This is significant because Mythos possesses sophisticated cybersecurity capabilities that can identify software vulnerabilities and potentially write exploit code. The expansion could expose these powerful capabilities to more entities, raising concerns about misuse or unintended security breaches. The decision also reflects the broader tension between AI development and national security regulation. Mythos was developed by Anthropic as part of its broader Claude AI system and was released in early April as 'Mythos Preview'. It was specifically designed for defensive cybersecurity tasks and has advanced vulnerability detection capabilities. Currently, the model is only accessible to critical infrastructure operators and some government agencies. There are two ongoing lawsuits related to this matter, and the Trump administration is attempting to expand government usage of the model.

telegram · zaihuapd · May 2, 01:48

**Background**: Anthropic is one of the leading AI companies, competing with OpenAI's ChatGPT and Google's Gemini. Mythos is their most advanced AI model to date, specifically designed for cybersecurity tasks. Because it can identify system vulnerabilities and write exploit code, Anthropic decided to withhold it from public release. The model was initially only available to critical infrastructure managers and certain government agencies. This controversy highlights the broader debate about AI safety, national security, and the regulation of advanced AI capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/crk1py1jgzko">What is Anthopic's Claude Mythos and what risks does it pose?</a></li>
<li><a href="https://www.cbc.ca/news/business/mythos-anthropic-ai-explainer-9.7171597">Anthropic 's latest AI model is sparking fears from... | CBC News</a></li>
<li><a href="https://www.anthropic.com/glasswing">Project Glasswing: Securing critical software for the AI era \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#Anthropic`, `#national security`, `#AI safety`, `#government policy`

---

<a id="item-11"></a>
## [Super PAC Pays TikTok Influencers to Spread China AI Threat Narrative](https://www.wired.com/story/super-pac-backed-by-openai-and-palantir-is-paying-tiktok-influencers-to-fear-monger-about-china/) ⭐️ 7.0/10

A Super PAC called "Leading the Future" connected to OpenAI and Palantir executives, funded through dark money organization "Build American AI", is paying TikTok and Instagram influencers around $5,000 per video to spread "China AI threat" messaging. This raises serious concerns about covert political influence operations in AI geopolitics, where dark money from tech executives is used to manipulate public opinion through social media influencers without transparent disclosure, potentially corrupting democratic discourse. The influencers are recruited by marketing agency SM4, who first promote US AI innovation and then directly frame China's technological rise as a threat to American jobs and privacy. Some influencers only label "advertisement" without disclosing the actual funding source.

telegram · zaihuapd · May 2, 02:43

**Background**: Super PACs are independent expenditure-only political committees in the United States that can raise and spend unlimited money to influence elections, but are not required to disclose their donors. "Dark money" refers to political spending where the source of the funding is not disclosed to the public. This specific case connects to the broader US-China tech rivalry narrative.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Super_PAC">Super PAC - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Dark_money">Dark money - Wikipedia</a></li>
<li><a href="https://www.opensecrets.org/dark-money/basics">Dark Money Basics - OpenSecrets</a></li>

</ul>
</details>

**Discussion**: While no direct community comments are available for this specific news item, this investigative report has raised concerns about transparency in political messaging and the potential influence of tech industry money on public discourse around AI geopolitics.

**Tags**: `#AI_geopolitics`, `#influence_operations`, `#dark_money`, `#US_China_tech_rivalry`, `#media_literacy`

---