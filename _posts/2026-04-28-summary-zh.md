---
layout: default
title: "Horizon Summary: 2026-04-28 (ZH)"
date: 2026-04-28
lang: zh
---

> From 165 items, 27 important content pieces were selected

---

1. [Mercor 公司 4TB 语音数据遭窃，影响 4 万名 AI 承包商](#item-1) ⭐️ 9.0/10
2. [vLLM v0.20.0 发布：CUDA 13.0 设为默认，支持 PyTorch 2.11 升级](#item-2) ⭐️ 8.0/10
3. [微软结束与 OpenAI 的独家收入分成协议](#item-3) ⭐️ 8.0/10
4. [GitHub Copilot 转向按量计费模式](#item-4) ⭐️ 8.0/10
5. [开源代理 Dirac 登顶 TerminalBench，准确率达 65.2%](#item-5) ⭐️ 8.0/10
6. [FDA 批准首个遗传性耳聋基因疗法](#item-6) ⭐️ 8.0/10
7. [“何不直接使用 Lean？”——证明助手比较讨论](#item-7) ⭐️ 8.0/10
8. [DeepMind 联合创始人 David Silver 融资 11 亿美元打造无人类数据 AI](#item-8) ⭐️ 8.0/10
9. [谷歌员工要求皮查伊阻止五角大楼使用 AI](#item-9) ⭐️ 8.0/10
10. [小米玄戒 O1 芯片出货量突破 100 万颗](#item-10) ⭐️ 8.0/10
11. [科学家实现创纪录高次谐波产生，接近施温格极限](#item-11) ⭐️ 8.0/10
12. [SVG 清理漏洞：Scratch XSS 案例分析](#item-12) ⭐️ 7.0/10
13. [中国阻止 Meta 收购 AI 初创公司 Manus](#item-13) ⭐️ 7.0/10
14. [Super ZSNES：GPU 加速的 SNES 模拟器项目](#item-14) ⭐️ 7.0/10
15. [pgBackRest 维护者宣布停止开发 已运营 13 年](#item-15) ⭐️ 7.0/10
16. [美国最高法院审查警方运用手机位置数据](#item-16) ⭐️ 7.0/10
17. [OpenAI 企业产品获得 FedRAMP 中等授权](#item-17) ⭐️ 7.0/10
18. [OpenAI 从微软获得 50B 美元协议中的 AWS 销售权](#item-18) ⭐️ 7.0/10
19. [马斯克对阵 Altman：OpenAI 使命审判开审](#item-19) ⭐️ 7.0/10
20. [Canva AI 工具替换用户设计中 Palestine 一词后道歉](#item-20) ⭐️ 7.0/10
21. [重建 AI 数据基础设施](#item-21) ⭐️ 7.0/10
22. [谷歌警告恶意网页正在劫持企业 AI 代理](#item-22) ⭐️ 7.0/10
23. [AlphaGo 创造者 David Silver 推出 11 亿美元超级学习者 AI 公司](#item-23) ⭐️ 7.0/10
24. [开发者分享 ChatGPT 应用 3 个月审核历程](#item-24) ⭐️ 7.0/10
25. [摩尔线程财报：研发占比超 86%，万卡级智算集群落地](#item-25) ⭐️ 7.0/10
26. [云区域失效：地缘政治风险下的高可用架构重构](#item-26) ⭐️ 7.0/10
27. [小米正式开源 MiMo-V2.5 系列 AI 模型](#item-27) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Mercor 公司 4TB 语音数据遭窃，影响 4 万名 AI 承包商](https://app.oravys.com/blog/mercor-breach-2026) ⭐️ 9.0/10

Lapsus$黑客组织入侵了 AI 承包商平台 Mercor，窃取了 4TB 的语音样本数据，涉及 4 万名承包商并与其身份文档配对。这构成了一个完整的深度伪造工具包，可通过银行声纹验证绕过、类似 Arup 的视频通话冒名顶替和保险欺诈来进行身份欺诈。 这次泄露之所以重要，是因为它将语音生物识别数据与身份文档结合在一起——这是绕过银行语音认证所需的两个组件。受害者面临一种讽刺的情况：他们可能需要提交更多语音数据来验证自己是否被泄露，形成了一个递归的隐私陷阱。 这次泄露特别危险，因为大多数泄露事件要么暴露语音数据，要么暴露身份文档，而不是两者同时泄露。这种组合允许攻击者创建合成语音来绕过语音生物识别系统，进行视频通话冒名顶替，并伪造身份进行保险索赔。ORAVYS 为受影响的承包商提供前三个可疑样本的免费分析服务。

hackernews · Oravys · Apr 27, 09:57

**背景**: 语音生物识别认证在银行业中越来越多地用于「生命证明」验证，通过识别超过 140 个语音特征来验证身份。深度伪造技术现在可以从短至几秒的样本中克隆声音，使语音数据对欺诈非常有价值。德国人提出的「Datensparsamkeit」（数据节俭）概念主张尽量减少收集的数据量以减少泄露影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gnani.ai/resources/blogs/voice-biometric-security-instantly-reduces-banking-fraud-386b3">Instant Banking Fraud Prevention with Voice Biometric Security</a></li>
<li><a href="https://www.phonexia.com/blog/voice-biometrics-in-the-banking-industry/">Voice Biometrics in the Banking Industry | PHONEXIA</a></li>
<li><a href="https://www.respeecher.com/blog/everything-you-need-know-about-deepfake-voice-its-synthetic-voice-ethical-counterpart">Everything You Need to Know about Deepfake Voice and Its...</a></li>

</ul>
</details>

**社区讨论**: 讨论强调了受害者必须提交更多语音数据来验证自己的声音是否被盗的讽刺意味——为了寻求帮助，又要向另一家人工智能公司发送语音样本。评论者指出，生物识别本质上是「永久密码」，一旦泄露就无法更改。德国人提出的「Datensparsamkeit」概念被誉为解决方案：唯一真正安全的数据是不存在的数据。

**标签**: `#data-breach`, `#biometric-security`, `#deepfakes`, `#voice-recognition`, `#AI-security`, `#privacy`

---

<a id="item-2"></a>
## [vLLM v0.20.0 发布：CUDA 13.0 设为默认，支持 PyTorch 2.11 升级](https://github.com/vllm-project/vllm/releases/tag/v0.20.0) ⭐️ 8.0/10

此版本意义重大，因为它提供了重要的基础设施升级，包括 CUDA 13.0 和 PyTorch 2.11，这将提升推理性能和兼容性。添加 DeepSeek V4 支持和 Python 3.14 兼容性表明 vLLM 致力于与最新 AI 模型架构和 Python 版本保持同步。 关键突破性变更：现在需要 PyTorch 2.11（XPU 也升级到 2.11，不再锁定在 2.10）。FlashAttention 4 重新启用为默认 MLA 预填充后端。TurboQuant 2 位 KV 缓存提供 4 倍容量和压缩效果。该版本还包括 vLLM IR 初始框架（为未来内核工作奠定基础）以及大规模 MoE 重构。

github · khluu · Apr 27, 21:20

**背景**: vLLM 是一个高性能大语言模型(LLM)推理引擎，旨在优化吞吐量和延迟。CUDA 是 NVIDIA 的并行计算平台，新版本如 CUDA 13.0 提供更好的性能。PyTorch 2.11 带来了可能影响现有设置的重要变更。DeepSeek V4 是一个混合专家模型(MoE)，拥有 1 万亿参数和 100 万 token 上下文窗口支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://build.nvidia.com/deepseek-ai/deepseek-v4-pro/modelcard">deepseek - v 4 -pro Model by Deepseek -ai | NVIDIA NIM</a></li>
<li><a href="https://arxiv.org/html/2512.02556v1">DeepSeek -V3.2: Pushing the Frontier of Open Large Language Models</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#PyTorch`, `#CUDA`, `#deep learning`

---

<a id="item-3"></a>
## [微软结束与 OpenAI 的独家收入分成协议](https://www.bloomberg.com/news/articles/2026-04-27/microsoft-to-stop-sharing-revenue-with-main-ai-partner-openai) ⭐️ 8.0/10

这一终止标志着 AI 行业权力结构的重大转变。OpenAI 现在可以将云基础设施分散到 Azure 之外，可能会削弱微软的影响力，同时加剧云服务提供商之间的竞争。此举表明即使是深入的合作关系也面临市场压力。 微软此前持有 OpenAI 约 49%的股份，但已降至 27%。独家协议原本阻止 OpenAI 与 AWS 等竞争云服务提供商合作，为 Azure 在该合作关系中创造了近乎垄断的地位。OpenAI 现在可以自由地与 AWS 及其他提供商合作。

hackernews · helsinkiandrew · Apr 27, 13:22

**背景**: 微软从 2019 年开始向 OpenAI 投资数十亿美元，成为其独家云计算合作伙伴和训练及部署 OpenAI 模型的基础设施唯一提供商。该收入分成协议在行业中是独一无二的，以其巨额计算投资换取微软的优惠条款。该合作伙伴关系是 Azure 相对于 AWS 和谷歌云在 AI 领域定位的核心。

**社区讨论**: 评论者认为谷歌可能是最大赢家，因为几乎所有前沿 AI 实验室都使用 TPU，OpenAI 现在可以在 Gen 8 TPU 发布后选择使用 TPU。一些人质疑微软为何接受对 OpenAI 如此有利的条款，暗示 Azure'命悬一线'，微软担心在 Anthropic 竞争下其投资面临风险。还有人指出微软的持股比例从 49%下降到 27%，质疑微软的弱势地位。

**标签**: `#microsoft`, `#openai`, `#ai-industry`, `#cloud-computing`, `#partnership`

---

<a id="item-4"></a>
## [GitHub Copilot 转向按量计费模式](https://github.blog/news-insights/company-news/github-copilot-is-moving-to-usage-based-billing/) ⭐️ 8.0/10

GitHub Copilot 正在从固定的月度订阅模式（Pro 每月 10 美元，Pro+每月 39 美元）转向基于使用量的 AI 积分计费方式，这标志着微软补贴 AI 推理时代的结束。 新的模型倍率从新版 GPT 和 Sonnet 模型的 1x 到 6x 不等，Opus 模型高达 27x。用户以前只需支付每月 10 美元，通过大量提示就能获得超过 500 美元的价值，对于重度用户来说，实际增长可能达到 50 倍甚至更多。

hackernews · frizlab · Apr 27, 16:03

**背景**: GitHub Copilot 是一款集成在流行 IDE 中的 AI 代码补全工具。自推出以来，它一直采用固定订阅模式，用户按月付费而不考虑使用量。微软的大量补贴让开发者能以远低于市场价的方式访问 GPT-4 等先进 AI 模型。转向按量计费反映了整个行业在推理成本依然高企的情况下向计量 AI 定价的转变。

**社区讨论**: 社区对价格上涨表现出强烈担忧，许多用户指出补贴推理时代的结束。评论强调 GitHub 的定价与直接 API 提供商相似且没有折扣，导致用户考虑 OpenRouter 或 Deepseek 等替代方案。一些用户计算得出，对于以前利用 10 美元计划无限潜力的重度用户来说，实际增长可能达到 50 倍。

**标签**: `#github-copilot`, `#pricing`, `#developer-tools`, `#ai-billing`, `#usage-based-pricing`

---

<a id="item-5"></a>
## [开源代理 Dirac 登顶 TerminalBench，准确率达 65.2%](https://github.com/dirac-run/dirac) ⭐️ 8.0/10

这表明 AI 代理架构对基准测试性能的影响有多大——通过更好的工程设计而非模型变更，实现了比 Google 官方结果高出 17.4 个百分点的提升。这凸显了公平比较 AI 代理需要控制 harness 差异，而开源性质允许社区验证并在此基础上进行构建。 Dirac 使用基于哈希的编辑，通过为每行计算稳定的加密哈希来锚定更改（即使文件移动仍然有效）；基于 AST 的上下文获取使用语言的 AST 来选择性检索相关代码片段（避免大文件读取）；并批处理所有操作以同时执行多个读取和编辑。

hackernews · GodelNumbering · Apr 27, 12:35

**背景**: TerminalBench 是一个用于测试 AI 代理在命令行环境中完成真实困难任务的基准。该基准评估 AI 代理完成复杂终端操作的能力。最近的报告强调了 TerminalBench 2.0 上的作弊问题，某些代理会利用基准测试来虚高分数。基于哈希的文件编辑技术提供了更改的加密验证，而基于 AST 的获取帮助 LLM 理解代码结构而无需读取整个文件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2601.11868">[2601.11868] Terminal-Bench: Benchmarking Agents on Hard, Realistic Tasks in Command Line Interfaces</a></li>
<li><a href="https://github.com/laude-institute/terminal-bench">GitHub - harbor-framework/terminal-bench: A benchmark for LLMs on complicated tasks in the terminal · GitHub</a></li>
<li><a href="https://www.aitoolnet.com/dirac">Dirac - Open-Source Coding Agent with Hash - Anchored ... - Aitoolnet</a></li>

</ul>
</details>

**社区讨论**: 评论者赞赏技术创新的同时提出了重要担忧：一人指出基准测试应测试不同模型家族的泛化能力（不仅仅是 Gemini），并指出着陆页未提及 Gemini 3 Flash。另一人强调 harness 差异可能比模型差异更重要，询问是否有比较 harness 的排行榜。一位用户还注意到向 dirac.run 发送了遥测数据，询问收集了什么内容。

**标签**: `#open-source`, `#ai-agents`, `#benchmarking`, `#gemini`, `#terminal-bench`, `#llm-harnesses`

---

<a id="item-6"></a>
## [FDA 批准首个遗传性耳聋基因疗法](https://www.fda.gov/news-events/press-announcements/fda-approves-first-ever-gene-therapy-treatment-genetic-hearing-loss-under-national-priority-voucher) ⭐️ 8.0/10

FDA 批准了 Otarmeni（lunsotogene parvec-cwha），这是首个用于治疗由 OTOF 基因突变引起的遗传性耳聋的基因疗法。该疗法适用于患有与双等位基因 OTOF 变异相关的中度至极重度感音神经性耳聋的儿童和成人患者。 这一批准标志着历史性里程碑，成为 FDA 批准的首个遗传性耳聋基因疗法，为治疗此前无法治愈的遗传性耳聋开辟了新可能性。该疗法使用 AAV 载体向细胞内递送功能正常的 OTOF 基因副本，可能使面临终身失聪的患者恢复听力功能。

hackernews · JeanKage · Apr 27, 10:15

**背景**: OTOF 基因突变导致听觉神经病谱系障碍，声音正常进入内耳，但由于耳蜗蛋白缺陷，从内耳到大脑的传输受损。耳蜗蛋白对内毛细胞带状突触的突触囊泡外泌至关重要。该疗法代表了 Decibel Therapeutics（已被 Regeneron 收购）多年的研究，并基于长达 2.5 年随访的临床试验显示出安全性和有效性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fda.gov/news-events/press-announcements/fda-approves-first-ever-gene-therapy-treatment-genetic-hearing-loss-under-national-priority-voucher">FDA Approves First-Ever Gene Therapy for Treatment of Genetic Hearing Loss Under National Priority Voucher Program | FDA</a></li>
<li><a href="https://www.nature.com/articles/s41586-026-10393-y">Multicentre gene therapy for OTOF-related deafness followed up to 2.5 years | Nature</a></li>
<li><a href="https://investor.regeneron.com/news-releases/news-release-details/otarmenitm-lunsotogene-parvec-cwha-approved-fda-first-and-only">Otarmeni™ (lunsotogene parvec-cwha) Approved by FDA as First and Only Gene Therapy for Genetic Hearing Loss; Regeneron to Provide Otarmeni for Free in the U.S. | Regeneron Pharmaceuticals Inc.</a></li>

</ul>
</details>

**社区讨论**: 社区反应普遍积极，许多人庆祝这一突破，为受 OTOF 相关耳聋影响的儿童和家庭带来希望。一些评论者分享了个人与听力损失作斗争的经历，并对未来涵盖其他遗传原因（如 GJB2）的治疗表示期待。其他人注意到该疗法的局限性，即无法帮助因腮腺炎等疾病导致获得性听力损失的人。

**标签**: `#gene-therapy`, `#FDA`, `#medical-breakthrough`, `#biotechnology`, `#hearing-loss`

---

<a id="item-7"></a>
## [“何不直接使用 Lean？”——证明助手比较讨论](https://lawrencecpaulson.github.io//2026/04/23/Why_not_Lean.html) ⭐️ 8.0/10

讨论显示出不同的观点：有人认为 Lean 在依赖类型方面相比 Agda 是“笨重的降级”，而其他人欣赏其均衡的方法。Isabelle 用户指出不同的权衡而非明显优越性。一个关键纠正是，Lean 实际上不会像原帖声称的那样保留大型证明对象。 一位评论者澄清说，Lean 实际上不会在最终证明中保留证明对象——与原帖作者的声称相反。来自 Agda、Coq 和 Isabelle 背景的社区成员分享道，Lean 的主要优势在于各方面都不错且拥有庞大的社区，而不是在某一方面最为出色。

hackernews · ibobev · Apr 27, 14:24

**背景**: 证明助手是一种形式化验证工具，用于在计算机辅助下证明数学定理。Lean 将函数式编程和定理证明结合在一个框架中。Agda 是一种基于 Martin-Löf 类型理论的依赖类型编程语言。Coq 以其强大的基于战术的证明开发而著称。Isabelle/HOL 使用高阶逻辑进行证明构建。每种工具在编程表达力和证明验证能力之间都做出了不同的权衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Isabelle_(proof_assistant)">Isabelle (proof assistant) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agda_(programming_language)">Agda (programming language) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: The discussion revealed mixed opinions: some found Lean a 'clunky downgrade' from Agda in terms of dependent types, while others appreciated its balanced approach. Isabelle users noted different tradeoffs rather than clear superiority. A key correction was that Lean doesn't actually retain large proof objects as the original post suggested.

**标签**: `#formal methods`, `#lean`, `#proof assistants`, `#theorem proving`, `#functional programming`

---

<a id="item-8"></a>
## [DeepMind 联合创始人 David Silver 融资 11 亿美元打造无人类数据 AI](https://techcrunch.com/2026/04/27/deepminds-david-silver-just-raised-1-1b-to-build-an-ai-that-learns-without-human-data/) ⭐️ 8.0/10

Ineffable Intelligence 是一家英国人工智能实验室，由前 DeepMind 研究员 David Silver 于数月前创立，现已融资 11 亿美元，估值达 51 亿美元。该公司致力于开发无需人类数据即可学习的 AI 系统，这是一种被称为自监督学习或零数据学习的研究方向。 这笔融资是针对单一人工智能研究实验室在传统监督学习之外的替代学习范式方面最大规模的投资之一。如果成功，此类系统可以大幅减少对昂贵人工标注数据集的依赖，并可能发现人类尚未考虑到的解决方案。 David Silver 此前领导了 DeepMind 的 AlphaZero 项目，该项目通过自我对弈的“白板”强化学习在国际象棋、将棋和围棋中达到了超越人类的水平。新实验室将以这一成果为基础，开发更通用的人工智能系统，实现无需人类干预或外部监督的自主学习。

rss · TechCrunch AI · Apr 27, 17:24

**背景**: 传统人工智能模型通常需要大量人工标注的数据进行训练，这些数据的制作成本高昂且耗时。自监督学习是一种机器学习技术，使用无监督方法完成通常需要监督学习的任务，无需标注数据。David Silver 的 AlphaZero 表明，系统可以通过自我对弈和强化学习从零开始纯粹通过自我学习来掌握复杂任务，无需任何人类知识。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/self-supervised-learning">What Is Self-Supervised Learning? | IBM</a></li>
<li><a href="https://arxiv.org/html/2406.00606v2">LLMs Could Autonomously Learn Without External Supervision</a></li>
<li><a href="https://en.wikipedia.org/wiki/AlphaZero">AlphaZero - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI_Research`, `#Funding`, `#DeepMind`, `#Machine_Learning`, `#David_Silver`

---

<a id="item-9"></a>
## [谷歌员工要求皮查伊阻止五角大楼使用 AI](https://www.theverge.com/ai-artificial-intelligence/919326/google-ai-pentagon-classified-letter) ⭐️ 8.0/10

超过 600 名谷歌员工，包括 DeepMind 人工智能实验室的工作人员以及 20 多名高级领导人（首席研究员、总监和副总裁），签署了一封致首席执行官桑达尔·皮查伊的信，要求谷歌阻止五角大楼将该公司的人工智能模型用于机密军事目的。 这次抗议代表了科技员工行动主义的重大升级，因为其参与者包括高级领导人而不仅仅是普通员工，表明了对军事人工智能应用伦理影响的高度机构性担忧。 组织者特别声称，DeepMind 员工在签名者中占很大比例，表明谷歌顶级人工智能研究部门对其技术被用于机密军事目的抱有严重保留意见。

rss · The Verge AI · Apr 27, 18:17

**背景**: 这封信呼应了谷歌早期的争议，特别是 2018 年的 Project Maven 抗议活动，当时员工成功抵制了五角大楼的人工智能合同，该合同涉及无人机镜头分析。在此抗议之后，谷歌制定了人工智能伦理原则，并拒绝续签该合同。DeepMind 是作为一个独立的人工智能研究部门成立的，其对负责任的人工智能开发做出了明确承诺，因此其员工参与此次抗议尤其值得关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/">Google DeepMind</a></li>
<li><a href="https://www.youtube.com/watch?v=1XF-NG_35NE">What's next for AI at DeepMind , Google 's artificial intelligence lab</a></li>

</ul>
</details>

**社区讨论**: 来源材料中未提供社区评论。

**标签**: `#ai-ethics`, `#corporate-responsibility`, `#employee-activism`, `#google-deepmind`, `#military-ai`

---

<a id="item-10"></a>
## [小米玄戒 O1 芯片出货量突破 100 万颗](https://weibo.com/1997509257/5292279283585125) ⭐️ 8.0/10

这对中国半导体行业具有重要意义，表明小米已成为少数具备设计制造先进 3nm 芯片能力的中国公司之一。超过 20 亿美元的研发投入和 10 年 70 亿美元的承诺显示出与全球芯片巨头竞争的长期战略决心。 玄戒 O1 采用台积电第二代 3nm（N3E）制程，集成 190 亿个晶体管，与高通骁龙 8 Elite、联发科天玑 9400 和苹果 A18 Pro 采用相同制程。芯片首发机型为小米 15S Pro 及高端平板。截至 2025 年 4 月，研发投入已达 135 亿元，计划 10 年投入至少 500 亿元。

telegram · zaihuapd · Apr 27, 05:50

**背景**: 3nm 制程是目前智能手机芯片最先进的量产制造工艺。玄戒 O1 是中国大陆首款采用第二代 3nm 工艺的系统级芯片，标志着中国在高端移动处理器开发方面的突破。此前，中国智能手机芯片在先进制程方面落后于全球领先厂商。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/玄戒">玄戒 - 维基百科，自由的百科全书</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1913543324637329084">破而后立，一鸣惊人！——小米玄戒O1芯片（小米15S Pro）详细评测 - 知乎</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#China tech`, `#Xiaomi`, `#3nm chip`, `#EV chips`

---

<a id="item-11"></a>
## [科学家实现创纪录高次谐波产生，接近施温格极限](https://www.nature.com/articles/s41586-026-10400-2) ⭐️ 8.0/10

实验通过精确调控亚皮秒尺度的飞秒激光脉冲对比度，实现了与理论高度吻合的高次谐波转换效率。这证实了实现相干谐波聚焦（CHF）的关键要素已经完备。

telegram · zaihuapd · Apr 27, 16:00

**背景**: 高次谐波产生（HHG）是一种非线性光学过程，其中暴露在强激光脉冲下的材料会发射入射激光的高阶谐波。施温格极限是量子电动力学中的一个理论阈值，当电磁场超过该极限时，电磁场将变得非线性，导致真空表现出非线性特性。该极限代表了物理学中最极端的条件之一，此前在实验室中从未被实现过。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Schwinger_limit">Schwinger limit - Wikipedia</a></li>
<li><a href="https://zh.wikipedia.org/zh-cn/高次諧波產生">高次谐波产生 - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**标签**: `#laser_physics`, `#quantum_electrodynamics`, `#high_harmonic_generation`, `#extreme_light`, `#Schwinger_limit`

---

<a id="item-12"></a>
## [SVG 清理漏洞：Scratch XSS 案例分析](https://muffin.ink/blog/scratch-svg-sanitization/) ⭐️ 7.0/10

此案例揭示了網路安全中的一個常見陷阱：使用正則表達式來清理像 SVG 這樣的複雜標記容易被繞過。討論強調了像內容安全策略(CSP)這樣的正確解決方案的重要性，並提出了關于負責任披露實踐的倫理問題。 Scratch 的漏洞涉及通過 SVG 上傳进行 XSS 攻击，可在用戶瀏覽器中執行任意 JavaScript。雖然 Scratch 嘗試了基於正則表達式的修復，但研究人員證明這可以被繞過。DOMPurify 等專門的清理庫代表了正確的解決方案，而 CSP 提供了最強大的防御。

hackernews · varun_ch · Apr 27, 15:31

**背景**: SVG（可縮放矢量圖形）是一種基於 XML 的圖像格式，支援嵌入 JavaScript 和事件處理器，這使其在上传到 Web 應用程序時可能成為跨站腳本（XSS）攻擊的向量。XSS 攻擊允許攻擊者在受害者的瀏覽器中執行惡意腳本，可能窃取會話 Cookie 或代表用戶執行操作。內容安全策略（CSP）是一種 HTTP 頭，告訴瀏覽器頁面可以加載哪些資源，提供深度防御來抵禦 XSS。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dompurify.com/">DOMPurify – Fast & Secure XSS Sanitizer for HTML</a></li>
<li><a href="https://portswigger.net/web-security/cross-site-scripting/contexts/lab-some-svg-markup-allowed">Lab: Reflected XSS with some SVG markup allowed | Web Security Academy</a></li>
<li><a href="https://rietta.com/blog/svg-xss-injection-attacks/">Cross-site Scripting Injection Attacks Using SVG Images</a></li>

</ul>
</details>

**社区讨论**: 評論者稱讚 CSP 是正確的解決方案，simonw 指出 CSP 可以通過 meta 標籤直接在 HTML 中設置。andybak 建議只支援安全的 SVG 子集。nmilo 批評 Scratch 使用正則表達式清理，並質疑是否遵循了適當的負責任披露原則。其他人討論了需要沙箱屬性來隔離 SVG 內容。

**标签**: `#security`, `#svg`, `#xss`, `#web-security`, `#sanitization`

---

<a id="item-13"></a>
## [中国阻止 Meta 收购 AI 初创公司 Manus](https://www.cnbc.com/2026/04/27/meta-manus-china-blocks-acquisition-ai-startup.html) ⭐️ 7.0/10

中国阻止了 Meta 收购 AI 初创公司 Manus 的计划，以出口管制法为由阻止了这笔涉及新加坡公司的交易。据媒体报道，该收购于 2025 年 12 月宣布，估值约为 20 至 30 亿美元。 这一决定表明，中国愿意对源自其境内的 AI 技术执行严格管控，即使公司为规避监管而搬迁至新加坡等管辖区。这开创了一个与 TikTok 监管风波类似的先例，可能影响涉及中国原创技术的国际 AI 收购的架构方式。 Manus 在 2025 年 5 月完成由美国风投公司 Benchmark 领投的 7500 万美元融资后搬迁至新加坡，关闭了在中国的业务并裁减了数十名员工。据报道，中国援引出口管制法第 12 条（兜底条款）和离岸关联公司规定来阻止这笔收购，Manus 的联合创始人据报正因涉嫌违反出口管制和国家安全法而接受调查。

hackernews · yakkomajuri · Apr 27, 11:43

**背景**: 中国的出口管制法于 2020 年颁布，此后不断扩展，赋予监管机构广泛的权力来规范敏感技术的出口，包括某些 AI 相关知识产权。一个被称为"兜底条款"的关键条款允许监管机构在认定技术可能威胁国家安全时，控制未明确列出的出口。新加坡已成为中国科技公司寻求国际业务中立基地的热门管辖区，但中国更新的法规已试图封堵一些人所说的"新加坡漏洞"。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Manus_(AI_agent)">Manus (AI agent) - Wikipedia</a></li>
<li><a href="https://www.kingandwood.com/us/en/insights/latest-thinking/chinas-technology-import-export-control-a-crucial-compliance-landscape.html">China’s Technology Import/Export Control: A Crucial ...</a></li>
<li><a href="https://fdichina.com/blog/blog-china-export-restrictions-12-rules-2025/">China Export Restrictions: 12 Essential Rules & 5 Costly ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论者注意到一个讽刺之处：世界上许多 AI 进展都归功于 Meta 和 Google 的开源发布，包括 Llama 模型。评论者指出，中国实际上在应用与美国出口管制相同的逻辑——主张对源自本国的算法进行控制。有人讨论了打破新加坡作为监管虚饰的地位如何可能产生有问题的先例，并对中国将如何实际撤销一笔已完成交易表示怀疑。

**标签**: `#AI regulation`, `#China-US tech relations`, `#Meta`, `#export controls`, `#geopolitics`

---

<a id="item-14"></a>
## [Super ZSNES：GPU 加速的 SNES 模拟器项目](https://zsnes.com/) ⭐️ 7.0/10

评论显示了怀旧和技术兴趣的混合，用户讨论了对 ZSNES 的童年记忆，并就 PPU 实现方法展开辩论。一位用户提出了关于合法获取游戏的问题，另一位则赞扬了 Mathew Valente 的音频样本恢复工作。总体情绪积极，技术讨论深入。

hackernews · haunter · Apr 27, 17:50

**背景**: 原始 SNES 游戏机包含两个图片处理单元(PPU)芯片，负责生成视频输出、处理背景、精灵和色彩效果。ZSNES 是 1990 年代末和 2000 年代初一款流行的 SNES 模拟器，帮助推广了模拟技术。GPU 加速模拟利用显卡的并行处理来执行传统上在 CPU 上运行的计算任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fabiensanglard.net/snes_ppus_how/">How the SNES Graphics System works</a></li>
<li><a href="https://sneslab.net/wiki/PPU_Registers">PPU Registers - SnesLab</a></li>

</ul>
</details>

**社区讨论**: 评论展现了怀旧与技术兴趣的交织，用户讨论了对 ZSNES 的童年记忆，并就 PPU 实现方法展开辩论。一位用户提出了关于合法获取游戏的问题，另一位则赞扬了 Mathew Valente 的音频样本恢复工作。总体情绪积极，技术讨论深入。

**标签**: `#emulator`, `#SNES`, `#GPU`, `#retro-gaming`, `#open-source`

---

<a id="item-15"></a>
## [pgBackRest 维护者宣布停止开发 已运营 13 年](https://github.com/pgbackrest/pgbackrest) ⭐️ 7.0/10

pgBackRest 支持完整、差异和增量备份，采用异步归档和恢复功能，专为处理最大规模的数据库和工作负载而设计。该项目在 13 年的历史中部分得到了企业赞助支持。

hackernews · c0l0 · Apr 27, 10:56

**背景**: pgBackRest 是一款面向 PostgreSQL 的开源备份和恢复解决方案，提供可靠的备份、恢复和归档功能。它在生产环境中广泛使用，以高效处理大型数据库而闻名。PostgreSQL 是全球最受欢迎的开源关系型数据库之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pgbackrest.org/">pgBackRest - Reliable PostgreSQL Backup & Restore</a></li>
<li><a href="https://medium.com/@yaseminbsra.sergen/setting-up-and-using-pgbackrest-with-patroni-7161024cc898">Setting Up and Using pgBackRest with Patroni | by Yasemin... | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区对开发者 13 年的奉献表示感谢，一些人分享了他们使用 pgBackRest 的指南和 positive experiences。讨论还集中在开源可持续性上，建议有盈利能力的公司可能接管这款广泛使用工具的维护工作。

**标签**: `#open-source`, `#postgresql`, `#pgbackrest`, `#devops`, `#database`

---

<a id="item-16"></a>
## [美国最高法院审查警方运用手机位置数据](https://www.nytimes.com/2026/04/27/us/politics/supreme-court-cell-data-geofence.html) ⭐️ 7.0/10

此案可能为数字时代的第四次修正案保护建立关键先例。该裁决可能决定通过地理围栏令进行的大规模位置数据收集是否违反宪法隐私权，影响执法部门如何使用技术追踪公民。 谷歌此前将位置数据存储在一个名为 Sensorvault 的数据库中，执法部门曾用它来识别特定时间和区域内的所有设备。除谷歌外，执法部门还向苹果、Lyft、Snapchat、Uber、微软和雅虎寻求地理围栏数据。

hackernews · unethical_ban · Apr 27, 15:29

**背景**: 地理围栏令是一种逆向位置令，允许警方在特定时间段内请求特定地理区域内的所有移动设备。第四修正案保护免受不合理的搜查和扣押，但第三方学说历来对与第三方共享的信息给予较少的隐私保护。最高法院此前在 Carpenter 诉美国案（2018 年）中裁定，警方需要获得令才能访问历史手机位置数据，但此案可能会澄清实时地理围栏请求的适用范围。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Geofence_warrant">Geofence warrant</a></li>
<li><a href="https://thehill.com/regulation/court-battles/5848192-geofence-warrants-fourth-amendment-supreme-court/">Geofence warrants case tests Fourth Amendment at Supreme Court</a></li>

</ul>
</details>

**社区讨论**: 社区评论显示混合反应——一些人赞扬谷歌保护隐私的改变，而另一些人批评允许政府潜在访问任何共享数据的第三方学说。人们对司法公正性表示怀疑，并担心一些法官已经做好了决定。评论者还讨论了将数字地理围栏与物理监控方法进行比较的道德问题。

**标签**: `#privacy`, `#law`, `#supreme-court`, `#surveillance`, `#geofencing`

---

<a id="item-17"></a>
## [OpenAI 企业产品获得 FedRAMP 中等授权](https://openai.com/index/openai-available-at-fedramp-moderate) ⭐️ 7.0/10

OpenAI 已获得 ChatGPT 企业版和 OpenAI API 的 FedRAMP 中等授权，使美国联邦机构能够采用安全的 AI 解决方案。 此授权允许联邦机构在敏感政府工作中合法使用 OpenAI 的企业级 AI 工具，开辟了巨大的市场机会，并为公共部门的 AI 治理树立了先例。 FedRAMP 中等授权需要基于 FIPS 199 的 325 项安全控制，用于保护受控非机密信息(CUI)，具有中等保密性、完整性和可用性要求。

rss · OpenAI News · Apr 27, 14:00

**背景**: FedRAMP（联邦风险与授权管理计划）是美国政府的一项计划，为云产品提供标准化的安全评估和授权方法。它基于 FIPS 199 定义了三个影响等级（低、中、高），用于分类信息系统被破坏时潜在不利影响的严重程度。中等授权是政府云部署最常见的授权等级，需要比低等级更多的安全控制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.vanta.com/collection/fedramp/fedramp-moderate">FedRAMP Moderate : Who’s in scope and how to prepare | Vanta</a></li>
<li><a href="https://secureframe.com/hub/fedramp/impact-levels">FedRAMP Levels & Baselines, Explained</a></li>
<li><a href="https://secureframe.com/hub/fedramp/moderate">FedRAMP Moderate : Requirements & How to Prepare</a></li>

</ul>
</details>

**标签**: `#AI compliance`, `#enterprise AI`, `#government AI`, `#OpenAI`, `#FedRAMP`

---

<a id="item-18"></a>
## [OpenAI 从微软获得 50B 美元协议中的 AWS 销售权](https://techcrunch.com/2026/04/27/openai-ends-microsoft-legal-peril-over-its-50b-amazon-deal/) ⭐️ 7.0/10

OpenAI 已获得微软的让步，允许其在 AWS（亚马逊云平台）上销售产品，同时微软在这笔涉及亚马逊的复杂三方交易中获得更优惠的收入分成条款。 这笔交易重塑了 AI 和云服务市场的竞争格局。通过直接接触 AWS 庞大的客户群，OpenAI 能够更有效地与其他 AI 提供商竞争，同时微软从其对 OpenAI 的大量投资中获得更丰厚的财务回报。 该交易估值约 500 亿美元，标志着 AI 云计算领域的重大转变。微软作为 OpenAI 的最大股东，此前一直限制该公司直接通过竞争激烈的云平台进行销售。

rss · TechCrunch AI · Apr 27, 17:40

**背景**: 微软已向 OpenAI 投资约 130 亿美元，并一直是其独家云基础设施合作伙伴，为 OpenAI 提供运行模型的 Azure 服务。最初的合作赋予微软通过 Azure 商业化 GPT 模型的独家权利，这在一定程度上限制了 OpenAI 独立分销产品的能力。

**标签**: `#OpenAI`, `#Microsoft`, `#Amazon AWS`, `#AI business`, `#cloud computing`

---

<a id="item-19"></a>
## [马斯克对阵 Altman：OpenAI 使命审判开审](https://www.theverge.com/tech/917225/sam-altman-elon-musk-openai-lawsuit) ⭐️ 7.0/10

审判结果可能决定 OpenAI 是否允许作为营利企业存续，甚至可能影响管理层，可能影响该公司备受期待的 IPO 以及作为全球最具影响力 AI 公司之一的未来方向。 马斯克的诉讼挑战 OpenAI 在萨姆·阿尔特曼领导下的演变，特别是该公司从非营利研究实验室向获得微软投资的商业企业的转型。在陪审团遴选期间，数位潜在陪审员对马斯克本人表达了负面看法。

rss · The Verge AI · Apr 27, 15:50

**背景**: OpenAI 于 2015 年作为非营利 AI 研究公司成立，使命是确保人工智能造福人类。马斯克是早期联合创始人之一，但于 2018 年离开该公司。随后公司创建了营利子公司并获得了微软的大量投资，导致其结构和方向发生重大变化。

**标签**: `#OpenAI`, `#AI Industry`, `#Legal Battle`, `#Elon Musk`, `#Sam Altman`

---

<a id="item-20"></a>
## [Canva AI 工具替换用户设计中 Palestine 一词后道歉](https://www.theverge.com/ai-artificial-intelligence/919028/canva-magic-layers-ai-replacing-palestine) ⭐️ 7.0/10

Canva 的 AI 功能 Magic Layers 被发现自动替换用户设计中的 Palestine 一词，进行了未经授权的内容修改。该公司随后为此问题公开道歉。 Magic Layers 旨在将平面图像分离为可编辑组件，而不是更改可见的文本内容。该问题首先由 X 用户@ros_ie9 发现并报告。

rss · The Verge AI · Apr 27, 14:29

**背景**: 此案例代表了一次重大 AI 伦理事件，即自动化内容修改在未经用户同意的情况下发生。Canva 将 Magic Layers 营销为一种在保持原始视觉完整性的同时使设计更具可编辑性的工具。特定词语的静默替换引发了对 AI 偏见和设计工具内容过滤的质疑。

**社区讨论**: 这一事件引发了关于 AI 内容操纵和企业责任的讨论。许多用户对 AI 工具未经授权更改其创意作品表示担忧，部分人质疑其他词语或内容是否也可能被静默修改。

**标签**: `#AI ethics`, `#content moderation`, `#Canva`, `#AI bias`, `#technology controversy`

---

<a id="item-21"></a>
## [重建 AI 数据基础设施](https://www.technologyreview.com/2026/04/27/1136322/rebuilding-the-data-stack-for-ai/) ⭐️ 7.0/10

MIT Technology Review Insights 报道称，企业正在意识到大规模有效采用 AI 的最大障碍是数据基础设施而非 AI 模型本身，这促使企业广泛重建数据堆栈。 这很重要因为大多数企业在 AI 模型上投入巨资，却忽略了基础数据层，导致尽管获得了董事会支持和预算，却仍无法大规模部署 AI。 现代 AI 数据基础设施的技术组件包括数据湖仓架构（结合数据仓库和数据湖功能）、用于管理机器学习特征的特征存储，以及用于模型部署和维护的 MLOps 管道。

rss · MIT Technology Review · Apr 27, 13:00

**背景**: 数据湖仓是一种新架构，结合了数据仓库（结构化、优化用于分析）和数据湖（灵活、用于原始数据）的优点。特征存储是用于存储机器学习管道中精选特征的集中式存储库。MLOps（机器学习运营）是指在生产中可靠高效地部署和维护机器学习模型的实践。传统企业数据系统并非为大规模 AI 需求而设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data_warehouse_architectures">Data warehouse architectures</a></li>
<li><a href="https://www.featurestore.org/">Feature Store For ML</a></li>
<li><a href="https://en.wikipedia.org/wiki/MLOps">MLOps - Wikipedia</a></li>

</ul>
</details>

**标签**: `#enterprise AI`, `#data infrastructure`, `#AI adoption`, `#digital transformation`, `#data stack`

---

<a id="item-22"></a>
## [谷歌警告恶意网页正在劫持企业 AI 代理](https://www.artificialintelligence-news.com/news/google-warns-malicious-web-pages-poisoning-ai-agents/) ⭐️ 7.0/10

谷歌研究人员发现，恶意行为者在公共网页的标准 HTML 中嵌入隐藏指令，通过间接提示注入攻击劫持企业 AI 代理。安全团队在扫描 Common Crawl 资料库（一个包含数十亿公共网页的海量数据库）时，发现了这些数字陷阱的不断增长的趋势。 这种攻击向量对在生产环境中部署 AI 代理的企业构成了关键安全威胁，因为它利用了 AI 代理浏览网站和处理网页内容的固有行为。依赖 AI 代理进行自动化的组织面临数据泄露、未授权代码执行和系统完全被接管的风险。 隐藏指令嵌入在 HTML 中，对人类用户不可见，但可以被处理网页内容的 AI 代理解析。安全研究人员表示，这种攻击技术在过去 12 个月中已从理论威胁转变为已确认的漏洞利用，有记录的 CVE 显示了通过 AI 编码助手实现的零点击远程代码执行能力。

rss · Artificial Intelligence News · Apr 27, 11:12

**背景**: 间接提示注入（IPI）攻击是一类威胁，通过将恶意指令与可信内容混合，嵌入在外部内容中的对抗性指令劫持 LLM 的行为。AI 代理通常依赖网页浏览和内容检索来收集信息，这使它们特别容易受到这种攻击向量的影响。Common Crawl 是一个 501(c)(3)非营利组织，维护着一个免费开放的网页抓取数据资料库，广泛用于 AI 训练和研究。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://commoncrawl.org/">Common Crawl - Open Repository of Web Crawl Data</a></li>
<li><a href="https://www.emergentmind.com/topics/indirect-prompt-injection-ipi-attacks">Indirect Prompt Injection Attacks</a></li>
<li><a href="https://www.sentinelone.com/cybersecurity-101/cybersecurity/indirect-prompt-injection-attacks/">What is Indirect Prompt Injection ? Risks & Prevention</a></li>

</ul>
</details>

**社区讨论**: 安全研究人员和 AI 从业者对这种攻击向量表示了重大担忧，许多人指出为人类用户设计的传统网络安全措施无法充分保护 AI 代理。该社区正在积极讨论潜在的缓解策略，包括内容清理、沙箱化和为 AI 代理操作实施更严格的信任边界。

**标签**: `#AI security`, `#prompt injection`, `#enterprise AI`, `#cybersecurity`, `#AI agents`

---

<a id="item-23"></a>
## [AlphaGo 创造者 David Silver 推出 11 亿美元超级学习者 AI 公司](https://www.wired.com/story/david-silver-ai-ineffable-intelligence-reinforcement-learning/) ⭐️ 7.0/10

Ineffable Intelligence 的方法以自我监督学习技术为中心，AI 系统通过环境交互发展能力，而非从大量人工标注示例中学习。这代表了一种与当前主导 AI 行业的数据密集型方法根本不同的范式。

rss · Hacker News - AI / LLM / Agent · Apr 28, 00:35

**背景**: David Silver 领导了创建 AlphaGo 的 DeepMind 团队，AlphaGo 是首个在围棋中击败职业人类选手的 AI。AlphaGo 的突破使用了深度强化学习结合树搜索。自我监督学习不同于传统监督学习，允许 AI 从原始数据中学习，无需人工标注，可能减少目前训练大型语言模型所需的大量人力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/04/27/deepminds-david-silver-just-raised-1-1b-to-build-an-ai-that-learns-without-human-data/">DeepMind's David Silver just raised $1.1B to build an AI that ...</a></li>
<li><a href="https://www.aibusinessreview.org/2026/04/27/david-silver-raises-1-1-billion-self-learning-ai/">David Silver Raises $1.1B for Self-Learning AI</a></li>

</ul>
</details>

**标签**: `#AI Research`, `#DeepMind`, `#Reinforcement Learning`, `#AlphaGo`, `#AI Industry`

---

<a id="item-24"></a>
## [开发者分享 ChatGPT 应用 3 个月审核历程](https://news.ycombinator.com/item?id=47923382) ⭐️ 7.0/10

一位开发者用仅仅 2 周的编程时间构建了一款名为 Tredict 的 ChatGPT 健身应用，但花费了 3 个月时间通过 OpenAI 的审核流程，最终获批并上架到 ChatGPT 应用商店。 这个案例为开发者提供了关于 OpenAI 应用提交时间和合规要求的罕见洞察。3 个月的审核周期以及为符合 OpenAI 的健身/健康准则而需要移除某些功能的要求，对其他计划提交 ChatGPT 应用的开发者来说是宝贵的学习经验。 该应用使用 MCP UI Apps 的交互式小部件而非仅仅是工具，在聊天窗口内渲染实际活动数据和训练计划。将用户认证内容嵌入沙盒 iframe 是最困难的技术挑战，因为 iframe 无法访问 OAuth 令牌。与 Claude 相比，ChatGPT 在创建多周训练计划方面存在更大的上下文窗口限制。

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Apr 27, 16:05

**背景**: OpenAI 于 12 月推出了 ChatGPT 应用目录，允许第三方开发者提交应用。该目录类似于应用商店，让用户可以浏览和安装集成了 ChatGPT 的应用程序。OpenAI 制定了健身/健康准则，应用必须遵守，审核流程确保合规性。MCP（模型上下文协议）是一种开放协议，使 AI 模型能够连接外部工具和服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://help.openai.com/en/articles/11487775-connectors-in-chatgpt">Apps in ChatGPT | OpenAI Help Center</a></li>
<li><a href="https://indianexpress.com/article/technology/artificial-intelligence/chatgpt-app-store-directory-third-party-services-how-to-use-10428147/">ChatGPT gets an app store-style directory , bringing third - party apps ...</a></li>

</ul>
</details>

**标签**: `#ChatGPT`, `#OpenAI`, `#App Development`, `#Fitness Tech`, `#Developer Experience`

---

<a id="item-25"></a>
## [摩尔线程财报：研发占比超 86%，万卡级智算集群落地](https://www.infoq.cn/article/GitNHq2Sa7K34WjiqmNq?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

摩尔线程发布最新财报显示，研发投入占比超过 86%，并宣布成功部署了万卡级（一万块 GPU）人工智能计算集群，这标志着中国本土 AI 基础设施建设的重大里程碑。 根据财报数据，摩尔线程持续加大研发投入，研发占比超过 86%。此次部署的万卡 GPU 集群是中国首个实际落地的国产万卡级 AI 集群系统，标志着 AI 基础设施能力的重大飞跃。

rss · InfoQ 中文站 · Apr 27, 15:32

**背景**: 摩尔线程科技有限公司成立于 2020 年 10 月，专注于图形处理器（GPU）设计。公司致力于为各行业提供先进的基础设施和一站式加速计算解决方案，推动数字化转型。万卡级集群概念代表了中国 AI 基础设施的新一代发展，标志着行业从传统计算向人工智能驱动的数字化转型的重要转变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Moore_Threads">Moore Threads - Wikipedia</a></li>
<li><a href="https://freshfromchina.com/chinas-ai-supercluster-scalex-ten-thousand-card-system-redefines-ai-computing-power/">China’s AI Supercluster: ScaleX “Ten Thousand Card” System ...</a></li>
<li><a href="https://en.mthreads.com/about">About Us | Moore Threads</a></li>

</ul>
</details>

**标签**: `#AI基础设施`, `#GPU计算`, `#中国芯片`, `#摩尔线程`, `#智算集群`

---

<a id="item-26"></a>
## [云区域失效：地缘政治风险下的高可用架构重构](https://www.infoq.cn/article/5qXyqHdrXhaT7iEr24l6?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

这个问题很重要，因为地缘政治紧张局势可能突然导致云区域不可访问或强制数据主权合规，直接影响具有全球云部署的组织的业务连续性。 文章探讨的策略包括在政治多元化地区进行主动-主动和主动-被动架构部署、地理冗余以及灾难恢复规划，以在整个云区域发生故障时保持服务可用性。

rss · InfoQ 中文站 · Apr 27, 13:00

**背景**: 云提供商将服务组织成地理区域，每个区域都有独立的基础设施。当地缘政治事件导致区域级故障（如制裁、监管或基础设施接管）时，工程团队需要预先规划的策略。地理冗余将工作负载分布在不同政治管辖区的区域中，以减轻单点故障。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/azure/well-architected/reliability/redundancy">Architecture Strategies for Designing for Redundancy ...</a></li>
<li><a href="https://www.cisco.com/c/en/us/td/docs/wireless/ucc/cpc/cnaaa/2026-02/geo-redundancy/cpc-geo-redundancy-guide-2026-02-0/m-pre-requisites-and-ip-allocation.html">UCC CPC AAA Geo Redundancy Guide, Release 2026.02.0</a></li>

</ul>
</details>

**标签**: `#cloud-infrastructure`, `#high-availability`, `#disaster-recovery`, `#geopolitical-risk`, `#cloud-architecture`

---

<a id="item-27"></a>
## [小米正式开源 MiMo-V2.5 系列 AI 模型](https://x.com/XiaomiMiMo/status/2048821516079661561) ⭐️ 7.0/10

小米正式开源 MiMo-V2.5 系列模型，采用 MIT 协议，允许免授权的商业部署、持续训练和微调。该系列包含两款模型：专注于复杂 Agent 和代码任务的 MiMo-V2.5-Pro，以及具备较强 Agent 能力的原生全模态模型 MiMo-V2.5。 此次开源使小米在与其它开源 AI 提供商的竞争中占据有利地位，其中 MiMo-V2.5-Pro 在 GDPVal-AA 和 ClawEval 评测中位列开源模型第一。这种商业友好的许可协议有望加速企业 AI 的采用，并促进更广泛的生态系统创新。 两款模型均支持高达 100 万 token 的上下文窗口，可处理长文档和进行扩展对话。MiMo-V2.5-Pro 专注于复杂的 agentic 工作流程和编码任务，而 MiMo-V2.5 则为多样化应用提供均衡的原生全模态能力。

telegram · zaihuapd · Apr 28, 00:27

**背景**: GDPVal-AA 是 Artificial Analysis 推出的评估框架，通过盲测对比评分（Elo 评分）测试 AI 模型在 44 个职业和 9 个主要行业中的经济价值知识工作表现。ClawEval 是用于真实世界 agent 工作流程的端到端基准评测，评估工具使用、规划、执行和恢复等能力。这两个基准评测都是独立评估，为 AI 模型在实际应用中的表现提供严格衡量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/evaluations/gdpval-aa">GDPval-AA Leaderboard | Artificial Analysis</a></li>
<li><a href="https://claw-eval.github.io/">Claw-Eval: A Transparent Benchmark for Real-World Agents</a></li>
<li><a href="https://llm-stats.com/benchmarks/gdpval-aa">GDPval-AA Leaderboard</a></li>

</ul>
</details>

**标签**: `#Xiaomi`, `#MiMo`, `#open-source AI`, `#multi-modal models`, `#LLM release`

---