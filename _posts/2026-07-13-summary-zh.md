---
layout: default
title: "Horizon Summary: 2026-07-13 (ZH)"
date: 2026-07-13
lang: zh
---

> From 117 items, 13 important content pieces were selected

---

1. [xAI Grok CLI 被曝默认上传整个代码库](#item-1) ⭐️ 9.0/10
2. [Math.tanh()指纹识别通过浏览器揭示操作系统](#item-2) ⭐️ 8.0/10
3. [Claude Code sends 33k tokens before reading the prompt; OpenCode sends 7k](#item-3) ⭐️ 8.0/10
4. [全球首款侵入式脑机接口医疗器械获批上市](#item-4) ⭐️ 8.0/10
5. [将生产级 AI 智能体迁移至 GPT-5.6：性能提升 2.2 倍，成本降低 27%](#item-5) ⭐️ 7.0/10
6. [菲尔兹奖得主陶哲轩使用 LLM 编码代理构建应用](#item-6) ⭐️ 7.0/10
7. [研究人员将因果理论应用于大型语言模型的机制可解释性研究](#item-7) ⭐️ 7.0/10
8. [无理解之自动化](#item-8) ⭐️ 7.0/10
9. [乔治·霍茨：我热爱 LLM，厌恶炒作](#item-9) ⭐️ 7.0/10
10. [反对有用性：反思科技行业对实用性的过度追求](#item-10) ⭐️ 7.0/10
11. [NeuroVFM：使用 Vol-JEPA 的新型神经影像基础模型](#item-11) ⭐️ 7.0/10
12. [Simon Willison：AI 代理不应成为直接责任人](#item-12) ⭐️ 7.0/10
13. [Grok Build CLI 紧急更新阻止未授权代码上传](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [xAI Grok CLI 被曝默认上传整个代码库](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547) ⭐️ 9.0/10

这是一个重大的安全和隐私违规行为，暴露了开发者的知识产权和凭证。该工具绕过用户指令和设置，且无法禁用此行为，从根本上破坏了人们对 AI 开发工具的信任。 该工具使用两个上传渠道：1）文件内容被嵌入模型对话请求并上传到 Google Cloud Storage 存储桶；2）整个代码库以 git bundle 形式上传。在 12 GB 仓库测试中，超过 5 GiB 数据成功上传且无存储端拒绝。"改进模型"开关无法阻止上传。

telegram · zaihuapd · Jul 12, 04:19

**背景**: Grok Build 是 xAI 官方的编程命令行工具，用于帮助开发者完成编码任务。git bundle 是 Git 的一个功能，可以将整个仓库打包成单个二进制文件以便传输。.env 文件通常存储 API 密钥、数据库凭证和其他不应共享的敏感配置数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build Beta | SpaceXAI</a></li>
<li><a href="https://git-scm.com/docs/git-bundle">Git - git - bundle Documentation</a></li>

</ul>
</details>

**标签**: `#security`, `#privacy`, `#xAI`, `#AI-tools`, `#data-exfiltration`, `#vulnerability`

---

<a id="item-2"></a>
## [Math.tanh()指纹识别通过浏览器揭示操作系统](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 8.0/10

研究人员发现，Chromium 148+中的 Math.tanh()函数可以通过暴露不同操作系统（Linux 上的 glibc、macOS 上的系统库等）的数学库实现差异来识别底层操作系统。 这代表了一种新颖的浏览器指纹识别向量，即使用户更改用户代理或使用 Tor 等注重隐私的浏览器，追踪者也可以跨会话识别用户，这给网络用户带来了重大隐私担忧。 这种指纹识别之所以有效，是因为不同的操作系统使用不同的数学库——Linux 通常使用 glibc，而 macOS 使用自己的系统库。这些差异体现在 NaN 规范化、SIMD 舍入上，特别是 Math.tanh、CSS 三角函数和 WebAudio 实现上。特征信号主要集中在 ARM 与 x86 架构的差异上。

hackernews · joahnn_s · Jul 12, 21:12

**背景**: 浏览器指纹识别是一种追踪技术，用于收集各种浏览器和设备特征来为用户创建唯一标识，即使没有 cookie 也能追踪。不同操作系统中的数学库在浮点运算方面存在细微的实现差异，可以通过 JavaScript 函数（如 Math.tanh()）检测到。这一漏洞在 Chromium 148 中被引入或变得可被利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://scrapfly.dev/posts/browser-math-os-fingerprint/">Your Browser Does Math Differently on Every OS, and Anti-Bot Systems Read the Bits · scrapfly.dev</a></li>
<li><a href="https://news.ycombinator.com/item?id=48884853">Since Chromium 148, Math.tanh is now fingerprintable to link underlying OS | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 讨论显示出复杂的情绪：一些评论者批评 Scrapfly 的动机，认为他们从指纹识别中获利却推动修复。其他人指出，这项技术也可能用于指纹识别浏览器版本范围。一个建设性的建议是实施正确舍入的超越函数作为修复方案。评论者还指出，即使 Tor 浏览器也放弃了掩盖操作系统的努力，因为指纹识别向量太多了。

**标签**: `#browser-fingerprinting`, `#security`, `#privacy`, `#chromium`, `#web-tracking`

---

<a id="item-3"></a>
## [Claude Code sends 33k tokens before reading the prompt; OpenCode sends 7k](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

A benchmark comparing Claude Code and OpenCode reveals Claude Code sends ~33k tokens before reading the prompt versus OpenCode's ~7k, raising questions about efficiency and cost implications for developers.

hackernews · systima · Jul 12, 18:25

**标签**: `#AI coding tools`, `#Claude Code`, `#OpenCode`, `#token optimization`, `#developer productivity`

---

<a id="item-4"></a>
## [全球首款侵入式脑机接口医疗器械获批上市](https://t.me/zaihuapd/42515) ⭐️ 8.0/10

此次批准标志着脑机接口技术首次以医疗器械身份进入临床应用阶段，实现了该类医疗器械的全球首发上市，为颈段脊髓损伤患者带来了新的希望。 该系统适用于 18 至 60 岁的颈段脊髓损伤患者（C2-C6 节段，损伤评级 A-C 级），确诊超过 1 年且病情稳定至少 6 个月。系统通过硬脑膜外电极采集信号，配合气动手套辅助实现手部抓握功能代偿。

telegram · zaihuapd · Jul 12, 14:39

**背景**: 脑机接口（BCI）是在大脑与外部设备之间建立直接通信通道的技术。侵入式脑机接口需要通过手术将电极植入脑组织或硬脑膜上。硬脑膜外植入是一种折中方案，信号质量优于非侵入式方法，同时避免直接损伤脑组织。颈段脊髓损伤常导致四肢瘫，即使保留部分手臂功能也会丧失手部抓握能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tsinghua.edu.cn/info/2063/125128.htm">全球首款侵入式脑机接口医疗器械上市！-清华大学</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/2016611717912744266">何以博睿康？全球首个半侵入式脑机接口医疗器械获批上市的背后</a></li>
<li><a href="https://baike.baidu.com/item/气动手套设备/67672656">气动手套设备 - 百度百科</a></li>

</ul>
</details>

**标签**: `#brain-computer-interface`, `#medical-devices`, `#neurotechnology`, `#healthcare-innovation`, `#China-regulatory`

---

<a id="item-5"></a>
## [将生产级 AI 智能体迁移至 GPT-5.6：性能提升 2.2 倍，成本降低 27%](https://ploy.ai/blog/migrating-a-production-ai-agent-to-gpt-5-6) ⭐️ 7.0/10

这一案例研究提供了具体的生产级证据，表明 GPT-5.6 为 AI 智能体工作负载带来了显著的性能和成本提升，可能加速企业采用新模型层级，并为类似部署验证升级路径。 Ploy 的智能体处理复杂的网站构建任务，包括规划、代码读取、组件编写、图像生成和自我评估。对于许多公司来说，这种迁移基本上是一行代码的改动。有评论者指出，对于各种小型简单工作流，无论是否有路由架构，模型升级本质上都是单行代码的变更。

hackernews · brryant · Jul 12, 17:13

**背景**: GPT-5.6 是 OpenAI 的最新模型版本，分为三个层级：Sol（旗舰款'主力模型'，适用于复杂推理和编码）、Terra（中级），以及第三个层级。Sol 被描述为 OpenAI'迄今为止最好的编码模型'，适用于智能体工作流。该模型于 4 天前预览发布，代表了 GPT-5 系列的重大更新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT-5.6 Sol: a next-generation model | OpenAI</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论显示情绪复杂。虽然多项改进得到了多位从业者的验证（thiagoperes 确认了分类任务类似的收益），但有人批评文章的 LLM 生成风格。有人对生产级智能体的一致性表示担忧，并质疑提示工程或工具调用工作流是否需要重大改变。一位评论者指出，Opus 模型曾连续四个月保持默认地位而未被超越。

**标签**: `#ai-agents`, `#gpt-5`, `#performance-optimization`, `#production-systems`, `#model-migration`

---

<a id="item-6"></a>
## [菲尔兹奖得主陶哲轩使用 LLM 编码代理构建应用](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 7.0/10

这篇文章之所以重要，是因为它提供了一位世界上最受尊敬的数学家对 AI 辅助开发的切实可行且专家级的视角，对 LLM 编码代理在软件开发中的能力和局限性给出了现实的期望。 陶哲轩强调，LLM 生成的可视化工具是有用的补充，但对于关键任务不应盲目信任。他指出这些工具在快速原型设计和构建补充教育工具方面表现出色，但对于构成核心研究或教育内容的工作需要仔细验证。

hackernews · subset · Jul 12, 11:09

**背景**: LLM 编码代理是一类可以根据自然语言指令自主编写、编辑和调试代码的 AI 工具。Cursor、OpenCode 和 Pi 等工具代表了 AI 辅助开发环境的新类别。陶哲轩是菲尔兹奖（数学界最高荣誉）得主，以其在数论、调和分析和偏微分方程方面的研究而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cursor.com/">Cursor: AI coding agent</a></li>
<li><a href="https://opencode.ai/">OpenCode | The open source AI coding agent</a></li>
<li><a href="https://pi.dev/">A terminal-based coding agent</a></li>

</ul>
</details>

**社区讨论**: 讨论显示社区对 LLM 在非关键教育工具方面的价值达成了强烈共识，用户们分享了在课堂上的类似经历。评论从关于专家面临普通技术问题（如 Docker 调试）的幽默观察，到关于非传统领域软件潜在巨大需求的严肃讨论，不一而足。许多人欣赏陶哲轩的平衡观点——将 LLM 视为某些任务的有用工具，但不应盲目信任。

**标签**: `#llm`, `#coding-agents`, `#software-development`, `#ai-tools`, `#terry-tao`

---

<a id="item-7"></a>
## [研究人员将因果理论应用于大型语言模型的机制可解释性研究](https://cacm.acm.org/news/can-we-understand-how-large-language-models-reason/) ⭐️ 7.0/10

研究人员正在使用机制可解释性和因果理论，通过操纵权重和激活的实验来研究神经网络中编码的知识是否对应于类似推理的概念。 这项研究对人工智能安全和可解释性具有重要意义，因为理解大型语言模型如何内化和处理知识可以帮助确保其可靠性并检测潜在的偏见或不安全行为。 一个值得注意的例子是研究人员观察模型进行时钟时间计算的方法，展示了如何通过仔细的实验在神经网络权重中识别特定的算法模式。

hackernews · adunk · Jul 12, 18:04

**背景**: 机制可解释性是可解释人工智能的一个子领域，旨在通过分析神经网络的具体结构、算法和电路来理解其内部运作。该领域由于神经网络的固有复杂性（通常被称为“参数意面代码”）而面临重大挑战。一些研究人员认为，机制可解释性可能永远无法将大型语言模型简化为简单的方程，但它可以使隐藏的算法逐渐变得至少部分可理解。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Causal_AI">Causal AI - Wikipedia</a></li>
<li><a href="https://blog.bluedot.org/p/introduction-to-mechanistic-interpretability">Introduction to Mechanistic Interpretability - by Sarah</a></li>

</ul>
</details>

**社区讨论**: 社区成员澄清说，这篇文章主要关注机制可解释性研究，而不是抽象的哲学推理，一位评论者提到了关于相关论文的 2MP 视频。一些人对神经网络是否能够被真正理解表示怀疑，另有评论者引用了 Icard 的观点，即这项研究可能“逐渐将深度神经网络转变为其隐藏算法至少可以部分理解的系统”。

**标签**: `#mechanistic-interpretability`, `#large-language-models`, `#causality`, `#neural-network-analysis`, `#ai-safety`

---

<a id="item-8"></a>
## [无理解之自动化](https://arxiv.org/abs/2607.06377) ⭐️ 7.0/10

这很重要，因为它揭示了一个根本性问题：人工智能系统可能自信地做出错误决策，而只有人类专家才能发现；此外，自动化可能通过减少人们发展深度领域知识的机会而随着时间推移削弱人类专业知识。 论文探讨了人工智能系统如何可能产出听起来合理但错误的输出同时显得自信，以及对人工智能日益增长的依赖可能阻碍新一代人发展验证和发现人工智能错误所需的专业知识。

hackernews · root-parent · Jul 12, 16:54

**背景**: 可解释人工智能（XAI）是一个专注于使人工智能决策过程对人类透明和可理解的研究领域。机器学习中的知识保留传统上指的是模型在学习新任务时保持先前学习任务表现的能力。社区讨论反映了更广泛的担忧，即人工智能自动化可能会削弱人类专业知识，类似于人们认为对计算器的依赖会影响数学能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Explainable_artificial_intelligence">Explainable artificial intelligence - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/explainable-ai">What is Explainable AI (XAI)? | IBM</a></li>

</ul>
</details>

**社区讨论**: 评论者表示担忧，人工智能可能不会直接取代专家，但可能通过消除来自基础工作的学习机会而阻止未来专家的发展。一位评论者提议，人工智能系统应该被要求通过形式化证明和执行追踪来展示其工作过程。其他人提出了哲学层面的担忧，即我们是否正在接近一个奇点，在那个点上人类知识降到理解人工智能系统所需的阈值以下。

**标签**: `#ai-safety`, `#automation`, `#machine-learning`, `#knowledge`, `#explainability`

---

<a id="item-9"></a>
## [乔治·霍茨：我热爱 LLM，厌恶炒作](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html) ⭐️ 7.0/10

这一分析挑战了前沿 AI 实验室的万亿美元估值，论证它们无法捕获 AI 创造的价值。它强调了向私有 AI 部署和开源定制的日益增长的转变，从根本上改变了开发者的软件开发方式。 前沿实验室目前对有限 tokens 访问收取每月 100-200 美元的订阅费，但霍茨认为开源模型使用户能够私下运行 AI。评论者注意到 LLM 生成软件的「参差不齐」质量，并讨论 fork 开源项目的便利性如何可能破坏传统的上游激励。

hackernews · therepanic · Jul 12, 18:31

**背景**: 乔治·霍茨是一位著名的黑客，以破解 iPhone 和 PlayStation 闻名，后来创立了 comma.ai 开发自动驾驶技术。前沿实验室指 OpenAI、Anthropic 和 Google 等领先 AI 模型开发的公司。「随心所欲」时代描述了一种转变，开发者可以轻松 fork 和定制开源 AI 模型，而非依赖专有 API。

**社区讨论**: 评论者大多同意霍茨关于前沿实验室无法捕获 AI 价值的论点。有人讨论了在私人 homelab 中运行 AI，另一位描述了为特定用例构建精简的定制软件。担忧浮现于当 fork 变得如此容易以至于上游失去其价值时，开源的未来将何去何从。有些人注意到 LLM 生成软件的「参差不齐」质量反映了技术的局限性。

**标签**: `#LLMs`, `#AI-hype`, `#open-source`, `#software-development`, `#AI-economics`

---

<a id="item-10"></a>
## [反对有用性：反思科技行业对实用性的过度追求](https://www.motivenotes.ai/p/against-usefulness) ⭐️ 7.0/10

一篇名为《反对有用性》的哲学文章批评了科技行业对实用性的执着，引用了 Bret Victor 的 Dynamicland 研究项目，并质疑现代技术开发中独立思考的缺失。 这一批评揭示了科技研究领域日益严重的同质化问题，大多数项目由相同的资金来源支持，追求相似的目标，可能会扼杀不会立即转化为商业价值的探索性和前瞻性工作。 文章特别提到了 Dynamicland，这是 Bret Victor 位于奥克兰的研究实验室，以将整栋建筑变成协作式计算机而闻名，并批评了当代技术开发中缺乏"独立思考者"的现象。

hackernews · supo · Jul 12, 17:47

**背景**: Dynamicland 是由 Bret Victor 创立的一个独特研究项目。Bret Victor 是一位著名的界面设计师，曾在苹果公司工作，并为 iPad 设计了早期概念。与传统计算不同，Dynamicland 将整个物理空间转变为计算环境，人们可以通过物理对象和空间交互进行协作。该项目强调探索性研究，而非直接的商业应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dynamicland.org/2019/Bootstrapping_Research/">Bootstrapping Research & Dynamicland</a></li>
<li><a href="https://en.wikipedia.org/wiki/Bret_Victor">Bret Victor - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者深入参与了文章主题的讨论。有人讨论了将这些想法应用于任务规划，注意到更丰富的视觉画布在理解战术信息方面的价值。另一位批评了文章本身对"无用性"论点的使用，指出它仍然以潜在有用性来评价项目。第三位强调了触控笔作为一种未被充分探索的输入方式，可以实现更具表现力的计算，让用户摆脱受限制的思维模式。

**标签**: `#technology-philosophy`, `#innovation`, `#research-culture`, `#Bret-Victor`, `#independent-thinking`

---

<a id="item-11"></a>
## [NeuroVFM：使用 Vol-JEPA 的新型神经影像基础模型](https://www.marktechpost.com/2026/07/12/meet-neurovfm-a-new-neuroimaging-foundation-model-trained-with-vol-jepa-on-uncurated-clinical-mri-and-ct-volumes/) ⭐️ 7.0/10

密歇根大学研究人员开发了 NeuroVFM，这是一种神经影像基础模型，使用 Vol-JEPA（一种自监督方法）在 524 万份临床 MRI 和 CT 扫描数据上训练而成，该方法将 I-JEPA 和 V-JEPA 扩展到 3D 体积医学影像，且无需放射学报告标签。 这代表了医学人工智能的重大进步，证明了自监督学习可以在大规模未整理的临床数据上有效运行，无需人工标注。直接从原始 MRI/CT 扫描中学习大脑解剖结构和病理的能力，可以为缺乏标注数据集的医疗机构 democratize 基础模型的开发。

rss · MarkTechPost · Jul 13, 00:35

**背景**: JEPA（联合嵌入预测架构）是一种由 Meta AI 和 Yann LeCun 开发的自监督学习方法。与重建像素的生成方法不同，JEPA 在潜在空间中进行预测。I-JEPA 将这种方法应用于图像，V-JEPA 应用于视频，现在 Vol-JEPA 将其扩展到 3D 体积医学影像。自监督学习消除了对昂贵人工标注的需求，这在医学影像领域尤其有价值，因为专业标注既稀缺又耗时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2511.18640">Health system learning achieves generalist neuroimaging models</a></li>
<li><a href="https://www.linkedin.com/posts/yann-lecun_neurovfm-a-foundation-model-for-neuroimaging-activity-7481833908603416576-qlbS">NeuroVFM: A foundation model for neuroimaging from the University of...</a></li>
<li><a href="https://github.com/facebookresearch/jepa">GitHub - facebookresearch/jepa: PyTorch code and models for V ... [2506.09985] V-JEPA 2: Self-Supervised Video Models Enable ... Introducing the V-JEPA 2 world model and new benchmarks for ... What Is JEPA? Joint Embedding Predictive Architecture Deep Dive into Yann LeCun’s JEPA | Rohit Bandaru GitHub - facebookresearch/vjepa2: PyTorch code and models for ...</a></li>

</ul>
</details>

**标签**: `#medical-ai`, `#neuroimaging`, `#foundation-models`, `#self-supervised-learning`, `#volumetric-imaging`, `#machine-learning`

---

<a id="item-12"></a>
## [Simon Willison：AI 代理不应成为直接责任人](https://simonwillison.net/2026/Jul/12/directly-responsible-individuals/#atom-everything) ⭐️ 7.0/10

Simon Willison 探讨了苹果和 GitLab 的直接责任人（DRI）概念，认为 LLM 驱动的 AI 代理永远不应被指定为 DRI，因为只有人类才能真正对结果负责。 这很重要，因为随着 AI 代理在组织中变得更加自主，清晰的责任框架变得至关重要。如果 AI 代理无法被追究责任，人类必须保留对 AI 辅助工作的最终责任——这引发了关于 AI 治理和负责任部署的关键问题。 DRI 概念起源于苹果公司，在 GitLab 手册中被定义为对特定项目成败最终负责的人。Willison 引用了 IBM 1979 年的培训幻灯片，上面写着"电脑永远不能被追究责任，因此电脑永远不能做出管理决策"。

rss · Simon Willison · Jul 12, 23:57

**背景**: 直接责任人（DRI）是一种管理概念，指定一个人对项目的成功或失败承担最终责任。苹果公司创造了这个术语，GitLab 将其编入公开手册。该概念解决了常见的组织责任分散问题，即没有人真正感到 ownership。随着 AI 代理变得越来越有能力自主决策，关于它们是否能像人类一样被追究责任的问题出现了。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://handbook.gitlab.com/handbook/people-group/directly-responsible-individuals/">Directly Responsible Individuals ( DRI ) | The GitLab Handbook</a></li>
<li><a href="https://simonwillison.net/2026/Jul/12/directly-responsible-individuals/">Directly Responsible Individuals ( DRI ) | Simon Willison’s Weblog</a></li>

</ul>
</details>

**标签**: `#AI accountability`, `#organizational management`, `#AI governance`, `#responsible AI`, `#technology ethics`

---

<a id="item-13"></a>
## [Grok Build CLI 紧急更新阻止未授权代码上传](https://www.reddit.com/r/LocalLLaMA/comments/1ut7tis/comment/ox4zamk/?utm_source=share&amp;utm_medium=web3x&amp;utm_name=web3xcss&amp;utm_term=1&amp;utm_content=share_button) ⭐️ 7.0/10

7 月 13 日，xAI 发布紧急更新，在 Grok Build CLI 中禁用代码上传功能，此前安全研究员发现该工具默认将整个代码库（包括密钥文件）上传到 xAI 服务器。 该漏洞允许 Grok Build CLI 将每个跟踪的文件、完整的 git 历史甚至代理从未读取的文件上传到 Google Cloud Storage 存储桶（grok-code-session-traces），无论用户是否禁用"改进模型"设置。

telegram · zaihuapd · Jul 13, 00:52

**背景**: Grok Build 是 xAI 的命令行编程代理，由 Grok 4.5 驱动，旨在协助完成复杂的编码任务。安全研究人员可以进行网络层面分析，监控 AI 工具向远程服务器传输哪些数据。这一事件凸显了对 AI 编程助手进行审计以防止意外数据外传的重要性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://byteiota.com/grok-build-cli-uploads-repo-xai-servers/">Grok Build CLI Uploads Your Entire Repo to xAI Servers</a></li>
<li><a href="https://github.com/cereblab/grok-build-exfil-repro">GitHub - cereblab/grok-build-exfil-repro: Reproduce it ...</a></li>
<li><a href="https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547">What xAI Grok Build CLI actually sends to xAI - a wire-level analysis...</a></li>

</ul>
</details>

**社区讨论**: 安全研究员发布了网络层面证据，证明该 CLI 正在上传存储库，且与代理实际读取的内容无关。许多开发者表示担忧，因为"改进模型"开关实际上并未阻止数据传输。

**标签**: `#security`, `#privacy`, `#xAI`, `#Grok`, `#vulnerability`, `#AI tools`, `#code leakage`

---