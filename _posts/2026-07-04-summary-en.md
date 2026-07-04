---
layout: default
title: "Horizon Summary: 2026-07-04 (EN)"
date: 2026-07-04
lang: en
---

> From 137 items, 15 important content pieces were selected

---

1. [Hugging Face Diffusers v0.39.0 Adds NVIDIA Cosmos 3 for Physical AI](#item-1) ⭐️ 8.0/10
2. [European Parliament Member Hacked with Pegasus Spyware](#item-2) ⭐️ 8.0/10
3. [Anthropic Accuses Alibaba of Largest-Ever AI Distillation Attack](#item-3) ⭐️ 8.0/10
4. [Costco: The Anti-Amazon Warehouse Model](#item-4) ⭐️ 7.0/10
5. [Starlink's Rapid Adoption Across Africa](#item-5) ⭐️ 7.0/10
6. [FreeBSD Kernel Memory Bug Investigation and Fix](#item-6) ⭐️ 7.0/10
7. [PostgreSQL and OOM Killer: Why Ubicloud Uses Strict Memory Overcommit](#item-7) ⭐️ 7.0/10
8. [Anthropic Launches Claude Science AI Workbench for Drug Development](#item-8) ⭐️ 7.0/10
9. [Device Revives Eyes From Dead Donors, Enabling Potential Eye Transplants](#item-9) ⭐️ 7.0/10
10. [Current AI Launches Open Source AI Gap Map](#item-10) ⭐️ 7.0/10
11. [OpenAI Anthropic Develop Custom AI Chips Challenge NVIDIA](#item-11) ⭐️ 7.0/10
12. [Claude Fable 5 Relaunch Disappoints Users with Reduced Performance](#item-12) ⭐️ 7.0/10
13. [Huawei Atlas 350 Launches with Ascend 950PR, 2.87x NVIDIA H20 Performance](#item-13) ⭐️ 7.0/10
14. [Alibaba Orders All Employees to Uninstall Claude by July 10](#item-14) ⭐️ 7.0/10
15. [Atuin AI Outperforms Claude Mythos on CyberGym Benchmark](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Hugging Face Diffusers v0.39.0 Adds NVIDIA Cosmos 3 for Physical AI](https://github.com/huggingface/diffusers/releases/tag/v0.39.0) ⭐️ 8.0/10

Hugging Face released diffusers v0.39.0, featuring NVIDIA's Cosmos 3 as a unified world foundation model for Physical AI. Cosmos 3 combines world generation, physical reasoning, and action generation into a single omni-model using a Mixture-of-Transformers (MoT) architecture, replacing the separate Predict, Reason, and Transfer models from previous releases. This release represents a significant advancement in Physical AI by integrating generation, reasoning, and action capabilities into a single unified model. The MoT architecture enables the model to handle multiple processing strategies for different inputs while maintaining a shared representation space, which could accelerate development of autonomous machines that can perceive and interact with the physical world. The Cosmos3OmniTransformer runs a Qwen-style language model in parallel with a diffusion generation pathway, joined by a 3D multimodal RoPE. This release also includes video-to-video generation, action-conditioned generation, and a sound encoder. Additional new pipelines include Ideogram 4 (flow-matching text-to-image), Krea 2 (single-stream MMDiT), DreamLite (ByteDance text-to-image), and PRX Pixel (pixel-space generation).

github · sayakpaul · Jul 3, 08:55

**Background**: Physical AI refers to AI systems that can perceive, understand, and perform complex actions in the real physical world, connecting digital AI to hardware that senses and executes actions. World Foundation Models (WFMs) are a key component of Physical AI, providing visual understanding of environments through video-based observations. Mixture-of-Transformers (MoT) is an architecture that combines multiple transformer blocks to enable appropriate processing strategies for different inputs while maintaining a shared representation space.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/glossary/generative-physical-ai/">What is Physical AI? | NVIDIA Glossary</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/mixture-of-transformers/">Mixture of Transformers (MoT) Definition & Architecture | NVIDIA</a></li>
<li><a href="https://arxiv.org/html/2501.03575v1?ref=whoisyan.com">Cosmos World Foundation Model Platform for Physical AI</a></li>

</ul>
</details>

**Tags**: `#diffusion-models`, `#physical-ai`, `#nvidia`, `#computer-vision`, `#multimodal-ai`, `#machine-learning`

---

<a id="item-2"></a>
## [European Parliament Member Hacked with Pegasus Spyware](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

Citizen Lab confirmed that European Parliament member Stelios Kouloglou's iPhone was successfully infected with Pegasus spyware on October 21, 2022, and again on March 6-7, 2023, suggesting a European intelligence service was responsible for the attack. This represents a significant abuse of government-grade spyware against an elected EU official, raising serious concerns about democratic surveillance and the rule of law within European member states. The incident highlights how Pegasus has been used to target not just journalists and activists, but also politicians within the EU. The forensic analysis found an overlap between the first infection and a previously identified Pegasus campaign targeting Russian and Belarusian-speaking exiled journalists and activists in Europe. The same device may have compromised both confidential personal medical information and confidential government documents, raising questions about EU Parliament's device separation policies.

hackernews · ledoge · Jul 3, 20:38

**Background**: Pegasus is sophisticated spyware developed by Israeli company NSO Group that can be deployed via zero-click exploits, requiring no user interaction. The Citizen Lab is a research unit at the University of Toronto's Munk School of Global Affairs that specializes in investigating spyware attacks against journalists, politicians, and human rights advocates. Multiple European countries including Greece, Poland, and Italy have faced scandals involving abuse of Pegasus against journalists, politicians, and citizens.

<details><summary>References</summary>
<ul>
<li><a href="https://citizenlab.ca/">The Citizen Lab - The Citizen Lab</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab</a></li>
<li><a href="https://www.kaspersky.com/resource-center/definitions/what-is-zero-click-malware">Zero - Click Exploits</a></li>

</ul>
</details>

**Discussion**: Community commenters noted an overlap with previously identified Pegasus campaigns targeting exiled journalists, and questioned why EU Parliament lacks device separation policies. Some highlighted that similar Pegasus abuses have occurred in Greece, Poland, and Italy, with some Israeli firms cutting ties with European clients due to widespread misuse. There was debate about whether to characterize this as an attack against the European Parliament specifically or part of broader pattern of domestic surveillance.

**Tags**: `#cybersecurity`, `#spyware`, `#pegasus`, `#surveillance`, `#european-parliament`, `#privacy`

---

<a id="item-3"></a>
## [Anthropic Accuses Alibaba of Largest-Ever AI Distillation Attack](https://t.me/zaihuapd/42327) ⭐️ 8.0/10

Anthropic has accused Alibaba of conducting the largest known 'distillation attack' in AI history, alleging the company used approximately 25,000 fraudulent accounts to make 28.8 million interactions with Claude between April 22 and June 5, 2026, to extract the model's capabilities. This represents a significant escalation in AI intellectual property disputes between US and Chinese companies, potentially setting a precedent for how AI model protection is regulated. The scale of the alleged attack (28.8M interactions) dwarfs previous incidents and could impact US-China tech competition dynamics. Anthropic sent a letter to the US Senate Banking Committee detailing the allegations. The attack involved Alibaba and its AI laboratory Qwen. Distillation is a technique where a weaker model learns from a stronger model's outputs to replicate its capabilities.

telegram · zaihuapd · Jul 3, 06:21

**Background**: Model distillation is a legitimate AI training technique where a smaller 'student' model learns to mimic a larger 'teacher' model's behavior and knowledge. When done without authorization, it can constitute intellectual property theft. Alibaba's Qwen is a major Chinese AI model family launched in 2023, originally under the name Tongyi Qianwen, and has become one of the leading open-source AI models in China.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gaussianwaves.com/2025/02/model-distillation-explained-how-deepseek-leverages-the-technique-for-ai-success/">Model Distillation Explained: How DeepSeek Leverages the ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI_IP_theft`, `#Anthropic_Claude`, `#Alibaba_Qwen`, `#US_China_AI_competition`, `#model_distillation`

---

<a id="item-4"></a>
## [Costco: The Anti-Amazon Warehouse Model](https://phenomenalworld.org/analysis/the-anti-amazon/) ⭐️ 7.0/10

An analysis compares Costco's warehouse pickup model to Amazon's home delivery model, highlighting how Costco avoids the last-mile delivery problem by requiring customers to transport goods themselves. This analysis highlights an alternative approach to e-commerce logistics that challenges the prevailing assumption that door-to-door delivery is always superior, showing how physical retail can offer a viable competitor to digital-first competitors. The last-mile delivery problem refers to the complex and expensive final leg of getting packages from distribution centers to customers' doorsteps, which Amazon must solve for every order, while Costco shifts this burden to customers who pick up bulk orders themselves.

hackernews · bookofjoe · Jul 3, 15:14

**Background**: The last-mile delivery problem is widely considered the most complicated and expensive part of e-commerce logistics, often accounting for a significant portion of total delivery costs. Costco operates a warehouse club model where customers pay annual memberships to shop in bulk at physical stores, picking up items directly rather than having them delivered. This model has made Costco one of the largest retailers globally while maintaining relatively low prices.

<details><summary>References</summary>
<ul>
<li><a href="https://onfleet.com/blog/last-mile-problem/">The Last Mile Delivery Problem : Here's How to Solve it</a></li>

</ul>
</details>

**Discussion**: 社区成员讨论了物流权衡问题，部分人质疑鉴于顾客需要开车前往门店，Costco的模式是否真正具有社会价值。另一些人引用工程格言：「智者解决问题，贤者避免问题」，认为Costco的做法体现了设计上的智慧。部分批评了仓储零售的汽车中心主义，而另一些人为其辩护，认为这对于喜欢每月批量购物的郊区消费者来说很实用。

**Tags**: `#retail`, `#business-model`, `#logistics`, `#e-commerce`, `#systems-thinking`

---

<a id="item-5"></a>
## [Starlink's Rapid Adoption Across Africa](https://www.economist.com/middle-east-and-africa/2026/07/02/africans-are-turning-to-starlink) ⭐️ 7.0/10

The Economist reports on Starlink's rapid adoption in Africa, where the satellite internet service is being embraced by populations previously unserved by traditional wired infrastructure. This adoption represents a significant shift in digital access for underserved populations, potentially bridging the digital divide in regions where laying cable or fiber infrastructure is impractical or impossible. Starlink uses low Earth orbit (LEO) satellites, achieving latency of 25-60ms compared to 600ms for traditional geostationary satellite internet. The service costs approximately $55/month in the US and can operate with alternative power sources like car chargers in areas with unreliable electricity.

hackernews · bookofjoe · Jul 3, 21:08

**Background**: Starlink is SpaceX's satellite internet constellation using low Earth orbit satellites to deliver broadband internet to remote locations. Unlike traditional geostationary satellites that orbit at 35,786 km above Earth, Starlink's satellites orbit at 540-570 km, dramatically reducing latency. This technology enables internet access in areas where laying traditional cable or fiber infrastructure is economically unfeasible.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Starlink">Starlink - Wikipedia</a></li>
<li><a href="https://www.satelliteinternet.com/providers/starlink/">Starlink Internet Plans and Cost [2026]</a></li>

</ul>
</details>

**Discussion**: Comments highlight the mission-driven aspect of Starlink, with a former engineer emphasizing its role in bringing internet to unserved populations as an 'equalizer'. South African users explain the severe infrastructure challenges including daily power outages lasting up to 10 hours. Others draw parallels to Africa's mobile phone adoption leapfrogging wired infrastructure, noting Starlink fills a similar gap for rural internet access.

**Tags**: `#Starlink`, `#satellite internet`, `#Africa`, `#digital divide`, `#infrastructure`

---

<a id="item-6"></a>
## [FreeBSD Kernel Memory Bug Investigation and Fix](https://crocidb.com/post/freebsd-ate-my-ram/) ⭐️ 7.0/10

A developer investigated and fixed a FreeBSD kernel bug where unused memory pages in the vm_map subsystem weren't being properly released, causing inflated memory usage reporting. The fixes have been merged upstream. This fix improves memory accounting accuracy in FreeBSD, which is critical for system administrators monitoring resource usage. Accurate memory reporting helps identify actual memory leaks versus healthy caching, and benefits anyone running FreeBSD in production environments. The bug was in the kernel's virtual memory map (vm_map) system, where unused memory pages weren't being properly released back to the system. The developer traced the issue through kernel memory debugging tools and vmstat, identifying where the accounting was incorrect.

hackernews · theanonymousone · Jul 3, 19:08

**Background**: FreeBSD uses a virtual memory subsystem called vm_map to manage kernel virtual address spaces. The zone allocator splits kernel virtual memory (KVM) into constant-sized blocks for different kernel structures. Memory usage can be checked with vmstat -m to see KVM utilization by zone. This bug caused the system to report more memory as 'used' than actually was.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.freebsd.org/en/books/arch-handbook/vm/">Chapter 7. Virtual Memory System | FreeBSD Documentation Portal</a></li>
<li><a href="https://man.freebsd.org/cgi/man.cgi?query=vm_map">vm_map</a></li>
<li><a href="https://forums.freebsd.org/threads/memory-management-freebsd-kernel.84787/">Memory management FreeBSD kernel | The FreeBSD Forums</a></li>

</ul>
</details>

**Discussion**: The community appreciated the quality technical deep-dive, with one commenter thanking the author for the post and another congratulating them on getting the fixes merged. There was also discussion about memory accounting heuristics - one commenter questioned why exact memory accounting requires heuristics rather than precise numbers, noting that 'used memory for the system is always total minus available.'

**Tags**: `#freebsd`, `#debugging`, `#memory`, `#systems-programming`, `#operating-systems`

---

<a id="item-7"></a>
## [PostgreSQL and OOM Killer: Why Ubicloud Uses Strict Memory Overcommit](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 7.0/10

Ubicloud explains their operational decision to use strict memory overcommit (vm.overcommit_memory=2) for PostgreSQL to avoid OOM killer issues in production, though the author later acknowledged the title was too strong and there are scenarios where this approach has side effects. This matters for database administrators and DevOps engineers managing PostgreSQL at scale, as the OOM killer can cause unpredictable database crashes under memory pressure. The discussion highlights real-world tradeoffs between memory overcommit modes. The strict overcommit mode (vm.overcommit_memory=2) enforces hard limits on memory allocation based on actual physical RAM + swap, rejecting allocations that would exceed this threshold. Community members warn this can prevent forks and cause instability when applications allocate large amounts of virtual memory alongside PostgreSQL on the same machine.

hackernews · furkansahin · Jul 3, 13:00

**Background**: Linux memory overcommit is a kernel feature that allows processes to allocate more virtual memory than is physically available. The OOM (Out of Memory) killer is a Linux kernel mechanism that terminates processes when the system runs out of memory. There are three overcommit modes: mode 0 (heuristic, the default), mode 1 (always overcommit), and mode 2 (never overcommit, aka strict mode). Mode 2 can cause malloc() to fail rather than trigger the OOM killer.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kernel.org/doc/html/v6.13/mm/overcommit-accounting.html">Overcommit Accounting — The Linux Kernel documentation</a></li>
<li><a href="https://www.baeldung.com/linux/overcommit-modes">Linux Overcommit Modes | Baeldung on Linux</a></li>

</ul>
</details>

**Discussion**: The discussion shows mixed sentiment - while some agree with the strict overcommit approach for databases, others warn about side effects including preventing forks and system instability. Community member Bender emphasizes testing in QA/Perf environments before production deployment. The author ozgune acknowledges the title was overly strong and that many scenarios could have unanticipated side-effects from strict overcommit.

**Tags**: `#postgresql`, `#linux`, `#memory-management`, `#oom-killer`, `#devops`, `#systems`

---

<a id="item-8"></a>
## [Anthropic Launches Claude Science AI Workbench for Drug Development](https://www.theverge.com/ai-artificial-intelligence/961311/anthropic-claude-science-ai-drug-development) ⭐️ 7.0/10

Anthropic announced Claude Science, a new AI workbench for scientists that consolidates fragmented tools and datasets into one environment for drug development research, and generates figures and visuals. This marks Anthropic's significant expansion into scientific research and drug development, signaling a major AI company's strategic entry into healthcare. The move positions Claude as a competitor to existing scientific research tools and could accelerate pharmaceutical research workflows. Claude Science was announced at 'The Briefing: AI for Science' event. The platform aims to unify the fragmented tool landscape in scientific research, allowing scientists to access multiple datasets and tools in a single interface while automating figure generation.

rss · The Verge AI · Jul 3, 13:56

**Background**: Drug development traditionally involves complex workflows with many disconnected tools and databases. AI companies like Google DeepMind and Microsoft have been increasingly investing in scientific research applications, using machine learning to accelerate molecule discovery, predict protein structures, and optimize clinical trials. Anthropic's entry into this space follows similar moves by competitors.

**Tags**: `#AI`, `#Anthropic`, `#drug development`, `#scientific research`, `#product launch`

---

<a id="item-9"></a>
## [Device Revives Eyes From Dead Donors, Enabling Potential Eye Transplants](https://www.technologyreview.com/2026/07/03/1140148/a-device-that-revives-eyeballs-from-dead-donors-could-make-eye-transplants-possible/) ⭐️ 7.0/10

Researchers have developed a device that can revive eyes from dead donors, potentially making whole eye transplants viable for restoring vision. The device addresses the critical problem of eye degeneration that begins immediately after death. This breakthrough could enable vision restoration for millions of people suffering from irreversible blindness. Whole eye transplants have been attempted before but failed because the transplanted eye could not see—primarily due to optic nerve regeneration challenges. The device maintains and revives eyes from dead donors using perfusion and preservation technology. Similar organ preservation devices like LifePort circulate preservation solutions, oxygenate organs, and maintain appropriate temperatures to prevent degeneration.

rss · MIT Technology Review · Jul 3, 17:34

**Background**: Whole eye transplantation has been a frontier in ophthalmology, promising transformative approaches to irreversible blindness. However, formidable challenges persist, including the need for optic nerve regeneration to restore vision. Previous transplant attempts resulted in eyes that could not see due to degeneration and failed neural connections.

<details><summary>References</summary>
<ul>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11212585/">Whole - eye transplantation : Current challenges and future...</a></li>
<li><a href="https://www.frontiersin.org/journals/medicine/articles/10.3389/fmed.2025.1691259/full">Frontiers | Allogeneic whole - eye transplantation : advancements...</a></li>
<li><a href="https://www.organ-recovery.com/always-listening-always-innovating/">Always Listening, Always Innovating: ORS... - Organ Recovery Systems</a></li>

</ul>
</details>

**Tags**: `#medical research`, `#eye transplant`, `#organ donation`, `#biomedical device`, `#vision restoration`

---

<a id="item-10"></a>
## [Current AI Launches Open Source AI Gap Map](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 7.0/10

Current AI, a non-profit organization backed by $400m in funding, launched the Open Source AI Gap Map v0.1 indexing 421 products across software tools, models, datasets, and hardware categories from 228 organizations. This comprehensive catalog provides a valuable reference for the AI community to understand the open source AI ecosystem's current state, though it's primarily a documentation and cataloging effort rather than a technical breakthrough. The Gap Map categorizes products into 14 categories across 3 stack layers (model components, product/UX, and infrastructure). The underlying data is released under an MIT license on GitHub, including 1,184 YAML files and 16,185 tracked GitHub repositories.

rss · Simon Willison · Jul 3, 22:04

**Background**: Current AI was founded as a non-profit at the AI Action Summit in Paris in February 2025 with a mission to 'build a public option for AI'. The organization has already secured $400m in committed funding. This Gap Map represents their first major public deliverable aimed at mapping the open source AI landscape.

**Tags**: `#open-source-ai`, `#ai-ecosystem`, `#resources`, `#tools`, `#datasets`

---

<a id="item-11"></a>
## [OpenAI Anthropic Develop Custom AI Chips Challenge NVIDIA](https://www.infoq.cn/article/MOqFJbvWYlJ9PXcfdfCC?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

OpenAI and Anthropic are both developing custom AI chips to reduce their reliance on NVIDIA's expensive GPUs. OpenAI announced its custom chip called Jalapeño in partnership with Broadcom, while Anthropic is in early-stage discussions with Samsung Electronics about manufacturing a custom AI chip using 2-nanometer process technology. This represents a direct challenge to NVIDIA's dominant position in the AI chip market, where its GPUs command premium pricing of $30,000-$40,000 per unit for Blackwell chips. If successful, these custom chips could significantly reduce AI infrastructure costs and break NVIDIA's pricing monopoly, potentially reshaping the entire AI hardware ecosystem. NVIDIA's H100 GPU costs up to $40,000, which is approximately four times more expensive than AMD's competing MI300X ($10-$15K). Anthropic has hired Clive Chan from OpenAI's chip division to lead its chip efforts. OpenAI's Jalapeño chip was built in collaboration with Broadcom, marking a significant shift toward custom silicon in the AI industry.

rss · InfoQ 中文站 · Jul 3, 18:00

**Background**: NVIDIA currently dominates the AI chip market with its CUDA ecosystem and high-performance GPUs, making it extremely difficult for competitors to break in. The high cost of NVIDIA GPUs (H100: $27K-$40K, Blackwell: $30K-$40K) has become a significant bottleneck for AI companies seeking to scale their operations. Major tech companies including Google, Amazon, and Microsoft have already developed custom chips, while OpenAI and Anthropic are now following suit to reduce their dependency on a single supplier.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2024/03/19/nvidias-blackwell-ai-chip-will-cost-more-than-30000-ceo-says.html">Nvidia's Blackwell AI chip will cost more than $30,000, CEO says</a></li>
<li><a href="https://www.reddit.com/r/hardware/comments/1ahgu7q/nvidias_h100_ai_gpus_cost_up_to_four_times_more/">r/hardware on Reddit: Nvidia's H100 AI GPUs cost up to four times more than AMD's competing MI300X — AMD's chips cost $10 to $15K apiece; Nvidia's H100 has peaked beyond $40,000: Report</a></li>
<li><a href="https://techcrunch.com/2026/07/02/anthropic-is-discussing-a-new-custom-chip-with-samsung/">Anthropic is discussing a new custom chip with Samsung</a></li>
<li><a href="https://blockonomi.com/anthropic-eyes-custom-ai-chip-development-with-samsung-as-manufacturing-partner/">Anthropic Eyes Custom AI Chip Development with Samsung as ...</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#NVIDIA`, `#OpenAI`, `#Anthropic`, `#Hardware`

---

<a id="item-12"></a>
## [Claude Fable 5 Relaunch Disappoints Users with Reduced Performance](https://www.bleepingcomputer.com/news/artificial-intelligence/claude-fable-relaunch-disappoints-users-with-nerfed-performance/) ⭐️ 7.0/10

Anthropic restored global access to Claude Fable 5 after US export controls were lifted, but users report significantly reduced experience including 50% quota limits until July 7th and frequent security false positives that automatically downgrade code processing to older models like Opus 4.8. This matters for developers who rely on Claude Fable 5 for complex coding tasks, as the security false positives frequently interrupt normal development work and force users to pay for the flagship model but receive older, less capable alternatives. The model performance itself was not nerfed - only the safety classifier thresholds were set too aggressively. API and enterprise pay-per-use customers can fully access Claude Fable 5, while subscription users face the 50% quota restriction until July 7th, after which Fable 5 will be pay-per-use only.

telegram · zaihuapd · Jul 3, 07:20

**Background**: In June 2024, the US Department of Commerce imposed export controls on Claude Fable 5, restricting its global availability. The controls were lifted on June 12th, allowing Anthropic to restore access. Claude Fable 5 is Anthropic's flagship model designed for complex reasoning and coding tasks, while Opus 4.8 is a more conservative fallback model with stricter safety measures.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropic-restores-claude-fable-5-as-us-lifts-export-controls">Anthropic restores Claude Fable 5 as US lifts... | Tom's Hardware</a></li>
<li><a href="https://www.techtimes.com/articles/319576/20260702/claude-fable-5-debugging-scores-drop-70-safety-classifier-reroutes-tasks-weaker-fallback-model.htm">Claude Fable 5 Debugging Scores Drop 70%: Safety Classifier...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Anthropic`, `#Claude`, `#Developer Tools`, `#API`

---

<a id="item-13"></a>
## [Huawei Atlas 350 Launches with Ascend 950PR, 2.87x NVIDIA H20 Performance](https://t.me/zaihuapd/42329) ⭐️ 7.0/10

At Huawei China Partner Conference 2026, Huawei officially launched the Atlas 350 AI training and inference accelerator powered by the new Ascend 950PR processor. The card delivers 2.87x the compute of NVIDIA H20 with 112GB HBM and is China's first domestic accelerator supporting FP4 low-precision inference. This launch represents Huawei's aggressive push to compete with NVIDIA in China's AI accelerator market. The FP4 support and massive HBM capacity could significantly reduce AI inference costs and enable larger model deployments, potentially accelerating China's AI hardware independence efforts. Atlas 350 claims 2.87x the compute of NVIDIA H20, features 112GB HBM, supports 70B parameter model single-card loading, and offers improved vector compute power and interconnect bandwidth over its predecessor. However, these are Huawei's claimed figures without independent verification.

telegram · zaihuapd · Jul 3, 08:35

**Background**: FP4 is a 4-bit floating-point precision format that reduces computational complexity while maintaining acceptable inference accuracy, significantly improving energy efficiency. High Bandwidth Memory (HBM) is a 3D-stacked memory technology that provides much higher bandwidth than traditional memory, crucial for data-intensive AI workloads. NVIDIA introduced NVFP4 in mid-2025 to optimize low-precision inference.

<details><summary>References</summary>
<ul>
<li><a href="https://www.micron.com/products/memory/hbm">High-bandwidth memory (HBM) | Micron Technology Inc.</a></li>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision ...</a></li>

</ul>
</details>

**Tags**: `#AI_hardware`, `#Huawei`, `#Ascend_950PR`, `#AI_accelerator`, `#China_tech`

---

<a id="item-14"></a>
## [Alibaba Orders All Employees to Uninstall Claude by July 10](https://t.me/zaihuapd/42334) ⭐️ 7.0/10

Alibaba has ordered all employees to uninstall Claude and other Anthropic products, including Sonnet, Opus, Fable models and Claude Code, with the ban taking effect on July 10. This reverses Alibaba's previous policy of reimbursing employees for using external AI models like Claude, GPT, and Gemini. This represents a significant escalation in US-China tech tensions in the AI sector. The unprecedented ban demonstrates how accusations of fake account abuse can rapidly deteriorate relations between major tech companies, potentially reshaping how Chinese companies access Western AI tools. Anthropic had accused Alibaba of using approximately 25,000 fake accounts to interact with Claude over 28 million times between April 22 and June 5, subsequently tightening its control measures. The ban specifically targets all Anthropic products including the Claude Code AI programming assistant.

telegram · zaihuapd · Jul 3, 13:00

**Background**: Alibaba had previously maintained a permissive policy toward external AI tools, reimbursing employees for using Claude, GPT, and Gemini. Claude Code is an AI-driven coding assistant developed by Anthropic that helps developers build features, fix bugs, and automate development tasks. The accusations of fake account abuse represent one of the largest reported cases of AI model manipulation.

<details><summary>References</summary>
<ul>
<li><a href="https://code.claude.com/docs/zh-CN/overview">概述 - Claude Code Docs</a></li>
<li><a href="https://www.cnblogs.com/knqiufan/p/19449849">Claude Code 完全指南：使用方式、技巧与最佳实践 - knqiufan - 博客园</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Alibaba`, `#Anthropic`, `#US-China Tech Relations`, `#Industry News`

---

<a id="item-15"></a>
## [Atuin AI Outperforms Claude Mythos on CyberGym Benchmark](https://mp.weixin.qq.com/s/BzU7g-2iG7d6h4ViwMhxyg) ⭐️ 7.0/10

Tencent Xuanwu Lab's Atuin AI achieved 84.0% on UC Berkeley's CyberGym cybersecurity benchmark, surpassing Anthropic's Claude Mythos while using less than 0.1% of the budget. It also discovered multiple high-severity logic vulnerabilities in major open-source projects including curl, OpenSSL, and Python cryptography that Mythos failed to detect. This demonstrates that locally deployable open-source models can outperform expensive frontier models in vulnerability detection, potentially democratizing access to advanced AI security tools. The ability to achieve similar or better results at a fraction of the cost could significantly impact how organizations approach software security audits. Atuin AI is built on Zhipu AI's GLM-5.1, an open-source Mixture-of-Experts model with 744 billion parameters. The highest vulnerability severity score detected was 9.3, and on Berkeley's BVI real-world vulnerability ranking, Atuin AI ranked #1 in severity and #5 in total vulnerabilities found.

telegram · zaihuapd · Jul 3, 16:12

**Background**: CyberGym is a comprehensive benchmark from UC Berkeley that evaluates AI agents' ability to discover and exploit real-world software vulnerabilities across massive codebases. GLM-5.1 is Zhipu AI's latest open-source model featuring 8-hour autonomous task execution capability. Project Glasswing is Anthropic's initiative using Claude Mythos to scan critical open-source software infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://rdi.berkeley.edu/blog/cybergym/">Center for Responsible, Decentralized Intelligence at Berkeley</a></li>
<li><a href="https://pandaily.com/zhipu-unveils-glm-5-1-its-most-advanced-open-source-model-with-8-hour-autonomous-task-capability">Zhipu Unveils GLM-5.1, Its Most Advanced Open-Source Model with 8-Hour Autonomous Task Capability - Pandaily</a></li>
<li><a href="https://www.anthropic.com/project/glasswing">Project Glasswing \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#cybersecurity`, `#vulnerability detection`, `#benchmark`, `#Tencent`, `#GLM`, `#Claude`

---