---
layout: default
title: "Horizon Summary: 2026-04-04 (ZH)"
date: 2026-04-04
lang: zh
---

> From 160 items, 24 important content pieces were selected

---

1. [vLLM v0.19.0 发布：支持 Gemma 4 架构和零气泡推测解码](#item-1) ⭐️ 8.0/10
2. [Anthropic 阻止 OpenClaw 使用，强制第三方工具额外付费](#item-2) ⭐️ 8.0/10
3. [犹他州允许 AI 在无医生监督下开具精神科药物处方](#item-3) ⭐️ 8.0/10
4. [AI 编码代理将实现零日漏洞自动发现](#item-4) ⭐️ 8.0/10
5. [什么让开源 AI 模型真正成功：超越基准测试](#item-5) ⭐️ 8.0/10
6. [KubeVirt v1.8 为 Kubernetes 带来多虚拟机管理程序和机密计算功能](#item-6) ⭐️ 8.0/10
7. [谷歌开源 Gemma 4：支持手机离线运行 Agent](#item-7) ⭐️ 8.0/10
8. [国家网信办发布数字虚拟人管理征求意见稿 拟禁向未成年人提供虚拟伴侣服务](#item-8) ⭐️ 8.0/10
9. [Anthropic 成立新政治行动委员会瞄准中期选举](#item-9) ⭐️ 7.0/10
10. [Meta 暂停与 Mercor 合作 因数据泄露危机](#item-10) ⭐️ 7.0/10
11. [AI 生成的内核安全报告激增 10 倍](#item-11) ⭐️ 7.0/10
12. [Linux 内核维护者称 AI 安全报告现已真正有用](#item-12) ⭐️ 7.0/10
13. [JavaScript 无法绑过 Iframe 中的 CSP 元标签](#item-13) ⭐️ 7.0/10
14. [Axios 供应链攻击采用针对性社会工程手段](#item-14) ⭐️ 7.0/10
15. [PyPI 供应链攻击入侵 LiteLLM，致敏感信息被窃取](#item-15) ⭐️ 7.0/10
16. [Discord 开源 Osprey 安全规则引擎](#item-16) ⭐️ 7.0/10
17. [Cloudflare 在边缘部署主动式 API 漏洞扫描](#item-17) ⭐️ 7.0/10
18. [Cursor 3：面向 AI 代理的统一开发工作区](#item-18) ⭐️ 7.0/10
19. [Google Vids 接入 Veo 3.1，普通用户可免费生成 AI 视频](#item-19) ⭐️ 7.0/10
20. [美国人形机器人关键零部件依赖中国供应链](#item-20) ⭐️ 7.0/10
21. [Adobe 帮助台泄露 1300 万条支持工单](#item-21) ⭐️ 7.0/10
22. [工信部通报苹果设备高危漏洞风险：涉及 iOS 17.2.1 及以下版本](#item-22) ⭐️ 7.0/10
23. [调查指 LinkedIn 扫描用户浏览器扩展并向第三方共享数据](#item-23) ⭐️ 7.0/10
24. [逆向工程 Claude Code 签名可脱离 Bun 运行时](#item-24) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.19.0 发布：支持 Gemma 4 架构和零气泡推测解码](https://github.com/vllm-project/vllm/releases/tag/v0.19.0) ⭐️ 8.0/10

vLLM v0.19.0 版本发布，包含 448 个提交和 197 位贡献者，引入了完整的 Google Gemma 4 架构支持（需要 transformers>=5.5.0）、零气泡异步调度推测解码、成熟的 Model Runner V2 与管道并行的分段 CUDA 图、ViT 完整 CUDA 图捕获，以及带可插拔缓存策略的通用 CPU KV 缓存卸载功能。 此版本对 LLM 推理从业者具有重要意义，因为它通过零气泡推测解码和分段 CUDA 图提供主要性能提升，同时将模型支持扩展到 Gemma 4 等前沿架构。CPU KV 缓存卸载和 DBO 泛化提供更灵活的部署选项和更广泛的硬件兼容性。 关键特性包括：零气泡异步调度与推测解码（#32951）、Model Runner V2 获得 PP CUDA 图（#35162）和推测解码拒绝采样器（#37238、#37237）、ViT 完整 CUDA 图捕获（#35963）、带块级抢占的通用 CPU KV 缓存卸载（#37160、#37874、#34805）、DBO 泛化到通用模型（#37926），以及默认启用 allreduce 融合的 NVIDIA B300/GB300（SM 10.3）支持。

github · khluu · Apr 3, 02:19

**背景**: vLLM 是用于大型语言模型的高性能推理引擎。推测解码使用较小的草稿模型预测令牌，由较大的模型验证，从而提高吞吐量。分段 CUDA 图将模型计算分割成片段，在保持 CUDA 图优势的同时减少编译开销。CPU KV 缓存卸载允许将 KV 缓存移动到 CPU 内存，以在有限的 GPU 内存中支持更长的序列或更大的模型。EPLB（专家并行负载均衡器）在 MoE 模型中重新分配专家映射，以平衡专家并行等级之间的负载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.sglang.io/advanced_features/piecewise_cuda_graph.html">Piecewise CUDA Graph — SGLang</a></li>
<li><a href="https://docs.vllm.ai/en/stable/design/cuda_graphs/">CUDA Graphs - vLLM</a></li>
<li><a href="https://docs.vllm.ai/en/latest/serving/expert_parallel_deployment/">Expert Parallel Deployment - vLLM</a></li>

</ul>
</details>

**标签**: `#llm-inference`, `#vllm`, `#machine-learning`, `#cuda`, `#speculative-decoding`

---

<a id="item-2"></a>
## [Anthropic 阻止 OpenClaw 使用，强制第三方工具额外付费](https://www.theverge.com/ai-artificial-intelligence/907074/anthropic-openclaw-claude-subscription-ban) ⭐️ 8.0/10

这项政策变化严重影响了依赖 OpenClaw 等第三方工具实现 Claude AI 自动化的开发者。这标志着 Anthropic 定价策略的重大转变，可能影响更广泛的 AI 代理生态系统，并迫使开发者承担更高成本或寻找替代方案。 这一政策变化严重影响依赖 OpenClaw 等第三方工具来自动化 Claude AI 的开发者。它代表了 Anthropic 定价策略的重大转变，可能影响更广泛的 AI 代理生态系统，迫使开发者承担更高成本或寻找替代方案。 Anthropic 提供一次性积分，金额等于月订阅价格（4 月 17 日前可兑换），并对预购使用套餐提供高达 30%的折扣。公司将原因归咎为"对我们的系统造成过度压力"，表示必须优先保障核心产品用户的容量。

rss · The Verge AI · Apr 3, 23:52

**背景**: OpenClaw 是一个开源的自主 AI 代理框架，起着"工具"的作用——即一种使 Claude 等 AI 模型能够自主执行编码等任务的框架。AI 中的"工具"一词指的是围绕 AI 代理构建环境使其能够可靠工作的工具。Anthropic 还发布了 Claude Code Channels，这是一款竞争产品，允许用户通过 Discord 或 Telegram 直接向 Claude Code 发送消息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://venturebeat.com/orchestration/anthropic-just-shipped-an-openclaw-killer-called-claude-code-channels">Anthropic just shipped an OpenClaw killer called Claude Code Channels, letting you message it over Telegram and Discord | VentureBeat</a></li>
<li><a href="https://docs.openclaw.ai/tools/acp-agents">ACP Agents - OpenClaw</a></li>
<li><a href="https://github.com/walkinglabs/awesome-harness-engineering">GitHub - walkinglabs/awesome- harness -engineering: Awesome...</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂。部分用户理解这一经济考量——自主代理（如 OpenClaw）的重度用户实际上通过订阅计划补贴了他们的使用量。其他用户则认为这是订阅模式与人类使用设计的"结构性错配"，与自主代理的基础设施负载相冲突。部分用户正考虑因成本增加而转向其他 AI 模型。

**标签**: `#Anthropic`, `#Claude AI`, `#OpenClaw`, `#AI pricing`, `#AI policy`

---

<a id="item-3"></a>
## [犹他州允许 AI 在无医生监督下开具精神科药物处方](https://www.theverge.com/ai-artificial-intelligence/906525/ai-chatbot-prescribe-refill-psychiatric-drugs) ⭐️ 8.0/10

犹他州成为美国第二个允许名为 Doctronic 的人工智能系统无需医生直接监督即可开具和续配精神科药物的州，这是该国第二次授予人工智能此类临床处方权。 这标志着可能在全国范围内开创人工智能医疗先例的重要监管里程碑。虽然州官员称赞此举可以降低医疗成本并缓解心理健康护理短缺问题，但医生们对透明度、患者安全以及人工智能驱动医疗决策缺乏监督感到担忧。 该人工智能仅处理处方续配，不处理初始处方——必须由人类医生首先开具处方。它涵盖多达 190 种常用药物，但无法处理需要血液检测监测的药物。在与犹他州监管机构共享的数据中，Doctronic 将其人工智能系统与人类临床医生在 500 个紧急护理病例中进行了比较。

rss · The Verge AI · Apr 3, 11:43

**背景**: 这是美国第二次授予人工智能临床处方权，之前仅有加州获得批准。该系统代表了医疗授权方式的重大转变，引发了关于人工智能在高风险医疗决策中问责性的问题。犹他州官员认为，这一试点项目可以帮助解决农村地区精神科护理提供者短缺的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theverge.com/ai-artificial-intelligence/906525/ai-chatbot-prescribe-refill-psychiatric-drugs">Chatbots are now prescribing psychiatric drugs | The Verge</a></li>
<li><a href="https://www.thewellnesslondon.com/ai-doctor/blog/ai-prescribing-is-here-what-utah-s-doctronic-pilot-means-for-healthcare">AI Prescribing Is Here: What Utah's Doctronic Pilot Means for...</a></li>

</ul>
</details>

**社区讨论**: 医生们对该系统的不透明度表达了严重担忧，警告人工智能驱动的处方缺乏患者安全所需的透明度。批评者认为，如果没有明确的监督机制，患者可能面临算法错误或不当处方的风险。支持者则反驳说，该系统可以显著降低医疗成本并改善心理健康服务的可及性。

**标签**: `#AI regulation`, `#healthcare AI`, `#medical AI`, `#AI policy`, `#psychiatric care`

---

<a id="item-4"></a>
## [AI 编码代理将实现零日漏洞自动发现](https://simonwillison.net/2026/Apr/3/vulnerability-research-is-cooked/#atom-everything) ⭐️ 8.0/10

Thomas Ptacek 认为，AI 编码代理只需指向源代码并输入「帮我找零日漏洞」，就能实现零日漏洞的自动发现，这将在未来几个月内从根本上改变漏洞研究的经济学和工作方式。 这代表了网络安全的基本范式转变。大型语言模型可能会自动化大多数高影响力漏洞研究，使零日发现变得任何人都可以访问，只需使用前沿 AI 模型即可，从而极大降低漏洞开发的准入门槛。 大型语言模型特别适合漏洞研究，因为它们的权重中编码了大量源代码关联知识和已记录的漏洞类别（陈旧指针、整数误用、类型混淆、分配器美化等）的信息。它们擅长对漏洞类别进行模式匹配，并能够进行约束求解以实现可达性和可利用性评估，而且可以进行无限的试错而不会感到厌倦。

rss · Simon Willison · Apr 3, 23:59

**背景**: 漏洞研究是发现软件中可被利用的安全缺陷的实践。零日漏洞是指尚未修补的未知缺陷。传统上，这需要高素质的安全研究人员手动分析源代码。前沿 AI 模型指的是最新一代的大型语言模型。这篇文章的灵感来自于对 Anthropic 公司 Nicholas Carlini 的播客采访。

**社区讨论**: 原文曾在 Security Cryptography Whatever 播客上讨论，并在 Simon Willison 的博客上标记为 ai-security-research，该标签下已有 11 篇文章。

**标签**: `#AI`, `#cybersecurity`, `#vulnerability-research`, `#LLMs`, `#exploit-development`, `#AI-agents`

---

<a id="item-5"></a>
## [什么让开源 AI 模型真正成功：超越基准测试](https://www.interconnects.ai/p/gemma-4-and-what-makes-an-open-model) ⭐️ 8.0/10

这个分析很重要，因为它将注意力从单纯的性能指标转移到实际元素上，这些元素决定了开源权重模型在日益拥挤的 AI 领域是否能产生实际影响并获得开发者采用。 Gemma 4 在宽松的 Apache 2.0 许可证下发布，可从 Hugging Face、Kaggle 和 Ollama 获取，支持在 Google Colab、Vertex AI 或消费级 GPU 等平台上进行定制—— Lambert 认为这些是超越原始能力的关键差异因素。

rss · Interconnects · Apr 3, 16:57

**背景**: "开源权重"与"完全开源"模型之间的辩论是 AI 生态系统讨论的核心。像 Gemma 这样的开源权重模型提供用于推理和微调的模型参数，但不披露训练代码或数据集，这与真正开源的替代方案不同。Google 最近的 Gemma 4 发布强调代理 AI 和编码能力，将这些模型定位为对抗中国开源权重竞争者的产品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/gemma-4/">Gemma 4: Byte for byte, the most capable open models</a></li>
<li><a href="https://www.theregister.com/2026/04/02/googles_gemma_4_open_weights/">Google battles Chinese open weights models with Gemma 4 • The Register</a></li>
<li><a href="https://ai.google.dev/gemma/docs/core">Gemma 3 model overview | Google AI for Developers</a></li>

</ul>
</details>

**标签**: `#open-source AI`, `#Gemma`, `#Google AI`, `#model ecosystem`, `#AI strategy`

---

<a id="item-6"></a>
## [KubeVirt v1.8 为 Kubernetes 带来多虚拟机管理程序和机密计算功能](https://www.infoq.cn/article/kwmoqShV5lx0TslYbo3j?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

此版本显著扩展了 Kubernetes 的虚拟化和安全功能，使用户能够使用不同的虚拟机管理程序管理虚拟机，同时在处理过程中保护敏感数据。 多虚拟机管理程序支持使组织能够在 Kubernetes 中利用不同的虚拟化技术，而机密计算通过将敏感信息隔离在受保护的 CPU 飞地中来保护使用中的数据。

rss · InfoQ 中文站 · Apr 3, 15:00

**背景**: KubeVirt 是一个用于 Kubernetes 的虚拟机管理附加组件，它扩展了平台能力，使其能够使用相同的 API、工具和工作流程与容器一起运行和管理虚拟机。机密计算是一种安全技术，通过使用 CPU 飞地在内存中加密数据来保护处理中的数据，解决了传统数据保护（通常仅涵盖传输中和静态数据）的空白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kubevirt.io/">KubeVirt.io</a></li>
<li><a href="https://cloud.google.com/security/products/confidential-computing">Confidential Computing | Google Cloud</a></li>
<li><a href="https://www.ibm.com/think/topics/confidential-computing">What Is Confidential Computing? | IBM</a></li>

</ul>
</details>

**标签**: `#Kubernetes`, `#KubeVirt`, `#Virtualization`, `#Confidential Computing`, `#Cloud Native`

---

<a id="item-7"></a>
## [谷歌开源 Gemma 4：支持手机离线运行 Agent](https://www.infoq.cn/article/X1c6ZllztrQhGEIoYrBR?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

谷歌正式发布开源 AI 模型 Gemma 4，这是一款面向终端设备优化的模型，具备手机离线运行 AI Agent 的能力，并显著降低内存占用，可在支流智能手机上无网络连接部署运行。 此版本发布使 Gemma 4 成为与阿里巴巴 Qwen 在开源模型竞争中的直接对手，标志着谷歌持续推进终端 AI 前沿。它实现了移动设备上的离线、低延迟、高隐私智能交互能力。 Gemma 4 由 Google DeepMind 开发，采用与专有 Gemini 模型相同的安全评估方法。该模型专为边缘计算场景设计，在保持推理能力的同时大幅压缩参数规模和运行开销。

rss · InfoQ 中文站 · Apr 3, 14:40

**背景**: Gemma 是谷歌开源的轻量级 AI 模型系列。此前的 Gemma 3 强调效率，可单 GPU 或 TPU 运行，甚至在手机上运行。Mobile-Agent 指能够通过视觉感知自主操作智能手机应用程序的 AI 智能体，可自动规划、执行和反思操作步骤。Qwen（通义千问）是阿里巴巴的开源大语言模型系列。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.google.dev/gemma/docs/core/model_card_4?hl=zh-cn">Gemma 4 模 型 卡片 | Google AI for Developers</a></li>
<li><a href="https://www.winandmac.com/2025/03/google-gemma-3-open-source-model/">Google 發佈開 源 Gemma ... - winandmac.com 視麥媒體</a></li>
<li><a href="https://github.com/QwenLM/Qwen">GitHub - QwenLM/ Qwen : The official repo of Qwen (通义千问) chat...</a></li>

</ul>
</details>

**标签**: `#Google Gemma`, `#Open Source AI`, `#Mobile AI`, `#Large Language Models`, `#AI Model Competition`

---

<a id="item-8"></a>
## [国家网信办发布数字虚拟人管理征求意见稿 拟禁向未成年人提供虚拟伴侣服务](https://mp.weixin.qq.com/s/EHpjg2sfth0W7OE-v6hq9g) ⭐️ 8.0/10

国家互联网信息办公室于 2026 年 4 月 3 日发布征求意见稿，要求数字虚拟人服务展示区域全程显著标识「数字人」字样，使用自然人敏感个人信息建模需取得单独同意，并禁止向未成年人提供虚拟伴侣服务，违规最高可处 20 万元罚款。 具有舆论属性或社会动员能力的服务提供者须履行算法备案和安全评估手续。用户撤回同意后有权注销数字虚拟人。征求意见截止时间为 2026 年 5 月 6 日。

telegram · zaihuapd · Apr 3, 09:39

**背景**: 数字虚拟人是通过 AI 技术生成的数字形象，可与用户在线互动。该法规出台正值全球对 AI 伴侣产品监管日益严格之际——从欧盟《人工智能法案》将「情绪识别」类 AI 列为高风险应用，到美国联邦贸易委员会对 AI 伴侣产品展开调查。中国的方法旨在将工具型 AI（如知识问答、客服助手）与涉及情感交流的陪伴型 AI 区分开来，对后者实施更严格的监管。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cac.gov.cn/2025-12/28/c_1768662848000498.htm">专家解读｜规范人工智能前沿业态健康发展的新探索：解读《人工智能拟...</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1994117858939135385">剑悬“虚拟恋人”：中国AI伴侣新规深度解析 - 知乎</a></li>
<li><a href="https://beian.cac.gov.cn/">互联网信息服务算法备案系统</a></li>

</ul>
</details>

**社区讨论**: 行业专家将该征求意见稿视为平衡创新与风险防范的积极举措，为 AI 伴侣、虚拟偶像等新兴业态提供明确指引。然而，部分担忧仍存在于工具型与陪伴型 AI 的定义边界上，混合型产品如何进行合规处理也成为讨论焦点。

**标签**: `#AI regulation`, `#virtual companions`, `#China tech policy`, `#minor protection`, `#digital virtual humans`

---

<a id="item-9"></a>
## [Anthropic 成立新政治行动委员会瞄准中期选举](https://techcrunch.com/2026/04/03/anthropic-ramps-up-its-political-activities-with-a-new-pac/) ⭐️ 7.0/10

这一发展标志着 Anthropic 直接进入选举政治，标志着人工智能行业企业政治参与的显著升级，并可能影响未来的科技政策和监管。 该政治行动委员会准备支持符合 Anthropic 在人工智能监管、安全标准和行业治理方面政策立场的候选人，但具体财务细节和目标候选人尚未披露。

rss · TechCrunch AI · Apr 3, 20:22

**背景**: 政治行动委员会(PAC)是一种筹集和支出资金以选举或击败候选人的组织。在美国，企业被禁止直接向候选人捐款，但可以组建政治行动委员会，从员工和股东那里收集自愿捐款用于选举目的。人工智能行业政治参与度不断上升，因为各公司试图影响围绕人工智能安全、治理和竞争定位的新兴法规。

**标签**: `#AI policy`, `#corporate politics`, `#Anthropic`, `#lobbying`, `#tech industry`

---

<a id="item-10"></a>
## [Meta 暂停与 Mercor 合作 因数据泄露危机](https://www.wired.com/story/meta-pauses-work-with-mercor-after-data-breach-puts-ai-industry-secrets-at-risk/) ⭐️ 7.0/10

Meta 已暂停与主要 AI 数据供应商 Mercor 的合作关系，此前发生的安全漏洞可能暴露了多家领先 AI 实验室的专有 AI 训练数据和方法。 这一事件凸显了 AI 供应链中的安全风险，可能对整个 AI 行业产生深远影响，因为泄露的数据可能包含各公司花费数年时间开发的敏感训练方法。 漏洞发生在 Mercor，该公司为 AI 模型训练提供数据标注和处理服务。多家人工智能实验室目前正在调查数据泄露的具体程度。泄露数据的具体性质和事件时间线尚不清楚。

rss · WIRED AI · Apr 3, 21:28

**背景**: Mercor 是一家为 AI 公司提供训练数据服务的数据供应商，包括数据标注、整理和处理，这些对开发大型语言模型和其他 AI 系统至关重要。像 Mercor 这样的数据处理商处理大量用于训练 AI 模型的潜在敏感信息，使其成为安全漏洞的有吸引力的目标。

**标签**: `#AI security`, `#data breach`, `#Meta`, `#AI industry`, `#Mercor`, `#corporate news`

---

<a id="item-11"></a>
## [AI 生成的内核安全报告激增 10 倍](https://simonwillison.net/2026/Apr/3/willy-tarreau/#atom-everything) ⭐️ 7.0/10

这代表了开源安全维护的重大转变，因为 AI 工具现在正在大规模发现真正的漏洞。Linux 内核维护者面临着前所未有的工作负载增加，同时还要处理来自不同 AI 工具的重复报告。 大多数 AI 生成的报告都是有效的，维护人员现在每天都会看到重复的报告——同一个小漏洞被使用不同 AI 工具的人发现。周五和周二是最糟糕的日子。

rss · Simon Willison · Apr 3, 21:48

**背景**: Willy Tarreau 是 HAProxy（一个流行的开源负载均衡器和代理服务器）的首席软件开发人员。他也在 Linux 内核安全邮件列表上活跃。Linux 内核是 Android 和 Linux 操作系统的核心，其安全维护依赖于志愿维护者。

**标签**: `#security`, `#linux-kernel`, `#AI`, `#vulnerability-reports`, `#open-source-maintenance`

---

<a id="item-12"></a>
## [Linux 内核维护者称 AI 安全报告现已真正有用](https://simonwillison.net/2026/Apr/3/greg-kroah-hartman/#atom-everything) ⭐️ 7.0/10

这标志着 AI 在实际安全工作中的实用性取得了显著里程碑，来自一位备受尊敬的权威来源。这表明 AI 工具在开源项目的真实安全漏洞检测中正变得可行。 Kroah-Hartman 指出，“一个月前发生了一些事情”导致了这一转变。以前 AI 生成的报告“明显错误或质量低劣”“有点可笑”，但现在所有开源项目都收到了 AI 生成的优质真实安全报告。

rss · Simon Willison · Apr 3, 21:44

**背景**: Greg Kroah-Hartman 是一位备受尊敬的 Linux 内核维护者，以维护稳定内核版本和直接、技术性的方式著称。他此前曾对低质量的内核贡献持批评态度。Linux 内核项目是全球最大、最重要的开源项目之一，其安全流程对整个软件生态系统具有重要意义。

**标签**: `#linux`, `#ai`, `#security`, `#open-source`, `#kernel`

---

<a id="item-13"></a>
## [JavaScript 无法绑过 Iframe 中的 CSP 元标签](https://simonwillison.net/2026/Apr/3/test-csp-iframe-escape/#atom-everything) ⭐️ 7.0/10

安全研究员 Simon Willison 发现，即使后续的不可信 JavaScript 试图操纵，在 iframe 内容顶部注入的 CSP 元标签仍然会被执行，从而实现无需单独域的安全沙箱隔离。 这一发现使开发者无需使用单独域名即可构建具有 CSP 保护的工件/沙箱代码执行环境（类似 Claude Artifacts），从而简化了交互式 Web 应用的安全架构。 研究表明，放在 iframe srcdoc 内容开头的 meta http-equiv="Content-Security-Policy"标签会被浏览器遵守，且 JavaScript 无法在页面加载后修改或移除它们。

rss · Simon Willison · Apr 3, 16:05

**背景**: 内容安全策略(CSP)是一种通过控制页面可以加载的资源来帮助防止 XSS 和数据注入攻击的安全头。Iframe 通常用于隔离不可信内容，但传统上需要单独的域名才能实现有效隔离。srcdoc 属性允许直接在 iframe 中嵌入 HTML，而无需外部 URL。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/bhaveshk90/Content-Security-Policy-CSP-Bypass-Techniques">GitHub - bhaveshk90/Content-Security-Policy-CSP-Bypass-Techniques: Content-Security-Policy (CSP) Bypass Techniques · GitHub</a></li>
<li><a href="https://www.browserstack.com/guide/csp-bypass">Learn & bypass Content Security Policy HTTP Response Header | BrowserStack</a></li>

</ul>
</details>

**标签**: `#iframes`, `#security`, `#javascript`, `#content-security-policy`, `#sandboxing`

---

<a id="item-14"></a>
## [Axios 供应链攻击采用针对性社会工程手段](https://simonwillison.net/2026/Apr/3/supply-chain-social-engineering/#atom-everything) ⭐️ 7.0/10

这次攻击表明，供应链威胁正在从自动化漏洞利用演变为高度针对性的、以人为中心的社会工程活动。每个维护被广泛使用的开源软件包的开发者都需要了解这种攻击策略。 攻击者克隆了一家公司及其创始人的形象，创建了一个品牌化的 Slack 工作空间，其中包含似乎是开源软件维护者的虚假资料，安排了一次 Microsoft Teams 会议，并说服维护者安装看似系统更新的东西——实际上是一个远程访问木马(RAT)，用于窃取凭据以发布恶意的 npm 包。

rss · Simon Willison · Apr 3, 13:54

**背景**: UNC1069 是一个自 2018 年以来活跃的、受到经济利益驱动的朝鲜威胁行为者，与 BlueNoroff（专门从事加密货币盗窃的 Lazarus Group 子组织）有关联。此次攻击部署了 WAVESHAPER.V2，这是一个跨平台后门的更新版本。这标志着针对开源维护者的最复杂供应链攻击之一，通过直接的社会工程手段实施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.google.com/blog/topics/threat-intelligence/unc1069-targets-cryptocurrency-ai-social-engineering">UNC1069 Targets Cryptocurrency Sector with New ... - Google Cloud</a></li>
<li><a href="https://thehackernews.com/2026/04/google-attributes-axios-npm-supply.html">Google Attributes Axios npm Supply Chain Attack to North ...</a></li>
<li><a href="https://cybersecsentinel.com/axios-npm-backdoored-unc1069-deploys-cross-platform-rat-via-supply-chain-attack/">Axios npm Backdoored: UNC1069 Deploys Cross-Platform RAT via ...</a></li>

</ul>
</details>

**社区讨论**: 讨论强调开发者经常需要在时间压力下安装会议软件，并经常快速点击确认提示，使得这成为一种非常有效的攻击向量。许多人评论说，热门软件包的维护者是这种针对性攻击的主要目标。

**标签**: `#supply-chain-security`, `#social-engineering`, `#axios`, `#security-incident`, `#malware`

---

<a id="item-15"></a>
## [PyPI 供应链攻击入侵 LiteLLM，致敏感信息被窃取](https://www.infoq.cn/article/YqWdW6lF74rlqXkJ5AMJ?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

PyPI 供应链攻击入侵了 LiteLLM 库，导致敏感数据被窃取。被篡改的版本下载次数超过 4 万次。 此事件凸显了开源包仓库的脆弱性，以及开发者在使用第三方库时面临的风险。被入侵的依赖项可能导致数百万应用程序面临数据泄露和进一步攻击的风险。 此次攻击由 FutureSearch 研究员 Callum McMahon 发现。LiteLLM 通过标准化 API 兼容性简化了对 100 多个 LLM 的访问。这并非孤立事件——PyPI 近期已发生多起供应链攻击。

rss · InfoQ 中文站 · Apr 3, 15:00

**背景**: 供应链攻击的目标是软件分发渠道，旨在将恶意代码注入合法包中。PyPI（Python 包索引）是 Python 包的官方仓库，每天服务数百万开发者。当攻击者入侵热门库时，所有下游用户都会变得脆弱。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.litellm.ai/">LiteLLM</a></li>
<li><a href="https://blog.eimoon.com/p/litellm-pypi-supply-chain-attack-analysis/">LiteLLM PyPI 供 应 链 攻 击 复盘：受影响版本、 攻 击 方式与止损建议</a></li>
<li><a href="https://www.infoq.cn/article/YqWdW6lF74rlqXkJ5AMJ">PyPI 供 应 链 攻 击 导致 LiteLLM 遭入侵，致使敏感信息被窃取 - InfoQ</a></li>

</ul>
</details>

**社区讨论**: Andrej Karpathy 向开发者发出了关于此次攻击的警报，该事件迅速在 AI 和 Python 社区中传播。此事引发了人们对软件包仓库安全性和更佳验证机制需求的担忧。

**标签**: `#供应链攻击`, `#PyPI`, `#安全`, `#LiteLLM`, `#数据泄露`

---

<a id="item-16"></a>
## [Discord 开源 Osprey 安全规则引擎](https://www.infoq.cn/article/Wz12mUPtcy79cyTsIOwV?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Discord 开源了其内部安全规则引擎 Osprey，该引擎由 ROOST 团队开发，每秒可处理 230 万条规则，每天处理 4 亿次操作。 Osprey 采用 Rust 协调器构建，以实现高性能和低延迟。它作为一个事件流决策引擎设计，用于大规模检测和移除有害内容。

rss · InfoQ 中文站 · Apr 3, 11:00

**背景**: 规则引擎是一种软件系统，用于根据预定义的规则对传入的事件或数据进行自动决策。Discord 每天处理数十亿次用户操作，因此快速规则评估对于内容审核和用户安全至关重要。Discord 的 ROOST 团队专注于平台信任与安全基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/roostorg/osprey">GitHub - roostorg/ osprey : Automate the obvious and investigate the...</a></li>
<li><a href="https://www.live-feeds.com/2026/03/31/discord-open-sources-osprey-safety-rules-engine-processing-2-3-million-rules-per-second/">Discord Open Sources Osprey Safety Rules Engine ... - Live Feeds</a></li>
<li><a href="https://discord.com/press-releases/roost-announces-coop-and-osprey-free-open-source-trust-and-safety-infrastructure-for-the-ai-era">ROOST Announces “Coop” and “ Osprey ”: Free, Open-Source Trust...</a></li>

</ul>
</details>

**标签**: `#security`, `#open-source`, `#rules-engine`, `#performance`, `#Discord`

---

<a id="item-17"></a>
## [Cloudflare 在边缘部署主动式 API 漏洞扫描](https://www.infoq.cn/article/8LBRc9hODxYmCvKU85fy?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

扫描在边缘进行，意味着它可以实时分析 API 流量而不会引入延迟。Cloudflare 的方法允许持续监控，并可识别常见漏洞，如身份验证缺陷、数据过度暴露和缺乏速率限制。 这代表了向边缘安全的重要转变，使组织能够在网络边缘识别 API 漏洞，从而在恶意行为者利用之前进行修复。随着 API 成为现代应用的主要攻击向量，这一功能解决了人们日益关注的 API 安全问题。

rss · InfoQ 中文站 · Apr 3, 10:30

**背景**: 随着组织越来越依赖 API 来连接服务和暴露数据，API 安全已成为一个关键问题。传统的 API 安全解决方案通常需要代理或 API 网关，这会增加复杂性和潜在的故障点。边缘扫描提供了一种替代方法，利用现有的 Cloudflare 网络基础设施。

**标签**: `#cloud-security`, `#api-security`, `#edge-computing`, `#vulnerability-scanning`, `#cloudflare`

---

<a id="item-18"></a>
## [Cursor 3：面向 AI 代理的统一开发工作区](https://cursor.com/blog/cursor-3) ⭐️ 7.0/10

Cursor 发布版本 3，将自身定位为面向 AI 代理的统一开发工作区，采用全新设计的以代理为中心的界面，支持多仓库工作区，并通过移动端、网页、桌面端以及 Slack、GitHub、Linear 等集成入口提供跨平台访问。 这代表了从管理代码到管理 AI 代理的重大转变，使开发者能够并行运行多个代理，并在本地（用于快速迭代）和云端（用于离线或切换任务时持续运行）之间无缝切换，从而显著提升开发效率。 Cursor 3 支持云端本地混合会话，本地代理用于修改和测试，云端代理可在离线或切换任务时继续运行。新增的集成 diff 视图可更快地编辑和审查变更，并继续支持暂存、提交和管理 Pull Request。Composer 2 在 Terminal-Bench 2.0 上获得 61.7 分。

telegram · zaihuapd · Apr 3, 02:00

**背景**: Cursor 是一款基于 VS Code 构建的 AI 优先代码编辑器，广泛用于 AI 辅助软件开发。向以代理为中心的工作流的转变反映了 AI 代理从对话工具向实际生产辅助工具发展的更广泛趋势。云端本地混合开发环境已成为在不同工作场景下保持 AI 代理持续运行的关键能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/ai-software-engineer/cursor-3-has-arrived-and-just-went-agent-first-b8a078d87c93">Cursor 3 Has Arrived — And Just Went Agent-First... | Medium</a></li>
<li><a href="https://railsdrop.com/2026/01/03/engineers-guide-to-cursor-ai-mastering-the-ai-first-ide-in-2026/">Engineer’s Guide to Cursor AI : Mastering the AI -First IDE in 2026</a></li>
<li><a href="https://blog.eimoon.com/p/claude-code-remote-control-guide/">Claude Code 远程控制指南：随时随地掌控你的本地开发环境</a></li>

</ul>
</details>

**社区讨论**: 开发者社区认为这是从代码编辑器向 AI 代理管理平台的重要演进。用户特别看重并行代理执行能力和无缝的云端本地切换功能，尽管有人指出传统 IDE 在需要时仍然可用。这一变化被视为向管理 AI 代理而非仅编写代码的实际进步。

**标签**: `#AI code editor`, `#Cursor`, `#software development tools`, `#AI agents`, `#developer productivity`

---

<a id="item-19"></a>
## [Google Vids 接入 Veo 3.1，普通用户可免费生成 AI 视频](https://www.techradar.com/ai-platforms-assistants/google-is-pushing-ai-video-into-ordinary-life-just-as-openai-pulls-sora-back) ⭐️ 7.0/10

Google 更新了基于浏览器的 AI 视频创作工具 Google Vids，接入 Veo 3.1 模型，所有 Google 账号用户每月可免费生成 10 次视频。该更新还整合了 Lyria 3 音乐生成功能，可创作 30 秒至 3 分钟的配乐，但该功能仅向 Google AI Pro 和 Ultra 订阅用户开放。 这标志着 AI 视频创作的重大民主化，使先进视频生成技术对普通用户可访问，同时为付费用户保留高级功能。这一举措与 OpenAI 对 Sora 的限制性做法形成鲜明对比，凸显了 Google 将 AI 能力嵌入主流平台以实现大规模采用的战略。 此次更新包含可自定义外观、语音和道具的数字化身功能，AI Ultra 订阅用户每月可获得最多 1,000 次视频生成额度。Veo 3.1 支持 4K 输出，具备 16:9 横向和 9:16 纵向宽高比，并可生成原生音频。

telegram · zaihuapd · Apr 3, 05:23

**背景**: Google Vids 是 Google 创意套件中的浏览器端 AI 视频制作工具，使用户能够通过文本提示生成专业级视频。Veo 3.1 于 2025 年 10 月发布，是 Google 最先进的视频生成模型，可生成长达 8 秒、最高 4K 分辨率并集成音频的片段。这一整合使 Google 能够在快速增长的 AI 视频生成市场与 OpenAI 的 Sora 直接竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aistudio.google.com/models/veo-3">Veo 3 | Google AI Studio</a></li>
<li><a href="https://deepmind.google/models/veo/">Veo — Google DeepMind</a></li>
<li><a href="https://deepmind.google/models/lyria/">Lyria 3 — Google DeepMind</a></li>

</ul>
</details>

**标签**: `#AI Video Generation`, `#Google Vids`, `#Veo 3.1`, `#Consumer AI Tools`, `#Google AI Strategy`

---

<a id="item-20"></a>
## [美国人形机器人关键零部件依赖中国供应链](https://www.wsj.com/tech/under-the-skin-of-americas-humanoid-robots-chinese-technology-27dd4fdf) ⭐️ 7.0/10

宇树科技（Unitree Robotics）是一家位于杭州的中国机器人公司，成立于 2016 年，最初专注于消费市场的四足机器人。摩根士丹利已发布多份关于人形机器人行业的报告，预测了潜在市场规模和成本结构。《华尔街日报》文中提到的机器人代表娱乐（迪士尼）和工业（特斯拉）应用的交叉领域。

telegram · zaihuapd · Apr 3, 08:55

**背景**: Unitree Robotics (宇树科技) is a Hangzhou-based Chinese robotics company founded in 2016, initially specializing in quadruped robots for the consumer market. Morgan Stanley has published multiple reports on the humanoid robot industry, projecting potential market sizes and cost structures. The robots mentioned in the WSJ article represent the intersection of entertainment (Disney) and industrial (Tesla) applications.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unitree_Robotics">Unitree Robotics - Wikipedia</a></li>
<li><a href="https://www.unitree.com/">Unitree Robotics | Robot Dog_Quadruped_Humanoid Robotics ...</a></li>
<li><a href="https://news.qq.com/rain/a/20240628A07LSS00">解读摩根士丹利最新人形机器人报告：30万亿美金市场规模与特斯拉Optim...</a></li>

</ul>
</details>

**标签**: `#humanoid_robots`, `#supply_chain`, `#us_china_tech`, `#manufacturing`, `#tesla_optimus`

---

<a id="item-21"></a>
## [Adobe 帮助台泄露 1300 万条支持工单](https://cybernews.com/security/threat-actor-claims-adobe-data-theft/?utm_source=flipboard&amp;utm_content=CyberNews_com%2Fmagazine%2FLatest+cybersecurity+news) ⭐️ 7.0/10

该新闻项带有"茶馆讨论"标签，表明社区参与度，但撰写时未显示具体的讨论内容。 这一事件凸显了帮助台系统的脆弱性，以及第三方供应商访问带来的潜在风险。研究人员指出，此次泄露的范围似乎仅限于帮助台系统，而非 Adobe 的核心内部网络。员工记录和内部通信的潜在泄露仍可能引发重大的安全和隐私问题。

telegram · zaihuapd · Apr 3, 10:40

**背景**: HackerOne 是一个众包安全平台，组织使用它来运行漏洞赏金项目，允许安全研究人员报告漏洞以获取奖励。帮助台系统通常包含客户支持工单、员工信息和内部通信，使其成为威胁行为者的有价值目标，即使这些系统不包含核心网络访问权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HackerOne">HackerOne - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: The news item carries a '茶馆讨论' (tea house discussion) tag indicating community engagement, however no specific discussion content was visible at the time of reporting.

**标签**: `#data-breach`, `#adobe`, `#cybersecurity`, `#threat-actor`, `#corporate-security`

---

<a id="item-22"></a>
## [工信部通报苹果设备高危漏洞风险：涉及 iOS 17.2.1 及以下版本](https://www.nvdb.org.cn/publicAnnouncement/2040008892420247553) ⭐️ 7.0/10

工业和信息化部网络安全威胁和漏洞信息共享平台（NVDB）近日监测发现，有攻击者利用苹果公司终端产品漏洞实施网络攻击，可导致信息窃取和系统受控。受影响范围涵盖运行 iOS 13.0 至 17.2.1 的 iPhone 和 iPad 等产品。 此通报影响中国数以百万计尚未升级到 iOS 17.3 或更高版本的 iPhone 和 iPad 用户。攻击者可通过社会工程学手段获得最高权限，导致设备完全被控，包括数据窃取和未经授权的系统控制。 攻击者通过短信、邮件或网页投毒诱导用户访问恶意网页，进而向终端植入远程控制木马并获取最高权限。NVDB 建议相关用户做好风险排查，尽快通过系统升级或安装补丁等方式修复漏洞，并强化安全意识，避免点击来源不明的链接。

telegram · zaihuapd · Apr 3, 11:23

**背景**: NVDB（网络安全威胁和漏洞信息共享平台）是工业和信息化部管理的网络安全威胁和漏洞信息共享平台。iOS 17.2.1 于 2023 年 12 月发布，后续版本已修复相关漏洞。

**标签**: `#cybersecurity`, `#apple`, `#ios`, `#vulnerability`, `#government-advisory`

---

<a id="item-23"></a>
## [调查指 LinkedIn 扫描用户浏览器扩展并向第三方共享数据](https://cybernews.com/privacy/linkedin-surveillance-browsergate/?utm_source=flipboard&amp;utm_content=CyberNews_com%2Fmagazine%2FLatest+cybersecurity+news) ⭐️ 7.0/10

一项调查指称，LinkedIn 在网站中部署代码扫描用户已安装的浏览器扩展程序，收集超过 6000 个扩展程序和 200 多款竞品工具的数据，然后加密并传回服务器，可能影响约 4.05 亿用户。 这一隐私违规行为非常重要，因为它涉及敏感用户数据，包括宗教信仰、政治倾向、健康状况和求职状态，且在未获得用户同意的情况下与第三方共享，可能违反 GDPR 要求。 扫描的数据会与包括 HUMAN Security 在内的第三方公司共享，在欧盟 GDPR 框架下，此类数据处理通常需要获得用户的明确同意，而 LinkedIn 未取得此类同意也未披露相关做法。

telegram · zaihuapd · Apr 3, 12:09

**背景**: 浏览器指纹识别是一种从用户浏览器和设备收集详细信息以创建唯一标识符的技术。LinkedIn 据称扫描扩展程序以检测用户敏感信息，如宗教信仰、政治派别、健康状况和就业状态，可能在未获得同意的情况下建立详细用户画像。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybernews.com/privacy/linkedin-surveillance-browsergate/">LinkedIn secretly injects code to spy on your browser | Cybernews</a></li>
<li><a href="https://www.gadgetreview.com/linkedin-allegedly-scans-your-browser-and-sends-the-data-to-third-parties">LinkedIn Allegedly Scans Your Browser - and Sends... - Gadget Review</a></li>
<li><a href="https://fingerprint.com/blog/browser-fingerprinting-techniques/">Browser Fingerprinting Techniques : 6 Top Methods Explained</a></li>

</ul>
</details>

**标签**: `#privacy`, `#LinkedIn`, `#data-collection`, `#GDPR`, `#cybersecurity`

---

<a id="item-24"></a>
## [逆向工程 Claude Code 签名可脱离 Bun 运行时](https://a10k.co/b/reverse-engineering-claude-code-cch.html) ⭐️ 7.0/10

该研究在一个中文技术社区（花频道茶馆）中讨论，表明逆向工程社区对此感兴趣。能够在 Python 中复制该签名表明这不是一个强安全边界，而是一个功能门控和归因系统。 `cch` 头部使用 xxHash64 对完整 JSON 请求体进行哈希（当存在占位符 `cch=00000` 时），而 `cc_version` 的最后三位则由首条用户消息中的指定字符与内置盐值和版本号通过 SHA-256 计算得出。

telegram · zaihuapd · Apr 3, 15:00

**背景**: Claude Code 是 Anthropic 的 AI 辅助编码 CLI 工具，它向 Anthropic API 发送带有专有头部的请求。`cch` 头部作为请求完整性检查——签名错误的请求会被拒绝。Bun 运行时之前是计算这些签名的必要条件，因为它们不是在 JavaScript 中计算的，而是在 Claude Code 私有 Bun 运行时的原生 fetch 实现中完成的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/fast-mode">Speed up responses with fast mode - Claude Code Docs</a></li>
<li><a href="https://github.com/Cyan4973/xxHash">xxHash - Extremely fast hash algorithm - GitHub xxHash: xxHash XXHash Algorithm Implementation | ceph/xxHash | DeepWiki xxHash - Extremely fast hash algorithm - Google Open Source xxhash64 - Azure Databricks | Microsoft Learn xxHash: xxHash XxHash64 Class (System.IO.Hashing) | Microsoft Learn xxhash64 - Azure Databricks | Microsoft Learn XXHash Algorithm Implementation | ceph/xxHash | DeepWiki xxHash in C# | SSOJet</a></li>
<li><a href="https://xxhash.com/doc/v0.8.2/index.html">xxHash: xxHash</a></li>

</ul>
</details>

**社区讨论**: The research was discussed in a Chinese-language tech community (花频道茶馆), suggesting interest in the reverse engineering community. The ability to replicate the signature in Python demonstrates that the mechanism is not a strong security boundary but rather a functional gating and attribution system.

**标签**: `#reverse-engineering`, `#claude-code`, `#anthropic`, `#bun-runtime`, `#api-security`, `#xxhash`

---