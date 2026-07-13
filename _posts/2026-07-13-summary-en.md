---
layout: default
title: "Horizon Summary: 2026-07-13 (EN)"
date: 2026-07-13
lang: en
---

> From 117 items, 13 important content pieces were selected

---

1. [xAI Grok CLI Found Uploading Entire Codebases by Default](#item-1) ⭐️ 9.0/10
2. [Math.tanh() Fingerprinting Reveals OS via Browser](#item-2) ⭐️ 8.0/10
3. [Claude Code sends 33k tokens before reading the prompt; OpenCode sends 7k](#item-3) ⭐️ 8.0/10
4. [World's First Invasive Brain-Computer Interface Medical Device Approved](#item-4) ⭐️ 8.0/10
5. [Migrating Production AI Agent to GPT-5.6: 2.2x Faster, 27% Cheaper](#item-5) ⭐️ 7.0/10
6. [Fields Medalist Terry Tao Builds Apps with LLM Coding Agents](#item-6) ⭐️ 7.0/10
7. [Mechanistic Interpretability Researchers Apply Causality to LLMs](#item-7) ⭐️ 7.0/10
8. [Automation Without Understanding](#item-8) ⭐️ 7.0/10
9. [George Hotz: I Love LLMs, I Hate the Hype](#item-9) ⭐️ 7.0/10
10. [Against Usefulness: A Critique of Tech Industry's Utility Obsession](#item-10) ⭐️ 7.0/10
11. [NeuroVFM: New Neuroimaging Foundation Model with Vol-JEPA](#item-11) ⭐️ 7.0/10
12. [Simon Willison: AI Agents Should Never Be Directly Responsible Individuals](#item-12) ⭐️ 7.0/10
13. [Grok Build CLI Emergency Update Blocks Unauthorized Code Upload](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [xAI Grok CLI Found Uploading Entire Codebases by Default](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547) ⭐️ 9.0/10

Security researchers discovered that xAI's Grok Build CLI tool (v0.2.93) secretly uploads entire codebases including sensitive .env files with API keys to xAI servers by default, even when users explicitly instruct the tool not to access certain files. This represents a major security and privacy violation, exposing developers' intellectual property and credentials. The tool bypasses user instructions and settings, with no way to disable the behavior, fundamentally breaking trust in AI development tools. The tool uses two upload channels: 1) File contents are embedded in model conversation requests and uploaded to Google Cloud Storage buckets; 2) The entire repository is uploaded as a git bundle. In tests with a 12 GB repository, over 5 GiB was successfully uploaded with no storage rejection. The 'improve model' toggle does not prevent uploads.

telegram · zaihuapd · Jul 12, 04:19

**Background**: Grok Build is xAI's official programming CLI tool that helps developers with coding tasks. The git bundle command is a Git feature that packages entire repositories into a single binary file for easy transfer. .env files commonly store API keys, database credentials, and other sensitive configuration data that should never be shared.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build Beta | SpaceXAI</a></li>
<li><a href="https://git-scm.com/docs/git-bundle">Git - git - bundle Documentation</a></li>

</ul>
</details>

**Tags**: `#security`, `#privacy`, `#xAI`, `#AI-tools`, `#data-exfiltration`, `#vulnerability`

---

<a id="item-2"></a>
## [Math.tanh() Fingerprinting Reveals OS via Browser](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 8.0/10

Researchers discovered that Math.tanh() in Chromium 148+ can fingerprint the underlying operating system by exposing differences in math library implementations across different OSes (glibc on Linux, system libraries on macOS, etc.). This represents a novel browser fingerprinting vector that could allow trackers to identify users across sessions even when they change user agents or use privacy-focused browsers like Tor, raising significant privacy concerns for web users. The fingerprinting works because different OSes use different math libraries - Linux typically uses glibc while macOS uses its own system libraries. These differences manifest in NaN canonicalization, SIMD roundings, and specifically Math.tanh, CSS trig functions, and Web Audio implementations. The telltale signatures cluster around ARM-versus-x86 architecture differences.

hackernews · joahnn_s · Jul 12, 21:12

**Background**: Browser fingerprinting is a tracking technique that collects various browser and device characteristics to create a unique identifier for users, even without cookies. Math libraries in different operating systems have subtle implementation differences in floating-point operations, which can be detected through JavaScript functions like Math.tanh(). This vulnerability was introduced or became exploitable in Chromium 148.

<details><summary>References</summary>
<ul>
<li><a href="https://scrapfly.dev/posts/browser-math-os-fingerprint/">Your Browser Does Math Differently on Every OS, and Anti-Bot Systems Read the Bits · scrapfly.dev</a></li>
<li><a href="https://news.ycombinator.com/item?id=48884853">Since Chromium 148, Math.tanh is now fingerprintable to link underlying OS | Hacker News</a></li>

</ul>
</details>

**Discussion**: The discussion reveals mixed sentiments: some commenters criticized Scrapfly's motives, suggesting they profit from fingerprinting yet push for fixes. Others noted this technique could also fingerprint browser version range. A constructive suggestion was to implement correctly rounded transcendental functions as a fix. Commenters also observed that even Tor Browser has abandoned efforts to obscure OS due to the sheer number of fingerprinting vectors.

**Tags**: `#browser-fingerprinting`, `#security`, `#privacy`, `#chromium`, `#web-tracking`

---

<a id="item-3"></a>
## [Claude Code sends 33k tokens before reading the prompt; OpenCode sends 7k](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

A benchmark comparing Claude Code and OpenCode reveals Claude Code sends ~33k tokens before reading the prompt versus OpenCode's ~7k, raising questions about efficiency and cost implications for developers.

hackernews · systima · Jul 12, 18:25

**Tags**: `#AI coding tools`, `#Claude Code`, `#OpenCode`, `#token optimization`, `#developer productivity`

---

<a id="item-4"></a>
## [World's First Invasive Brain-Computer Interface Medical Device Approved](https://t.me/zaihuapd/42515) ⭐️ 8.0/10

China's National Medical Products Administration (NMPA) has approved the world's first invasive brain-computer interface medical device, developed by Boruikang Medical Technology (Shanghai). The NEO system uses epidural minimally invasive implantation and wireless power communication technology to restore hand grip function in quadriplegic patients. This approval marks the first time a brain-computer interface device has entered clinical practice as an officially registered medical device globally, representing a major milestone in BCI technology translation from research to practical healthcare applications and offering new hope for patients with cervical spinal cord injuries. The system is indicated for quadriplegic patients aged 18-60 with cervical spinal cord injuries (C2-C6, grades A-C), at least 1 year post-diagnosis with stable condition for 6 months. It works with a pneumatic glove to assist hand grip function through signals captured via epidural electrodes.

telegram · zaihuapd · Jul 12, 14:39

**Background**: Brain-computer interfaces (BCI) create direct communication pathways between the brain and external devices. Invasive BCI requires surgical implantation of electrodes into the brain tissue or on the dura mater. Epidural implantation offers a middle ground - better signal quality than non-invasive methods while avoiding direct brain tissue damage. Spinal cord injuries at the cervical level often result in quadriplegia, losing hand function even while preserving some arm movement.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tsinghua.edu.cn/info/2063/125128.htm">全球首款侵入式脑机接口医疗器械上市！-清华大学</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/2016611717912744266">何以博睿康？全球首个半侵入式脑机接口医疗器械获批上市的背后</a></li>
<li><a href="https://baike.baidu.com/item/气动手套设备/67672656">气动手套设备 - 百度百科</a></li>

</ul>
</details>

**Tags**: `#brain-computer-interface`, `#medical-devices`, `#neurotechnology`, `#healthcare-innovation`, `#China-regulatory`

---

<a id="item-5"></a>
## [Migrating Production AI Agent to GPT-5.6: 2.2x Faster, 27% Cheaper](https://ploy.ai/blog/migrating-a-production-ai-agent-to-gpt-5-6) ⭐️ 7.0/10

Ploy, an AI agent builder, migrated their production AI agent to GPT-5.6 and achieved 2.2x faster performance and 27% cost reduction while maintaining or improving quality metrics, with other practitioners confirming similar improvements across their workflows. This case study provides concrete production evidence that GPT-5.6 offers significant performance and cost improvements for AI agent workloads, potentially accelerating enterprise adoption of the new model tier and validating the upgrade path for similar deployments. Ploy's agent handles complex website building tasks including planning, code reading, component writing, image generation, and self-evaluation. The migration is described as nearly trivial for many companies. One commenter noted that for varied, tiny, simple workflows, model upgrades are essentially one-line changes regardless of routing architecture.

hackernews · brryant · Jul 12, 17:13

**Background**: GPT-5.6 is OpenAI's latest model release available in three tiers: Sol (flagship 'workhorse' for complex reasoning and coding), Terra (intermediate), and a third tier. Sol is described as OpenAI's 'best coding model yet' suited for agentic workflows. The model was previewed 4 days ago and represents a significant update to the GPT-5 family.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT-5.6 Sol: a next-generation model | OpenAI</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments show mixed sentiment. While improvements are validated by multiple practitioners (thiagoperes confirmed similar gains across classification tasks), some criticize the article's LLM-generated writing style. Concerns were raised about consistency in production agents and whether prompt engineering or tool-calling workflows needed significant changes. One commenter noted that Opus models had held the default slot for four months without being beaten.

**Tags**: `#ai-agents`, `#gpt-5`, `#performance-optimization`, `#production-systems`, `#model-migration`

---

<a id="item-6"></a>
## [Fields Medalist Terry Tao Builds Apps with LLM Coding Agents](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 7.0/10

Renowned mathematician Terry Tao (Fields Medalist) shares his experience using LLM coding agents to build interactive educational visualizations and apps, providing a balanced perspective on their utility for non-mission-critical supplementary tasks. This post matters because it provides a grounded, expert perspective on AI-assisted development from one of the world's most respected mathematicians, offering realistic expectations about what LLM coding agents can and cannot do in software development. Tao emphasizes that LLM-generated visualizations are useful supplements but should not be trusted for mission-critical tasks. He notes the tools excel at rapid prototyping and building supplementary educational tools, but require careful verification for any work that forms part of the core research or educational content.

hackernews · subset · Jul 12, 11:09

**Background**: LLM coding agents are AI tools that can autonomously write, edit, and debug code based on natural language instructions. Tools like Cursor, OpenCode, and Pi represent a new category of AI-assisted development environments. Terry Tao is a Fields Medalist (the highest honor in mathematics) known for his work in number theory, harmonic analysis, and partial differential equations.

<details><summary>References</summary>
<ul>
<li><a href="https://cursor.com/">Cursor: AI coding agent</a></li>
<li><a href="https://opencode.ai/">OpenCode | The open source AI coding agent</a></li>
<li><a href="https://pi.dev/">A terminal-based coding agent</a></li>

</ul>
</details>

**Discussion**: 讨论显示社区对LLM在非关键教育工具方面的价值达成了强烈共识，用户们分享了在课堂上的类似经历。评论从关于专家面临普通技术问题（如Docker调试）的幽默观察，到关于非传统领域软件潜在巨大需求的严肃讨论，不一而足。许多人欣赏陶哲轩的平衡观点——将LLM视为某些任务的有用工具，但不应盲目信任。

**Tags**: `#llm`, `#coding-agents`, `#software-development`, `#ai-tools`, `#terry-tao`

---

<a id="item-7"></a>
## [Mechanistic Interpretability Researchers Apply Causality to LLMs](https://cacm.acm.org/news/can-we-understand-how-large-language-models-reason/) ⭐️ 7.0/10

Researchers are using mechanistic interpretability and causality theory to investigate whether knowledge encoded in neural networks corresponds to reasoning-like concepts through experiments manipulating weights and activations. This research is significant for AI safety and interpretability, as understanding how LLMs internalize and process knowledge could help ensure their reliability and detect potential biases or unsafe behaviors. One notable example is researchers observing a model approaching clock time calculations, demonstrating how specific algorithmic patterns can be identified within neural network weights through careful experimentation.

hackernews · adunk · Jul 12, 18:04

**Background**: Mechanistic interpretability is a subfield of explainable AI that aims to understand the internal workings of neural networks by analyzing their concrete structures, algorithms and circuits. The field faces significant challenges due to the inherent complexity of neural networks, often described as 'parameter spaghetti code'. Some researchers believe it may never fully reduce large language models to simple equations, but it could gradually make hidden algorithms at least partly understandable.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Causal_AI">Causal AI - Wikipedia</a></li>
<li><a href="https://blog.bluedot.org/p/introduction-to-mechanistic-interpretability">Introduction to Mechanistic Interpretability - by Sarah</a></li>

</ul>
</details>

**Discussion**: Community members clarified that the article focuses on mechanistic interpretability research rather than abstract philosophical reasoning, with one commenter noting a 2MP video about the related paper. Some expressed skepticism about whether neural networks can ever be truly understood given their complexity, while others cited Icard's view that this research may 'gradually turn deep neural networks into systems whose hidden algorithms can at least partly be understood.'

**Tags**: `#mechanistic-interpretability`, `#large-language-models`, `#causality`, `#neural-network-analysis`, `#ai-safety`

---

<a id="item-8"></a>
## [Automation Without Understanding](https://arxiv.org/abs/2607.06377) ⭐️ 7.0/10

An arXiv paper titled "Automation Without Understanding" examines the risks of AI automation proceeding without human understanding, sparking community debate about AI explainability, knowledge retention, and the future of human expertise. This matters because it highlights fundamental concerns about AI systems making confidently wrong decisions that only human experts can catch, and the risk that automation may erode human expertise over time by reducing opportunities for people to develop deep domain knowledge. The paper examines how AI systems can produce plausible-sounding but incorrect outputs while appearing confident, and how increasing reliance on AI may prevent new generations from developing the expertise needed to verify and catch AI errors.

hackernews · root-parent · Jul 12, 16:54

**Background**: Explainable AI (XAI) is a field of research focused on making AI decision-making processes transparent and understandable to humans. Knowledge retention in machine learning traditionally refers to a model's ability to maintain performance on previously learned tasks when learning new ones. The community discussion reflects broader concerns about whether AI automation might degrade human expertise, similar to how calculator reliance has been argued to affect mathematical proficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Explainable_artificial_intelligence">Explainable artificial intelligence - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/explainable-ai">What is Explainable AI (XAI)? | IBM</a></li>

</ul>
</details>

**Discussion**: Commenters express concern that AI might not replace experts directly but could prevent the development of future experts by eliminating the learning opportunities that come from doing foundational work. One commenter proposes that AI systems should be required to show their work through formal proofs and execution traces. Others raise philosophical concerns about whether we're approaching a 'singularity' where human knowledge falls below the threshold needed to understand AI systems.

**Tags**: `#ai-safety`, `#automation`, `#machine-learning`, `#knowledge`, `#explainability`

---

<a id="item-9"></a>
## [George Hotz: I Love LLMs, I Hate the Hype](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html) ⭐️ 7.0/10

George Hotz published a blog post discussing his love for LLMs while criticizing AI hype, arguing that frontier AI labs may not capture the value AI creates, and that open-source alternatives are enabling a 'have it your way' era of custom software development. This analysis challenges the trillion-dollar valuations of frontier AI labs by arguing they won't capture the value AI creates. It highlights the growing shift toward private AI deployments and open-source customization, fundamentally changing how developers build software. Frontier labs currently charge $100-200/month subscriptions for bounded token access, but Hotz argues open-source models enable users to run AI privately. Commenters note the 'jagged' quality of LLM-generated software and discuss how the ease of forking open-source projects may undermine traditional upstreaming incentives.

hackernews · therepanic · Jul 12, 18:31

**Background**: George Hotz is a renowned hacker known for jailbreaking iPhone and PlayStation, then founding comma.ai for autonomous driving. Frontier labs refer to companies like OpenAI, Anthropic, and Google leading AI model development. The 'have it your way' era describes a shift where developers can easily fork and customize open-source AI models rather than relying on proprietary APIs.

**Discussion**: Commenters largely agree with Hotz's thesis that frontier labs won't capture AI's value. One discusses running AI privately in their homelab, while another describes building stripped-down one-off software for specific use-cases. Concerns emerge about the future of open source when forking becomes so easy that upstreaming loses its value. Some note the 'jagged' quality of LLM-generated software reflects the technology's limitations.

**Tags**: `#LLMs`, `#AI-hype`, `#open-source`, `#software-development`, `#AI-economics`

---

<a id="item-10"></a>
## [Against Usefulness: A Critique of Tech Industry's Utility Obsession](https://www.motivenotes.ai/p/against-usefulness) ⭐️ 7.0/10

A philosophical essay titled "Against Usefulness" critiques the tech industry's obsession with utility, referencing Bret Victor's Dynamicland research project and questioning where independent thinking has gone in modern technology development. This critique highlights growing concerns about conformity in tech research, where most projects are funded by the same sources and pursue similar goals, potentially stifling exploratory and visionary work that doesn't immediately translate to commercial value. The essay specifically mentions Dynamicland, Bret Victor's Oakland-based research lab known for making entire buildings into collaborative computers, and calls out the lack of 'independent thinkers' in contemporary tech development.

hackernews · supo · Jul 12, 17:47

**Background**: Dynamicland is a unique research project founded by Bret Victor, a renowned interface designer who previously worked at Apple and designed early concepts for the iPad. Unlike traditional computing, Dynamicland transforms entire physical spaces into computational environments where people can collaborate using physical objects and spatial interactions. The project emphasizes exploratory research over immediate commercial applications.

<details><summary>References</summary>
<ul>
<li><a href="https://dynamicland.org/2019/Bootstrapping_Research/">Bootstrapping Research & Dynamicland</a></li>
<li><a href="https://en.wikipedia.org/wiki/Bret_Victor">Bret Victor - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters engaged deeply with the essay's themes. One discussed applying these ideas to mission operations planning, noting the value of richer visual canvases for understanding tactical information. Another critiqued the essay's own use of 'uselessness' argument, noting it still frames projects by their potential usefulness. A third highlighted the stylus as an under-explored input method for more expressive computing that could free users from confined thinking patterns.

**Tags**: `#technology-philosophy`, `#innovation`, `#research-culture`, `#Bret-Victor`, `#independent-thinking`

---

<a id="item-11"></a>
## [NeuroVFM: New Neuroimaging Foundation Model with Vol-JEPA](https://www.marktechpost.com/2026/07/12/meet-neurovfm-a-new-neuroimaging-foundation-model-trained-with-vol-jepa-on-uncurated-clinical-mri-and-ct-volumes/) ⭐️ 7.0/10

University of Michigan researchers developed NeuroVFM, a neuroimaging foundation model trained on 5.24M clinical MRI and CT volumes using Vol-JEPA, a self-supervised approach that extends I-JEPA and V-JEPA to 3D volumetric medical imaging without requiring radiology report labels. This represents a significant advance in medical AI by demonstrating that self-supervised learning can work effectively on large-scale uncurated clinical data without manual annotations. The ability to learn brain anatomy and pathology directly from raw MRI/CT volumes could democratize foundation model development for healthcare institutions lacking annotated datasets. Vol-JEPA根据可见的3D上下文patch预测被遮挡的3D目标patch的表示，学习CT和MRI两种模态的统一潜在空间。该模型在来自临床环境的524万份扫描数据上训练，处理前已去除背景。

rss · MarkTechPost · Jul 13, 00:35

**Background**: JEPA (Joint Embedding Predictive Architecture) is a self-supervised learning method developed by Meta AI and Yann LeCun. Unlike generative methods that reconstruct pixels, JEPA predicts representations in latent space. I-JEPA applies this to images, V-JEPA to videos, and now Vol-JEPA extends this to 3D volumetric medical imaging. Self-supervised learning eliminates the need for expensive manual labeling, which is particularly valuable in medical imaging where expert annotations are scarce and time-consuming to obtain.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2511.18640">Health system learning achieves generalist neuroimaging models</a></li>
<li><a href="https://www.linkedin.com/posts/yann-lecun_neurovfm-a-foundation-model-for-neuroimaging-activity-7481833908603416576-qlbS">NeuroVFM: A foundation model for neuroimaging from the University of...</a></li>
<li><a href="https://github.com/facebookresearch/jepa">GitHub - facebookresearch/jepa: PyTorch code and models for V ... [2506.09985] V-JEPA 2: Self-Supervised Video Models Enable ... Introducing the V-JEPA 2 world model and new benchmarks for ... What Is JEPA? Joint Embedding Predictive Architecture Deep Dive into Yann LeCun’s JEPA | Rohit Bandaru GitHub - facebookresearch/vjepa2: PyTorch code and models for ...</a></li>

</ul>
</details>

**Tags**: `#medical-ai`, `#neuroimaging`, `#foundation-models`, `#self-supervised-learning`, `#volumetric-imaging`, `#machine-learning`

---

<a id="item-12"></a>
## [Simon Willison: AI Agents Should Never Be Directly Responsible Individuals](https://simonwillison.net/2026/Jul/12/directly-responsible-individuals/#atom-everything) ⭐️ 7.0/10

Simon Willison explores the Directly Responsible Individual (DRI) concept from Apple and GitLab, arguing that LLM-powered AI agents should never be designated as DRIs because only humans can truly be held accountable for outcomes. This matters because as AI agents become more autonomous in organizations, clear accountability frameworks become essential. If AI agents cannot be held responsible, humans must retain ultimate accountability for AI-assisted work—raising key questions about AI governance and responsible deployment. The DRI concept originated at Apple and is defined in the GitLab handbook as the person ultimately accountable for the success or failure of a specific project. Willison references IBM's 1979 training slide stating 'A computer can never be held accountable, therefore a computer must never make a management decision.'

rss · Simon Willison · Jul 12, 23:57

**Background**: Directly Responsible Individuals (DRI) is a management concept where one person is designated as ultimately accountable for a project's success or failure. Apple coined the term, and GitLab has codified it in their public handbook. The concept addresses the common organizational problem of diffused responsibility where no one feels truly ownership. As AI agents become more capable of autonomous decision-making, questions arise about whether they can be held accountable in the same way humans can.

<details><summary>References</summary>
<ul>
<li><a href="https://handbook.gitlab.com/handbook/people-group/directly-responsible-individuals/">Directly Responsible Individuals ( DRI ) | The GitLab Handbook</a></li>
<li><a href="https://simonwillison.net/2026/Jul/12/directly-responsible-individuals/">Directly Responsible Individuals ( DRI ) | Simon Willison’s Weblog</a></li>

</ul>
</details>

**Tags**: `#AI accountability`, `#organizational management`, `#AI governance`, `#responsible AI`, `#technology ethics`

---

<a id="item-13"></a>
## [Grok Build CLI Emergency Update Blocks Unauthorized Code Upload](https://www.reddit.com/r/LocalLLaMA/comments/1ut7tis/comment/ox4zamk/?utm_source=share&amp;utm_medium=web3x&amp;utm_name=web3xcss&amp;utm_term=1&amp;utm_content=share_button) ⭐️ 7.0/10

xAI released an emergency update on July 13 to disable code uploading in Grok Build CLI after a security researcher discovered the tool was uploading entire codebases including secret keys to xAI servers by default. 这一事件暴露了使用AI编程助手的开发者面临的重大隐私和安全风险，因为专有代码和密钥（API密钥、密码、.env文件）可能在不知情的情况下被传输到xAI的云基础设施。 The vulnerability allowed Grok Build CLI to upload every tracked file, full git history, and even files the agent never read to a Google Cloud Storage bucket (grok-code-session-traces), regardless of whether the user disabled "Improve the model" settings.

telegram · zaihuapd · Jul 13, 00:52

**Background**: Grok Build is xAI's command-line coding agent powered by Grok 4.5, designed to assist with complex coding tasks. Security researchers can perform wire-level analysis to monitor what data AI tools transmit to remote servers. This incident highlights the importance of auditing AI coding assistants for unintended data exfiltration.

<details><summary>References</summary>
<ul>
<li><a href="https://byteiota.com/grok-build-cli-uploads-repo-xai-servers/">Grok Build CLI Uploads Your Entire Repo to xAI Servers</a></li>
<li><a href="https://github.com/cereblab/grok-build-exfil-repro">GitHub - cereblab/grok-build-exfil-repro: Reproduce it ...</a></li>
<li><a href="https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547">What xAI Grok Build CLI actually sends to xAI - a wire-level analysis...</a></li>

</ul>
</details>

**Discussion**: 安全研究员发布了网络层面证据，证明该CLI正在上传存储库，且与代理实际读取的内容无关。许多开发者表示担忧，因为"改进模型"开关实际上并未阻止数据传输。

**Tags**: `#security`, `#privacy`, `#xAI`, `#Grok`, `#vulnerability`, `#AI tools`, `#code leakage`

---