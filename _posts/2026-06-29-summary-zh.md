---
layout: default
title: "Horizon Summary: 2026-06-29 (ZH)"
date: 2026-06-29
lang: zh
---

> From 110 items, 12 important content pieces were selected

---

1. [OpenAI Codex 敏感文件泄露问题仍待解决](#item-1) ⭐️ 8.0/10
2. [检方在帕拉塞兹大火纵火案审判中使用 ChatGPT 日志作为证据](#item-2) ⭐️ 8.0/10
3. [Nathan Lambert 发布 RLHF 书籍 v0.10 版本，修复数学符号错误](#item-3) ⭐️ 7.0/10
4. [GLM 5.2 声称在网络安全基准测试中击败 Claude](#item-4) ⭐️ 7.0/10
5. [布朗大学教授揭露大规模 AI 考试作弊](#item-5) ⭐️ 7.0/10
6. [KIDS Act 要求在线平台进行年龄验证](#item-6) ⭐️ 7.0/10
7. [福特在 AI 表现不佳后重新聘用"灰胡子"工程师](#item-7) ⭐️ 7.0/10
8. [Bash4LLM：无外部依赖的轻量级 Bash LLM API 封装工具](#item-8) ⭐️ 7.0/10
9. [奥地利游说欧盟接纳 Anthropic 公司](#item-9) ⭐️ 7.0/10
10. [谷歌限制 Meta 使用 Gemini AI 模型](#item-10) ⭐️ 7.0/10
11. [中国在网络安全 AI 领域追平 Anthropic](#item-11) ⭐️ 7.0/10
12. [GitLab 19.0 将 Agentic AI 嵌入凭证、合并请求与供应链安全](#item-12) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI Codex 敏感文件泄露问题仍待解决](https://github.com/openai/codex/issues/2847) ⭐️ 8.0/10

社区意见分歧：一些人主张选择性文件访问和自定义沙盒解决方案，而 petcat 等人认为考虑到 LLM 不可预测的特性，黑名单机制会提供虚假安全，用户应依赖 chmod 等现有工具。skybrian 建议使用 ssh-agent 替代.env 文件作为更好的方案。

hackernews · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Jun 28, 12:27

**背景**: OpenAI Codex is an AI coding assistant that can browse files and execute tools on behalf of users. Data exfiltration refers to unauthorized transfer of data from a computer. Prompt injection is an exploit where malicious inputs cause unintended behavior in LLMs. These concepts combine when AI agents can be tricked or inadvertently access sensitive files.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://en.wikipedia.org/wiki/Data_exfiltration">Data exfiltration - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: The community shows divided opinions: some advocate for opt-in file access and custom sandboxing solutions, while others like petcat argue that blocklists would provide false security given LLMs' unpredictable nature and that users should rely on existing tools like chmod. skybrian suggests using ssh-agent instead of .env files as a better alternative.

**标签**: `#AI security`, `#OpenAI Codex`, `#prompt injection`, `#file exfiltration`, `#sandboxing`

---

<a id="item-2"></a>
## [检方在帕拉塞兹大火纵火案审判中使用 ChatGPT 日志作为证据](https://www.theverge.com/ai-artificial-intelligence/958751/prosecutors-chatgpt-palisades-wildfire-arson-mistrial) ⭐️ 8.0/10

此案标志着一个重要的法律先例，即人工智能对话日志被用作与洛杉矶最致命野火之一的刑事纵火案的证据。它引发了关于数字隐私、人工智能生成内容的认证，以及执法部门如何通过法律程序从人工智能公司获取用户数据的新问题。 执法部门可以通过针对 OpenAI 等公司的搜查令、法院命令或传票获取 ChatGPT 日志。法院通常需要元数据、保管链，有时还需要专家证词，以根据达伯特标准或弗赖伊标准确定真实性，并满足相关性、可靠性和第 403 条偏见担忧的要求。

rss · The Verge AI · Jun 28, 14:12

**背景**: 法律系统仍在制定处理人工智能生成证据的框架。法院通常要求人工智能证据满足相关性、认证和可靠性等核心要求。帕拉塞兹大火是洛杉矶历史上最具破坏性的野火之一，使此案特别引人注目人工智能日志的开创性使用更加重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.727defense.com/your-ai-conversations-are-not-private-how-law-enforcement-can-get-them-and-use-them-against-you/">Your AI Conversations Are Not Private: How Law Enforcement Can Get Them and Use Them Against You</a></li>
<li><a href="https://attorneys.media/when-ai-generated-evidence-is-admissible-in-court-and-when-it-isnt/">When AI-Generated Evidence Is Admissible in Court — and When It Isn’t</a></li>
<li><a href="https://www.thomsonreuters.com/en-us/posts/ai-in-courts/deepfakes-evidence-authentication/">Deepfakes on trial: How judges are navigating AI evidence authentication - Thomson Reuters Institute</a></li>

</ul>
</details>

**标签**: `#AI evidence`, `#legal proceedings`, `#ChatGPT`, `#wildfire`, `#criminal justice`

---

<a id="item-3"></a>
## [Nathan Lambert 发布 RLHF 书籍 v0.10 版本，修复数学符号错误](https://github.com/natolambert/rlhf-book/releases/tag/book/v0.10) ⭐️ 7.0/10

此版本对 LLM 对齐社区具有重要意义，因为它为实现 RLHF 系统的从业者和研究人员提供了重要的数学符号和推导修正。大幅扩展的配套课程材料使这成为学习后训练技术的更有价值的教育资源。 关键修正包括修复 Bradley-Terry 奖励模型损失推导，在取平均值之前取对数（第 5 章）、修正 DPO 梯度项中的 bare π → π_θ（第 8 章）、修复普通策略梯度方程中的 R_t / G_t 不一致、以及在第 6 章添加 PPO/GRPO 裁剪目标图。课程现在包含关于推理模型、DPO、合成数据的新内容以及扩展内容，还有深色模式网站。

github · natolambert · Jun 28, 17:42

**背景**: RLHF（来自人类反馈的强化学习）是将大型语言模型与人类偏好对齐的关键技术。Bradley-Terry 模型是通过建模成对偏好来训练 RLHF 中奖励模型的规范方法。GRPO（组相对策略优化）是一种简化的 RL 算法，通过使用组导出的基线来消除对单独价值函数模型的需求。这本书是学习 RLHF 实现的广泛使用的教育资源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datacamp.com/blog/what-is-grpo-group-relative-policy-optimization">What is GRPO? Group Relative Policy Optimization Explained | DataCamp</a></li>
<li><a href="https://rlhfbook.com/c/05-reward-models">Reward Modeling | RLHF and Post-Training Book by Nathan Lambert</a></li>
<li><a href="https://en.wikipedia.org/wiki/Reinforcement_learning_from_human_feedback">Reinforcement learning from human feedback - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 该版本在 AI 研究社区中受到广泛欢迎，有活跃的 Discord 社区和多项贡献被认可。数学推导的综合修正和扩展的课程材料展示了这一宝贵教育资源的持续维护。

**标签**: `#RLHF`, `#Reinforcement Learning`, `#LLM Alignment`, `#Educational Resources`, `#AI/ML`

---

<a id="item-4"></a>
## [GLM 5.2 声称在网络安全基准测试中击败 Claude](https://semgrep.dev/blog/2026/we-have-mythos-at-home-glm-52-beats-claude-in-our-cyber-benchmarks/) ⭐️ 7.0/10

智谱 AI 发布了 GLM 5.2，声称在网络安全基准测试中击败了 Claude。然而，社区讨论揭示了更为复杂的观点，部分用户提供了反驳证据，表明 DeepSeek 在他们自己的测试中表现优于 GLM。 这很重要，因为它凸显了开源 AI 模型与 Claude 等专有模型之间快速演变的竞争格局，并表明基准测试结果可能因测试方法和具体用例而显著不同。 GLM 5.2 是一个拥有 7530 亿参数、100 万上下文窗口的模型，针对编码、代理工作负载和超长周期任务进行了优化。一位用户指出硬件要求极高，使得本地部署具有挑战性，而另一位用户发现 DeepSeek V4 Pro 和 MiMo 2.5 Pro 在其安全漏洞狩猎基准测试中表现最佳。

hackernews · jms703 · Jun 28, 17:50

**背景**: 智谱 AI（又称 Z.ai）是一家位于北京的基础模型公司，2019 年从清华大学拆分出来。GLM-5.2 是他们最新的开源权重模型。网络安全基准测试如 CyberBattleSim 和 CyBench 评估 AI 模型在模拟网络环境中发现安全漏洞的能力。DeepSeek 模型采用 MIT 许可证，在 SWE-bench Verified 上以强大的编码性能著称。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.modular.com/models/glm-5-2">GLM - 5 . 2 | Modular</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://www.libertify.com/interactive-library/agentic-ai-cybersecurity-evolution-multi-agent-systems/">The Evolution of Agentic AI in Cybersecurity : From... | Libertify.com</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂但普遍对基准测试工作表示赞赏。一位重度用户（pimeys）确认 GLM-5.2 作为日常编程工作模型表现良好。另一位用户（SwellJoe）提供了反驳证据，表明 DeepSeek 在其安全漏洞狩猎中始终优于 GLM，并指出 DeepSeek 的卓越缓存性能。有些人对中国在特定网络类别中的潜在进步表示惊讶。

**标签**: `#AI`, `#LLM`, `#benchmarking`, `#machine-learning`, `#open-source-models`

---

<a id="item-5"></a>
## [布朗大学教授揭露大规模 AI 考试作弊](https://english.elpais.com/education/2026-06-28/ai-fraud-at-brown-university-academic-integrity-is-at-risk.html) ⭐️ 7.0/10

布朗大学的一位教授揭露了大规模 AI 考试作弊事件，学生使用大型语言模型完成考试题目，引发了严重的学术诚信危机，并促使人们广泛讨论如何调整大学评估方式以适应 AI 时代。 这一事件突显了全球大学在 AI 工具能够通过大多数标准考试后维护学术诚信所面临的紧迫挑战。它不仅影响布朗大学，还影响全球所有努力调整评估方法以检测和防止 AI 辅助作弊的教育机构。 该教授的研究领域是博弈论，评论者指出了博弈论式的讽刺——当所有竞争者都可能使用大型语言模型时，最佳策略选择就是使用它们。提议的解决方案包括现场纸质手写考试、设计对抗性课程确保学生学习目标得以实现（无论学生如何优化分数），以及一对一口头面试以验证学生的真实理解。

hackernews · geox · Jun 28, 16:41

**背景**: 像 GPT-4 这样的大型语言模型现在可以通过许多标准考试，使得传统的在线或带回家作业极易受到 AI 辅助的影响。这一技术颠覆已迫使全球大学重新考虑其评估策略，并寻求新方法来验证学生的学习成果和学术诚信。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tandfonline.com/doi/full/10.1080/14703297.2023.2190148">tandfonline.com/doi/full/10.1080/14703297.2023.2190148</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S2666659623000033">sciencedirect.com/science/article/pii/S2666659623000033</a></li>

</ul>
</details>

**社区讨论**: Hacker News 讨论区的观点多种多样：一些教授主张手写现场考试是唯一可靠的方法，而其他人提议设计对抗性课程，确保作业无论如何使用 AI 都能实现学习目标。一些评论者批判性地质疑传统评分系统在 AI 时代的相关性，指出分数早已膨胀，公司应该自己进行筛选。

**标签**: `#AI-education`, `#academic-integrity`, `#university-assessment`, `#educational-technology`, `#AI-cheating`

---

<a id="item-6"></a>
## [KIDS Act 要求在线平台进行年龄验证](https://www.eff.org/deeplinks/2026/06/kids-act-would-require-age-checks-get-online) ⭐️ 7.0/10

美国立法者提出了 KIDS Act 法案，该法案要求面向未成年人的在线平台进行年龄验证，平台需实施年龄确定方法，否则将因"故意忽视"而面临责任追究。 这项立法可能会从根本上改变美国在线平台的运营方式，要求平台收集和验证用户年龄信息，在儿童保护的幌子下，可能让数百万未成年人及其家人面临数据收集和隐私风险。 该法案在第 201(E)节将"承保平台"定义为"使用用户个人信息进行广告、营销或内容推荐"的平台。社区分析表明，HackerNews 等平台可能不符合这一定义下的承保平台资格。

hackernews · bilsbie · Jun 28, 11:56

**背景**: KIDS Act 和 KOSA 等年龄验证法律代表了美国立法中保护未成年人上网的趋势。这些法律要求平台通过第三方验证服务验证用户年龄，造成新的合规负担，并引发对数据处理的重大隐私担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.newamerica.org/insights/age-verification-the-complicated-effort-to-protect-youth-online/">Age Verification Laws and Youth Online Safety: Overview and...</a></li>
<li><a href="https://xident.io/blog/kosa-kids-act-federal-age-verification-platforms-2026/">KOSA, the KIDS Act , and the Federal Age Verification Shift... | Xident</a></li>

</ul>
</details>

**社区讨论**: 评论者对隐私影响表示强烈担忧，有人认为该立法将在保护儿童的幌子下建立"监控状态"。另一人引用研究表明，社交媒体与青少年心理健康影响之间几乎没有证据，驳斥了政客们推动的叙事。还有人呼吁公民联系他们的代表。

**标签**: `#legislation`, `#privacy`, `#age-verification`, `#internet-regulation`, `#children-online-safety`

---

<a id="item-7"></a>
## [福特在 AI 表现不佳后重新聘用"灰胡子"工程师](https://techcrunch.com/2026/06/28/ford-rehires-gray-beard-engineers-after-ai-falls-short/) ⭐️ 7.0/10

福特公开承认，仅靠人工智能无法产生高质量的工程工作，因此正在重新聘用之前被解雇的资深"灰胡子"工程师。公司车辆硬件工程副总裁查尔·庞表示，他们曾错误地认为引入人工智能就会自动产生优质产品。 这一重要实例表明，在汽车制造等复杂技术领域，人工智能无法取代人类的专业知识。该事件可能会影响整个行业的企业人工智能战略，成为过度依赖人工智能而不考虑人类监督的警示性案例。 这些重新聘用的工程师将在零件到达装配线之前识别故障点，培训年轻员工，并帮助重新编程人工智能工具以提高准确性。福特表示并不会完全放弃人工智能，而是将人类专业知识整合以增强人工智能的产出。

rss · TechCrunch AI · Jun 28, 19:05

**背景**: "灰胡子"是行业术语，指经验丰富的资深工程师，通常拥有数十年专业知识，担任导师和知识来源。在汽车制造中，复杂的工程决策需要人工智能系统难以复制的隐性知识，这使得人类经验对于质量控制来说非常宝贵。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/06/28/ford-rehires-gray-beard-engineers-after-ai-falls-short/">Ford rehires ‘ gray beard ’ engineers after AI falls short | TechCrunch</a></li>
<li><a href="https://deepintellica.com/ai-work/ford-rehires-gray-beard-engineers-after-ai-falls-short/">Ford rehires ‘ gray beard ’ engineers after AI falls short - Deep Intellica</a></li>

</ul>
</details>

**社区讨论**: 这一事件被广泛认为是工程领域采用人工智能的转折点。许多行业专家将此视为人类专业知识仍然必不可少的验证，而其他人则认为这是对人机协作而非替代的呼吁。共识强调人工智能应该增强而非取代经验丰富的工程师。

**标签**: `#AI limitations`, `#automotive industry`, `#engineering expertise`, `#corporate strategy`, `#human-AI collaboration`

---

<a id="item-8"></a>
## [Bash4LLM：无外部依赖的轻量级 Bash LLM API 封装工具](https://github.com/kamaludu/bash4llm/) ⭐️ 7.0/10

该工具满足了开发者对轻量级 CLI 访问 LLMs 的真正需求，无需繁重的依赖，使其成为最小化 Linux 环境、快速原型开发或不愿仅为了与 LLM 聊天而安装 Python/Node 的用户的理想选择。 Bash4LLM 支持发送提示、启动聊天会话逐行处理文件、流式输出以及以 JSON 格式保存会话元数据。设计注重安全性：不使用系统/tmp 且不使用 eval。默认支持 Groq，其他 LLM 提供商可通过 extras/providers/文件夹中的专用 Bash 脚本添加。

rss · Hacker News - Show HN · Jun 28, 19:43

**背景**: jq 是一个轻量灵活的命令行 JSON 处理器，在 Linux 系统上通常可用。Groq 是一个以通过快速推理运行开源模型提供即时响应而闻名的 LLM 提供商。该工具面向喜欢基于终端的工作流程并希望避免安装完整编程运行时的用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/jqlang/jq">GitHub - jqlang/ jq : Command - line JSON processor · GitHub</a></li>
<li><a href="https://console.groq.com/docs/quickstart">Quickstart - GroqDocs</a></li>

</ul>
</details>

**社区讨论**: 该 HN 帖子获得 35 分和 15 条评论，表明开发者社区有一定兴趣。讨论可能集中在用例、提供商兼容性以及与现有 LLM CLI 工具的比较上。

**标签**: `#bash`, `#llm`, `#cli-tools`, `#open-source`, `#developer-tools`

---

<a id="item-9"></a>
## [奥地利游说欧盟接纳 Anthropic 公司](https://www.bloomberg.com/news/articles/2026-06-28/austria-lobbies-eu-to-host-anthropic-after-us-access-curbs) ⭐️ 7.0/10

在美国对先进 AI 技术实施出口限制后,奥地利正在积极游说欧盟接纳 Anthropic 这家美国人工智能公司，该公司以其 Claude 语言模型而闻名。 这一事态发展代表了 AI 企业之间激烈的地缘政治竞争,因为在美国出口管制收紧的情况下,各国争相吸引领先的 AI 公司。未来结果可能影响尖端 AI 企业选择在哪里建立运营。 奥地利的游说努力正值美国 AI 出口管制法规不断演变之际,这些法规通过实体清单和商业管制清单限制出口先进 AI 加速器及相关技术。

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Jun 28, 13:34

**背景**: Anthropic 是一家美国 AI 公司,成立于 2021 年,由 OpenAI 前成员,包括兄弟 Dario Amodei 和 Daniela Amodei 创立。该公司开发了 Claude 系列大型语言模型,并专注于 AI 安全。美国通过出口管理条例下的实体清单和商业管制清单对先进 AI 芯片和技术实施了出口管制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (AI) - Wikipedia</a></li>
<li><a href="https://aiwiki.ai/wiki/export_controls">AI chip export controls | AI Wiki</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论显示有 134 条评论,用户就美国出口管制的效力、美国与中国之间技术脱钩的可能性,以及欧洲是否能吸引领先 AI 公司展开辩论。一些用户表达了对监管不确定性影响创新的担忧,而另一些则认为出口管制最终可能加强非美国 AI 生态系统的发展。

**标签**: `#AI industry`, `#geopolitics`, `#EU`, `#Anthropic`, `#policy`

---

<a id="item-10"></a>
## [谷歌限制 Meta 使用 Gemini AI 模型](https://www.cnbc.com/2026/06/28/google-limits-metas-use-of-its-gemini-ai-models-ft-reports.html) ⭐️ 7.0/10

行业观察人士指出，这可能引发 Meta 对独立 AI 开发投资的热潮。该限制还可能鼓励其他公司分散其 AI 模型来源，以避免类似的依赖。

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Jun 28, 13:30

**背景**: 大型科技公司之间的 AI 模型许可协议变得越来越复杂。谷歌的 Gemini API 提供对先进语言模型的访问，但附带禁止竞争性使用的条款。Meta 一直在大力投资其自身的 AI 能力，包括 LLaMA 模型系列。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.google.dev/gemini-api/docs/api-key">Using Gemini API keys | Google AI for Developers</a></li>
<li><a href="https://ai.google.dev/gemini-api/terms">Gemini API Additional Terms of Service | Google AI for Developers</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的讨论显示反应不一——一些用户认为这是鉴于激烈的 AI 竞争而不可避免的自然竞争举措，而其他用户则对市场集中度以及大公司可能将竞争对手锁定在必要 AI 基础设施之外表示担忧。

**标签**: `#AI`, `#Google`, `#Meta`, `#Competition`, `#Industry`

---

<a id="item-11"></a>
## [中国在网络安全 AI 领域追平 Anthropic](https://www.wsj.com/tech/ai/chinese-ai-anthropic-mythos-cybersecurity-574b02c2) ⭐️ 7.0/10

这标志着全球人工智能竞争格局的重大转变，表明中国的人工智能能力现已能在专业领域与西方领先的人工智能公司相媲美。该发展对国家安全和技术领导地位具有重大影响。 Anthropic 的网络安全人工智能模型 Mythos 旨在发现软件漏洞，并于 2026 年 6 月获得美国政府批准扩大使用范围。中国现已追平这些能力，表明在专业人工智能领域的快速进步。

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Jun 28, 10:22

**背景**: Anthropic 开发了 Mythos 网络安全人工智能模型来识别软件漏洞。2026 年 3 月，该模型的细节被意外泄露。2026 年 6 月，Mythos 5 模型在解决国家安全问题后获得美国政府批准扩大部署。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-06-26/us-allows-trusted-partners-to-use-anthropic-s-mythos-5-ai-model">Anthropic ’s Mythos 5 AI Model Cleared by US for Wider... - Bloomberg</a></li>
<li><a href="https://fortune.com/2026/03/27/anthropic-leaked-ai-mythos-cybersecurity-risk/">Anthropic accidentally leaked details of a new AI model that... | Fortune</a></li>

</ul>
</details>

**标签**: `#AI`, `#cybersecurity`, `#geopolitics`, `#Anthropic`, `#China`

---

<a id="item-12"></a>
## [GitLab 19.0 将 Agentic AI 嵌入凭证、合并请求与供应链安全](https://www.infoq.cn/article/ICdHZotGllYog0ocIrxA?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

这一整合意义重大，因为它将自主 AI 操作带入安全关键的 DevOps 工作流程中——可能减少凭证处理中的人为错误、自动化代码审查辅助，并改善供应链安全监控。它影响 DevOps 团队、安全工程师和使用 GitLab 进行 CI/CD 的组织。 Agentic AI 与生成式 AI 的不同之处在于它能够自主操作和执行动作，而不仅仅是响应查询——AI 作为执行任务的运行时运行。该更新涵盖三个核心领域：凭证管理、合并请求工作流程和供应链安全功能。

rss · InfoQ 中文站 · Jun 28, 09:00

**背景**: GitLab 是一个广泛使用的 DevOps 平台，提供 Git 仓库管理、CI/CD 管道和安全扫描功能。Agentic AI 代表人工智能的新趋势，系统可以自主规划和执行任务，而不仅仅是生成内容。近年来，随着备受关注的软件供应链攻击事件，供应链安全变得越来越重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.autolearningagents.com/agentic-ai/agentic-vs-generative">Agentic AI vs Generative AI : Key Differences</a></li>
<li><a href="https://www.molted.net/guides/agentic-ai-vs-generative-ai">Agentic AI vs Generative AI : What's the Difference ?</a></li>

</ul>
</details>

**标签**: `#GitLab`, `#DevOps`, `#Agentic AI`, `#Supply Chain Security`, `#CI/CD`

---