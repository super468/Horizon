---
layout: default
title: "Horizon Summary: 2026-06-03 (ZH)"
date: 2026-06-03
lang: zh
---

> From 182 items, 21 important content pieces were selected

---

1. [KDE Plasma 宣布最后一个支持 X11 的版本](#item-1) ⭐️ 8.0/10
2. [微软和 NVIDIA 推出 Windows 本地 AI 智能体开发工具](#item-2) ⭐️ 8.0/10
3. [微软发布 AI 智能体行为控制规范](#item-3) ⭐️ 8.0/10
4. [微软发出信号：从操作系统和应用转向 AI 代理平台](#item-4) ⭐️ 8.0/10
5. [英伟达发布 Cosmos 3 开源物理 AI 大模型](#item-5) ⭐️ 8.0/10
6. [llama.cpp b9468 新增实时推理中断控制功能](#item-6) ⭐️ 7.0/10
7. [Kapa.ai 如何利用主动处理为 RAG 索引图片](#item-7) ⭐️ 7.0/10
8. [特朗普签署缩减版人工智能行政令](#item-8) ⭐️ 7.0/10
9. [为什么 systemd 定时器比 Cron 更适合 Linux 自动化](#item-9) ⭐️ 7.0/10
10. [微软发布 ASSERT 开源 AI 行为测试框架](#item-10) ⭐️ 7.0/10
11. [谷歌推出虚假来电检测功能防范 AI 声音伪造诈骗](#item-11) ⭐️ 7.0/10
12. [OpenAI 发布六个针对白领职业的 Codex 工作专用插件](#item-12) ⭐️ 7.0/10
13. [Anthropic 将 Claude Mythos 扩展至 15 个以上国家的关键基础设施](#item-13) ⭐️ 7.0/10
14. [特朗普签署人工智能模型发布前审查行政令](#item-14) ⭐️ 7.0/10
15. [微软发布首款旗舰推理 AI 模型 MAI-Thinking-1](#item-15) ⭐️ 7.0/10
16. [微软发布面向 AI 代理设备的 Project Solara 操作系统](#item-16) ⭐️ 7.0/10
17. [微软发布 MAI-Thinking-1 和 MAI-Code-1-Flash 模型](#item-17) ⭐️ 7.0/10
18. [Datasette-Agent-MicroPython 0.1a0：WebAssembly 沙盒保护的 AI 代理代码执行](#item-18) ⭐️ 7.0/10
19. [Scholar Sidekick - 针对"真 DOI 指向错误论文"的引用验证工具](#item-19) ⭐️ 7.0/10
20. [高德在 AICon 上海展示自动驾驶世界模型](#item-20) ⭐️ 7.0/10
21. [LinkedIn 排查导致系统反复崩溃的内核锁竞争问题](#item-21) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [KDE Plasma 宣布最后一个支持 X11 的版本](https://blog.davidedmundson.co.uk/blog/596/) ⭐️ 8.0/10

KDE Plasma 已宣布即将发布的版本将是最后一个支持 X11 的版本，标志着传统 Linux 显示服务器协议的终结。

hackernews · jandeboevrie · Jun 2, 14:16

**背景**: X11（X 窗口系统）作为 Linux 桌面主要显示协议已有超过 35 年的历史。Wayland 是作为现代替代方案开发的，重点关注安全性和简洁性，但故意省略了 X11 支持的许多功能。Wayland 无障碍协议（wl-a11y）自 2014 年以来一直在开发中，但仍不完整，使得盲人用户无法使用任何基于 Wayland 的桌面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/splondike/wayland-accessibility-notes/blob/main/README.md">wayland-accessibility-notes/README.md at main · splondike/wayland-accessibility-notes</a></li>
<li><a href="https://www.reddit.com/r/linux/comments/1ed0j10/the_state_of_accessibility_is_worse_than_i/">r/linux on Reddit: The state of accessibility is worse than I thought, with progress getting undone every time gtk and qt update, let alone Wayland breaking screen readers.</a></li>
<li><a href="https://lwn.net/Articles/980811/">Accessibility in Wayland [LWN.net]</a></li>

</ul>
</details>

**社区讨论**: 社区成员表达了复杂的感受：一些人赞扬 KDE 流畅的 Wayland 体验并认可单一代码路径的好处，而另一些人则哀悼 X11 功能的丧失并强调严重的无障碍功能退化。一位用户指出，解决无障碍功能问题仍需数年时间。担忧的问题包括缺少窗口位置保存、全屏纵横比校正以及由于安全原因无法使窗口保持在顶层等功能。

**标签**: `#KDE`, `#Wayland`, `#X11`, `#Linux Desktop`, `#Open Source`

---

<a id="item-2"></a>
## [微软和 NVIDIA 推出 Windows 本地 AI 智能体开发工具](https://developer.nvidia.com/blog/build-personal-ai-agents-on-windows-pcs-with-new-tools-from-microsoft-and-nvidia/) ⭐️ 8.0/10

这些工具专为在 Windows 本地运行 AI 智能体而设计，借助 NVIDIA 的 GPU 加速和微软的 Windows 平台集成，实现无需依赖云端的实时 AI 处理。

rss · NVIDIA Developer Blog · Jun 2, 19:00

**背景**: AI 智能体是使用人工智能代表用户执行任务、实现目标的软件系统，具备推理、规划和记忆等能力。边缘计算（或本地 AI/设备端 AI）是指在本地设备上处理数据，而非发送到远程云服务器，这样可以提高响应速度并保护数据隐私。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.google.com/discover/what-are-ai-agents">What are AI agents? Definition, examples, and types</a></li>
<li><a href="https://en.wikipedia.org/wiki/Edge_computing">Edge computing - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#Microsoft Windows`, `#NVIDIA`, `#local AI`, `#edge computing`

---

<a id="item-3"></a>
## [微软发布 AI 智能体行为控制规范](https://techcrunch.com/2026/06/02/microsoft-offers-devs-a-better-way-to-control-ai-agent-behavior/) ⭐️ 8.0/10

该规范通过提供一种标准化方法来定义 AI 智能体被允许或禁止执行的操作，解决了企业 AI 部署中的关键治理和合规挑战，从而加强了安全监督和监管合规性。 ACS 规范被设计为一个可移植的策略框架，可以应用于不同的 AI 智能体实现，使组织能够在其使用的底层智能体技术中保持一致的行为控制。

rss · TechCrunch AI · Jun 2, 18:00

**背景**: AI 智能体是能够代表用户执行任务的自主软件系统，但如果缺乏适当的管理控制，它们可能会表现出违反组织政策或监管要求的行为。企业对 AI 智能体的采用催生了对标准化治理框架的需求，这些框架可以定义可接受的智能体行为，管理对敏感工具和数据的访问，并确保问责制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/06/02/microsoft-offers-devs-a-better-way-to-control-ai-agent-behavior/">Microsoft offers devs a better way to control AI agent ... | TechCrunch</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ai-agents/governance-security-across-organization">Governance and security for AI agents across the organization - Cloud Adoption Framework | Microsoft Learn</a></li>

</ul>
</details>

**标签**: `#AI Agents`, `#Microsoft`, `#AI Governance`, `#Developer Tools`, `#AI Security`

---

<a id="item-4"></a>
## [微软发出信号：从操作系统和应用转向 AI 代理平台](https://9to5mac.com/2026/06/02/microsoft-ceo-were-moving-from-os-and-apps-to-agents-instead/) ⭐️ 8.0/10

微软 CEO 萨提亚·纳德拉宣布，微软正在从传统的操作系统和应用战略性地转向 AI 代理作为新的平台模式，这标志着用户与计算技术交互方式的根本性变革。 这代表着计算行业的一次重大范式转变，可能影响全球数十亿用户，并从根本上颠覆围绕操作系统和生产力应用构建的传统软件商业模式。 根据麦肯锡的分析，这种新范式将人类和 AI 代理联合起来，以接近零边际成本的大规模方式并肩工作，代表着从确定性计算向概率性计算的转变，自然语言作为连接层。

rss · Lobsters - AI · Jun 2, 20:25

**背景**: AI 代理代表了人工智能的范式转变——与其将 AI 模型视为产品，不如将其视为能够规划、行动、观察、反思、使用工具、记忆并迭代直到实现目标的系统。与简单的聊天机器人不同，AI 代理可以自主采取行动来完成跨不同应用和数据源的复杂多步骤任务。这标志着从"会说话的 AI"向"会行动的 AI"的转变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mckinsey.com/capabilities/people-and-organizational-performance/our-insights/the-agentic-organization-contours-of-the-next-paradigm-for-the-ai-era">The agentic organization: Contours of the next paradigm for the AI era</a></li>
<li><a href="https://www.linkedin.com/pulse/why-everyone-talking-ai-agents-what-actually-kim-brian-fn8ff">Why Everyone Is Talking About AI " Agents " (And What They Actually...)</a></li>
<li><a href="https://ki-campus.org/en/blog/agentic-ai">Agentic AI: The New Software Paradigm | AI Campus</a></li>

</ul>
</details>

**社区讨论**: The Lobste.rs discussion shows mixed reactions—some commenters see this as a legitimate and inevitable direction for Microsoft given the rise of agentic AI, while others express skepticism about whether AI agents truly represent a platform shift rather than just another iteration of existing AI capabilities.

**标签**: `#AI Agents`, `#Microsoft`, `#Satya Nadella`, `#Computing Paradigm Shift`, `#Industry Strategy`

---

<a id="item-5"></a>
## [英伟达发布 Cosmos 3 开源物理 AI 大模型](https://www.infoq.cn/article/Ahsy8EcCLj8ESwbkJxu8?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

这一发布代表了行业的重要转变，使全球开发者能够使用先进的物理人工智能能力，并对封闭式竞争对手形成挑战。这种开源方式结合实用工具可能会加速机器 人、自动驾驶和模拟等行业的采用。 Cosmos 3 通过基于世界模型的统一架构，支持文生文、图生图、视频生成和 3D 生成。该模型能够实现零样本任务泛化，让机器人在没有明确编程的情况下处理未见过的场景。

rss · InfoQ 中文站 · Jun 2, 18:44

**背景**: 物理人工智能是指为物理世界交互而设计的人工智能系统，通过传感器和执行器使机器能够理解物理现象并做出决策。传统人工智能模型缺乏机器人所需的物理动力学理解。英伟达与 Agile Robots、Runway、Skild AI、Black Forest Labs、Generalist 和 LTX 等合作伙伴共同成立了 Cosmos 联盟，以构建开放式世界模型生态系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.infoq.cn/article/Ahsy8EcCLj8ESwbkJxu8">英伟达甩出物理AI王炸！ Cosmos 3 全 模 态 模 型 开源，Agent... - InfoQ</a></li>
<li><a href="https://www.mydigit.cn/thread-607327-1-1.html">英伟达推出 全 球首款 全 开源 全 模 态 物理AI大 模 型 Cosmos ...</a></li>
<li><a href="https://www.93913.com/122008.html">英伟达发布 全 球首款 全 开源 全 模 态 物理AI大 模 型 Cosmos 3 – 93913...</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#Artificial Intelligence`, `#Open Source`, `#Physical AI`, `#Machine Learning`

---

<a id="item-6"></a>
## [llama.cpp b9468 新增实时推理中断控制功能](https://github.com/ggml-org/llama.cpp/releases/tag/b9468) ⭐️ 7.0/10

llama.cpp b9468 版本引入了新的 CONTROL 端点（POST /v1/chat/completions/control），支持实时推理中断，允许开发者通过{id_slot, action}参数在大语言模型思考过程中停止生成。该版本还在 WebUI 中添加了推理阶段跟踪功能，通过 isReasoning 标志直观显示模型是否处于思考阶段。 此功能对于实际应用中需要中断长时间运行的推理过程而无需等待完整生成的场景非常重要。它满足了实际需求，允许对 LLM 行为进行精细控制，并通过允许提前终止不需要的思考来改善用户体验，这对于交互式应用至关重要。 CONTROL 端点使用聊天完成 ID（oaicompat_cmmpl_id）而非 slot ID 来避免 TOCTOU 竞态条件。服务器调用 common_sampler_reasoning_budget_force 在推理过程中终止生成。UI 仅在推理阶段（isReasoning 为真时）显示中断按钮，而非整个生成过程期间。

github · github-actions[bot] · Jun 2, 05:53

**背景**: 推理预算是一种令牌限制机制，用于有效管理大语言模型的思考时间。一些较新的 LLM（如 OpenAI o1 和 DeepSeek R1）使用显式推理阶段，模型在给出最终答案之前先产生内部思考。llama.cpp 服务器提供用于 LLM 推理的 REST API，WebUI 则提供基于浏览器的界面与模型交互。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2412.18547v1">Token-Budget-Aware LLM Reasoning</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/blob/master/tools/server/README.md">llama.cpp/tools/server/README.md at master · ggml-org/llama.cpp</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#llm-inference`, `#reasoning-interruption`, `#api-endpoint`, `#open-source`

---

<a id="item-7"></a>
## [Kapa.ai 如何利用主动处理为 RAG 索引图片](https://www.kapa.ai/blog/how-we-index-images-for-rag) ⭐️ 7.0/10

Kapa.ai 采用主动处理（eager processing）为 RAG 索引图片——他们在索引时使用廉价的视觉模型从图像生成文本描述，然后将这些描述作为文本存储，以便在后续检索时与普通文本块一起使用。 这种方法与在查询时使用多模态模型相比大幅降低成本，同时使图像内容可以通过标准文本检索访问。对于处理大量图像内容的 RAG 系统来说，这代表了在成本效率和功能性之间的实用权衡。 该方法遵循媒体摄取的常见“主动处理”模式——预先处理图像而不是按需处理。主要考虑因素包括 LLM 的非确定性（不同模型可能从同一图像中提取不同的信息）以及在图像更改时需要更新描述。

hackernews · mooreds · Jun 2, 16:13

**背景**: RAG（检索增强生成）系统通常检索相关文本上下文来增强 LLM 响应。对于图像，主要存在两种方法：图像 Captioning（将图像转换为文本）和多模态嵌入（将图像和文本映射到共享向量空间）。主动处理预先处理所有数据，而延迟处理则推迟到需要时才处理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://milvus.io/ai-quick-reference/what-is-the-difference-between-image-captioning-and-multimodal-embedding-approaches">What is the difference between image captioning and multimodal ...</a></li>

</ul>
</details>

**社区讨论**: 社区成员普遍支持这种方法，有些人指出他们已经使用了类似的方法多年。提出的担忧包括 LLM 的非确定性（未来模型可能在图像中揭示新信息），以及在源图像更改时保持图像描述更新的挑战。如何处理混合图像文本内容以及描述所需的详细程度仍有疑问。

**标签**: `#RAG`, `#image-retrieval`, `#multimodal-AI`, `#vector-database`, `#knowledge-management`

---

<a id="item-8"></a>
## [特朗普签署缩减版人工智能行政令](https://www.politico.com/news/2026/06/02/trump-signs-downsized-ai-order-00946389) ⭐️ 7.0/10

特朗普总统签署了一份缩减版的人工智能行政令，要求部分人工智能公司在公开发布强大新模型前自愿提交给政府进行 30 天审查（较早期草案中的 90 天有所缩短）。该行政令聚焦于网络安全基准测试，执行机制有限。 这代表了从最初提议的更严格监管到轻触式方法的重大转变。自愿性质意味着效果很大程度上取决于行业合作，批评者认为除了建立一个可用于日后限制人工智能发布的框架外，该行政令缺乏实质内容。 该行政令指示司法部追究滥用人工智能的个人刑事责任。早期草案包含 90 天的自愿审查期，人工智能行业官员认为过于繁重，最终妥协为 30 天窗口。该行政令鼓励开发网络安全性能基准，供开发者选择用于模型评估。

hackernews · _alternator_ · Jun 2, 16:40

**背景**: 该行政令是在特朗普政府与人工智能行业领袖之间数周的反复和谈判后出台的。原本的提案要严格得多，但激烈的行业游说导致强制性要求大幅减少。该行政令代表了现任政府在平衡人工智能创新与国家安全和金融系统风险担忧方面的做法。

**社区讨论**: 社区评论对该行政令的实质性表示怀疑，用户指出第 1 条似乎空洞，第 2 条归结为模糊的网络安全措辞。有些人认为这是未来准入管制的前奏——现在要求自愿审查是为日后强制审批铺路。关于具体审查流程如何运作以及公司是否真的会自愿参与，仍存在疑问。

**标签**: `#AI-regulation`, `#US-government-policy`, `#AI-safety`, `#tech-industry`, `#executive-order`

---

<a id="item-9"></a>
## [为什么 systemd 定时器比 Cron 更适合 Linux 自动化](https://blog.tjll.net/you-dont-love-systemd-timers-enough/) ⭐️ 7.0/10

这一点很重要，因为 cron 作为 Linux 默认的任务调度器已经使用了数十年，但 systemd 定时器解决了长期以来关于系统宕机容错、日志记录和调试的企业自动化工作流痛点。 systemd 定时器在系统重启后可以运行遗漏的任务，而 cron 只在精确计划的时间触发。它们还与 journalctl 集成以实现集中日志记录，并且可以手动触发便于调试。

hackernews · yacin · Jun 2, 09:34

**背景**: 自 2015 年以来，systemd 已成为 Linux 发行版中占主导地位的初始化系统，提供统一的服务管理。定时器是单元文件（.timer），可以在指定的时间间隔触发事件，类似于 cron 但集成在 systemd 生态系统中。虽然 cron 在基本需求上更简单，但 systemd 定时器对系统宕机的容错性更强，并提供更复杂的作业执行控制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wiki.archlinux.org/title/Systemd/Timers">systemd/Timers - ArchWiki</a></li>
<li><a href="https://opensource.com/article/20/7/systemd-timers">Use systemd timers instead of cronjobs | Opensource.com</a></li>

</ul>
</details>

**社区讨论**: HN 上的讨论显示社区对 systemd 定时器表示强烈支持，用户分享了实际案例如备份自动化（Borg）和每周打印机维护以防止喷嘴堵塞。一些人争论关于 cron PATH 歧义的抱怨，指出可以在 crontab 本身中配置。

**标签**: `#systemd`, `#linux`, `#cron`, `#devops`, `#automation`

---

<a id="item-10"></a>
## [微软发布 ASSERT 开源 AI 行为测试框架](https://techcrunch.com/2026/06/02/new-microsoft-tool-lets-devs-spin-up-ai-behavior-tests-using-text-descriptions/) ⭐️ 7.0/10

微软发布了"自适应规范驱动的评估与回归测试"(ASSERT)，这是一个开源框架，允许开发者使用简单的文本描述而非编写代码来创建 AI 行为测试。 该框架解决了 AI 开发中的一个关键需求，通过自动化创建评估测试，可能为开发者节省大量时间，并确保不同模型和代理之间的一致性 AI 行为评估。 ASSERT 利用 AI 将高层次的自然语言目标、政策或预期行为描述转化为详细的、可执行的评分测试，从而验证 AI 模型的响应。

rss · TechCrunch AI · Jun 2, 19:02

**背景**: AI 行为测试对于确保 AI 模型按预期运行并遵守既定策略至关重要。传统上，创建此类测试需要大量的手动工作和编码专业知识。自然语言处理的进步使得可以将文本描述直接转换为自动化评估框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://commandline.microsoft.com/assert-written-intent-executable-evals/">Turn specs into evals for any agent with ASSERT - Command Line</a></li>
<li><a href="https://aitoolly.com/ai-news/article/2026-06-03-microsoft-unveils-open-source-framework-for-ai-behavior-testing-via-text-descriptions">Microsoft Launches Open Source AI Behavior Testing Framework</a></li>

</ul>
</details>

**标签**: `#AI testing`, `#microsoft`, `#open-source`, `#AI evaluation`, `#developer tools`

---

<a id="item-11"></a>
## [谷歌推出虚假来电检测功能防范 AI 声音伪造诈骗](https://techcrunch.com/2026/06/02/google-rolls-out-fake-call-detection-to-protect-against-ai-deepfake-impersonation-scams/) ⭐️ 7.0/10

谷歌推出了虚假来电检测技术，以保护用户免受人工智能语音冒充诈骗的攻击。在这类诈骗中，攻击者会伪装可信电话号码，并利用深度伪造 AI 模仿家人、雇主或权威人士。 这一功能应对了日益严峻的现实威胁，因为诈骗者越来越多地利用人工智能语音合成来欺骗受害者。由于越来越多的人拒绝接听陌生号码的来电，欺诈者现在会伪装熟悉的联系人来绕过信任，使其成为关键的消费者保护工具。 该检测系统分析呼叫元数据和音频模式，以识别伪装和人工智能生成语音的迹象。谷歌将这种保护直接集成到其电话应用程序中，在运营商使用的现有 STIR/SHAKEN 来电验证协议之上增加了重要的一层防御。

rss · TechCrunch AI · Jun 2, 18:00

**背景**: 来电号码伪装允许欺诈者在接收方屏幕上显示伪造的电话号码，使恶意电话看起来来自家人、银行或政府机构等可信来源。STIR/SHAKEN 是一套行业协议，旨在通过确认呼叫者被授权使用所显示的电话号码来验证呼叫者的真实性。与此同时，人工智能语音克隆工具变得越来越普及，只需简短的音频样本就能制作出令人信服的深度伪造语音录音。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/STIR/SHAKEN">STIR / SHAKEN - Wikipedia</a></li>
<li><a href="https://www.fcc.gov/consumers/guides/spoofing">Caller ID Spoofing - Federal Communications Commission</a></li>
<li><a href="https://en.wikipedia.org/wiki/Caller_ID_spoofing">Caller ID spoofing - Wikipedia</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#AI safety`, `#consumer-protection`, `#scam-prevention`, `#Google`

---

<a id="item-12"></a>
## [OpenAI 发布六个针对白领职业的 Codex 工作专用插件](https://techcrunch.com/2026/06/02/openai-launches-new-codex-tools-for-white-collar-work/) ⭐️ 7.0/10

这标志着从通用型人工智能助手向工作专用人工智能工具的重大转变，可能会改变金融、销售和创意产业等多个专业领域知识工作者的运作方式。它可以让白领专业人士更便捷地获取专业技能并提高工作效率。 这六个 Codex 插件针对不同的专业领域：数据分析（用于分析数据集）、创意制作（用于内容创作）、销售（用于客户获取和管理）、产品设计（用于用户体验和功能规划）、股权投资（用于财务分析）和投资银行（用于交易结构设计）。每个工具都设计为在 Codex 应用程序环境中运行。

rss · TechCrunch AI · Jun 2, 16:00

**背景**: Codex 是 OpenAI 的人工智能编程和生产力助手。这些新的工作专用插件代表了 OpenAI 超越通用人工智能、进入专业专业工具领域的战略。该计划针对的是白领知识工作者——这是一个庞大的劳动力群体，虽然人们对人工智能自动化越来越感兴趣，但直到现在还很少有专门针对工作的解决方案。

**标签**: `#OpenAI`, `#Codex`, `#AI tools`, `#productivity automation`, `#white-collar work`

---

<a id="item-13"></a>
## [Anthropic 将 Claude Mythos 扩展至 15 个以上国家的关键基础设施](https://techcrunch.com/2026/06/02/anthropic-scales-claude-mythos-to-critical-infrastructure-in-15-countries/) ⭐️ 7.0/10

Anthropic 正在将其安全漏洞项目 Project Glasswing 和 Claude Mythos 人工智能工具扩展至 15 个以上国家的 150 个组织，重点保护电力、水资源、医疗保健和通信等关键基础设施，这些设施一旦遭受网络攻击可能影响 1 亿人。 这是人工智能在关键基础设施网络安全领域最大规模的实际应用之一，可能影响数百万人的基本服务。 针对电网、水系统、医院和通信网络等脆弱领域的部署，表明人工智能可以被主动用于预防大规模网络事件的发生。 Project Glasswing 于 2026 年 4 月初步面向约 50 个合作伙伴推出，用于测试该模型检测网络安全漏洞的能力。该联盟包括苹果、亚马逊、谷歌、微软、英伟达等行业领导者。

rss · TechCrunch AI · Jun 2, 14:44

**背景**: Project Glasswing 是 Anthropic 的安全项目，汇集了亚马逊网络服务、苹果、思科、CrowdStrike、谷歌、摩根大通、微软、英伟达和 Palo Alto Networks 等主要科技公司，以保护关键软件系统。Claude Mythos 是 Anthropic 开发的最新人工智能模型之一，作为更广泛的 Claude AI 系统的一部分，专为网络安全应用而设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/glasswing">Project Glasswing: Securing critical software for the AI era</a></li>
<li><a href="https://www.cnbc.com/2026/06/02/anthropic-mythos-ai-project-glasswing.html">Anthropic expands Mythos to 150 additional organizations - CNBC</a></li>
<li><a href="https://techcrunch.com/2026/06/02/anthropic-scales-claude-mythos-to-critical-infrastructure-in-15-countries/">Anthropic scales Claude Mythos to critical infrastructure in ...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#critical infrastructure`, `#cybersecurity`, `#Anthropic`, `#Project Glasswing`

---

<a id="item-14"></a>
## [特朗普签署人工智能模型发布前审查行政令](https://www.theverge.com/policy/941775/trump-ai-executive-order) ⭐️ 7.0/10

唐纳德·特朗普总统签署了一项行政令，建立了一个自愿框架，要求人工智能公司在公开发布前与美国联邦机构分享其前沿模型，旨在促进安全创新并加强关键基础设施的网络安全。 行政命令具体针对前沿模型（最先进的人工智能系统），要求公司在发布前与联邦机构分享这些模型，以帮助保护电力网和金融系统等关键基础设施。该框架仍是自愿性的，而非强制性的。

rss · The Verge AI · Jun 2, 18:33

**背景**: 行政令是总统管理联邦政府运作的指令，无需国会批准。前沿模型指目前可用的最先进的人工智能系统。关键基础设施包括社会依赖的电力网、金融网络和电信等基本系统。

**标签**: `#AI policy`, `#US government regulation`, `#executive order`, `#AI governance`, `#technology regulation`

---

<a id="item-15"></a>
## [微软发布首款旗舰推理 AI 模型 MAI-Thinking-1](https://www.theverge.com/tech/941664/microsoft-ai-model-reasoning-mai-thinking-1-build-2026) ⭐️ 7.0/10

在 Build 2026 大会上，微软发布了 MAI-Thinking-1，这是其首款专用推理模型，也是新的旗舰 AI。该模型从头开始训练，未使用蒸馏技术，采用商业许可数据。 MAI-Thinking-1 是一款中型模型，在关键软件工程基准测试中与领先模型相当，并展示先进的数学推理能力。在盲测人类对比评估中，它比 Sonnet 4.6 更受青睐。它与 Copilot Enterprise 捆绑，用于架构审查、迁移规划和事件分析。

rss · The Verge AI · Jun 2, 18:12

**背景**: 微软和 OpenAI 在 2025 年 4 月重新调整了合作伙伴关系，结束了自 2019 年以来定义的独家合作。自 2025 年底以来，Copilot 已开始在 Anthropic 的 Claude、xAI 的 Grok 和微软自己的 MAI 模型之间路由任务。MAI-Thinking-1 专为无法离开数据中心的，企业工作负载而设计，以解决数据隐私问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://microsoft.ai/news/introducing-mai-thinking-1/">Introducing MAI-Thinking-1 | Microsoft AI</a></li>
<li><a href="https://www.neowin.net/news/microsoft-unveils-mai-thinking-1-reasoning-and-mai-code-1-coding-models/">Microsoft unveils MAI-Thinking-1 reasoning and MAI-Code-1 ...</a></li>
<li><a href="https://www.linkedin.com/posts/adumey_msft-openai-restructure-activity-7459958109973667840-kcwg">Microsoft and OpenAI Partnership Restructured, Not Broken | LinkedIn</a></li>

</ul>
</details>

**标签**: `#microsoft`, `#AI models`, `#reasoning AI`, `#MAI-Thinking-1`, `#AI industry`

---

<a id="item-16"></a>
## [微软发布面向 AI 代理设备的 Project Solara 操作系统](https://www.theverge.com/news/941830/microsoft-project-solara-os-ai-agent-gadgets) ⭐️ 7.0/10

微软在 Build 2026 大会上宣布了 Project Solara，这是一款基于 Android 构建的专為 AI 代理设备设计的新操作系统。公司展示了两款概念设备：Desk 概念设备和 badge 徽章设备。 这代表了微软在新兴 AI 设备市场的战略布局，使用 Android 而非 Windows 表明了一种务实的策略来快速抢占这一新品类。随着 AI 代理在决策上变得更加自主，拥有专用操作系统将使微软能够塑造人机交互的未来。 Project Solara 被描述为"一个从根本上构建的全新平台，用于驱动代理驱动的体验。"与传统应用不同，AI 代理（也称为代理 AI）可以自主追求目标、使用工具，并根据推理和规划以不同程度的独立性采取行动。

rss · The Verge AI · Jun 2, 17:31

**背景**: AI 代理代表了一种从传统 AI 应用的转变——虽然传统 AI 专注于完成预定义任务，但代理 AI 系统可以代表用户进行推理、规划和自主决策。微软选择 Android 而非 Windows 作为基础，这务实地表明 Android 广泛的设备生态系统和开发者工具更适合碎片化的 AI 设备市场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://cloud.google.com/discover/what-are-ai-agents">What are AI agents? Definition, examples, and types</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#AI agents`, `#operating systems`, `#artificial intelligence`, `#hardware`

---

<a id="item-17"></a>
## [微软发布 MAI-Thinking-1 和 MAI-Code-1-Flash 模型](https://simonwillison.net/2026/Jun/2/microsofts-new-models/#atom-everything) ⭐️ 7.0/10

这些模型代表了微软在竞争激烈的大语言模型领域推动成本优化解决方案的努力。值得注意的是，活跃参数数量较少（350 亿和 50 亿）使这些模型的运行成本大大低于全规模模型，可能会扰乱数百万开发人员使用的编码辅助工具的价格格局。 MAI-Thinking-1 是一个总参数达一万亿的模型（混合专家架构），活跃参数 350 亿，目前仅向选定的早期合作伙伴开放。MAI-Code-1-Flash 是一个总参数 1370 亿的模型，活跃参数 50 亿。微软的两个公告都声称模型基于“适当许可的干净数据”训练，未从第三方模型蒸馏，尽管技术论文显示它们是基于包括 Common Crawle 在内的网络爬取数据训练的。

rss · Simon Willison · Jun 2, 22:21

**背景**: 总参数与活跃参数的差异涉及混合专家（MoE）架构，在这种架构中，每个推理只激活模型“专家”的子集，使模型更加高效。推理模型是经过优化的大语言模型，可以将复杂问题分解为思维链步骤。Claude Sonnet 4.6 是 Anthropic 的中端模型，在编码、代理和专业工作方面表现出色。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.f22labs.com/blogs/active-vs-total-parameters-whats-the-difference/">Active vs Total Parameters : What’s the Difference?</a></li>
<li><a href="https://www.ibm.com/think/topics/reasoning-model">What Is a Reasoning Model? | IBM</a></li>
<li><a href="https://www.anthropic.com/claude/sonnet">Claude Sonnet 4 . 6 \ Anthropic</a></li>

</ul>
</details>

**社区讨论**: 原报告作者西蒙·威廉森公开纠正了他最初对参数数量的误解——他错误地将活跃参数与总参数混为一谈。他还承认在最初报道中没有深入挖掘训练数据的细节。部分讨论围绕着微软使用“适当许可”的措辞与实际使用网络爬取数据的真相之间的差距展开。

**标签**: `#LLM`, `#Microsoft`, `#AI Models`, `#GitHub Copilot`, `#Code Generation`

---

<a id="item-18"></a>
## [Datasette-Agent-MicroPython 0.1a0：WebAssembly 沙盒保护的 AI 代理代码执行](https://simonwillison.net/2026/Jun/2/datasette-agent-micropython/#atom-everything) ⭐️ 7.0/10

Simon Willison 发布了 datasette-agent-micropython 0.1a0，这是一款 alpha 版本的工具，通过将 MicroPython 编译为 WebAssembly 进行沙盒化，使 Datasette Agent 能够安全地生成和执行 Python 代码。 这解决了 AI 代理系统中的一个关键安全问题——防止 AI 生成的代码从执行沙盒中逃脱并影响主机系统。早期的测试结果表明，GPT-5.5 未能突破沙盒防护。 该工具在 WebAssembly 运行时中运行 MicroPython，提供强大的隔离边界。作为 alpha 版本（0.1a0），它仍是实验性的，但展示了一种将 MicroPython 与 WebAssembly 结合用于安全代码执行的新方法。

rss · Simon Willison · Jun 2, 19:28

**背景**: AI 代理通常需要动态生成和执行代码，如果生成的代码可以访问敏感的系统资源，就会带来安全风险。WebAssembly 提供了具有内存隔离的沙盒执行环境，使其非常适合安全地运行不受信任的代码。MicroPython 是为受限环境设计的轻量级 Python 实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://til.simonwillison.net/webassembly/python-in-a-wasm-sandbox">Run Python code in a WebAssembly sandbox - Simon Willison: TIL</a></li>
<li><a href="https://addozhang.medium.com/ai-agent-code-execution-sandboxes-isolation-from-containers-to-microvms-e80848effea5">AI Agent Code Execution Sandboxes: Isolation from... | Medium</a></li>
<li><a href="https://northflank.com/blog/how-to-sandbox-ai-agents">How to sandbox AI agents in 2026: MicroVMs, gVisor... — Northflank</a></li>

</ul>
</details>

**标签**: `#python`, `#sandboxing`, `#webassembly`, `#datasette`, `#ai-agents`

---

<a id="item-19"></a>
## [Scholar Sidekick - 针对"真 DOI 指向错误论文"的引用验证工具](https://scholar-sidekick.com/tools/citation-verifier) ⭐️ 7.0/10

该工具解决了学术出版中的一个 genuine 且被低估的问题。Topaz 等人估计学术文章中每 277 条引用就有 1 条是伪造的，其中 DOI 可以解析，但指向的是另一篇论文。这直接影响到依赖准确引用进行工作的临床医生、研究人员和学者，防止虚假引用在文献中的传播。 在使用 350 条之前未见过的引用进行测试时，该工具正确识别了所有 37 条伪造引用，同时错误标记了 285 条真实引用中的 5 条（错误率 1.8%，95%置信区间 0.8-4.0%）。该工具将引用中的标题与 DOI 解析器返回的元数据进行比较，但不判断所引用的论文是否支持你的主张。网络版本免费且匿名，REST API 和 MCP 服务器可在 RapidAPI 上获取（有免费套餐），还提供浏览器扩展和 Obsidian 插件。

rss · Hacker News - Show HN · Jun 2, 22:29

**背景**: 引用幻觉指的是看起来可信但实际上是伪造或不准确的 AI 生成引用。Topaz 等人在《柳叶刀》上的研究扫描了 250 万篇 PubMed Central 文章，发现这种模式很常见：一个真实的 DOI 可以正确解析，但指向的是与所引用的完全不同的论文。这类错误特别成问题，因为标识符是有效的，使得手动验证变得困难。此类工具连接 Crossref 的 DOI 元数据 API 来检索论文标题进行比较。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.crossref.org/documentation/retrieve-metadata/rest-api/">REST API - Crossref</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S221462962600191X">Hallucinations in generative AI: A threat to scholarly ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 帖子只有 1 条评论，显示社区参与度非常低。这条单独评论没有提出任何实质性反馈或担忧。

**标签**: `#academic-publishing`, `#citation-verification`, `#research-tools`, `#doi`, `#academic-integrity`

---

<a id="item-20"></a>
## [高德在 AICon 上海展示自动驾驶世界模型](https://www.infoq.cn/article/o8yskfI4cb2msdcz2Pz1?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

该方法强调使用大规模真实时空数据（来自高德导航系统）、端到端演进（从感知到决策的完整流水线训练）和量产实践（可扩展部署）。这使其区别于纯仿真为基础的方法。

rss · InfoQ 中文站 · Jun 3, 10:00

**背景**: 自动驾驶世界模型是学习物理世界运作规律的 AI 系统——预测场景变化和车辆响应方式。它们形成「感知-预测-决策-仿真」全链路技术体系。Waymo 世界模型和高德的 FantasyWorld（获 WorldScore Leaderboard 综合第一）等最新进展表明，业界对该技术用于创建训练数据和仿真场景的兴趣日益增长。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.csdn.net/Bonaventure/article/details/155980214">自动驾驶世界模型核心成果、论文代码与最新进展全景解析_智驾感知模型...</a></li>
<li><a href="https://news.aibase.com/zh/news/24463">高德FantasyWorld一经发布就登顶世界模型榜首，阿里空间智能再下一城...</a></li>

</ul>
</details>

**标签**: `#autonomous-driving`, `#world-models`, `#computer-vision`, `#end-to-end-learning`, `#AI-conference`

---

<a id="item-21"></a>
## [LinkedIn 排查导致系统反复崩溃的内核锁竞争问题](https://www.infoq.cn/article/Z1dyOAN4lXUys1CNAzBK?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

LinkedIn 工程师分享了如何发现并排查导致系统反复崩溃的内核级锁竞争问题的技术实践过程。排查发现，根本原因是一次约 3.5 GB 的大规模内存分配，导致 mmap_lock 信号量在内核级被锁定，从而阻塞了所有线程。 mmap_lock 是内核信号量，任何修改进程虚拟地址空间的操作（如大规模 mmap 分配）都必须以写模式持有此锁。当一个线程执行 3.5 GB 内存分配持有该锁时，所有其他尝试修改虚拟地址空间的线程都会被阻塞，可能导致系统范围的死锁和崩溃。

rss · InfoQ 中文站 · Jun 2, 19:03

**背景**: 内核锁竞争发生在多个线程竞争同一同步原语时。mmap_lock 专门保护 Linux 中进程的虚拟内存映射。当一个线程长时间持有此锁（如在大内存分配期间），其他请求虚拟内存操作的线程就会被阻塞，在内核层面造成拒绝服务状态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.infoq.cn/article/Z1dyOAN4lXUys1CNAzBK">LinkedIn 如何发现导致系统反复死机的内核锁竞争问题 - InfoQ</a></li>
<li><a href="https://blog.csdn.net/qq_44378083/article/details/147376192">高并发下锁竞争排查与优化全攻略：从定位到落地的5步实战法_锁竞争怎...</a></li>
<li><a href="https://geek-blogs.com/blog/linux-debug-kernel/">Linux 内核调试完全指南：从工具到实战 — geek-blogs.com</a></li>

</ul>
</details>

**标签**: `#锁竞争`, `#内核调试`, `#系统可靠性`, `#性能优化`, `#生产故障排查`

---