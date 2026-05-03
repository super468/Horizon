---
layout: default
title: "Horizon Summary: 2026-05-03 (ZH)"
date: 2026-05-03
lang: zh
---

> From 120 items, 11 important content pieces were selected

---

1. [VS Code 未经同意自动插入 Copilot 合著信息到提交记录](#item-1) ⭐️ 8.0/10
2. [Dav2d](#item-2) ⭐️ 8.0/10
3. [NetHack 5.0.0 发布——历经 37 年重大更新](#item-3) ⭐️ 7.0/10
4. [加州将开始对自动驾驶违章车辆开罚单](#item-4) ⭐️ 7.0/10
5. [Roblox 股价暴跌 18%，儿童安全措施影响预订收入](#item-5) ⭐️ 7.0/10
6. [Refusal in Language Models Is Mediated by a Single Direction](#item-6) ⭐️ 7.0/10
7. [学院将 AI 生成的演员和剧本排除在奥斯卡参选资格之外](#item-7) ⭐️ 7.0/10
8. [CISA、NSA 与五眼联盟联合发布 AI Agent 安全部署指南](#item-8) ⭐️ 7.0/10
9. [OpenAI o1 在急诊室分诊诊断试验中胜过医生](#item-9) ⭐️ 7.0/10
10. [白宫反对 Anthropic 扩大 Mythos AI 模型使用范围](#item-10) ⭐️ 7.0/10
11. [超级 PAC 付费网红渲染中国 AI 威胁论](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [VS Code 未经同意自动插入 Copilot 合著信息到提交记录](https://github.com/microsoft/vscode/pull/310226) ⭐️ 8.0/10

VS Code 会自动在 git 提交中添加「Co-Authored-by Copilot」脚注，即使开发者根本没有使用 Copilot AI 辅助。这是由于配置架构默认值被改为「all」，但运行时 repository.ts 中的回退仍调用 config.get('addAICoAuthor', 'off')，导致行为不一致——无论是否实际使用 Copilot 都会触发此功能。 技术上的不一致在于架构默认被改为「all」，而运行时回退仍返回「off」，导致意外行为。值得注意的是，Copilot 自己的 AI 在 PR 上建议撤销更改，称其不会改变行为，只会造成为不一致——这一建议显然被忽视了。

hackernews · indrora · May 2, 19:57

**背景**: Git 提交可以通过「Co-Authored-By」 trailers 格式包含多位作者，GitHub 会在提交历史中识别并显示这些信息。开发者来源证书(DCO)是许多开源项目使用的逐提交签名的要求，声明贡献者有权提交他们的贡献。未经同意伪造作者身份会损害这两个标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/creating-a-commit-with-multiple-authors">Creating a commit with multiple authors - GitHub Docs</a></li>
<li><a href="https://developercertificate.org/">Developer Certificate of Origin</a></li>
<li><a href="https://wiki.linuxfoundation.org/dco">Developer Certificate of Origin (DCO) - Linux Foundation</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示强烈反对，开发者将此举比作更具侵犯性的「发自我的 iPhone」现象，但更糟的是因为提交是法律记录。批评者谴责微软在重建声誉数十年后优先考虑 AI 品牌而非开发者信任。批准该 PR 的一位评论者已公开道歉。情绪压倒性地负面，许多人认为这背叛了开发者友好的 VS Code 传统。

**标签**: `#vscode`, `#copilot`, `#git`, `#developer-trust`, `#ai-ethics`

---

<a id="item-2"></a>
## [Dav2d](https://code.videolan.org/videolan/dav2d) ⭐️ 8.0/10

dav2d is a new open-source AV2 video decoder from VideoLAN claiming to be the fastest implementation across all platforms, released as the upcoming AV2 codec promises 30% better compression than AV1

hackernews · dabinat · May 2, 17:32

**标签**: `#video-codec`, `#AV2`, `#open-source`, `#performance-optimization`, `#video-streaming`

---

<a id="item-3"></a>
## [NetHack 5.0.0 发布——历经 37 年重大更新](https://nethack.org/v500/release.html) ⭐️ 7.0/10

这对于一款自 1987 年就已存在的游戏来说，是一次根本性的架构转变，从传统编译器工具转向嵌入式脚本语言。这一变化使 MOD 制作和工具开发更加灵活，但破坏了与之前版本存档的兼容性，影响了投入多年时间通关游戏的老玩家。 早期版本的存档和骨架文件将无法在 NetHack 5.0.0 中使用。NetHack 比 Lua（1993 年出现）更早问世，此次替换真正标志着一个时代的终结。新的 Lua API 还暴露了地图生成逻辑和其他数据，供第三方工具和分支版本使用。

hackernews · rsaarelm · May 2, 18:03

**背景**: NetHack 是一款 1987 年首次发布的经典 roguelike 游戏，以极高难度和程序化生成的地城著称。Roguelike 游戏是回合制 RPG，具有基于瓦片的地探索、永久死亡和程序化生成的地城关卡。2008 年的《柏林解释》以 Rogue、NetHack 和 Angband 为参考，编纂了 roguelike 游戏的核心元素。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Roguelike">Roguelike - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/List_of_roguelikes">List of roguelikes - Wikipedia</a></li>
<li><a href="https://libregamewiki.org/Roguelike_games">Roguelike games - Libregamewiki</a></li>

</ul>
</details>

**社区讨论**: 社区反应将怀旧与技术赞赏融为一体。老玩家们对完成十几年前的存档感到兴奋，但沮丧的是这些存档无法在 5.0.0 版本中使用。开发者和 MOD 制作者欢迎 Lua 转型，认为这能带来新的工具和分支版本，有人称这是古老的 yacc/lex 构建系统「真正标志着一个时代的终结」。

**标签**: `#NetHack`, `#roguelike`, `#game-development`, `#Lua`, `#legacy-software`

---

<a id="item-4"></a>
## [加州将开始对自动驾驶违章车辆开罚单](https://www.bbc.com/news/articles/clypjx3rg2go) ⭐️ 7.0/10

这很重要，因为它为自动驾驶汽车公司建立了明确的责任机制，防止它们以“没有司机”为借口逃避违规责任。这一做法可能为全球自动驾驶汽车的监管树立先例，并解决了公众对自动驾驶汽车阻塞车道和违反交通礼仪的担忧。 罚单系统可能会采用与人类司机相同的交通违章分类，以提供关于自动驾驶汽车具体行为问题的具体数据。例如，Waymo 车辆被发现在繁忙街道上阻塞整条车道，而不是使用更安静的小路——这些行为在安全或碰撞统计数据中未被体现。

hackernews · geox · May 2, 17:59

**背景**: 自动驾驶汽车已在加州道路上测试多年，但监管机构一直苦于在没有人类司机的情况下如何执法。新方法将自动驾驶汽车公司视为责任实体，类似于公司因其他违规行为而被追究责任的方式。加州是自动驾驶技术的重要测试地，因为 Waymo 和 Cruise 等主要公司都位于该州。

**社区讨论**: 讨论中出现了不同的观点——一些评论者赞成将罚单作为改进信号，而另一些人则对这一做法之前未已实施感到惊讶。主要担忧包括对自动驾驶汽车公司高管在过失杀人等严重违规行为中进行刑事问责，防止公司将罚款视为“业务成本”，以及解决自动驾驶汽车阻塞车道等实际问题。一名用户质疑为什么在自动驾驶汽车获准上路时没有立即开始开罚单。

**标签**: `#autonomous-vehicles`, `#regulation`, `#self-driving-cars`, `#california`, `#policy`

---

<a id="item-5"></a>
## [Roblox 股价暴跌 18%，儿童安全措施影响预订收入](https://www.cnbc.com/2026/05/01/roblox-rblx-stock-child-safety-earnings.html) ⭐️ 7.0/10

在新系统下，玩家被分为六个年龄组（9 岁以下、9-12 岁、13-15 岁、16-17 岁、18-20 岁、21 岁以上），用户只能与±1 年龄组内的其他人交流。根据 Roblox 的数据，截至 1 月 31 日，73%的年龄验证日活跃用户未满 18 岁，其中 35%未满 13 岁。

hackernews · 1vuio0pswjnm7 · May 2, 17:10

**背景**: 预订收入是 Roblox 的关键财务指标，代表用户在特定时期内购买 Robux（虚拟货币）的总金额，无论该收入何时确认。2025 财年，Roblox 报告了 68 亿美元的预订收入。公司从每次 Robux 购买中抽取 30%的分成，使预订收入成为平台健康状况的关键指标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fool.com/investing/2026/02/11/roblox-sees-huge-bookings-growth-but-this-metric/">Roblox Sees Huge Revenue and Bookings Growth, But This Metric ...</a></li>
<li><a href="https://ir.roblox.com/news/news-details/2025/Roblox-Reports-Fourth-Quarter-and-Full-Year-2024-Financial-Results/default.aspx">Roblox Reports Fourth Quarter and Full Year 2024 Financial ...</a></li>
<li><a href="https://www.metricduck.com/blog/roblox-10k-analysis-bookings-losses-deferred-revenue">Roblox 10-K Analysis: $6.8 Billion in Bookings, $1.1 Billion ...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍支持安全措施，但批评实施方式。一位用户认为强制人脸验证是“一个完全忽略了其造成的人际问题的好技术方案”。其他人指出 Roblox 上几乎每款游戏都是社交性质的，而配对系统还不够成熟，无法确保大厅中的所有玩家都能交流。部分评论者为投资者辩护，表示安全措施对长期可行性是必要的——没有这些措施，家长就不会让孩子使用该平台。

**标签**: `#roblox`, `#child-safety`, `#stock-market`, `#gaming-industry`, `#product-strategy`

---

<a id="item-6"></a>
## [Refusal in Language Models Is Mediated by a Single Direction](https://arxiv.org/abs/2406.11717) ⭐️ 7.0/10

Research finding that LLM refusal behavior is controlled by a single direction in the model's latent space, discussed on HN with additional context about later work and practical implications.

hackernews · fagnerbrack · May 2, 13:15

**标签**: `#language-models`, `#model-alignment`, `#refusal-mechanisms`, `#abliteration`, `#ai-safety`

---

<a id="item-7"></a>
## [学院将 AI 生成的演员和剧本排除在奥斯卡参选资格之外](https://techcrunch.com/2026/05/02/ai-generated-actors-and-scripts-are-now-ineligible-for-oscars/) ⭐️ 7.0/10

美国电影艺术与科学学院已正式更新参选规则，将 AI 生成的演员和剧本排除在奥斯卡评选之外，明确了对 AI 创作内容在剧情片中的立场。 这一政策变化代表了电影行业的重要时刻，在电影最高荣誉层面上确立了人类创意 authorship 与 AI 生成之间的明确界限。它向制片厂和创作者发出了关于学院对保护人类艺术贡献之承诺的强烈信号。 目前尚不清楚界定 AI 生成内容的具体标准和执行机制。文章中简短提及 Tilly Norwood 表明这可能涉及某个引发此次政策响应的 AI 生成电影项目或角色。

rss · TechCrunch AI · May 2, 21:54

**背景**: 美国电影艺术与科学学院组织举办的奥斯卡奖是娱乐行业最具影响力的电影奖项。参选规则决定哪些电影和创意贡献符合提名和评选资格。这一新政策出台前，好莱坞关于 AI 在电影制作中角色的争论日益激烈。

**社区讨论**: 行业反应尚在形成中，但这一政策可能会在电影制作人、AI 研究人员和制片厂之间引发关于什么是真正的创意 authorship 以及电影行业应如何适应不断发展的 AI 技术的重大争论。

**标签**: `#AI in entertainment`, `#Oscars`, `#film industry`, `#AI policy`, `#Academy Awards`

---

<a id="item-8"></a>
## [CISA、NSA 与五眼联盟联合发布 AI Agent 安全部署指南](https://cyberscoop.com/cisa-nsa-five-eyes-guidance-secure-deployment-ai-agents/) ⭐️ 7.0/10

美国网络安全与基础设施安全局（CISA）和国家安全局（NSA）联合五眼情报联盟成员国（美国、英国、加拿大、澳大利亚、新西兰）发布了关于在企业环境中安全部署 AI Agent 的联合安全指南。 这具有重要意义，因为它代表了首个专门针对企业环境中 AI Agent 安全的权威政府级指导。随着 AI Agent 变得更加自主并能够代表组织采取行动，来自可信情报机构的明确安全框架对企业采用至关重要。 该指南提供了保护 AI Agent 工作流程的最佳实践，包括管理 RAG（检索增强生成）安全边界和为自主系统实施治理框架。其目标是帮助首席技术官和企业安全团队建立安全的多 Agent 工作流程。

rss · Hacker News - AI / LLM / Agent · May 2, 21:10

**背景**: 五眼联盟（FVEY）是一个由澳大利亚、加拿大、新西兰、英国和美国组成的情报联盟，根据多边《UKUSA 协议》建立，旨在进行信号情报合作。AI Agent 是自主软件系统，能够使用 AI 模型为用户进行推理、规划和执行操作，由于其访问敏感数据和自主执行任务的能力，企业部署需要谨慎的安全治理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Five_Eyes">Five Eyes - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ai-agents/governance-security-across-organization">Governance and security for AI agents across the organization</a></li>

</ul>
</details>

**标签**: `#ai-security`, `#government-guidance`, `#cisa`, `#five-eyes`, `#ai-agents`

---

<a id="item-9"></a>
## [OpenAI o1 在急诊室分诊诊断试验中胜过医生](https://www.theguardian.com/technology/2026/apr/30/ai-outperforms-doctors-in-harvard-trial-of-emergency-triage-diagnoses) ⭐️ 7.0/10

OpenAI 的 o1 推理模型在哈佛大学的一项试验中正确诊断了 67%的急诊室患者，显著优于在相同条件下仅达到 50-55%准确率的分诊医生。 急诊室分诊是在资源有限的情况下根据患者病情的严重程度进行分诊的过程。分诊护士和医生由于时间压力和复杂的症状表现，通常只能达到 50-55%的诊断准确率。OpenAI o1 是一个专注于推理的模型，使用思维链提示来提高复杂任务的准确性。 该试验由哈佛医学院研究人员进行，利用 o1 模型的思维链推理能力来分析患者症状和病史。该模型处理信息的方式与医生进行诊断推理的方式类似，逐步分解复杂的病例。

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · May 3, 00:30

**背景**: Emergency room triage is the process of prioritizing patients based on the severity of their conditions when resources are limited. Triage nurses and doctors typically achieve 50-55% diagnostic accuracy due to time pressures and complex symptom presentations. OpenAI o1 is a reasoning-focused model that uses chain-of-thought prompting to improve accuracy on complex tasks.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Triage">Triage - Wikipedia</a></li>
<li><a href="https://www.datacamp.com/blog/open-ai-o1">OpenAI o1 Guide: How It Works, Use Cases, API & More</a></li>

</ul>
</details>

**标签**: `#AI in healthcare`, `#medical diagnosis`, `#emergency triage`, `#OpenAI o1`, `#AI benchmarking`

---

<a id="item-10"></a>
## [白宫反对 Anthropic 扩大 Mythos AI 模型使用范围](https://t.me/zaihuapd/41172) ⭐️ 7.0/10

白宫反对 Anthropic 将 Mythos AI 模型的使用权限从约 50 家实体扩展至约 120 家的提议，以国家安全为由表示担忧，并担心该公司的算力无法同时满足新实体和政府用户的需求。 这一点非常重要，因为 Mythos 具备尖端的安全能力，能够发现软件漏洞并可能编写利用代码。扩展使用范围可能会将这些强大能力暴露给更多实体，引发对滥用或意外安全漏洞的担忧。该决定还反映了人工智能发展与国家安全监管之间更广泛的紧张关系。 Mythos 是由 Anthropic 作为其更广泛的 Claude AI 系统的一部分开发的，于 4 月初作为"Mythos Preview"发布。它专门为防御性网络安全任务设计，具有先进的漏洞检测能力。目前，该模型仅向关键基础设施运营商和部分政府机构开放。目前有两起与此事项相关的诉讼正在进行，特朗普政府正试图扩大政府对该模型的使用。

telegram · zaihuapd · May 2, 01:48

**背景**: Anthropic 是领先的 AI 公司之一，与 OpenAI 的 ChatGPT 和 Google 的 Gemini 竞争。Mythos 是他们迄今为止最先进的 AI 模型，专门为网络安全任务设计。由于该模型能够识别系统漏洞并编写利用代码，Anthropic 决定不向公众发布。该模型最初仅向关键基础设施管理方和部分政府机构开放。这一争议凸显了关于 AI 安全、国家安全和先进 AI 能力监管的更广泛辩论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/crk1py1jgzko">What is Anthopic's Claude Mythos and what risks does it pose?</a></li>
<li><a href="https://www.cbc.ca/news/business/mythos-anthropic-ai-explainer-9.7171597">Anthropic 's latest AI model is sparking fears from... | CBC News</a></li>
<li><a href="https://www.anthropic.com/glasswing">Project Glasswing: Securing critical software for the AI era \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#Anthropic`, `#national security`, `#AI safety`, `#government policy`

---

<a id="item-11"></a>
## [超级 PAC 付费网红渲染中国 AI 威胁论](https://www.wired.com/story/super-pac-backed-by-openai-and-palantir-is-paying-tiktok-influencers-to-fear-monger-about-china/) ⭐️ 7.0/10

一个由 OpenAI 和 Palantir 高管支持的超级 PAC"Leading the Future"，通过黑钱组织"Build American AI"资助，正在向 TikTok 和 Instagram 网红支付约 5000 美元/视频的费用，以传播"中国 AI 威胁论"。 这引发了对 AI 地缘政治领域隐性政治影响力操作的严重担忧，科技高管的黑钱被用于通过社交媒体网红操纵舆论，且未进行透明披露，这可能会腐蚀民主讨论。 网红由营销机构 SM4 招募，他们首先推广美国 AI 创新，然后再直接将中国技术崛起描述为对美国就业和隐私的威胁。一些网红仅标注"广告"而不披露实际资金来源。

telegram · zaihuapd · May 2, 02:43

**背景**: 超级 PAC 是美国独立的支出型政治行动委员会，可以筹集和支出无限资金来影响选举，但不需要披露其捐赠者。"黑钱"指的是政治支出中资金来源不对公众披露的情况。此案例与更广泛的中美科技竞争叙事相关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Super_PAC">Super PAC - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Dark_money">Dark money - Wikipedia</a></li>
<li><a href="https://www.opensecrets.org/dark-money/basics">Dark Money Basics - OpenSecrets</a></li>

</ul>
</details>

**社区讨论**: 虽然没有关于此具体新闻的直接社区评论，但这份调查报道引发了人们对政治信息透明度的担忧，以及科技行业资金对 AI 地缘政治公共讨论的潜在影响。

**标签**: `#AI_geopolitics`, `#influence_operations`, `#dark_money`, `#US_China_tech_rivalry`, `#media_literacy`

---