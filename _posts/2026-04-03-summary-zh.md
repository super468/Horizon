---
layout: default
title: "Horizon Summary: 2026-04-03 (ZH)"
date: 2026-04-03
lang: zh
---

> From 215 items, 23 important content pieces were selected

---

1. [Google 发布 Gemma 4 开源模型，性能表现强劲](#item-1) ⭐️ 9.0/10
2. [Cursor 3 发布引争议 AI 编程工具方向引热议](#item-2) ⭐️ 8.0/10
3. [LinkedIn 静默扫描浏览器扩展进行指纹识别](#item-3) ⭐️ 8.0/10
4. [Nekogram 12.5.2 后门静默窃取用户手机号](#item-4) ⭐️ 8.0/10
5. [Google 发布 Gemma 4 开放模型家族 四种规格覆盖移动端到工作站](#item-5) ⭐️ 8.0/10
6. [Hugging Face Transformers v5.5.0 添加 Gemma4 支持](#item-6) ⭐️ 7.0/10
7. [前 Azure 工程师指控微软忽视平台警告](#item-7) ⭐️ 7.0/10
8. [阿里发布 Qwen3.6-Plus：仅限托管服务，不开放权重](#item-8) ⭐️ 7.0/10
9. [AMD Lemonade：支持 GPU 和 NPU 的开源本地大语言模型服务器](#item-9) ⭐️ 7.0/10
10. [OpenAI 收购 TBPN 播客网络](#item-10) ⭐️ 7.0/10
11. [TGS 在 AWS 上实现地震基础模型近线性扩展](#item-11) ⭐️ 7.0/10
12. [NVIDIA 批量模式 VC-6 将视觉 AI 解码时间缩短 85%](#item-12) ⭐️ 7.0/10
13. [NVIDIA GH200 实现个位数微秒级延迟推理](#item-13) ⭐️ 7.0/10
14. [微软发布三个新型基础 AI 模型](#item-14) ⭐️ 7.0/10
15. [Moonlake：通过游戏引擎代理构建多模态因果世界模型](#item-15) ⭐️ 7.0/10
16. [Trytet：面向状态化 AI 代理的确定性 WASM 底层平台](#item-16) ⭐️ 7.0/10
17. [Google 禁止了一款实际控制应用的人工智能代理应用](#item-17) ⭐️ 7.0/10
18. [用户起诉 Anthropic 未经授权使用其人格](#item-18) ⭐️ 7.0/10
19. [Cloudflare 用 AI 周末复刻 Next.js 功能，花费 1100 美元](#item-19) ⭐️ 7.0/10
20. [智谱 AI 发布首款多模态编程基础模型 GLM-5V-Turbo](#item-20) ⭐️ 7.0/10
21. [我国首部移动电源安全国标发布，2027 年强制实施](#item-21) ⭐️ 7.0/10
22. [英伟达中国 AI 芯片市场份额降至 55%，本土厂商崛起](#item-22) ⭐️ 7.0/10
23. [微软发布 3 款自研 AI 模型直接挑战 OpenAI](#item-23) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Google 发布 Gemma 4 开源模型，性能表现强劲](https://deepmind.google/models/gemma/gemma-4/) ⭐️ 9.0/10

Google DeepMind 发布了 Gemma 4 开源模型，包含 2B、4B、26B-a4b、31B 和 E4B 等多个版本，性能表现强劲，与 Qwen 3.5 相当，同时社区也分享了量化资源与本地部署指南。 关键技术设置包括 temperature=1.0、top_p=0.95、top_k=64，EOS 标记为"<turn|>"，思维追踪使用"<|channel>thought\n"。31B 模型在本地测试中出现问题，无论输入什么提示都输出"---"，而 26B-a4b 在本地设备上表现异常出色。

hackernews · jeffmcjunkin · Apr 2, 16:10

**背景**: Gemma 是 Google 的轻量级开源模型系列，基于与 Gemini 模型相同的技术构建。这些模型专为各种生成式 AI 任务设计，包括问答、摘要和推理。Gemma 4 系列是最新迭代版本，具有改进的多模态能力和推理功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/gemma/">Gemma — Google DeepMind</a></li>
<li><a href="https://ai.google.dev/gemma/docs">Gemma models overview | Google AI for Developers</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示了强烈的兴趣和实际测试结果。用户报告 26B-a4b 在笔记本电脑上表现优异，而 31B 模型存在问题。UNSLOTH 提供了量化指南，Gemma 团队成员也加入回答问题。与 Qwen 3.5 的基准对比显示在多个指标上具有竞争力的结果。

**标签**: `#AI`, `#Google DeepMind`, `#Open Models`, `#Gemma`, `#LLM`

---

<a id="item-2"></a>
## [Cursor 3 发布引争议 AI 编程工具方向引热议](https://cursor.com/blog/cursor-3) ⭐️ 8.0/10

Cursor 3 作为热门 AI 代码编辑器的新版本发布，引入了增强的智能体功能 Composer 2。该版本引发了热烈的社区讨论，用户对新版智能体功能的看法呈现两极分化——有人赞赏新功能，也有人担忧传统 IDE 功能会被削弱。 这很重要，因为 Cursor 已成为最受欢迎的 AI 编程工具之一，社区的反应反映了开发者社区关于 AI 编程工具应该向智能体化功能还是保持传统 IDE 功能发展的更广泛辩论。此次发布也突显了 Cursor 与 Claude Code 等工具之间日益激烈的竞争。 关键的技术细节包括 Composer 2 作为新的默认模型，用户将其与 Claude Code 的智能体能力进行比较。部分用户已完全关闭 LLM 功能，倾向于手动编码同时保留 Cursor 的自动补全功能。企业版定价也受到批评，被认为与免费替代方案相比过于昂贵。

hackernews · adamfeldman · Apr 2, 18:13

**背景**: Cursor 是一款将大语言模型集成到开发环境中的 AI 代码编辑器。自主编码智能体是设计用于在最小人力干预下独立计划、生成、执行和验证代码的 AI 系统。Cursor 3 周围的 debate 反映了更广泛的行业趋势，即 Claude Code 和 Windsurf 等工具正在推动更加智能体化的 AI 编码体验，而一些开发者则更喜欢传统的 IDE 工作流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.qodo.ai/blog/best-ai-coding-assistant-tools/">Top 15 AI Coding Assistant Tools to Try in 2026</a></li>
<li><a href="https://www.emergentmind.com/topics/autonomous-coding-agents">Autonomous Coding Agents</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示出对 Cursor 方向存在强烈分歧。像 athoscouto 这样的支持者赞赏增强的智能体功能，认为 Composer 2 虽然不如旗舰模型智能，但很有效。而 bastawhiz 和 nu11ptr 等批评者更喜欢传统 IDE 功能，担心行业正在向削弱用户控制的'氛围编程'发展。Gimpei 等其他用户则质疑，考虑到来自 Claude Code 的竞争加剧，Cursor 的价值定位是什么。

**标签**: `#Cursor`, `#AI coding`, `#IDE`, `#Product release`, `#Claude Code`

---

<a id="item-3"></a>
## [LinkedIn 静默扫描浏览器扩展进行指纹识别](https://browsergate.eu/) ⭐️ 8.0/10

研究人员发现，当用户在基于 Chrome 的浏览器中打开 LinkedIn 时，LinkedIn 的 JavaScript 会静默扫描已安装的浏览器扩展，通过 ID 探测数千个特定扩展，对结果进行加密后传输到 LinkedIn 的服务器。 这是浏览器指纹识别领域的重要隐私问题，通过扫描扩展可以创建独特的用户指纹，即使清除 cookie 或更换浏览器也能追踪用户，侵犯了用户隐私权。 这种方法被称为"spectroscopy"（光谱分析），结合了扩展探测和 DOM 残留检测技术。LinkedIn 声称这是为了检测违反服务条款的数据抓取扩展，但研究者因此被限制账户。

hackernews · digitalWestie · Apr 2, 13:09

**背景**: 浏览器指纹识别是一种在不依赖 cookie 的情况下识别和追踪用户的技术，通过收集浏览器和系统配置信息创建独特标识。设备指纹可以在用户隐藏 IP 或切换浏览器时仍能部分识别设备，这也引发了隐私倡导者的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Browser_fingerprinting">Browser fingerprinting</a></li>
<li><a href="https://en.wikipedia.org/wiki/Device_fingerprint">Device fingerprint - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一，有人认为这虽然是入侵性的，但符合现代浏览器指纹识别的预期；也有人批评这种行为在缺乏披露的情况下本质上是间谍软件。LinkedIn 官方回应称这些指控是错误的，并表示只检测违反服务条款的扩展。

**标签**: `#privacy`, `#browser-security`, `#fingerprinting`, `#linkedin`, `#web-tracking`

---

<a id="item-4"></a>
## [Nekogram 12.5.2 后门静默窃取用户手机号](https://thebadinteger.github.io/nekogram-phone-exfiltration/) ⭐️ 8.0/10

安全研究人员发现第三方 Telegram 客户端 Nekogram 12.5.2（Google Play 版）存在后门，会在用户不知情的情况下收集所有已登录账号的手机号，并通过 Inline Query 外传至开发者控制的 Bot（@nekonotificationbot）。该恶意代码仅存在于编译发布的 APK 中，不在公开的 GitHub 源码里。 后门代码位于 Extra.java（混淆后为 uo5），核心逻辑为遍历 8 个账号槽位，提取 UserID 与手机号，拼接密钥后通过 Inline Query 发送。所有关键字符串均采用自定义加密混淆。独立反编译对比验证了从源码自行编译的版本不含后门组件。

telegram · zaihuapd · Apr 2, 12:58

**背景**: Nekogram 是一款第三方 Telegram 客户端，具有头像抽屉背景、使用系统表情符号等特色功能。Telegram 的 Inline Query API 允许用户直接在聊天中查询 Bot。安全专家长期以来一直警告第三方客户端可以获取账户凭证、读取聊天记录并收集设备可识别信息，包括手机号。此事件凸显了盲目信任开源客户端而不验证编译后二进制文件的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://play.google.com/store/apps/details?id=tw.nekomimi.nekogram&hl=en_US">Nekogram - Google Play 上的应用</a></li>
<li><a href="https://core.telegram.org/api/bots/inline">Users can interact with your bot via inline queries , straight from the...</a></li>
<li><a href="https://medium.com/@lookess/电报各种第三方客户端-e81f22f294ef">电报各种第三方客户端</a></li>

</ul>
</details>

**标签**: `#security`, `#telegram`, `#backdoor`, `#privacy`, `#supply-chain-attack`, `#vulnerability`

---

<a id="item-5"></a>
## [Google 发布 Gemma 4 开放模型家族 四种规格覆盖移动端到工作站](https://blog.google/innovation-and-ai/technology/developers-tools/gemma-4/) ⭐️ 8.0/10

此次发布为开发者提供了从边缘设备到工作站的灵活部署选项，31B 模型在 Arena AI 开放模型排行榜中位列第 3，26B 模型位列第 6，展现了强劲的基准测试性能。 E2B 和 E4B 支持原生音频输入和 128K 上下文窗口用于离线边缘运行，更大模型支持最高 256K 上下文。Gemma 自首次发布以来累计下载量已超过 4 亿次，衍生版本超过 10 万个。

telegram · zaihuapd · Apr 2, 16:12

**背景**: Gemma 是 Google 为开发者设计的开放模型家族。MoE（混合专家）架构允许模型仅对每个输入使用部分参数，从而实现更高效的计算。Arena AI 是一个社区驱动的 LLM 排行榜，通过真实用户查询和投票来评估模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arena.ai/">Arena AI: The Official AI Ranking & LLM Leaderboard</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>

</ul>
</details>

**标签**: `#Google Gemma`, `#Open Source AI`, `#LLM`, `#Edge AI`, `#Model Release`

---

<a id="item-6"></a>
## [Hugging Face Transformers v5.5.0 添加 Gemma4 支持](https://github.com/huggingface/transformers/releases/tag/v5.5.0) ⭐️ 7.0/10

Hugging Face transformers v5.5.0 添加了对谷歌 Gemma4 多模态模型的支持，该模型有 1B/13B/27B 三种参数规模，配备固定令牌预算的视觉处理器和空间二维 RoPE 编码。 此更新使开发者能够轻松使用 Gemma4 的高级多模态功能，特别是其能够以固定令牌预算处理不同尺寸图像并保持宽高比的能力。 视觉处理器支持每张图像 70 到 1120 个软令牌（默认 280），高度和宽度需能被 48 整除。它使用空间二维 RoPE 独立旋转注意力头在 x 轴和 y 轴上的维度，使模型能够理解空间关系。与标准视觉模型不同，Gemma4 不应用 ImageNet 均值/标准差归一化。

github · ArthurZucker · Apr 2, 16:15

**背景**: Gemma4 是谷歌最新的开放多模态模型系列，支持图像、文本和音频输入。其关键创新在于视觉处理器能够在将图像适配到固定令牌预算的同时保持自然宽高比，这与以往将图像压缩成固定正方形的模型不同。空间二维 RoPE 将旋转位置嵌入扩展到二维，使模型能够理解「上方」和「下方」等空间关系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/gemma-4/">Gemma 4: Our most capable open models to date - The Keyword</a></li>
<li><a href="https://huggingface.co/blog/gemma4">Welcome Gemma 4: Frontier multimodal intelligence on device</a></li>
<li><a href="https://www.emergentmind.com/topics/2d-rotary-position-embedding-rope">2D Rotary Position Embedding (RoPE)</a></li>

</ul>
</details>

**社区讨论**: 该发布在多模态 AI 社区引发了关注，特别是固定令牌预算功能和用于视觉理解的空间二维 RoPE 编码引起了热烈讨论。

**标签**: `#huggingface`, `#transformers`, `#gemma4`, `#multimodal`, `#machine learning`, `#release`

---

<a id="item-7"></a>
## [前 Azure 工程师指控微软忽视平台警告](https://isolveproblems.substack.com/p/how-microsoft-vaporized-a-trillion) ⭐️ 7.0/10

这很重要，因为它可能影响数百万依赖 Azure 云服务的企业客户，并引发人们对微软在大幅裁员和 AI 投资期间对平台质量承诺的质疑。 该工程师于 2025 年 1 月 7 日向 CEO 发送了执行摘要，在没有收到回复后，通过公司秘书向董事会写信。微软在 2025 年 5 月和 7 月进行了约 15,000 人的裁员。

hackernews · axelriet · Apr 2, 16:00

**背景**: Azure 是微软的云计算平台，与 AWS 和谷歌云竞争。这些指控表明平台质量和文档存在系统性问题，可能影响企业客户对云计算基础设施的决策。

**社区讨论**: 评论显示反应不一——一些用户从自己的经历证实了文档和 UI 问题，而其他人则质疑这是真正的举报者还是怀恨在心的前员工。一位评论者称这篇文章过于戏剧化。

**标签**: `#cloud-computing`, `#microsoft-azure`, `#whistleblower`, `#tech-industry`, `#platform-quality`

---

<a id="item-8"></a>
## [阿里发布 Qwen3.6-Plus：仅限托管服务，不开放权重](https://qwen.ai/blog?id=qwen3.6) ⭐️ 7.0/10

阿里发布了 Qwen3.6-Plus，这是一款仅通过托管 API 提供服务的新模型（不开放权重），标志着与之前开放权重发布策略的重大转变。该模型在基准测试中与 Claude Opus 4.5 和 Gemini Pro 3.0 进行对比，而非最新版本（Opus 4.6 和 Gemini Pro 3.1）。 与之前的 Qwen 模型不同，Qwen3.6-Plus 未公开其参数数量，也无法以开放权重形式获取。该模型可通过阿里的 Model Studio（需要绑定支付账户）或 OpenRouter（提供免费层级）访问。批评者指出基准测试对比使用了 2 个月前发布的竞争对手旧版本。

hackernews · pretext · Apr 2, 14:28

**背景**: 开放权重模型可以本地下载运行，提供更好的控制和隐私保护，而仅 API 模型则需要将数据发送到供应商云端。阿里的 Qwen 系列此前以发布开放权重模型而闻名，在社区中获得广泛关注。AI 领域的基准测试对比常因使用旧版本而非最新发布而受到批评。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.alibabacloud.com/help/en/model-studio/what-is-qwen-llm">Qwen LLMs - - Alibaba Cloud Documentation Center</a></li>
<li><a href="https://huggingface.co/Qwen">Qwen (Qwen)</a></li>
<li><a href="https://blog.gopenai.com/open-weight-models-vs-api-only-llms-663ad9895ab3">Open-Weight Models vs API- Only LLMs | by Zaina Haider | GoPenAI</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一——部分用户表达不满，认为阿里似乎将较小的开放权重模型用作"广告"，而将具有竞争力的模型仅托管服务化。另一些人为这些对比辩护，认为 AI 开发节奏快（每季度发布新版本），使用过时的基准测试对比选择问题不大。也有实际讨论如何通过 OpenRouter 的免费层级访问该模型。

**标签**: `#AI Models`, `#Qwen`, `#Alibaba`, `#Open Source`, `#LLM Benchmark`

---

<a id="item-9"></a>
## [AMD Lemonade：支持 GPU 和 NPU 的开源本地大语言模型服务器](https://lemonade-server.ai/) ⭐️ 7.0/10

AMD 发布了 Lemonade，这是一款开源的本地大语言模型服务器，支持 GPU 和 NPU 进行文本、图像和音频生成的推理，并获得了 AMD 官方的 ROCm 和驱动依赖支持。 这是 AMD 首款具有全面驱动支持官方推理服务器，可能解决 ROCm 兼容性问题，这些问题历来困扰着 AMD 硬件上的本地大语言模型部署。 Lemonade 支持多种后端，包括 ROCm、Vulkan、CPU、GPU 和 NPU。用户报告在 Strix Halo 设备上使用近一年，不过 NPU 模型/内核仍然是专有的，而非开源的。

hackernews · AbuAssar · Apr 2, 11:04

**背景**: ROCm 是 AMD 的 GPU 编程开源软件栈，类似于 NVIDIA 的 CUDA。NPU（神经处理单元）是用于 AI 推理操作的专用硬件，可将工作负载从 CPU 和 GPU 卸载。该项目定位介于 Ollama 的简洁性和 LM Studio 的功能之间，旨在成为文本、图像和音频模型编排的统一运行时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ROCm">ROCm - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neural_processing_unit">Neural processing unit - Wikipedia</a></li>
<li><a href="https://www.amd.com/en/products/software/rocm.html">AMD ROCm™ Software</a></li>

</ul>
</details>

**社区讨论**: 用户持谨慎乐观态度 - 一位用户报告在 Strix Halo 上成功使用近一年，而其他人质疑 NPU 相比 dGPU 的吞吐量，并指出 NPU 内核的专有性是一个限制。ROCm 在独立 GPU 上的驱动体验仍然参差不齐。

**标签**: `#amd`, `#local-llm`, `#llm-inference`, `#open-source`, `#hardware-acceleration`

---

<a id="item-10"></a>
## [OpenAI 收购 TBPN 播客网络](https://openai.com/index/openai-acquires-tbpn/) ⭐️ 7.0/10

OpenAI 已收购 TBPN（The Business Podcast Network），这是一家专注于人工智能的媒体公司，以播客访谈行业领袖闻名。 此次收购引发了对企业影响媒体独立性的重大担忧。批评者认为，即使出于善意，收购也可能产生隐性的编辑压力，无论是否有任何正式的自主权保证。 TBPN 拥有约 58,200 名 YouTube 订阅者，大多数视频观看量不足 3,000 次，使其成为一个相对较小的媒体渠道。此次收购是在 OpenAI 近期收购 OpenClaw 和 Astral 之后进行的，表明其正在实施更广泛的媒体扩张战略。

hackernews · OpenAI News · Apr 2, 17:26

**背景**: TBPN 作为一个独立播客网络运营，专注于人工智能行业报道，主要采访知名的人工智能研究人员和高管。此次收购是 OpenAI 建立媒体关系和影响人工智能话语权战略的一部分。

**社区讨论**: Hacker News 上的评论者对此次收购表示强烈质疑，质疑 OpenAI 的动机及其对媒体独立性的影响。一些人指出 TBPN 的受众规模相对较小，而其他人则批评他们所认为的公关活动——在更广泛的企业担忧中试图将 OpenAI 描绘成“好人”。

**标签**: `#openai`, `#acquisitions`, `#ai-industry`, `#media`, `#business`

---

<a id="item-11"></a>
## [TGS 在 AWS 上实现地震基础模型近线性扩展](https://aws.amazon.com/blogs/machine-learning/scaling-seismic-foundation-models-on-aws-distributed-training-with-amazon-sagemaker-hyperpod-and-expanding-context-windows/) ⭐️ 7.0/10

TGS 使用 Amazon SageMaker HyperPod 成功实现了基于 Vision Transformer 的地震基础模型(SFM)的分布式训练近线性扩展，将训练时间从 6 个月缩短至仅 5 天，同时扩大了可分析的地震数据量。 这一成果代表了地震成像领域的重大突破，近线性扩展使得训练大规模基础模型变得更加经济高效，为石油天然气勘探提供了更强大的 AI 工具。 该方案基于 Vision Transformer 架构，利用 SageMaker HyperPod 的分布式训练基础设施实现了接近线性的扩展效率，这一技术路线在地震分析领域具有开创性意义。

rss · AWS Machine Learning Blog · Apr 2, 13:30

**背景**: Vision Transformer(ViT)是一种将 Transformer 架构应用于图像处理的深度学习模型，它使用自注意力机制而非卷积操作来捕获图像块之间的全局关系。Amazon SageMaker HyperPod 是 AWS 专为大规模分布式训练设计的基础设施，旨在缩短基础模型的训练时间并提供自动化的集群健康监控和故障恢复能力。地震基础模型用于分析和解释地下地质结构，是石油天然气勘探的关键技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aws.amazon.com/blogs/aws/introducing-amazon-sagemaker-hyperpod-a-purpose-built-infrastructure-for-distributed-training-at-scale/">Introducing Amazon SageMaker HyperPod, a purpose-built ...</a></li>
<li><a href="https://www.geeksforgeeks.org/deep-learning/vision-transformer-vit-architecture/">Vision Transformer (ViT) Architecture - GeeksforGeeks</a></li>
<li><a href="https://aws.amazon.com/sagemaker/ai/hyperpod/">Scale Gen AI Model Development – Amazon SageMaker HyperPod – AWS</a></li>

</ul>
</details>

**标签**: `#distributed training`, `#AWS SageMaker`, `#foundation models`, `#Vision Transformers`, `#machine learning infrastructure`, `#seismic analysis`

---

<a id="item-12"></a>
## [NVIDIA 批量模式 VC-6 将视觉 AI 解码时间缩短 85%](https://developer.nvidia.com/blog/accelerating-vision-ai-pipelines-with-batch-mode-vc-6-and-nvidia-nsight/) ⭐️ 7.0/10

NVIDIA 为 VC-6 视频编解码器引入了优化的批处理模式，将每帧图像的解码时间缩短高达 85%。该公司利用 NVIDIA Nsight Systems 和 Nsight Compute 重新设计了 VC-6 CUDA 实现，以提升批处理吞吐量。 这一优化对部署视觉 AI 系统的机器学习工程师具有重大影响，使周围 Pipeline 阶段（解码、预处理和 GPU 推理）能够跟上快速提升的模型吞吐量。它解决了大规模处理视觉数据的 AI 训练和推理 Pipeline 中的关键瓶颈问题。 NVIDIA 使用 Nsight 分析工具识别了系统和内核级别的约束，以指导 VC-6 解码针对批处理推理和训练工作负载进行扩展所需的架构变更。CUDA 加速的 VC-6 编解码器提供原生多分辨率层级、选择性解码和选择性数据调用，可在减少 I/O 和内存带宽的同时在 GPU 上提供可直接用于 AI 的张量。

rss · NVIDIA Developer Blog · Apr 2, 20:00

**背景**: 视觉 AI Pipeline 由多个阶段组成，包括视频/图像解码、预处理和 GPU 推理。VC-6 编解码器由 NVIDIA 和 V-Nova 开发，专为大规模并行执行而设计，能够自然地映射到 GPU。NVIDIA Nsight Systems 和 Nsight Compute 是分析工具，帮助开发者在系统 和内核级别识别性能瓶颈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/accelerating-vision-ai-pipelines-with-batch-mode-vc-6-and-nvidia-nsight/">Accelerating Vision AI Pipelines with Batch Mode VC-6 and ...</a></li>
<li><a href="https://blockchain.news/news/nvidia-nsight-vc6-batch-mode-85-percent-faster-decode">NVIDIA Nsight Tools Slash Vision AI Decode Times by 85% in ...</a></li>
<li><a href="https://brainai.pro/news/en/2025/09/11/build-high-performance-vision-ai-pipelines-with-nvidia-cuda-accelerated-vc-6/">Build High-Performance Vision AI Pipelines with NVIDIA CUDA ...</a></li>

</ul>
</details>

**标签**: `#vision AI`, `#GPU optimization`, `#NVIDIA`, `#ML pipelines`, `#performance engineering`

---

<a id="item-13"></a>
## [NVIDIA GH200 实现个位数微秒级延迟推理](https://developer.nvidia.com/blog/achieving-single-digit-microsecond-latency-inference-for-capital-markets/) ⭐️ 7.0/10

英伟达宣布其 GH200 Grace Hopper 超级芯片在 STAC-ML 基准测试中实现了 4.61 微秒的 99 百分位延迟，用于资本市场应用中的 LSTM 模型推理，采用了持久 CUDA 内核、绿色上下文分区和预计算等技术。 这一突破表明，通用 GPU 现在可以在超低延迟推理方面 match 或超越 FPGA 和 ASIC 等专用硬件，有可能为竞争激烈的算法交易市场中延迟敏感的贸易公司提供极高性能的获取途径。 基准测试在 Supermicro ARS-111GL-NHR 服务器上针对多个 LSTM 模型尺寸进行。关键优化包括使用持久 CUDA 内核消除内核启动开销、绿色上下文分区减少上下文切换延迟，以及预计算阶段优化推理计算。

rss · NVIDIA Developer Blog · Apr 2, 16:00

**背景**: STAC-ML（Markets）推理基准测试用于测量资本市场应用中 LSTM 模型的延迟——即接收新输入到生成输出之间的时间。具有长短期记忆（LSTM）的深度神经网络广泛用于算法交易中的时间序列预测。历来实现个位数微秒级延迟需要 FPGA 或 ASIC 等专用硬件，但英伟达的 GH200 现在证明通用 GPU 可以达到相当的性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/achieving-single-digit-microsecond-latency-inference-for-capital-markets/">Achieving Single-Digit Microsecond Latency Inference for ...</a></li>
<li><a href="https://blockchain.news/news/nvidia-gh200-microsecond-latency-trading-benchmark">NVIDIA GH200 Hits 4.6 Microsecond Latency in Trading Benchmark</a></li>

</ul>
</details>

**标签**: `#machine-learning`, `#inference-optimization`, `#algorithmic-trading`, `#low-latency`, `#performance`

---

<a id="item-14"></a>
## [微软发布三个新型基础 AI 模型](https://techcrunch.com/2026/04/02/microsoft-takes-on-ai-rivals-with-three-new-foundational-models/) ⭐️ 7.0/10

此次发布标志着微软在生成式 AI 领域的重要能力扩展，以与竞争对手抗衡。从团队成立到模型发布的六个月时间，体现了主要科技公司 AI 开发的快速步伐。 这三个模型涵盖不同模态：用于转录的语音识别、用于音频生成的语音合成，以及用于创建图像的视觉生成。这种多模态方法使微软能够提供更广泛的 AI 产品组合。

rss · TechCrunch AI · Apr 2, 16:48

**背景**: 基础模型是在海量数据上训练的大型 AI 模型，可以适应广泛的任务。它们是创建更专业应用的基础构建块。生成式 AI 应用（如大型语言模型(LLM)）是基础模型的常见例子。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Foundation_model">Foundation model - Wikipedia</a></li>
<li><a href="https://aws.amazon.com/what-is/foundation-models/">What are Foundation Models? - Foundation Models in Generative ...</a></li>
<li><a href="https://www.ibm.com/think/topics/foundation-models">What are foundation models? - IBM</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#AI Models`, `#Foundational Models`, `#Generative AI`, `#Tech Industry`

---

<a id="item-15"></a>
## [Moonlake：通过游戏引擎代理构建多模态因果世界模型](https://www.latent.space/p/moonlake) ⭐️ 7.0/10

Latent Space 播客讨论了 Moonlake，这是克里斯·曼宁和孙凡云提出的新研究方法，通过从游戏引擎引导的代理来构建多模态、交互式且高效的因果世界模型。 这代表了交互式多智能体世界模型的重要进展，通过使智能体能够在游戏引擎环境中学习和模拟复杂的真实世界动力学，可能会推动具身智能的进步。 Moonlake 提出因果世界模型应该是多模态的（处理不同的感官输入）、交互式的（实现智能体与世界的互动）且高效的（计算实用）。该方法从游戏引擎引导智能体，而不是从头开始训练。

rss · Latent Space · Apr 2, 17:55

**背景**: 世界模型是学习到的内部表示，用于模拟真实世界动力学并预测环境如何随时间演变。与被动感知模型不同，世界模型是生成式的和预测式的——它们允许智能体在执行行动之前进行规划和推理。这种能力对于具身智能至关重要，智能体必须理解物理世界原理才能有效地与其环境交互。从游戏引擎引导提供了成熟的物理和交互框架，可以加速世界模型的开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.latent.space/p/moonlake">Moonlake: Causal World Models should be Multimodal, Interactive ...</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/world-models/">What Is a World Model? | NVIDIA Glossary</a></li>
<li><a href="https://towardsai.net/p/machine-learning/what-are-world-models">What Are World Models? - Towards AI AI World Models: What Leaders Should Know - WSJ LLMs and World Models, Part 1 - by Melanie Mitchell World Models Are the Next Big Thing In AI. Here’s Why. | Built In World Models | Rohit Bandaru World Models in Artificial Intelligence: Sensing, Learning ...</a></li>

</ul>
</details>

**标签**: `#world-models`, `#causal-ai`, `#interactive-agents`, `#game-engines`, `#ai-research`, `#multimodal`

---

<a id="item-16"></a>
## [Trytet：面向状态化 AI 代理的确定性 WASM 底层平台](https://trytet.com/) ⭐️ 7.0/10

Trytet 是一个可嵌入的亚毫秒级 WebAssembly 底层平台，为状态化 AI 代理提供零信任执行、确定性状态捕获（通过线性内存快照，可导出为.tet 二进制文件）以及 P2P 代理迁移功能。 这解决了 AI 代理的关键挑战：非验证主机执行的安全风险、流式嵌入的 HTTP 开销，以及 API 速率限制或上下文边界导致的执行线程丢失。它支持将代理直接迁移到边缘节点以实现最低延迟。 Trytet 通过即时评估 volatile 机器生成代码来消除 Docker 初始化延迟。其 Context Router 实现了一个 O(N)滑动窗口估计器，可在没有原始内存开销的情况下对 LLM 上下文崩溃施加数学约束。代理可以在执行暂停的确切指令处进行快照、休眠或分支。

rss · Hacker News - Show HN · Apr 2, 23:54

**背景**: WebAssembly (WASM) 是一种基于堆栈的虚拟机的二进制指令格式，可实现接近本机的性能。确定性执行确保可重现的结果，这对状态一致性至关重要的 AI 代理非常重要。WASM 中的线性内存是 WASM 和主机代码都可以访问的连续缓冲区。滑动窗口技术是一种算法优化，将嵌套循环转换为单次遍历，降低时间复杂度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wasmruntime.com/en/tutorials/wasmi">Wasmi In-Depth Tutorial | wasmRuntime.com</a></li>
<li><a href="https://wasmbyexample.dev/examples/webassembly-linear-memory/webassembly-linear-memory.rust.en-us.html">WebAssembly Linear Memory</a></li>
<li><a href="https://builtin.com/data-science/sliding-window-algorithm">Sliding Window Algorithm Explained | Built In</a></li>
<li><a href="https://docs.wasmtime.dev/examples-deterministic-wasm-execution.html">Deterministic Execution - Wasmtime</a></li>

</ul>
</details>

**标签**: `#wasm`, `#ai-agents`, `#deterministic-execution`, `#infrastructure`, `#edge-computing`

---

<a id="item-17"></a>
## [Google 禁止了一款实际控制应用的人工智能代理应用](https://news.ycombinator.com/item?id=47613614) ⭐️ 7.0/10

这揭示了内置移动人工智能助手承诺的功能与实际执行之间的重大差距。它提出了关于应用商店政策、Android 无障碍 API 的预期用途，以及平台限制是否会阻碍人工智能代理技术创新的重要问题。 该应用作为标准 Kotlin 应用完全在设备上运行，无需 root、ADB 或 PC 连接。它将 LLM 输出转换为 X/Y 坐标以在数千种设备分辨率上进行交互。目前支持主要人工智能提供商（OpenAI、Claude、Gemini、Deepseek），采用 BYOK 定价模式，并计划通过 Ollama 和 LM Studio 添加本地模型支持。

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Apr 2, 12:35

**背景**: Android 无障碍 API 最初旨在帮助残障用户通过屏幕阅读和交互功能来导航设备。Google Play 对其使用有严格限制，以防止恶意自动化——应用必须真正为残障用户服务，而不仅仅是为了方便而使用该 API。像 Gemini 这样的内置助手受到平台限制和沙盒安全政策的约束，无法进行深度应用集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/android/treeview-in-android-with-example/">TreeView in Android with Example - GeeksforGeeks</a></li>

</ul>
</details>

**标签**: `#mobile AI`, `#Android`, `#AI agents`, `#Google Play Store`, `#accessibility API`

---

<a id="item-18"></a>
## [用户起诉 Anthropic 未经授权使用其人格](https://www.lesswrong.com/posts/zuAfLrApKg4CExzTw/i-m-suing-anthropic-for-unauthorized-use-of-my-personality) ⭐️ 7.0/10

该诉讼提出了 AI 模型是否可以在未经同意的情况下复制或模仿个人人格的问题。从消息来源几乎没有关于具体诉求或所谓人格特征的详细信息。 这场诉讼触及 AI 模型训练中关于同意和归属的新兴法律问题。如果胜诉，可能为 AI 公司如何处理人格权树立先例，可能需要建立新的同意机制和归属框架。

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Apr 2, 06:00

**背景**: 公开权是一种法律概念，保护个人身份免受未经授权的商业使用。这一权利源自沃伦和布兰代斯的隐私理论，防止对个人肖像或特征的未补偿经济使用。类似案例也出现在 AI 领域，例如 Grammarly 诉讼，该案同样以公开权问题为中心。加利福尼亚州、纽约州和田纳西州长期以来都有关于保护姓名、肖像和形象(NIL)权利的法律。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.globallegalpost.com/news/how-ai-digital-doubles-and-new-laws-are-rewriting-fashion-and-beauty-1113297119">How AI , digital doubles and new laws are... - The Global Legal Post</a></li>
<li><a href="https://aitoolsbee.com/news/right-of-publicity-at-center-of-grammarly-suit-amid-ai-scrutiny/">Right of publicity at center of Grammarly suit amid AI ... - Aitoolsbee</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论显示人们对案件的是非曲直感到好奇，评论者质疑人格如何被定义或版权保护，并指出在法庭上证明此类主张的难度。有些人表示对在这一新颖法律领域取得成功的可能性持怀疑态度。

**标签**: `#AI law`, `#Anthropic`, `#personality rights`, `#AI ethics`, `#intellectual property`

---

<a id="item-19"></a>
## [Cloudflare 用 AI 周末复刻 Next.js 功能，花费 1100 美元](https://www.infoq.cn/article/XNfsebiwgEd1hbcissWd?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Cloudflare 利用 AI 在一个周末内以 1100 美元的成本复刻了 Next.js 功能，完成了通常需要 5 名开发人员工作 6 个月才能完成的工作。目前该方案已部署到生产环境。 这一案例展示了 AI 在软件开发中的变革潜力，可能会重塑传统开发工作流程，显著降低构建复杂功能所需的时间和成本。 该 AI 系统据称在一个周末内完成了相当于 30 人月的开发工作量，代表了显著的生产力提升。部署到生产环境为这种方法增添了可信度。

rss · InfoQ 中文站 · Apr 2, 19:07

**背景**: Next.js 是一个流行的 React 框架，提供服务器端渲染、路由和 API 路由等功能。Cloudflare Workers 是一个无服务器平台，在 Cloudflare 的全球边缘网络上运行代码，使开发者无需管理基础设施即可部署应用程序。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://workers.cloudflare.com/">Cloudflare Workers</a></li>
<li><a href="https://www.antstack.com/guides/cloudflare-workers-explained/">Cloudflare Workers Explained: Your First Step into Serverless Edge...</a></li>

</ul>
</details>

**标签**: `#AI-assisted development`, `#Cloudflare`, `#Next.js`, `#Developer productivity`, `#Production deployment`

---

<a id="item-20"></a>
## [智谱 AI 发布首款多模态编程基础模型 GLM-5V-Turbo](https://docs.bigmodel.cn/cn/update/new-releases) ⭐️ 7.0/10

智谱 AI 发布了首款多模态编程基础模型 GLM-5V-Turbo，原生支持图像、视频、文本等多模态输入，专注视觉编码任务，可完成「理解环境—规划动作—执行任务」的完整 Agent 闭环。 该版本标志着智谱 AI 进入编程 Agent 领域，直接针对 Claude Code 和 OpenClaw 进行优化，在快速增长的 AI 开发者工具市场中展开竞争。该模型的原生视觉编码与 Agent 协同能力填补了当前多模态编程模型的空白。 该模型支持 GUI 自主探索、代码调试、网页复现等复杂任务，并扩展了画框、截图、读网页（含图片识别）等多模态工具链。同期升级的还有 GLM-4-Air/Flash 基座模型、GLM-Z1 系列推理模型及支持多引擎切换的 AI 搜索工具。

telegram · zaihuapd · Apr 2, 01:48

**背景**: 智谱 AI 是一家专注于大模型和多模态 AI 的中国 AI 公司。Claude Code 是 Anthropic 的 AI 编程代理，可在终端运行，以模型与产品的紧密集成著称。OpenClaw 是一个开源个人 AI 助手，拥有 100+内置技能可将 AI 模型连接到应用、浏览器和系统工具。用于编程的多模态基础模型代表了一个新兴前沿领域，将视觉理解与代码生成相结合。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.ai/">Claude.ai</a></li>
<li><a href="https://openclaw.ai/">OpenClaw — Personal AI Assistant</a></li>
<li><a href="https://www.reddit.com/r/ClaudeAI/comments/1p92gdn/claude_code_is_the_best_coding_agent_in_the/">Claude Code is the best coding agent in the market and it's not close</a></li>

</ul>
</details>

**标签**: `#AI`, `#多模态模型`, `#编程Agent`, `#智谱AI`, `#计算机视觉`

---

<a id="item-21"></a>
## [我国首部移动电源安全国标发布，2027 年强制实施](https://news.mydrivers.com/1/1113/1113153.htm) ⭐️ 7.0/10

我国正式发布首部移动电源安全技术规范强制性国家标准（GB 47372-2026），要求电芯必须通过针刺测试、热滥用测试和机械安全试验，严禁使用梯次回收或二手翻新电芯。该标准将于 2027 年 4 月 1 日起强制执行，由工信部归口，华为、小米、OPPO、安克、绿联等三十余家头部企业共同起草。 这被称为“史上最严”充电宝安全标准，旨在解决消费电子市场日益严峻的安全问题。该法规将淘汰使用回收电芯的劣质产品，降低起火爆炸风险，推动行业向更高安全标准迈进，同时促使市场向头部品牌集中。 标准要求电芯通过针刺测试不起火不爆炸，加严热滥用与过充测试，新增整机跌落、挤压等机械安全试验，并强制标注安全使用年限。目前已有 ATL、比亚迪等 28 家电芯企业通过摸底测试。新规预计使行业成本上升 20%至 30%，加速淘汰劣质产能。

telegram · zaihuapd · Apr 2, 02:23

**背景**: 这是我国首部针对移动电源的强制性国标，是消费电子市场的重要配件。該标准建立在电动汽车和电动自行车锂电池安全标准的基础上，针对便携式电源设备的特殊风险。针刺测试是评估锂电池内部短路风险的关键安全测试。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.miit.gov.cn/zwgk/zcjd/art/2025/art_1dc33720e07640428fe4de1d2049075b.html">全国电动自行车安全隐患全链条整治工作专班印发《电动自行车锂离子电...</a></li>
<li><a href="https://www.scribd.com/document/979753770/EVS-04-16e">Nail Penetration Test Standards and Mechanisms | Lithium Ion Battery</a></li>

</ul>
</details>

**标签**: `#consumer-electronics`, `#safety-standard`, `#power-bank`, `#regulation`, `#china`

---

<a id="item-22"></a>
## [英伟达中国 AI 芯片市场份额降至 55%，本土厂商崛起](https://www.tomshardware.com/tech-industry/nvidia-market-share-in-china-falls-to-less-than-60-percent-chinese-chip-makers-deliver-1-65-million-ai-gpus-as-the-government-pushes-data-centers-to-use-domestic-chips) ⭐️ 7.0/10

这一市场转变反映了美国出口管制对英伟达的严重影响，也展示了中国在建设本土半导体生态系统方面取得的进展。英伟达失去主导地位标志着更广泛的地缘政治竞争在先进计算技术领域的体现。 华为以约 81.2 万块领先中国厂商，阿里旗下平头哥以 25.6 万块位居第三，AMD、百度昆仑芯和寒武纪等厂商也有贡献。上周华为发布了 Atlas 350 加速器，声称性能是英伟达 H20 的 2.8 倍，具备 1.56 PFLOPS FP4 算力和最高 112GB HBM。

telegram · zaihuapd · Apr 2, 06:08

**背景**: 美国对华出口先进 AI 芯片的管制政策始于 2022 年，此后多次收紧，限制了英伟达向中国市场出售最强 GPU 的能力。作为回应，中国通过政策倡议推动本土芯片开发，鼓励数据中心采用国产芯片。这符合中国实现半导体自主可控的更广泛目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/gpus/huawei-unveils-new-atlas-350-ai-accelerator-with-1-56-pflops-of-fp4-compute-and-up-to-112gb-of-hbm-claims-2-8x-more-performance-than-nvidias-h20">Huawei unveils new Atlas 350 AI accelerator with 1.56 PFLOPS of ...</a></li>
<li><a href="https://www.uscc.gov/sites/default/files/2024-11/Chapter_3--U.S.-China_Competition_in_Emerging_Technologies.pdf">[PDF] Chapter 3 - U.S.-China Competition in Emerging Technologies</a></li>

</ul>
</details>

**标签**: `#ai-chips`, `#semiconductors`, `#nvidia`, `#huawei`, `#geopolitics`, `#china-tech`

---

<a id="item-23"></a>
## [微软发布 3 款自研 AI 模型直接挑战 OpenAI](https://venturebeat.com/technology/microsoft-launches-3-new-ai-models-in-direct-shot-at-openai-and-google) ⭐️ 7.0/10

微软 4 月 2 日发布了三款完全自研的基础 AI 模型：语音转写模型 MAI-Transcribe-1、语音生成模型 MAI-Voice-1 和图像生成模型 MAI-Image-2，已通过 Microsoft Foundry 和新上线的 MAI Playground 上线。 这标志着微软的战略重大转变——在企业 AI 应用领域定位为独立于 OpenAI 的供应商。通过声称在基准测试中优于 OpenAI 的 Whisper 并实现显著的速度提升，微软直接挑战了 OpenAI 和谷歌在企业 AI 市场的地位。 MAI-Transcribe-1 在 FLEURS 多语言基准测试的 25 种语言上平均词错误率达到 3.8%，全面领先 OpenAI 的 Whisper-large-v3。MAI-Voice-1 可在 1 秒内生成 60 秒语音，并支持用数秒音频定制声音。MAI-Image-2 在 Foundry 和 Copilot 中的生成速度至少提升 2 倍，已开始向 Bing 和 PowerPoint 推出。

telegram · zaihuapd · Apr 2, 11:31

**背景**: FLEURS（少样本学习的通用语音表示评估）是一个覆盖 102 种语言的多语言基准数据集，用于评估语音识别、分类和检索方法。Microsoft Foundry（前身为 Azure AI Studio）是一个统一的企业级 AI 平台即服务产品，使开发者能够构建、优化和治理 AI 应用程序。此次发布标志着微软使用完全自研模型直接竞争，而非依赖 OpenAI 技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/datasets/google/fleurs">google/fleurs · Datasets at Hugging Face arXiv:2501.06117v1 [cs.CL] 10 Jan 2025 - ResearchGate [PDF] Fleurs-SLU: A Massively Multilingual Benchmark for ... FLEURS: FEW-SHOT LEARNING EVALUATION OF UNIVERSAL ... Fleurs-SLU: A Massively Multilingual Benchmark for FLEURS : FEW-SHOT LEARNING EVALUATION OF google/ fleurs · Datasets at Hugging Face FLEURS : FEW-SHOT LEARNING EVALUATION OF Fleurs-SLU: A Massively Multilingual Benchmark for Spoken ...</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/foundry/what-is-foundry">What is Microsoft Foundry? - Microsoft Foundry - Microsoft Learn</a></li>
<li><a href="https://azure.microsoft.com/en-us/products/ai-foundry">Microsoft Foundry</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#AI Models`, `#Speech Recognition`, `#Text-to-Speech`, `#Image Generation`, `#Enterprise AI`

---