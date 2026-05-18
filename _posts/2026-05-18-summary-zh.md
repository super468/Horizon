---
layout: default
title: "Horizon Summary: 2026-05-18 (ZH)"
date: 2026-05-18
lang: zh
---

> From 129 items, 11 important content pieces were selected

---

1. [Semble：代码搜索工具，token 消耗比 grep 减少 98%](#item-1) ⭐️ 8.0/10
2. [原生 iOS 文本编辑：TextKit 2 性能与 SwiftUI 局限性对比](#item-2) ⭐️ 8.0/10
3. [长鑫科技递交科创板 IPO 申请，营收同比增长 719%](#item-3) ⭐️ 8.0/10
4. [极客在 80 美元 RK3562 平板电脑上运行 Debian 系统](#item-4) ⭐️ 7.0/10
5. [伊波加因临床试验显示有望治疗退伍军人 PTSD](#item-5) ⭐️ 7.0/10
6. [理解 TCP ECONNRESET 连接重置问题](#item-6) ⭐️ 7.0/10
7. [AI 是技术而非产品](#item-7) ⭐️ 7.0/10
8. [GDS 建议公共部门代码默认保持开源](#item-8) ⭐️ 7.0/10
9. [arXiv 新規：作者若完全使用 AI 寫論文將被禁一年](#item-9) ⭐️ 7.0/10
10. [Zero：Vercel 推出的面向 AI 智能体的新系统编程语言](#item-10) ⭐️ 7.0/10
11. [民调显示公众对 AI 技术的抵制情绪日益增长](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Semble：代码搜索工具，token 消耗比 grep 减少 98%](https://github.com/MinishLab/semble) ⭐️ 8.0/10

Stephan 和 Thomas 开源了 Semble，这是一款面向 AI 代理的代码搜索工具，结合了静态 Model2Vec 嵌入（potion-code-16M）与 BM25，通过 RRF 融合并使用代码感知信号重排序，在 CPU 上完全运行，实现了相比 grep 减少 98%的 token 消耗。 这非常重要，因为像 Claude Code 这样的 AI 编码代理在直接查找代码失败时经常回退到 grep，消耗大量 token 却常常仍然遗漏相关代码。Semble 提供了一个 token 高效的替代方案，在无需 GPU 或 API 密钥的情况下保持接近 transformer 级别的精度。 在涵盖 63 个仓库和 19 种语言的约 1250 个查询/文档对的基准测试中，Semble 达到 0.854 NDCG@10，检索质量达到 137M 参数代码训练 transformer 的 99%，同时快约 200 倍。在 CPU 上索引一个典型仓库需要约 250ms，查询处理仅需约 1.5ms。

hackernews · Bibabomas · May 17, 15:37

**背景**: Model2Vec 是一种将句子 transformer 转换为紧凑静态嵌入模型的技术，通过计算每个 token 的固定向量并对其求平均来生成句子嵌入。BM25（最佳匹配 25）是信息检索中用于根据词频和文档长度归一化来估计文档相关性的排序函数。Reciprocal Rank Fusion（RRF）将多个排名结果集合并为一个统一的相关性优化列表，无需调优。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/MinishLab/model2vec">GitHub - MinishLab/model2vec: Fast State-of-the-Art Static ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Okapi_BM25">Okapi BM25 - Wikipedia</a></li>
<li><a href="https://www.elastic.co/docs/reference/elasticsearch/rest-apis/reciprocal-rank-fusion">Reciprocal rank fusion</a></li>

</ul>
</details>

**社区讨论**: 社区成员提出了关于模型信任问题的重要担忧——经过大量强化学习依赖 grep 的代理可能不信任替代工具的结果，会不断重试或重新读取，可能导致 token 节省付诸东流。还有一些问题将 Semble 与 LSP、colgrep 和 RTK 进行比较，并请求提供实际的代理基准测试而不仅仅是检索指标。一些用户指出，语义代码搜索对人类开发者也可能很有用，而不仅仅是针对代理。

**标签**: `#AI-coding-assistants`, `#code-search`, `#open-source`, `#token-optimization`, `#Model2Vec`

---

<a id="item-2"></a>
## [原生 iOS 文本编辑：TextKit 2 性能与 SwiftUI 局限性对比](https://justsitandgrin.im/posts/native-all-the-way-until-you-need-text/) ⭐️ 8.0/10

一场技术讨论探讨了为何 iOS 原生开发在文本编辑方面仍然面临挑战，尽管 TextKit 2 取得了令人印象深刻的性能基准测试结果，评论者分享了实际指标，显示按键处理在 8 毫秒内完成，20 次快速按键在 150 毫秒内完成。 TextKit 2 实现了比全文档样式快 25 倍的可见范围渲染，标签和布尔搜索在 20 毫秒内完成。然而，一旦开发者需要富文本、选择处理、流式更新、语法高亮、差异对比或平滑滚动等功能，他们最终会陷入与 SwiftUI 的搏斗而非构建应用。

hackernews · dive · May 17, 11:49

**背景**: TextKit 是 Apple 的 iOS 和 macOS 文本渲染框架，TextKit 2 是完全重新设计以满足现代计算需求。SwiftUI 是 Apple 的声明式 UI 框架，但它底层包装了 UITextView/NSTextView，若不进行转换则无法正确识别 SwiftUI 的.Font。Tree-sitter 是一种解析器工具，用于代码编辑器中的语法高亮。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.apple.com/library/archive/documentation/StringsTextFonts/Conceptual/TextAndWebiPhoneOS/CustomTextProcessing/CustomTextProcessing.html">Using Text Kit to Draw and Manage Text</a></li>
<li><a href="https://fatbobman.com/en/posts/a-deep-dive-into-swiftui-rich-text-layout/">A Deep Dive into SwiftUI Rich Text Layout - Beyond AttributedString...</a></li>
<li><a href="https://cindori.com/developer/building-rich-text-editor">Building a rich text editor for UIKit, AppKit and SwiftUI</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为 TextKit 2 提供了卓越的性能，msephton 分享了处理 5000 行文件的生产级文本编辑器基准测试。然而，pornel 认为浏览器渲染引擎已经随着 GPU 加速而成熟，而 instagary 指出在 SwiftUI 中构建富文本功能很快就会变成与框架搏斗。Wowfunhappy 建议 WebKit 适用于 macOS 上的 Markdown 视图。

**标签**: `#ios-development`, `#swiftui`, `#performance`, `#textkit`, `#mobile-engineering`

---

<a id="item-3"></a>
## [长鑫科技递交科创板 IPO 申请，营收同比增长 719%](https://api3.cls.cn/share/article/2373399?os=android&amp;sv=8.7.8&amp;app=cailianpress) ⭐️ 8.0/10

长鑫科技向上交所递交科创板 IPO 招股说明书，披露 2026 年一季度营收 508 亿元，同比增长 719.13%，净利润 330.1 亿元。公司预计 2026 年上半年营收将达 1100 亿至 1200 亿元，扣非归母净利润 520 亿至 580 亿元。 这是中国本土 DRAM 产业的重大进展，长鑫科技作为国内领先的存储芯片制造商寻求上市。惊人的财务数据反映出全球 DRAM 持续供不应求的局面——仅 2026 年一季度 DRAM 价格就上涨了 80%至 90%，标志着全球存储器市场格局发生重大转变。 公司实现彻底扭亏为盈，2025 年亏损状态下 2026 年一季度扣非归母净利润达 263.4 亿元。归母净利润为 247.6 亿元。2026 年上半年营收预计同比增长 612%至 677%。行业分析显示，全球 DRAM 供不应求的局面预计将延续至 2027 年第四季度，存储器市场将迎来超级周期。

telegram · zaihuapd · May 17, 11:05

**背景**: 科创板是于 2019 年推出的中国版纳斯达克科技板块，旨在支持国内科技创新和高科技制造业。DRAM（动态随机存取存储器）是数据中心和消费电子设备使用的关键易失性存储器。当前 DRAM 短缺源于 AI 驱动的 HBM 需求挤占传统 DDR 产能，加上服务器换机周期和 SSD 需求增长，这是三十年来最严重的供应紧缺。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/上海證券交易所科創板">上海证券交易所科创板 - 维基百科，自由的百科全书</a></li>
<li><a href="https://t.cj.sina.com.cn/articles/view/7746897562/1cdc0469a00101biy0">2025-2026年全球DRAM市场涨价趋势及原因分析__财经头条__新浪财经</a></li>
<li><a href="https://finance.sina.com.cn/money/fund/jjgsgd/2026-05-13/doc-inhxtzpe0720799.shtml">DRAM缺口或延续至27年四季度！芯片存储超级周期如何布局？_新浪财经_新浪网</a></li>

</ul>
</details>

**标签**: `#IPO`, `#半导体`, `#DRAM`, `#科创板`, `#财报`

---

<a id="item-4"></a>
## [极客在 80 美元 RK3562 平板电脑上运行 Debian 系统](https://github.com/tech4bot/rk3562deb) ⭐️ 7.0/10

一位创客成功将 80 美元的 RK3562 安卓平板电脑转换为 Debian Linux 工作站，展示了预算型 ARM 硬件可以运行完整的 Linux 桌面环境。 这个项目展示了将低成本安卓设备重新改造成功能性 Linux 工作站的潜力，使计算更加普及，并为预算有限的硬件黑客教育提供了可能。 RK3562 是瑞芯微的四核 ARM 处理器，该平板电脑配备 4GB 内存。社区成员指出，在仅 4GB 内存的情况下，用户应该预期有限的网页浏览（少数标签页），并可能受益于轻量级桌面环境，如 WezTerm 加上 tmux。

hackernews · tech4bot · May 17, 13:16

**背景**: RK3562 是瑞芯微生产的高性能、低功耗四核应用处理器，常用于预算型安卓平板电脑。Debian 是一个以稳定性和广泛硬件支持而闻名的热门 Linux 发行版。在 ARM 设备上运行 Debian 使用户能够将旧设备或预算型硬件重新用于开发和计算任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://datasheet4u.com/datasheet/Rockchip/RK3562-1543273">RK3562 - high-performance and low-power quad-core application processor | Rockchip Datasheet</a></li>
<li><a href="https://armbian.com/">Armbian — Optimized Linux for 300+ ARM Boards</a></li>

</ul>
</details>

**社区讨论**: 社区成员讨论了 4GB 内存下的实际可用性，建议使用 WezTerm + tmux 等轻量级解决方案。一位评论者询问如何使用 AI 进行逆向工程以帮助将 postmarketOS 移植到新设备。另一位则指出，如果这类技术流行起来，可能会导致价格上涨，并指出 Doogee U10 平板电脑已经变得稀缺。

**标签**: `#linux`, `#hardware-hacking`, `# ARM`, `#debian`, `#embedded-systems`

---

<a id="item-5"></a>
## [伊波加因临床试验显示有望治疗退伍军人 PTSD](https://www.bbc.com/future/article/20260514-how-hallucinogenic-ibogaine-helps-veterans-overcome-ptsd) ⭐️ 7.0/10

针对退伍军人的临床试验表明，从非洲灌木伊波加中提取的致幻化合物伊波加因可能为 PTSD 提供新的治疗方法。该药物主要作用于κ-阿片受体(KOR)而非μ-阿片受体(MOR)。 这很重要，因为 PTSD 影响着美国约 4%的男性和 8%的女性(每年)，而目前治疗选择有限。如果证明安全有效，伊波加因可以满足退伍军人和其他难治性 PTSD 患者的紧急医疗需求，代表着迷幻医学领域的潜在突破。 伊波加因在μ-阿片受体上作为弱激动剂，但主要激活κ-阿片受体，可能在不产生快感的情况下减少对阿片类药物的渴求。然而，伊波加因与多例死亡相关，包括在临床试验中医疗监督下发生的病例，原因是其直接作用于心脏系统的副作用。

hackernews · bushwart · May 17, 12:03

**背景**: 伊波加因是一种精神活性生物碱，通过与多种神经递质系统相互作用展示复杂的药理学特性，包括阿片受体、血清素受体、σ受体、NMDA 受体和烟碱乙酰胆碱受体。其代谢物 noribogaine 主要作为血清素再摄取抑制剂和κ-阿片受体激动剂。自 1960 年代以来，伊波加因一直被研究用于治疗阿片成瘾，曾在某些国家商业销售，后因安全问题而受到限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ibogaine">Ibogaine - Wikipedia</a></li>
<li><a href="https://www.mindscaperetreat.com/news/ibogaine-clinical-trials-fda-2026">Ibogaine Clinical Trials & FDA Status in 2026: What Patients ...</a></li>
<li><a href="https://ibogainetreatmentguide.com/how-ibogaine-works/">How Ibogaine Works: Neuroscience, GDNF, & Mechanism of Action ...</a></li>
<li><a href="https://www.roothealing.com/post/unraveling-ibogaines-mechanisms-of-action-a-neuropharmacological-perspective">Unraveling Ibogaine's Mechanisms of Action: A ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论提出了重要的安全隐患关切，指出即使在医疗监督下的临床试验环境中也有死亡事件发生。批评者认为，从μ-阿片受体切换到κ-阿片受体可能只是用一种阿片类药物替代另一种，而非真正治疗成瘾。还有人质疑编辑选择关注退伍军人而非其他主要 PTSD 群体(如性侵害幸存者)，认为该治疗可能使更广泛的人群受益。

**标签**: `#PTSD`, `#ibogaine`, `#psychedelic-medicine`, `#veterans`, `#clinical-trials`

---

<a id="item-6"></a>
## [理解 TCP ECONNRESET 连接重置问题](https://movq.de/blog/postings/2026-05-05/1/POSTING-en.html) ⭐️ 7.0/10

一篇技术博客文章深入调查了 TCP ECONNRESET 错误，探讨了 RST 和 FIN 数据包行为的差异、 lingering close 模式，以及 Go 语言中连接复用问题的实用调试技巧。 调查引用了 Linux 内核代码，其中提及 RFC 2525 第 2.17 节，该节规定当数据丢失时应发送 RST 数据包而非采用优雅的 FIN 终止。博客还讨论了 lingering close 模式，并指出如果不读取 HTTP 响应体就关闭，Go 将无法复用连接。

hackernews · zdw · May 17, 17:09

**背景**: ECONNRESET 是一个 Unix/Linux 错误，表示 TCP 连接被远端发送 RST 数据包强制关闭。与执行优雅 4 次握手关闭的 FIN 不同，RST 会立即终止连接而不确认剩余数据。Lingering close 模式涉及在发送数据后调用 shutdown(SHUT_WR)，然后在关闭 socket 前排空传入数据，以避免产生不必要的 RST 数据包。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.baeldung.com/cs/tcp-fin-vs-rst">TCP: Differences Between FIN and RST - Baeldung</a></li>
<li><a href="https://ipwithease.com/tcp-fin-vs-rst-packets/">TCP FIN vs RST Packets: Know the Difference - IP With Ease</a></li>

</ul>
</details>

**社区讨论**: The community comments highlight that the RST behavior is specified in RFC 2525 section 2.17 to avoid long wait times from graceful FIN closure. One commenter shared a similar Go debugging experience where discarding the HTTP response body prevented connection reuse—likely the same RST behavior occurred under the hood. Another suggested reading Apache's documentation on lingering close for additional context.

**标签**: `#tcp`, `#networking`, `#socket-programming`, `#debugging`, `#linux-kernel`

---

<a id="item-7"></a>
## [AI 是技术而非产品](https://daringfireball.net/2026/05/ai_is_technology_not_a_product) ⭐️ 7.0/10

这一点之所以重要,是因为它质疑了目前 AI 行业构建独立产品的 prevailing 策略,转而建议 AI 公司应该将技术集成到现有生态系统中,以避免被淘汰。 Gruber 引用了史蒂夫·乔布斯的"从客户体验逆向推导"原则来解释为何苹果没有将 AI 作为独立产品纳入其路线图,因为将技术与产品区分开来是苹果的基因。

hackernews · ch_sm · May 17, 13:11

**背景**: "Dropbox 是功能而非产品"这一论点源于一个观察:Dropbox 没有生态系统,之所以幸存只是因为当时没有类似规模的服务存在。同样,史蒂夫·乔布斯领导下苹果的产品哲学将底层技术与终端产品区分开来,专注于客户体验而非技术本身。

**社区讨论**: 社区大体上认同 Gruber 的评估。评论者指出,苹果理想的 AI 实现应该是让 Siri 能够正常处理日常任务,如设置日历事件或运行快捷指令,而无需使用特定的触发词。其他评论者则与 Dropbox 的生态系统挑战进行类比,警告称 AI 公司必须构建自己的生态系统以变得不可替代,正如目前所有主要 AI 公司都在尝试做的那样。

**标签**: `#AI strategy`, `#product philosophy`, `#Apple`, `#technology vs product`, `#tech industry analysis`

---

<a id="item-8"></a>
## [GDS 建议公共部门代码默认保持开源](https://simonwillison.net/2026/May/17/gds-weighs-in/#atom-everything) ⭐️ 7.0/10

技术博主特伦斯·伊登认为 GDS 的指南是公务员体系中的"重大升级"，他指出虽然内部分歧很常见，但此类争议公开化是极为罕见的。开源社区普遍欢迎 GDS 的立场，认为这是对默认开源原则的权威背书。

rss · Simon Willison · May 17, 15:59

**背景**: Project Glasswing was a security research initiative that discovered vulnerabilities in NHS systems. In response, NHS decided to close access to their open source code repositories—which the community criticized as a disproportionate reaction. The UK Government Digital Service is the central agency responsible for digital services across the UK government, and their guidance carries significant policy weight.

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/May/17/gds-weighs-in/">GDS weighs in on the NHS's decision to retreat from Open Source</a></li>
<li><a href="https://www.periculo.co.uk/cyber-security-blog/project-glasswing-claude-mythos-nhs-cybersecurity">Project Glasswing and Claude Mythos: What AI-Powered ...</a></li>

</ul>
</details>

**社区讨论**: Technology blogger Terence Eden interprets the GDS guidance as a "major escalation" in civil service terms, noting that while internal disagreements are common, it is extremely rare for such disputes to spill over into public. The open source community has largely welcomed the GDS position as an authoritative endorsement of open by default.

**标签**: `#UK Government`, `#NHS`, `#Open Source`, `#Government Digital Service`, `#Cybersecurity`

---

<a id="item-9"></a>
## [arXiv 新規：作者若完全使用 AI 寫論文將被禁一年](https://techcrunch.com/2026/05/16/research-repository-arxiv-will-ban-authors-for-a-year-if-they-let-ai-do-all-the-work/) ⭐️ 7.0/10

arXiv 宣佈了一項新政策，如果作者使用 AI 完成論文的全部工作，他們將被禁止在 arXiv 上發表一年。該政策特別針對在研究論文提交中完全由 AI 替代人類貢獻的情況。 這非常重要，因為 arXiv 是學術界最具影響力的研究預印本存儲庫之一，托管著物理學、數學、電腦科學等領域數百萬篇預印本論文。該政策代表了學術出版領域對 AI 生成內容的明確立場，並可能為其他學術平台和期刊樹立先例。 該政策針對使用 AI 完成論文'全部工作'的情況，這意味著一定程度的人類監督或貢獻仍然是可以接受的。一年的禁令對於依賴 arXiv 在正式同行評審之前快速發表研究成果的研究人員來說是一個重要的威懾。

rss · Hacker News - AI / LLM / Agent · May 18, 01:27

**背景**: arXiv 是由康奈爾大學維護的免費開放獲取預印本存儲庫，研究人員在正式同行評審之前在那裡分享論文。它已成為 STEM 領域快速交流的關鍵平台。GPT-4 等大型語言模型的興起引發了整個學術界關於 AI 在學術寫作和研究誠信中角色的持續討論。

**社区讨论**: 該話題的社區參與度極低，只有 1 個點數和 0 條評論，表明該新聞尚未在 Hacker News 社區引發顯著討論。

**标签**: `#academic-publishing`, `#ai-policy`, `#research-integrity`, `#arxiv`, `#plagiarism`

---

<a id="item-10"></a>
## [Zero：Vercel 推出的面向 AI 智能体的新系统编程语言](https://github.com/vercel-labs/zero) ⭐️ 7.0/10

Vercel Labs 发布了 Zero，这是一门专门为构建轻量级原生 AI 智能体工具而设计的系统编程语言。该语言专注于小型高效智能体系统的开发。 这标志着系统编程语言领域一个罕见的新成员，它针对的是快速增长的 AI 智能体生态系统的专门需求。随着 AI 智能体变得越来越普及拥有一门专门为其打造的语言可能会显著影响开发者构建智能体应用的方式。 Zero 被定位为一门用于构建支撑 AI 智能体的基础设施和工具的「系统语言」，而非用于通用应用开发。它专注于性能、低级控制以及生成适合智能体工作负载的小型二进制文件。

rss · Hacker News - AI / LLM / Agent · May 17, 23:45

**背景**: 系统编程语言如 C、C++、Rust 和 Go 通常用于构建操作系统、编译器和其他底层基础设施。Vercel 以 Next.js 和前端部署工具闻名，如今扩展到 AI 智能体工具领域并推出一门专用语言，这表明智能体生态系统在开发者工具领域日益重要。

**标签**: `#programming-languages`, `#ai-agents`, `#vercel`, `#systems-programming`, `#developer-tools`

---

<a id="item-11"></a>
## [民调显示公众对 AI 技术的抵制情绪日益增长](https://www.axios.com/2026/05/17/ai-backlash-polling-sentiment) ⭐️ 7.0/10

民调显示，相当比例的受访者对 AI 的社会影响表示担忧，包括就业替代、隐私风险以及 AI 发展失控的速度。

rss · Hacker News - AI / LLM / Agent · May 17, 21:23

**背景**: AI 抵制是指公众对人工智能技术日益增长的抵抗和负面看法，通常源于对自动化取代人类工作的恐惧、对 AI 生成虚假信息的担忧以及对技术社会角色的普遍焦虑。这一现象与历史上技术抵制的模式相似，例如早期工业革命时期的卢德主义。了解这些情绪趋势对于开发 AI 产品的公司和制定技术政策的决策者至关重要。

**社区讨论**: The 90 comments on Hacker News reveal engaged debate about AI adoption concerns. Readers discuss the cyclical nature of technology hype and backlash, with many noting that similar negative sentiments eventually gave way to adoption in cases like the internet and smartphones. Others emphasize legitimate concerns about AI safety, job impacts, and the need for thoughtful regulation versus dismissal of the backlash as mere technophobia.

**标签**: `#AI sentiment`, `#public opinion`, `#AI backlash`, `#polling data`, `#technology adoption`

---