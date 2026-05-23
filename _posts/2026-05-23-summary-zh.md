---
layout: default
title: "Horizon Summary: 2026-05-23 (ZH)"
date: 2026-05-23
lang: zh
---

> From 162 items, 26 important content pieces were selected

---

1. [Vite 8.0 发布：基于 Rust 的统一打包工具，构建速度最高提升 30 倍](#item-1) ⭐️ 9.0/10
2. [Anthropic 玻璃 wing 项目初步成果公布](#item-2) ⭐️ 8.0/10
3. [Superset：YC 支持的并行编程 Agent 开源 IDE](#item-3) ⭐️ 8.0/10
4. [英伟达 Nemotron 扩散语言模型实现光速文本生成](#item-4) ⭐️ 8.0/10
5. [NVIDIA 展示如何大规模生成合成 3D 医学图像](#item-5) ⭐️ 8.0/10
6. [SpaceX 递交上市申请，或将创造美国史上最大 IPO](#item-6) ⭐️ 8.0/10
7. [TanStack 披露涉及 42 个包的复杂 npm 供应链攻击](#item-7) ⭐️ 8.0/10
8. [八部门发文整治非法跨境证券期货基金经营](#item-8) ⭐️ 8.0/10
9. [Cloudflare 全球网络故障：28% HTTP 流量受影响，持续 25 分钟](#item-9) ⭐️ 8.0/10
10. [PydanticAI v1.101.0 新增消息队列和 MCP 后台任务支持](#item-10) ⭐️ 7.0/10
11. [SpaceX 发射 Starship 原型火箭 经历多台发动机故障](#item-11) ⭐️ 7.0/10
12. [Antigravity 2.0 在 OpenSCAD 建筑 3D 大语言模型基准测试中夺冠](#item-12) ⭐️ 7.0/10
13. [yt-dlp 因无法审核 AI 代码库而移除 Bun 支持](#item-13) ⭐️ 7.0/10
14. [DeepSeek 将 V4 Pro API 定价永久降至原价的 25%](#item-14) ⭐️ 7.0/10
15. [企业 AI 采购：专业化优于规模化的战略考量](#item-15) ⭐️ 7.0/10
16. [AI 利用频谱图复活已故飞行员声音](#item-16) ⭐️ 7.0/10
17. [AI 生成小说入围英联邦短篇小说奖引争议](#item-17) ⭐️ 7.0/10
18. [海湾国家因 AI 基础设施发展被敦促多元化海底电缆](#item-18) ⭐️ 7.0/10
19. [FTC 对 CMG 处以 93 万美元罚款：涉欺骗性"主动监听"AI 营销服务](#item-19) ⭐️ 7.0/10
20. [深入解析 ThunderKittens：面向高性能 AI 内核的紧凑型领域特定语言](#item-20) ⭐️ 7.0/10
21. [企业 Token 成本焦虑推动 AI 基础设施新市场崛起](#item-21) ⭐️ 7.0/10
22. [Anthropic 推出 MCP 隧道供私有代理访问](#item-22) ⭐️ 7.0/10
23. [Cloudflare 推出 Dynamic Workflows 实现持久化执行动态扩展](#item-23) ⭐️ 7.0/10
24. [礼来 retatrutide 三期试验最高剂量平均减重 28.3%](#item-24) ⭐️ 7.0/10
25. [Take-Two 确认 GTA6 发售日期不变，宣发 6 月下旬启动](#item-25) ⭐️ 7.0/10
26. [字节跳动开源 30 亿参数统一多模态模型 Lance](#item-26) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Vite 8.0 发布：基于 Rust 的统一打包工具，构建速度最高提升 30 倍](https://www.infoq.cn/article/9gN7a2Dw8MOKN3WXqvxC?utm_source=rss&utm_medium=article) ⭐️ 9.0/10

此次发布标志着前端工具的重大范式转变，因为 Vite——最受欢迎的 JavaScript 构建工具之一——现在完全基于 Rust 运行。开发者可以在不更改项目配置的情况下获得显著更快的冷启动、HMR 更新和生产构建体验，使 Vite 8 成为类似 Turbopack 这种受限于特定生态系统的工具的框架无关替代方案。 Vite 8.0 使用 Rolldown（Rollup 的 Rust 重写版，API 兼容）以及 Oxc（另一个 Rust 项目）进行 TypeScript 和 JavaScript 解析。该版本还随附 @vitejs/plugin-react v6，用 Oxc 替代 Babel 进行 React Refresh 转换，从而使安装体积更小。对于大型项目，建议采用渐进式迁移路径：先在 Vite 7 上切换到 rolldown-vite 以隔离问题，然后升级到 Vite 8。

rss · InfoQ 中文站 · May 22, 13:31

**背景**: Vite 是一个广泛使用的前端构建工具，以其基于原生 ES 模块和 Rollup 的快速冷启动和 HMR 著称。Rolldown 是 Rollup 的 Rust 原生重写版，保持与 Rollup 兼容的 API。Oxc（JavaScript 氧化编译器）是一个用 Rust 编写的高性能 JavaScript 和 TypeScript 工具集合，提供解析、linting 和转换功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vite.dev/blog/announcing-vite8">Vite 8.0 is out! | Vite</a></li>
<li><a href="https://www.infoq.com/news/2026/05/vite-v8-rust/">Vite Version 8: Unified Rust-Based Bundler and Up to 30x Faster Builds - InfoQ</a></li>
<li><a href="https://www.reddit.com/r/rust/comments/1rs2d4j/vite_80_is_out_and_its_full_of_rust/">r/rust on Reddit: Vite 8.0 is out. And it's full of 🦀 Rust</a></li>

</ul>
</details>

**社区讨论**: Reddit 的 r/rust 社区将此视为 Rust 在网络工具领域的巨大进步，指出网络上最突出的构建工具现在已全面采用 Rust。开发者的反应认为 Vite 8 相比之前的版本有显著改进。

**标签**: `#Vite`, `#Rust`, `#build tools`, `#frontend development`, `#JavaScript bundling`

---

<a id="item-2"></a>
## [Anthropic 玻璃 wing 项目初步成果公布](https://www.anthropic.com/research/glasswing-initial-update) ⭐️ 8.0/10

Anthropic 发布了 Project Glasswing 的初步进展，透露其 Claude Mythos 预览模型已在全球关键软件系统中发现超过 10000 个高危或严重漏洞，其中经六家独立安全公司验证的 1752 个漏洞中，90.6%(1587 个)确认为真实漏洞。 这一进展对网络安全领域意义重大，因为它代表了 AI 驱动漏洞检测的突破，同时该项目联合了苹果、谷歌等约 50 家合作伙伴，形成了前所未有的行业协作安全联盟，但也引发了关于 AI 技术双重性的担忧。 验证结果显示，在确认的 1587 个真实漏洞中，62.4%(1094 个)被评定为高危或严重级别。该模型的 90.6%准确率获得了独立安全研究公司的背书，但 curl 维护者 Daniel Stenberg 质疑其是否显著优于现有工具。

hackernews · louiereederson · May 22, 19:31

**背景**: Project Glasswing 是 Anthropic 于今年 4 月启动的协作安全项目，利用 Claude Mythos 预览模型进行主动漏洞检测。该模型因在安全任务中表现出色而被 Anthropic 决定不公开发布，以防止被恶意利用。与传统静态分析工具相比，AI 模型具有更强的代码理解和模式识别能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/glasswing-initial-update">Project Glasswing: An initial update \ Anthropic</a></li>
<li><a href="https://www.wired.com/story/anthropic-mythos-preview-project-glasswing/">Anthropic Teams Up With Its Rivals to Keep AI From Hacking ...</a></li>
<li><a href="https://thehackernews.com/2026/04/anthropics-claude-mythos-finds.html">Anthropic's Claude Mythos Finds Thousands of Zero-Day Flaws ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应呈现两极化。用户 mdeeks 实测 Codex Security 后给予高度评价，称准确率约 90%，已成为团队必备工具。但 mukmuk 引用 curl 维护者 Daniel Stenberg 的观点提出质疑，认为该模型并未显著优于现有工具。nikcub 则强调 90.6%的独立验证准确率数据具有说服力。

**标签**: `#AI security`, `#code analysis`, `#vulnerability detection`, `#Anthropic`, `#Mythos`

---

<a id="item-3"></a>
## [Superset：YC 支持的并行编程 Agent 开源 IDE](https://github.com/superset-sh/superset) ⭐️ 8.0/10

Superset 管理所有 Agent 状态，包括 worktree、端口、终端会话、环境设置、diff、任务和 PR。它集成了问题跟踪，使工作流能从 issue→agent→diff→PR→review 而不丢失上下文。核心功能被抽象为无头 Hono 服务器，可部署到任何工作空间。

hackernews · avipeltz · May 22, 14:53

**背景**: Git worktree 是 Git 2.5 引入的功能，允许单个仓库关联多个工作树，使每个 Agent 都能获得独立的代码副本。Claude Code 是 Anthropic 的终端编程 Agent 工具，能理解代码库并通过自然语言命令执行任务。这些概念是 Superset 运行的基础。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/product/claude-code">Claude Code | Anthropic's agentic coding system</a></li>
<li><a href="https://git-scm.com/docs/git-worktree">Git - git - worktree Documentation</a></li>
<li><a href="https://github.com/anthropics/claude-code">GitHub - anthropics/claude-code: Claude Code is an agentic coding tool that lives in your terminal, understands your codebase, and helps you code faster by executing routine tasks, explaining complex code, and handling git workflows - all through natural language commands. · GitHub</a></li>

</ul>
</details>

**社区讨论**: 早期用户称赞 Superset 能够并行运行 40-50 个 Agent 会话而不失去跟踪，称其'完全围绕我的工作流程构建'。一些人表示对'沉重'工具感到不知所措，更喜欢 iTerm2/tmux 等轻量替代方案。其他人将其与 Harness 等项目进行比较，质疑与 emdash 和 conductor 等现有工具的区别。

**标签**: `#devtools`, `#ai-agents`, `#ide`, `#open-source`, `#yc-batch`

---

<a id="item-4"></a>
## [英伟达 Nemotron 扩散语言模型实现光速文本生成](https://huggingface.co/blog/nvidia/nemotron-labs-diffusion) ⭐️ 8.0/10

这一突破可以显著降低大型语言模型的推理延迟，使此前因计算限制而难以实现的实时应用成为可能，并可能改变生成式 AI 的大规模部署方式。 与自回归模型逐个令牌顺序生成不同，扩散模型可以并行预测多个令牌，从而消除了限制生成速度的顺序依赖瓶颈。

rss · Hugging Face Blog · May 23, 00:02

**背景**: 传统的大型语言模型使用自回归生成方式，每个新令牌都依赖于前面的所有令牌——类似于人类逐字写作的方式。这种顺序性质造成了根本性的速度瓶颈。扩散模型采用不同的方法，通过去噪过程并行生成整个序列，理论上可以提供数量级的速度提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/data-science-collective/autoregressive-vs-diffusion-large-language-models-llms-a-deep-dive-a41da6da0875">Autoregressive vs Diffusion Language Models : The... | Medium</a></li>
<li><a href="https://unstructured.io/blog/speeding-up-text-generation-with-non-autoregressive-language-models">Non-Autoregressive Text Generation Explained (NAR) | Unstructured</a></li>

</ul>
</details>

**标签**: `#diffusion-models`, `#nvidia`, `#llm-inference`, `#text-generation`, `#nemotron-labs`

---

<a id="item-5"></a>
## [NVIDIA 展示如何大规模生成合成 3D 医学图像](https://developer.nvidia.com/blog/synthesize-realistic-3d-medical-images-at-scale-to-ship-pre-trained-models/) ⭐️ 8.0/10

这一点很重要，因为真实世界的医学图像数据由于患者隐私法规（如 HIPAA）而极难获取，而合成数据生成使研究人员和开发人员能够在不访问敏感患者记录的情况下构建和训练 AI 模型，从而加速放射学 AI 的发展。 该博客利用了 NVIDIA 的 MONAI（医学开放式 AI 网络）框架，该框架提供用于医学成像深度学习任务的开源工具，包括图像分割、分类、注册和合成。该方法使用生成式 AI 方法来创建保留隐私的合成医学图像。

rss · NVIDIA Developer Blog · May 22, 16:00

**背景**: 医学成像 AI 需要大量训练数据，但真实患者的扫描受到隐私法保护，限制了数据共享。研究人员使用 GAN（生成对抗网络）和扩散模型等技术来生成合成医学图像，在保护患者身份的同时保持统计特性。NVIDIA MONAI 是一个基于 PyTorch 的框架，广泛用于医学成像研究，也可作为企业版 NVIDIA Clara 商业化部署。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.nvidia.com/clara/monai/index.html">MONAI Toolkit - NVIDIA Docs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Medical_open_network_for_AI">Medical open network for AI - Wikipedia</a></li>

</ul>
</details>

**标签**: `#medical imaging`, `#synthetic data`, `#AI/ML`, `#healthcare AI`, `#3D rendering`

---

<a id="item-6"></a>
## [SpaceX 递交上市申请，或将创造美国史上最大 IPO](https://techcrunch.com/video/spacex-files-to-go-public-and-the-math-requires-a-little-faith/) ⭐️ 8.0/10

SpaceX 已向美国证券交易委员会递交 S-1 注册文件，披露了雄心勃勃的数据，包括 28 万亿美元的总可寻址市场，以及与建立火星殖民地挂钩的高管薪酬，使其有望成为美国历史上最大的首次公开募股。 这次 IPO 代表了太空行业的一个分水岭时刻，因为 SpaceX 的潜在估值可能超越美国所有之前的公开募股。该文件标志着 SpaceX 从一家私营火箭公司转型为上市公司，而与火星殖民地挂钩的薪酬则表明了埃隆·马斯克超越地球业务的长期野心。 S-1 文件仅风险因素部分就长达 36 页，详细说明了公司对其市场机会的评估。28 万亿美元的可寻址市场涵盖了卫星互联网、火星殖民基础设施和行星际运输服务。高管薪酬方案包括与实现可持续火星殖民地相关的特定绩效里程碑。

rss · TechCrunch AI · May 22, 14:30

**背景**: S-1 文件是公司在进行 IPO 前向 SEC 提交的初始注册声明。它为潜在投资者提供有关公司财务、风险和商业模式的详细信息。SpaceX 由埃隆·马斯克于 2002 年创立，已从一家革命性的火箭初创公司发展成为商业太空发射服务的主导者，获得了 NASA 和美国国防部的合同。

**标签**: `#SpaceX`, `#IPO`, `#stock market`, `#space industry`, `# Elon Musk`

---

<a id="item-7"></a>
## [TanStack 披露涉及 42 个包的复杂 npm 供应链攻击](https://www.infoq.cn/article/ePxUGQ7cZvWNWkOhE1vT?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

这起攻击标志着 npm 供应链威胁的重大升级，直接瞄准了现代软件开发支柱的构建管道。由于数百万个项目依赖 npm 包，此类妥协可能在整个 JavaScript 生态系统中快速传播，影响无数应用程序和服务。 攻击者在约 19:20 和 19:26 UTC 发布恶意版本，将有效载荷注入已有信任的包而非创建新包。这种技术使检测更加困难，因为包名称保持合法而内部代码已被篡改。

rss · InfoQ 中文站 · May 22, 16:00

**背景**: npm（Node Package Manager）是 Node.js 的默认包管理器，拥有世界上最大的开源 JavaScript 包注册中心。供应链攻击通过篡改开发人员隐式信任的包来针对这种信任模型。类似的攻击包括 typosquatting（创建名称略微拼错的包）和依赖混淆（利用命名冲突）。早期事件包括 Axios 攻击和冒充 287+ 个流行包的活动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/tanstack-npm-packages-hacked/">84 TanStack npm Packages Hacked in Ongoing Supply-Chain ...</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/04/01/mitigating-the-axios-npm-supply-chain-compromise/">Mitigating the Axios npm supply chain compromise</a></li>
<li><a href="https://www.theregister.com/security/2024/11/05/typosquat-campaign-impersonates-287-popular-npm-packages/816810">Typosquat campaign impersonates 287+ popular npm packages</a></li>

</ul>
</details>

**社区讨论**: 安全社区对针对 CI/CD 基础设施的攻击表示强烈担忧，指出受攻击的构建管道可能会向所有下游用户传播恶意软件。许多开发人员呼吁改进包验证流程并加强自动化构建系统的保护措施。

**标签**: `#npm`, `#supply-chain-attack`, `#security`, `#JavaScript`, `#TanStack`

---

<a id="item-8"></a>
## [八部门发文整治非法跨境证券期货基金经营](https://mp.weixin.qq.com/s?__biz=MzA4NzAzMDgwMw==&amp;mid=2651090403&amp;idx=3&amp;sn=bca72a940ac72bef356f29b5b9576ac1&amp;chksm=8a1670281e2bc67d2df3608a313ba9fdaf0fcd2f43ce44475c6bf273b386af2e4f9d8e8e2e2b&amp;scene=0&amp;xtrack=1) ⭐️ 8.0/10

证监会等八部门联合印发整治方案，明确打击非法跨境证券期货基金经营。证监会对老虎证券、富途和长桥立案调查，设定 2 年集中整治期，期间仅允许存量投资者单向卖出并转出资金。期满后相关境内网站、交易软件和配套服务器要全面关停。 这是中国保护投资者免受无牌照境外金融机构服务的重要监管行动。被整治的老虎证券、富途和长桥是中国投资者最常用的跨境交易平台，此次打击将影响大量用户。2 年集中整治期为存量投资者提供了有序退出的机制。 被调查的平台被指控在未获监管批准的情况下开展证券营销、處理交易指令、提供融资融券服务,并涉嫌非法从事公募基金销售和期货经纪业务。证监会拟没收全部违法所得并依法严厉处罚。投资者可通过 QDII、港股通、跨境理财通等合法渠道开展境外投资。

telegram · zaihuapd · May 22, 08:26

**背景**: QDII（合格境内机构投资者）制度允许符合条件的境内金融机构在规定额度内投资境外证券市场。港股通使内地投资者可通过上交所或深交所交易合资格港股。跨境理财通允许粤港澳大湾区合资格居民投资对方金融产品。这些是经政府批准的合法境外投资渠道。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hkma.gov.hk/gb_chi/key-functions/international-financial-centre/wealth-management-connect/">粤港澳大湾区跨境理财通 - 香港金融管理局</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/18663032241">跨境理财通2.0版大揭秘——什么是跨境理财通？参与门槛是什么？跨境理财...</a></li>
<li><a href="https://www.sse.com.cn/services/hkexsc/home/">沪港通 - 上海证券交易所</a></li>

</ul>
</details>

**标签**: `#中国监管`, `#跨境证券`, `#证监会`, `#老虎证券`, `#富途牛牛`

---

<a id="item-9"></a>
## [Cloudflare 全球网络故障：28% HTTP 流量受影响，持续 25 分钟](https://t.me/zaihuapd/41527) ⭐️ 8.0/10

2024 年 12 月 5 日，Cloudflare 发生了一次持续约 25 分钟的全球重大网络故障，影响了约 28%的 HTTP 流量。事故源于部署 CVE-2025-55182（Next.js 中 React 服务器组件安全漏洞）安全补丁时的 WAF 规则冲突，主要影响使用旧版 FL1 代理且部署了 Cloudflare 托管规则集的客户。 此次故障发生于 UTC 时间 12 月 5 日 08:47 至 09:12 之间。根本原因是在部署 Next.js/React 服务器组件 CVE-2025-55182 安全补丁期间的 WAF（Web 应用防火墙）规则冲突。使用旧版 FL1 代理配置且部署了 Cloudflare 托管规则集的客户是主要受影响群体。

telegram · zaihuapd · May 22, 16:15

**背景**: CVE-2025-55182，也称为"React 2Shell"，是一个于 12 月 3 日在 React 服务器组件中发现的严重远程代码执行（RCE）漏洞，影响 Next.js。该漏洞会将默认配置转变为黑客远程执行任意代码的攻击向量。Cloudflare 通过其 WAF 部署了防护规则来缓解这一威胁，但规则配置与旧版 FL1 代理的冲突导致了这次大范围故障。FL1 代理似乎是 Cloudflare 网络架构中的旧版代理基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/critical-react-nextjs-security-vulnerability-what-cve-2025-55182-rfw5c">Critical React and Next . js Security Vulnerability : What...</a></li>
<li><a href="https://securitylabs.datadoghq.com/articles/cve-2025-55182-react2shell-remote-code-execution-react-server-components/">CVE - 2025 - 55182 ( React 2Shell): Remote code execution in React ...</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#network-outage`, `#infrastructure`, `#CVE-2025-55182`, `#WAF`

---

<a id="item-10"></a>
## [PydanticAI v1.101.0 新增消息队列和 MCP 后台任务支持](https://github.com/pydantic/pydantic-ai/releases/tag/v1.101.0) ⭐️ 7.0/10

PydanticAI v1.101.0 引入了待处理消息队列功能（通过 ctx.enqueue 和 agent_run.enqueue），增加了 MCP 后台任务支持（SEP-1686），使 XSearch 功能可通过子代理回退实现模型无关化，并为 GoogleModel、AnthropicModel 和 CohereModel 添加了 top_k 模型设置支持。 此版本通过消息队列增强了 pydantic-ai 的代理控制流能力，扩展了 MCP 后台任务集成，并在多个 LLM 提供商之间提供一致的 top_k 设置，使开发者更容易在不同后端上微调模型行为。 最值得注意的错误修复包括：修复 AnthropicModel 在继续对话时丢失代码执行工具结果的问题，保留 Bedrock 上 Claude Sonnet 4.6 和 Opus 4.6 的思考过程，以及要求 xai-sdk 1.6.0 以保留 Xai 工具结果 ID。XSearch 模型无关的更改允许在底层模型本身不支持时回退到子代理。

github · DouweM · May 22, 04:49

**背景**: PydanticAI 是一个利用 Pydantic 验证功能的 Python AI 代理框架。模型上下文协议（MCP）是一个开放协议，用于标准化应用程序如何向 LLM 提供工具和上下文，类似于 USB-C 端口的工作方式。XSearch 是 PydanticAI 中用于搜索的内置功能，而 top_k 是一个采样参数，用于控制模型如何从最可能的下一个标记中进行选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pydantic.dev/docs/ai/mcp/overview/">Overview | Pydantic Docs</a></li>
<li><a href="https://pydantic.dev/docs/ai/core-concepts/capabilities/">Capabilities | Pydantic Docs</a></li>

</ul>
</details>

**标签**: `#pydantic-ai`, `#AI agents`, `#Python`, `#model context protocol`, `#release notes`

---

<a id="item-11"></a>
## [SpaceX 发射 Starship 原型火箭 经历多台发动机故障](https://www.nbcnews.com/now/video/spacex-successfully-launches-prototype-of-starship-rocket-263835205505) ⭐️ 7.0/10

这次试飞展示了 SpaceX 快速发展的火箭技术所面临的挑战和成功，Raptor 发动机的可靠性成为社区讨论的焦点，截至目前工程团队已经进行了超过 300 次发动机发射测试。 关键技术事件包括：助推器上升阶段一台发动机失效、级分离后助推返回燃烧再点火失败（但发动机在着陆燃烧时确实再次点火）、Starship 级分离后不久损失一台发动机、再入时可见模拟载荷卫星燃烧解体、以及发动机舱红色光芒和损坏发动机部位的剧烈排气。

hackernews · busymom0 · May 22, 23:41

**背景**: Starship 是 SpaceX 设计的下一代可完全重复使用火箭，用于执行月球和火星任务。它采用 SpaceX 的 Raptor 发动机，这是一种甲烷燃料全流量分级燃烧循环发动机——这是一项如此先进的技术，以至于此前从未有类似的发动机成功飞行，这在火箭发动机开发史上是前所未有的。Starship V3 于 2026 年 5 月宣布重大升级，包括 280 吨推力的 Raptor V3 发动机和增大 50%的格栅翼。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://everydayastronaut.com/raptor-engine/">Is SpaceX 's Raptor engine the king of rocket... | Everyday Astronaut</a></li>
<li><a href="https://payloadspace.com/what-to-expect-from-starship-v3/">What to Expect from Starship V3</a></li>
<li><a href="https://science.slashdot.org/story/26/05/15/0225226/spacex-unveils-sweeping-starship-v3-upgrades">SpaceX Unveils Sweeping Starship V3 Upgrades - Slashdot</a></li>

</ul>
</details>

**社区讨论**: 社区的反响突出了令人印象深刻的软件制导性能（“飞船没有爆炸，而且不仅如此，还精准命中了目标”）、对发动机可靠性模式的担忧（“之前某次飞行中也有类似事故”）、对视觉画面的兴奋（“从飞船发动机舱看到的景象相当凶险”“多处可见红光”“可以看到模拟载荷卫星燃烧”），以及对超过 300 次发动机发射积累的海量数据的赞叹。

**标签**: `#spacex`, `#starship`, `#rocket-launch`, `#aerospace`, `#space-exploration`

---

<a id="item-12"></a>
## [Antigravity 2.0 在 OpenSCAD 建筑 3D 大语言模型基准测试中夺冠](https://modelrift.com/blog/openscad-llm-benchmark/) ⭐️ 7.0/10

谷歌的 Antigravity 2.0 在一项新的基准测试中夺冠，该测试用于评估大语言模型根据万神殿建筑生成 OpenSCAD 3D 模型代码的能力。一名用户报告称，通过简单提示成功生成了参数化的 OpenSCAD 模型，并首次尝试即获得了近乎完美的 3D 打印结果。 这一基准代表了首个系统性评估大语言模型生成 3D 建筑 CAD 模型代码能力的测试，开启了传统代码生成任务之外的新测试维度。它展示了 AI 辅助 3D 设计工作流的实际可行性，对创客、工程师和参数化设计师具有直接影响。 万神殿基准测试要求各大语言模型再现古罗马神庙的标志性特征，包括通过穹顶可见的方形天花板重复格子图案——这是只有 Antigravity 正确实现的细节。该基准测试比较了 Codex 5.5 High、Claude Sonnet、Claude Opus、Cursor Composer 和 ModelRift 等模型。

hackernews · jetter · May 22, 10:38

**背景**: OpenSCAD 是一款基于脚本的参数化 3D 建模软件，受到创客和工程师的欢迎，可通过代码创建精确的可打印 3D 模型。万神殿是古罗马神庙，以其带有穹顶（中央开口）和内部格子图案的巨大圆顶而闻名。这一基准代表了一种将大语言模型代码生成能力应用于建筑几何的新测试方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://modelrift.com/blog/openscad-llm-benchmark/">OpenSCAD LLM Benchmark : Building the Pantheon | ModelRift Blog</a></li>
<li><a href="https://openscad.org/">OpenSCAD - The Programmers Solid 3D CAD Modeller</a></li>
<li><a href="https://www.squaredtech.co/openscad-llm-benchmark-antigravity-20-takes-the-top-spot">OpenSCAD LLM Benchmark : Best AI Model Revealed</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：部分用户庆祝实际成功和技术成就（Antigravity 成功实现内部天花板图案），但 others 指出可用性问题，包括每次会话必须登录浏览器以及 IDE 更新失败。部分观点认为单一基准模型不足以证明整体能力，因为不同 3D 模型类型的性能差异显著。

**标签**: `#LLM`, `#OpenSCAD`, `#3D modeling`, `#benchmark`, `#code generation`

---

<a id="item-13"></a>
## [yt-dlp 因无法审核 AI 代码库而移除 Bun 支持](https://github.com/yt-dlp/yt-dlp/issues/16766) ⭐️ 7.0/10

评论者意见分歧：一些人同意 yt-dlp 的观点，认为审核 100 万行 AI 生成的代码不切实际，而另一些人则认为这个决定是出于政治动机而非技术正当性。一些人维护维护者选择技术栈的权利，而批评者指出 Rust 重写甚至尚未发布以证明实际存在稳定性问题。

hackernews · tamnd · May 22, 17:24

**背景**: yt-dlp 是一个从 youtube-dl 分发的流行开源视频下载器，支持数百个网站。Bun 是一个 JavaScript 运行时，最近经历了从 Zig 到 Rust 的大规模重写，据报道这一过程得到了 Anthropic AI 的协助。辩论的焦点在于维护者是否应该在未经人工审核的情况下接受 AI 生成的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/yt-dlp/yt-dlp">GitHub - yt-dlp/yt-dlp: A feature-rich command-line audio ...</a></li>
<li><a href="https://forums.freebsd.org/threads/ai-and-rust-triggers-all-in-one-commit-of-10-6-lines-of-code.102703/">AI and Rust triggers - all in one commit (of 10^6 lines of code)</a></li>

</ul>
</details>

**社区讨论**: 评论者意见分歧：一些人同意 yt-dlp 的观点，认为审核 100 万行 AI 生成的代码不切实际，而另一些人则认为这个决定是出于政治动机而非技术正当性。一些人维护维护者选择技术栈的权利，而批评者指出 Rust 重写甚至尚未发布以证明实际存在稳定性问题。

**标签**: `#JavaScript`, `#Bun Runtime`, `#Open Source`, `#Programming Tools`, `#AI-Coded Software`

---

<a id="item-14"></a>
## [DeepSeek 将 V4 Pro API 定价永久降至原价的 25%](https://api-docs.deepseek.com/quick_start/pricing) ⭐️ 7.0/10

DeepSeek 宣布，在 2026 年 5 月 31 日 75%折扣促销活动结束后，V4 Pro API 定价将永久降低至原价的 25%。 这使得 DeepSeek V4 Pro 比其他供应商托管的同款模型便宜得多，引发了关于成本可持续性的争论，以及低价是否通过使用用户数据训练模型来补贴的质疑。 除了永久降价外，DeepSeek 还将输入缓存命中价格降低至发布价的 1/10，V4 Pro 缓存命中现在仅为输入价的 0.8%，与竞争对手相比极低，已影响单位经济效益。

hackernews · Tiberium · May 22, 15:59

**背景**: DeepSeek 是一家中国 AI 公司，成立于 2023 年 7 月，由对冲基金 High-Flyer 联合创始人梁文锋创立。该公司因在 2024-2025 年发布 V3 和 R1 等开源模型而声名鹊起。其隐私政策规定，用户输入可用于改进和开发服务以及训练技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://aiwiki.ai/wiki/deepseek">DeepSeek - AI Wiki DeepSeek AI – History, Founders and the Open Source ... The history of Deepseek: A New Era in Artificial Intelligence DeepSeek's Timeline — Full Story History | Shapes AI Who created DeepSeek? Meet the company behind the Chinese AI DeepSeek（An AI Assistant launched by Hangzhou DeepSeek ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应两极分化。部分用户认为 DeepSeek 允许用户输入用于改进模型的隐私政策导致价格低得令人怀疑。另一些用户则称赞 DeepSeek 的开源模型、发表的研究和提供的优质价值。也有用户对极低的缓存定价及其对单位经济效益的影响感到好奇。

**标签**: `#ai-pricing`, `#deepseek`, `#llm-apis`, `#open-source-ai`, `#machine-learning`

---

<a id="item-15"></a>
## [企业 AI 采购：专业化优于规模化的战略考量](https://huggingface.co/blog/Dharma-AI/specialization-beats-scale) ⭐️ 7.0/10

Hugging Face 发布了一份战略分析，认为大多数企业在采购 AI 时错误地优先考虑模型规模而非专业化，从而忽视了专业化 AI 解决方案能够提供的关键竞争优势。 这一分析非常重要，因为企业可能正在浪费预算购买通用的大型模型，而更小、更专业化的模型可能为其实际用例提供更好的成本效益和领域特定性能。 "专业化优于规模化"的论点表明，按特定领域或任务微调的专业化 AI 模型可以在准确性和效率上优于更大的通用模型，同时部署和维护成本更低。

rss · Hugging Face Blog · May 22, 15:25

**背景**: AI 采购是指企业如何为其业务运营选择和购买 AI 工具、模型或服务。传统观点认为参数更多的更大模型提供更好的性能，但这份分析对此假设提出了挑战，认为针对特定任务优化的专业化模型可以在企业环境中提供更优的结果。

**标签**: `#AI procurement`, `#enterprise AI`, `#AI strategy`, `#business decision-making`, `#technology selection`

---

<a id="item-16"></a>
## [AI 利用频谱图复活已故飞行员声音](https://techcrunch.com/2026/05/22/ai-is-being-used-to-resurrect-the-voices-of-dead-pilots/) ⭐️ 7.0/10

这代表了一种危险的新能力，可以在未经同意的情况下复活声音，引发了关于个人隐私、家属权利以及航空调查完整性的深刻伦理问题。NTSB 前所未有的行动表明，现有的公共数据访问框架在生成式人工智能时代已经不够充分。 该人工智能技术分析频谱图图像（音频频率随时间变化的视觉表示），并从这些视觉模式中重建语音数据。NTSB 的案件系统中包含这些频谱图记录作为公共事故调查记录，这些记录被人功智能工具所利用。

rss · TechCrunch AI · May 22, 23:03

**背景**: 频谱图是音频录音频谱的视觉表示，以颜色或亮度显示随时间的变化。NTSB（美国国家运输安全委员会）是负责调查交通事故（包括飞机坠毁）的美国联邦机构，并维护着包含事故调查文件的公共案件系统。驾驶舱语音记录器（CVR）在事故期间捕获来自飞机驾驶舱的音频，是确定原因和促成因素的关键证据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ntsb.gov/pages/dockets-unavailable.aspx">Docket Status - National Transportation Safety Board</a></li>
<li><a href="https://aitoolly.com/ai-news/article/2026-05-23-ai-reconstructs-deceased-pilots-voices-from-spectrograms-prompting-ntsb-to-block-public-docket-acces">AI Reconstructs Pilot Voices: NTSB Blocks Docket Access</a></li>

</ul>
</details>

**标签**: `#AI ethics`, `#audio synthesis`, `#aviation safety`, `#NTSB`, `#deepfakes`

---

<a id="item-17"></a>
## [AI 生成小说入围英联邦短篇小说奖引争议](https://www.theverge.com/tech/936073/ai-writing-granta-commonwealth-prize) ⭐️ 7.0/10

这一事件标志着关于人工智能在创意产业中辩论的重要里程碑，引发了有关作者身份验证、检测可靠性以及生成式人工智能时代创意作品真实性的紧迫问题。 这篇小说表现出人工智能生成文本的多个特征，引起文学机构的审查。人工智能检测工具虽然存在，但其准确性仍不稳定，为验证作者身份声明带来了挑战。

rss · The Verge AI · May 22, 14:30

**背景**: 《格兰塔》是一家成立于 1889 年的著名英国文学杂志，每年都会发布英联邦短篇小说奖的地区获奖者，这是最著名的国际文学奖项之一。随着大型语言模型的普及，人工智能生成文本检测作为一个不断发展的领域应运而生，方法从统计启发式算法到机器学习分类器不等，但对其可靠性的担忧持续存在。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybernews.com/ai-tools/how-do-ai-detectors-work/">How Do AI Detectors Work? AI vs. Human Content Explained</a></li>
<li><a href="https://www.researchgate.net/publication/220433607_Computational_Methods_in_Authorship_Attribution">(PDF) Computational Methods in Authorship Attribution</a></li>

</ul>
</details>

**标签**: `#generative AI`, `#literature`, `#authorship`, `#AI detection`, `#creative industries`

---

<a id="item-18"></a>
## [海湾国家因 AI 基础设施发展被敦促多元化海底电缆](https://www.wired.com/story/the-gulfs-ai-boom-has-an-undersea-cable-problem/) ⭐️ 7.0/10

包括 AWS、谷歌云、微软 Azure 和甲骨文在内的超大规模云服务商正在向海湾国家施压，要求其多元化海底互联网电缆路由，因为 AI 驱动的数据中心增长正在创造前所未有的连接需求和安全问题。 这很重要，因为海底电缆是云计算的物理骨干，任何中断都可能瘫痪海湾国家正在积极建设的 AI 运营。从事 AI 系统的工程师和架构师需要了解这些物理依赖关系。 目前，大多数海湾地区的互联网流量通过有限的海底电缆路径传输，形成了单点故障。超大规模云服务商希望实现更多样化的路由，以提高冗余性、降低延迟并降低潜在破坏或自然灾害的安全风险。

rss · WIRED AI · May 22, 09:00

**背景**: 超大规模云服务商是指 AWS、谷歌云平台、微软 Azure 和甲骨文云计算基础设施等大型云计算提供商，它们运营着支持 AI 工作负载的大型数据中心。海底电缆承载着约 95%的国际互联网流量，使其成为全球数字连接的关键基础设施。海湾地区因丰富的能源资源和战略位置已成为 AI 数据中心建设的主要枢纽。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hyperscale_computing">Hyperscale computing - Wikipedia</a></li>
<li><a href="https://www.oracle.com/cloud/hyperscaler-cloud/">What Is a Hyperscale Cloud? - Oracle</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#undersea cables`, `#hyperscalers`, `#cloud computing`, `#geopolitical technology`

---

<a id="item-19"></a>
## [FTC 对 CMG 处以 93 万美元罚款：涉欺骗性"主动监听"AI 营销服务](https://simonwillison.net/2026/May/22/ftc-active-listening/#atom-everything) ⭐️ 7.0/10

美国联邦贸易委员会（FTC）已与考克斯媒体集团（CMG）及另外两家公司（MindSift 和 1010 Digital Works）达成和解，和解金总计 93 万美元。FTC 指控这些公司欺骗性地营销一项名为"主动监听"的 AI 服务，声称可利用智能设备对话中的语音数据进行广告定向，但实际上仅仅是转售从数据经纪人处获取的电子邮件列表。 此和解重要之处在于，它确立了明确的先例：仅仅点击同意强制服务条款并不构成对侵入性语音数据收集的有效同意。这一裁决还驳斥了智能手机会主动监听用户对话以进行广告定向这一长期流传的阴谋论。 根据 FTC 的投诉，CMG 的"主动监听"服务实际上并未监听消费者对话或使用语音数据。这些公司只是将从其他数据经纪人处获得的电子邮件列表加价转售。如果该服务如宣传所示运作，在未获得适当同意的情况下收集语音数据将违反 FTC 法案第 5 条。

rss · Simon Willison · May 22, 04:48

**背景**: "主动监听"营销概念于 2024 年出现，当时 CMG 的宣传被泄露，声称智能设备可以从对话中捕获实时意向数据，帮助广告商定向目标消费者。这加剧了手机通过麦克风监听用户以投放广告的广泛阴谋论。FTC 的和解明确指出，实际上并未发生真正的语音监听尝试，但如果在没有适当同意的情况下进行此类收集，将违反 FTC 法规。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ftc.gov/news-events/news/press-releases/2026/05/ftc-require-cox-media-group-two-other-firms-pay-nearly-1-million-settle-charges-they-deceived">FTC to Require Cox Media Group, Two Other Firms to Pay Nearly ...</a></li>
<li><a href="https://www.documentcloud.org/documents/25051283-cmg-pitch-deck-on-voice-data-advertising-active-listening/">CMG Pitch Deck on Voice - Data Advertising ' Active Listening '</a></li>

</ul>
</details>

**社区讨论**: 科技博主西蒙·威尔逊（Simon Willison）指出，这是他 ongoing efforts to 揭穿麦克风广告阴谋论的令人欣慰的"新弹药"。评论者们对 FTC 澄清服务条款点击不等于同意表示赞赏，尽管一些人仍对在其他情境下是否可能发生语音数据收集持怀疑态度。

**标签**: `#privacy`, `#AI regulation`, `#FTC`, `#surveillance advertising`, `#consumer protection`

---

<a id="item-20"></a>
## [深入解析 ThunderKittens：面向高性能 AI 内核的紧凑型领域特定语言](https://hamzaelshafie.bearblog.dev/dissecting-thunderkittens-anatomy-of-a-compact-dsl-for-high-performance-ai-kernels/) ⭐️ 7.0/10

该文章被提交到 Lobsters，一个技术新闻聚合平台。提供的内容仅显示评论链接，表明社区对该话题有兴趣，但没有可用的具体评论详情进行深入分析。

rss · Lobsters - AI · May 22, 05:38

**背景**: 领域特定语言（DSL）是一种专门针对特定问题领域的专用编程语言，不同于通用编程语言。在 AI/ML 上下文中，内核是在张量数据上执行数学变换的基础计算操作。像内存合并（将 warp 中线程的内存访问合并）以及避免 warp 分支（线程执行不同路径）是 GPU 优化的关键，对于在 AI 工作负载中实现高性能至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rightnowai.co/guides/cuda-operations/memory-coalescing">CUDA Memory Coalescing : Complete Optimization ... | RightNow AI</a></li>
<li><a href="https://modal.com/gpu-glossary/perf/warp-divergence">What is warp divergence ? | GPU Glossary</a></li>

</ul>
</details>

**标签**: `#domain-specific-languages`, `#ai-kernels`, `#high-performance-computing`, `#compiler-optimization`, `#machine-learning-infrastructure`

---

<a id="item-21"></a>
## [企业 Token 成本焦虑推动 AI 基础设施新市场崛起](https://www.infoq.cn/article/TLRAmZy8pPICVFVWmu6p?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

一篇中国科技文章探讨了企业对 AI token 成本日益增长的担忧如何推动 AI 基础设施市场的发展，揭示了仅购买 GPU 卡或 API token 等计算资源与实现实际生产力提升之间的鸿沟。 这一点很重要，因为企业在 AI 推理上投入巨大，却难以将这些投资转化为可衡量生产力提升，这催生了对专业基础设施解决方案的需求，这些方案可以优化 token 成本并提供真正的业务价值。 Token 定价通常采用按量计费模式，即客户按处理的 token 数量付费。当前的 LLM 推理优化技术包括量化、KV 缓存压缩、连续批处理、投机解码和上下文压缩等方法，这些方法可以在保持模型质量的同时将成本降低 10 倍。

rss · InfoQ 中文站 · May 22, 20:34

**背景**: AI token 是语言模型用于处理文本的子词片段，代表生成式 AI 服务的基本计算单元。随着企业将 AI 部署扩展到数十亿次请求，推理成本已 成为部署经济中的主导因素。使用量计费模式的兴起意味着组织直接为所消耗的计算资源付费，而不是授权固定的基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.solvimon.com/glossary/ai-token-pricing">What is AI Token Pricing ? | Solvimon Glossary</a></li>
<li><a href="https://www.programming-helper.com/tech/ai-inference-optimization-2026-techniques-reducing-llm-costs-10x">AI Inference Optimization 2026: How Quantization ...</a></li>

</ul>
</details>

**标签**: `#AI Infrastructure`, `#Enterprise AI`, `#Token Cost`, `#AI Chips`, `#Market Trends`

---

<a id="item-22"></a>
## [Anthropic 推出 MCP 隧道供私有代理访问](https://www.infoq.cn/article/jvoDNDaa2bRzwrHQy7lT?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Anthropic 发布了 MCP 隧道，这是模型上下文协议的新功能，使私有代理能够安全地访问内部企业系统，而无需将服务暴露到公共互联网。 MCP 隧道的工作原理是从私有网络建立到 Claude 的出站连接，这意味着不需要打开入站端口，组织也不需要将 Anthropic 的 IP 范围列入白名单。这与 OpenAI 的安全 MCP 隧道功能遵循相同的模式。

rss · InfoQ 中文站 · May 22, 20:00

**背景**: 模型上下文协议（MCP）是 Anthropic 于 2024 年 11 月推出的开放标准，被称为 AI 应用的 USB-C 端口，使 Claude 等 AI 助手能够与外部工具和系统连接并共享数据。MCP 隧道专门解决了将 AI 模型连接到位于防火墙后或私有网络中的内部系统的挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/model-context-protocol">Introducing the Model Context Protocol \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/mcp-tunnels/overview">MCP tunnels - Claude API Docs</a></li>
<li><a href="https://developers.openai.com/api/docs/guides/secure-mcp-tunnels">Secure MCP Tunnel | OpenAI API</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#MCP`, `#AI Security`, `#Enterprise AI`, `#Model Context Protocol`

---

<a id="item-23"></a>
## [Cloudflare 推出 Dynamic Workflows 实现持久化执行动态扩展](https://www.infoq.cn/article/4DhNBEdPJL4q8cA8cXso?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Cloudflare 发布了 Dynamic Workflows，这是一个 MIT 许可的库，将其持久化执行引擎扩展为允许工作流代码在运行时根据租户、AI 代理或请求的不同而变化，支持从单个调度程序 Worker 进行动态路由。 这使得多租户平台能够以接近零的空闲成本为数百万个独特的工作流提供服务，彻底改变了开发者构建无服务器应用的方式，可以为每个客户动态扩展而无需为每个租户部署单独的基础设施。 Dynamic Workflows 基于 Dynamic Workers 构建，并将持久化执行能力扩展到超越传统模型——传统上 Workflow 在部署时绑定到静态 class_name，现在则支持在运行时选择不同的工作流实现。

rss · InfoQ 中文站 · May 22, 09:47

**背景**: 持久化执行是一种编程范式，即使中途中断后代码仍能继续执行，在多次调用之间保持状态。多租户架构允许单个应用实例服务多个客户（租户）。在 Dynamic Workflows 之前，每个租户或用例通常需要单独部署工作流。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/dynamic-workflows/">Introducing Dynamic Workflows: durable execution that follows ...</a></li>
<li><a href="https://github.com/cloudflare/dynamic-workflows">GitHub - cloudflare/dynamic-workflows</a></li>
<li><a href="https://www.infoq.com/news/2026/05/cloudflare-dynamic-workflows/">Cloudflare Ships Dynamic Workflows, Bringing Durable ... - InfoQ</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#Serverless`, `#Durable Execution`, `#Multi-tenant`, `#Workflow Automation`

---

<a id="item-24"></a>
## [礼来 retatrutide 三期试验最高剂量平均减重 28.3%](https://www.prnewswire.com/news-releases/lillys-triple-agonist-retatrutide-delivered-powerful-weight-loss-in-pivotal-phase-3-obesity-trial-302778859.html) ⭐️ 7.0/10

这代表了迄今为止任何三期肥胖药物报告中最强的减重疗效，使 retatrutide 成为潜在的同类最佳治疗方法。靶向 GLP-1、GIP 和胰高血糖素受体的三重激动剂机制为单激动剂或双激动剂治疗反应不佳的患者提供了一种新方法。 这一消息之所以重要，是因为它代表了迄今为止任何三期肥胖药物中报告的最强减重疗效，确立了 retatrutide 作为潜在的同类最佳治疗方案。靶向 GLP-1、GIP 和胰高血糖素受体的三重激动剂机制为单激动剂或双激动剂治疗反应不佳的患者提供了一种新颖的方法。 试验纳入了约 2500 名肥胖或超重且伴至少一种体重相关合并症的无糖尿病成人。4mg 剂量组平均减重 19.0%。因不良事件停药率为 4.1%，低于安慰剂组的 4.9%。主要副作用为胃肠道反应，未观察到心脏或肝脏安全信号。

telegram · zaihuapd · May 22, 02:18

**背景**: Retatrutide (LY3437943)是礼来开发的一种实验性三重激素受体激动剂，同时激活 GLP-1、葡萄糖依赖性促胰岛素多肽(GIP)和胰高血糖素受体。这使其与司美格鲁肽(单一 GLP-1 激动剂)和替西帕肽(GLP-1/GIP 双激动剂)区别开来。据信，三重激动作用通过减少食欲、增加能量消耗和改善代谢功能等互补机制来增强减重效果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.drugs.com/history/retatrutide.html">Retatrutide: What is it and is it FDA approved? - Drugs.com Triple–Hormone-Receptor Agonist Retatrutide for Obesity — A ... What Is Retatrutide? Triple Agonist Drug Explained (2026) Top Stories Study Details | NCT07232719 | A Study of Retatrutide ... Retatrutide - Wikipedia What Is Retatrutide? Complete Guide to the Triple-Agonist ...</a></li>
<li><a href="https://www.nejm.org/doi/full/10.1056/NEJMoa2301972">Triple–Hormone-Receptor Agonist Retatrutide for Obesity — A ...</a></li>
<li><a href="https://www.lilly.com/news/stories/what-to-know-about-retatrutide">What to know about retatrutide - lilly.com</a></li>

</ul>
</details>

**标签**: `#pharmaceutical`, `#clinical-trials`, `#obesity-treatment`, `#weight-loss`, `#GLP-1-agonist`

---

<a id="item-25"></a>
## [Take-Two 确认 GTA6 发售日期不变，宣发 6 月下旬启动](https://bsky.app/profile/jasonschreier.bsky.social/post/3mmfadqfj4c2f) ⭐️ 7.0/10

发售日期维持在 2026 年 11 月 19 日。美国夏季通常从 6 月下旬持续到 9 月下旬。第三支预告片不会在 6 月前发布。预购将随营销活动同步开启，而非提前很久开放。

telegram · zaihuapd · May 22, 03:10

**背景**: 《侠盗猎车手》(GTA)是全球最畅销的电子游戏系列之一，由 Rockstar Games 开发。《GTA5》于 2013 年发售，成为历史上最畅销的电子游戏。自 2023 年首支预告片泄露以来，GTA6 一直备受期待。Take-Two Interactive 是 Rockstar 的母公司，为上市公司(股票代码：TTWO)。

**标签**: `#GTA6`, `#Take-Two`, `#Video Games`, `#Rockstar Games`, `#Gaming Industry`

---

<a id="item-26"></a>
## [字节跳动开源 30 亿参数统一多模态模型 Lance](https://mp.weixin.qq.com/s/Xbfq72cr1796RZxJIs3L1A) ⭐️ 7.0/10

这之所以重要是因为它证明了相对较小的 30 亿参数模型可以实现理解与生成任务之间的统一多模态能力，有望实现更高效的部署。Apache 2.0 许可证使其可用于商业用途，且其在基准测试中的领先结果表明具有实际可行性。 Lance 采用共享上下文与双流专家架构，分别由 Qwen2.5-VL 编码器处理理解任务、Wan2.2 编码器处理生成任务。它通过模态感知位置编码解决序列边界混淆。该模型在 GenEval 图像生成和 VBench 视频生成等基准上取得了领先结果，权重已在 Hugging Face 开放。

telegram · zaihuapd · May 22, 06:40

**背景**: 多模态 AI 模型通常将理解（分析图像/视频）和生成（创建图像/视频）作为独立系统来处理。Qwen2.5-VL 是阿里巴巴用于理解任务的视觉语言模型，而 Wan2.2 是其支持 720P 分辨率的开源视频生成模型。GenEval 和 VBench 分别是评估图像和视频生成质量的权威基准。位置编码帮助 Transformer 理解序列数据中的顺序和关系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wan22.io/">Wan 2 . 2 - Open Source MoE Video Generation | Every Shot... | wan22.io</a></li>
<li><a href="https://github.com/Vchitect/VBench">Vchitect/VBench: [CVPR2024 Highlight] VBench - GitHub</a></li>

</ul>
</details>

**标签**: `#multimodal AI`, `#open source`, `#image generation`, `#video generation`, `#ByteDance`

---