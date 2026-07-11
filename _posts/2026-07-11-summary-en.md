---
layout: default
title: "Horizon Summary: 2026-07-11 (EN)"
date: 2026-07-11
lang: en
---

> From 176 items, 30 important content pieces were selected

---

1. [Apple Sues OpenAI for Trade Secret Theft](#item-1) ⭐️ 9.0/10
2. [Google Introduces SensorFM: Wearable Health AI Model at Unprecedented Scale](#item-2) ⭐️ 8.0/10
3. [Airbnb Opens Sitar-agent: Kubernetes Dynamic Config Sidecar](#item-3) ⭐️ 8.0/10
4. [HubSpot Scales Semantic Search to 200 Billion Vectors](#item-4) ⭐️ 8.0/10
5. [OpenAI, Google Supply AI to Pentagon-Blacklisted Chinese Companies](#item-5) ⭐️ 8.0/10
6. [sglang v0.5.15 Brings Spec V2, IndexShare MTP, GLM-5.2 NVFP4](#item-6) ⭐️ 7.0/10
7. [Good Tools Are Invisible](#item-7) ⭐️ 7.0/10
8. [War Atlas: Interactive Map of Every Named War in History](#item-8) ⭐️ 7.0/10
9. [Build Semantic Layer for Agentic AI with Stardog and Bedrock](#item-9) ⭐️ 7.0/10
10. [KTern.AI Builds Agentic AI Platform for SAP on Amazon Bedrock AgentCore](#item-10) ⭐️ 7.0/10
11. [Disaggregated Prefill-Decode on SageMaker HyperPod](#item-11) ⭐️ 7.0/10
12. [NVIDIA JAX Host Offloading for LLM Training](#item-12) ⭐️ 7.0/10
13. [NVIDIA CUDA Kernel Fusion: Optimizing Memory Traffic and Launch Overhead](#item-13) ⭐️ 7.0/10
14. [Accelerating End-to-End Co-Folding with NVIDIA BioNeMo Agent Toolkit](#item-14) ⭐️ 7.0/10
15. [Meta Removes Instagram AI Image Feature Over Privacy Concerns](#item-15) ⭐️ 7.0/10
16. [Kyutai Releases MuScriptor for Multi-Instrument Music Transcription](#item-16) ⭐️ 7.0/10
17. [Ant Group Releases LingBot-World-Infinity 14B Causal Video Model](#item-17) ⭐️ 7.0/10
18. [Apple Sues OpenAI Over Alleged Theft of Hardware Secrets](#item-18) ⭐️ 7.0/10
19. [Cactus v2 Launches as On-Device AI Platform with Cloud Fallback](#item-19) ⭐️ 7.0/10
20. [Show HN: Spacemap.co – 3D Real-Scale Solar System Map](#item-20) ⭐️ 7.0/10
21. [chwire: High-Performance ClickHouse JavaScript Client with Native Format](#item-21) ⭐️ 7.0/10
22. [9lives: Self-Healing Test Runner for Playwright](#item-22) ⭐️ 7.0/10
23. [从零开始预训练，蚂蚁灵波发布具身原生世界动作模型LingBot-VA 2.0](#item-23) ⭐️ 7.0/10
24. [Claude Rewrites Bun Runtime Codebase in 11 Days](#item-24) ⭐️ 7.0/10
25. [vLLM Inference Optimization for Multimodal Models at AICon Shenzhen](#item-25) ⭐️ 7.0/10
26. [Long March 10B Achieves World's First Net-Based Sea Recovery](#item-26) ⭐️ 7.0/10
27. [China's Network Identity System Hits 40M Users After One Year](#item-27) ⭐️ 7.0/10
28. [Meta Faces €120B EU Fine for Addictive Facebook/Instagram Design](#item-28) ⭐️ 7.0/10
29. [SK Hynix ADR Jumps 14% on NASDAQ Debut, Raises $26.5B Record](#item-29) ⭐️ 7.0/10
30. [FCC Approves Giant Mirror Satellite to Reflect Sunlight at Night](#item-30) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Apple Sues OpenAI for Trade Secret Theft](https://www.bloomberg.com/news/articles/2026-07-10/apple-sues-openai-for-trade-secret-theft-in-blockbuster-case) ⭐️ 9.0/10

Apple has filed a lawsuit against OpenAI accusing the AI company of trade secret theft, alleging that OpenAI recruited Apple employees to steal confidential information including hardware details and trade secrets. This blockbuster case between two tech giants could have major implications for the AI industry, potentially reshaping how companies handle talent recruitment and protect their intellectual property in the highly competitive AI sector. According to the lawsuit, OpenAI allegedly instructed new hires on how to avoid scrutiny when leaving Apple, including advising them not to tell Apple about their new jobs. Apple claims it discovered a pattern of OpenAI recruits emailing themselves confidential information when leaving, including a senior employee named Tang Yew Tan who worked at Apple for 25 years.

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Jul 10, 20:42

**Background**: Trade secret theft claims involve allegations that a company illegally acquired or used confidential business information from a competitor. In the AI industry, such secrets could include training methodologies, model architectures, and hardware specifications. This lawsuit comes amid ongoing tensions between major tech companies competing for AI talent and market dominance.

**Discussion**: The community discussion shows strong consensus that Apple has a strong case, with commenters noting the detailed allegations about OpenAI's alleged systematic approach to recruiting Apple employees for their confidential information. Some commenters expressed concern that such behavior would undermine trust in OpenAI's enterprise products.

**Tags**: `#Apple`, `#OpenAI`, `#lawsuit`, `#trade secrets`, `#AI industry`

---

<a id="item-2"></a>
## [Google Introduces SensorFM: Wearable Health AI Model at Unprecedented Scale](https://www.marktechpost.com/2026/07/10/google-research-introduces-sensorfm-a-wearable-health-foundation-model-pretrained-on-one-trillion-minutes-of-sensor-data/) ⭐️ 8.0/10

Google Research unveils SensorFM, a wearable health foundation model pretrained on over one trillion minutes of sensor data from 5 million participants, achieving state-of-the-art results on 34 of 35 tasks using frozen embeddings with a PCA-50 linear probe. This represents a major advance in health AI foundation models, demonstrating that wearable sensor data at unprecedented scale can effectively train generalizable health prediction models. The approach could enable more accessible and continuous health monitoring through consumer wearables, potentially transforming preventive healthcare and clinical diagnostics. The model uses a ViT-1D encoder with a masked autoencoder objective at patch size [20,1], ingesting 34 one-minute aggregate features from five sensors (PPG, accelerometer, EDA, skin temperature, and altimeter) over a 24-hour context window. It demonstrates co-scaling across four model sizes and four data volumes, including cases where model capacity outruns available data.

rss · MarkTechPost · Jul 10, 08:52

**Background**: Foundation models are large AI models pretrained on massive data that can be adapted to many downstream tasks. In health AI, wearable devices like smartwatches collect continuous sensor data including heart rate (PPG), movement (accelerometer), skin conductance (EDA), temperature, and altitude. Linear probes are lightweight evaluation methods that train a simple classifier on frozen model embeddings to assess the model's learned representations without fine-tuning.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techtimes.com/articles/320098/20260710/wearable-ai-now-rivals-lab-tests-googles-sensorfm-trained-1-trillion-minutes.htm">Wearable AI Now Rivals Lab Tests: Google's SensorFM Trained on...</a></li>
<li><a href="https://overcentral.com/en/sensorfm-foundation-model/">Google Research SensorFM: Foundation Model for Wearable Health...</a></li>
<li><a href="https://www.marktechpost.com/2026/07/10/google-research-introduces-sensorfm-a-wearable-health-foundation-model-pretrained-on-one-trillion-minutes-of-sensor-data/">Google Research Introduces SensorFM: A Wearable... - MarkTechPost</a></li>

</ul>
</details>

**Tags**: `#foundation-models`, `#health-ai`, `#wearables`, `#google-research`, `#sensor-data`, `#machine-learning`

---

<a id="item-3"></a>
## [Airbnb Opens Sitar-agent: Kubernetes Dynamic Config Sidecar](https://www.infoq.cn/article/fO5byVPuZwwlBPosijBV?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

Airbnb engineers detailed Sitar-agent, a custom Kubernetes sidecar that delivers dynamic configuration updates to tens of thousands of pods, processing updates several times per minute with Java and Amazon S3 snapshot bootstrapping. This represents valuable production-grade engineering knowledge from a major tech company solving real configuration management challenges at scale, making it highly relevant for engineers dealing with similar infrastructure issues in Kubernetes environments. Sitar-agent is a lightweight sidecar that runs alongside every subscribed service pod, continuously synchronizing the latest configurations from the service backend and making them available on the local filesystem. The system was redesigned with Java for improved reliability and scalability.

rss · InfoQ 中文站 · Jul 11, 09:00

**Background**: The sidecar pattern is a Kubernetes deployment pattern where an additional container runs alongside the main application container to provide auxiliary functionality. Dynamic configuration is critical in microservices architectures where services need to adapt to changing parameters without requiring container restarts. This is particularly important at Airbnb's scale with tens of thousands of pods.

<details><summary>References</summary>
<ul>
<li><a href="https://www.infoq.com/news/2026/07/sitar-agent-sidecar-config/">Airbnb Shares Architecture behind Sitar-Agent Dynamic Configuration Sidecar for Kubernetes Services - InfoQ</a></li>
<li><a href="https://medium.com/airbnb-engineering/sitar-agent-building-a-reliable-dynamic-configuration-sidecar-at-scale-b7e00c152068">Sitar-agent: Building a reliable dynamic configuration sidecar at scale</a></li>

</ul>
</details>

**Tags**: `#Kubernetes`, `#Sidecar Pattern`, `#Configuration Management`, `#Infrastructure`, `#Airbnb`, `#DevOps`

---

<a id="item-4"></a>
## [HubSpot Scales Semantic Search to 200 Billion Vectors](https://www.infoq.cn/article/eRl25z5ewrRHjReWhOUX?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

HubSpot shared their technical practices for scaling their semantic search system to handle 200 billion vectors, including architecture design and optimization experience for vector search infrastructure. Scaling vector search to this magnitude represents significant engineering challenges in infrastructure, latency, and cost. This case study provides valuable insights for engineers working with vector databases and search systems at massive scale. The technical deep-dive covers specific architectural decisions, optimization techniques, and lessons learned from operating a vector search system at 20B scale in a production environment.

rss · InfoQ 中文站 · Jul 10, 12:00

**Background**: Semantic search uses vector embeddings (numerical representations of text in high-dimensional space) to find semantically similar content rather than just keyword matches. Vector databases specialize in storing and efficiently querying these embeddings using approximate nearest neighbor (ANN) algorithms. As AI applications grow, scaling vector search infrastructure to handle billions of vectors while maintaining low latency becomes a critical engineering challenge.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnblogs.com/cmt/p/18514667">AI之旅-语义搜索：初识 vector embedding 与部署向量数据库 qdrant - 博客园团队 - 博客园</a></li>
<li><a href="https://help.aliyun.com/document_detail/2510234.html">如何基于向量检索服务 DashVector与百炼实现语义搜索_向量检索服务 DashVector(DashVector)-阿里云帮助中心</a></li>
<li><a href="https://baoyu.io/translations/rag/search-vs-vector-db">构建搜索引擎，而非 向 量 数 据 库 （ Vector DB） [译] | 宝玉的分享</a></li>

</ul>
</details>

**Tags**: `#semantic-search`, `#vector-database`, `#scalability`, `#infrastructure`, `#search-engineering`

---

<a id="item-5"></a>
## [OpenAI, Google Supply AI to Pentagon-Blacklisted Chinese Companies](https://www.ft.com/content/5d6aafa1-5d47-4585-aa95-6ec06a6cd20f) ⭐️ 8.0/10

OpenAI and Google have been providing advanced AI services to Alibaba, Baidu, and Tencent subsidiaries in Singapore, despite their parent companies being on the Pentagon's 1260H blacklist of Chinese military-linked companies. OpenAI suspended an Alibaba-linked user's API access last month after detecting suspected 'model distillation' behavior and reported it to the US government. This exposes significant gaps in current US export controls, as Chinese companies can circumvent blacklist designations through offshore subsidiaries. The revelation has renewed calls in Washington for export controls on frontier AI software, highlighting the challenge of enforcing technology restrictions in a globally connected digital economy. The transactions remain legal because current US restrictions do not broadly prohibit Chinese headquarters from obtaining advanced AI models outside mainland China. Anthropic has taken a stricter approach, completely banning Chinese companies and their overseas entities from accessing its frontier AI models.

telegram · zaihuapd · Jul 10, 09:59

**Background**: The Pentagon's 1260H list identifies entities believed to be linked to China's military. Companies on this list face various restrictions, though current US AI export controls have loopholes that allow access through foreign subsidiaries. Model distillation is a technique where a smaller model learns from a larger model's outputs, allowing knowledge transfer without direct access to the original model's weights.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scmp.com/news/china/diplomacy/article/3356419/us-adds-alibaba-byd-and-other-chinese-tech-champions-military-company-list">US adds Alibaba, BYD and other Chinese tech champions to military company blacklist | South China Morning Post</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/knowledge-distillation">What is Knowledge distillation? | IBM</a></li>

</ul>
</details>

**Tags**: `#AI_policy`, `#US_China_relations`, `#export_controls`, `#OpenAI`, `#national_security`, `#tech_sanctions`

---

<a id="item-6"></a>
## [sglang v0.5.15 Brings Spec V2, IndexShare MTP, GLM-5.2 NVFP4](https://github.com/sgl-project/sglang/releases/tag/v0.5.15) ⭐️ 7.0/10

sglang v0.5.15 release introduces Spec V2 as default with +11% TPS improvement, IndexShare MTP for 1.9x lower draft-step cost, and production-optimized GLM-5.2 NVFP4 performance reaching 500+ tok/s/user on 8x B300 and 450 tok/s on 4x GB300 (bs=1). This release demonstrates meaningful performance improvements for LLM serving infrastructure. The 11% TPS gain from Spec V2 optimizations and 1.9x draft-step cost reduction directly improve inference throughput and cost-efficiency, while production-tuned GLM-5.2 on Blackwell hardware shows real engineering work for deploying LLMs at scale. Key optimizations include TopK V2 fusing top-k selection with page-table transform (runtime k up to 2048), Indexer prologue fusion reducing 12 kernels to 4 (~8% faster decode at bs=1), Breakable CUDA Graph as default, and FlashMLA sparse prefill now enabled by default for DeepSeek-V4 with >10% throughput gain on long context.

github · Fridge003 · Jul 10, 22:58

**Background**: sglang is an LLM serving framework that supports speculative decoding, a technique where a smaller 'draft' model predicts multiple tokens that a larger 'target' model then verifies, significantly speeding up inference. NVFP4 is NVIDIA's 4-bit floating-point format designed for high-performance inference on modern GPUs. Multi-Token Prediction (MTP) allows models to predict multiple future tokens simultaneously rather than just the next token, which can improve inference efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://introl.com/blog/speculative-decoding-llm-inference-speedup-guide-2025">Speculative Decoding : Achieving 2-3x LLM Inference... | Introl Blog</a></li>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision Inference</a></li>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/mtp/">MTP ( Multi - Token Prediction ) - vLLM</a></li>

</ul>
</details>

**Tags**: `#LLM serving`, `#performance optimization`, `#sglang`, `#speculative decoding`, `#GPU inference`

---

<a id="item-7"></a>
## [Good Tools Are Invisible](https://www.gingerbill.org/article/2026/07/10/good-tools-are-invisible/) ⭐️ 7.0/10

A thoughtful exploration of why effective tools should become 'invisible' to users, eliminating unnecessary complexity so users can focus on their actual work rather than wrestling with the tool itself.

hackernews · theanonymousone · Jul 10, 10:32

**Tags**: `#software-design`, `#ux`, `#developer-tools`, `#productivity`, `#philosophy`

---

<a id="item-8"></a>
## [War Atlas: Interactive Map of Every Named War in History](https://waratlas.org/) ⭐️ 7.0/10

War Atlas is an interactive cartography project that visualizes every named war in human history, allowing users to explore conflicts across time and space through a map-based interface. This project represents an ambitious effort to democratize access to historical conflict data, but its community discussion reveals significant concerns about data completeness, accuracy, and design choices that affect its usefulness as an educational tool. The visualization uses a dark-grey-on-black color scheme which critics argue makes borders nearly invisible; the project has been noted to crash Firefox browsers; and important wars like the Spanish Civil War (1936-1939) are reportedly missing from the dataset.

hackernews · NaOH · Jul 10, 17:52

**Background**: Interactive historical maps combine cartography with historical data to visualize events across time and space. War Atlas attempts to compile all named conflicts into a single searchable visualization, drawing from open datasets. Such projects face inherent challenges in defining what qualifies as a "war" and ensuring comprehensive global coverage across different historical periods and cultures.

**Discussion**: The community discussion reveals mixed reception: criticsfault the dark color scheme for poor visibility, note missing wars like Spain's Civil War, highlight accuracy concerns with border representations, and question whether balanced historical recording is a universal or Western-centric concept. One commenter also reported Firefox crashing issues.

**Tags**: `#data-visualization`, `#interactive-maps`, `#history`, `#open-data`, `#cartography`

---

<a id="item-9"></a>
## [Build Semantic Layer for Agentic AI with Stardog and Bedrock](https://aws.amazon.com/blogs/machine-learning/build-a-semantic-layer-for-agentic-ai-on-aws-with-stardog-and-amazon-bedrock-agentcore/) ⭐️ 7.0/10

AWS published a tutorial demonstrating how to build a semantic layer using Stardog's Semantic AI Application over Amazon Aurora and Amazon Redshift, combined with Strands Agents running on Amazon Bedrock AgentCore to answer customer 360 queries without ETL. This architecture enables organizations to build agentic AI applications that can query multiple data sources (data lakehouse and warehouse) without moving or copying data, significantly simplifying data integration and reducing infrastructure complexity. The same Stardog deployment works behind AWS compute services including Amazon EKS, Amazon ECS, and AWS Lambda. AgentCore bundles inbound auth, hosting, and tool credentials into one managed service, simplifying agent deployment.

rss · AWS Machine Learning Blog · Jul 10, 15:31

**Background**: A semantic layer is a data abstraction layer that provides a unified view of data from multiple sources. Stardog is a knowledge graph database that offers data virtualization, allowing queries across different data sources without moving data. Amazon Bedrock AgentCore is AWS's platform for building and deploying AI agents at scale. Strands Agents is AWS's open-source AI agent framework designed for building production-ready autonomous agents.

<details><summary>References</summary>
<ul>
<li><a href="https://www.stardog.com/">The Knowledge Graph-Powered Semantic Layer | Stardog</a></li>
<li><a href="https://aws.amazon.com/bedrock/">Amazon Bedrock – Build genAI applications and agents at production...</a></li>
<li><a href="https://strandsagents.com/">Strands Agents — Open Source AI Agent SDK for Python & TypeScript</a></li>
<li><a href="https://docs.aws.amazon.com/prescriptive-guidance/latest/agentic-ai-frameworks/strands-agents.html">Strands Agents - AWS Prescriptive Guidance</a></li>

</ul>
</details>

**Tags**: `#semantic layer`, `#AWS`, `#agentic AI`, `#Amazon Bedrock`, `#knowledge graph`

---

<a id="item-10"></a>
## [KTern.AI Builds Agentic AI Platform for SAP on Amazon Bedrock AgentCore](https://aws.amazon.com/blogs/machine-learning/how-ktern-ai-built-agentic-ai-for-sap-on-amazon-bedrock-agentcore/) ⭐️ 7.0/10

KTern.AI announced their journey building a production agentic AI platform for SAP using Amazon Bedrock AgentCore and the Strands Agents SDK, transitioning from a traditional SaaS platform to orchestrate multiple specialized agents across enterprise programs. This case study provides a practical blueprint for enterprise AI practitioners looking to build multi-agent systems with persistent context and secure tool access, demonstrating real-world architecture for production-grade agentic AI deployment. The architecture enables each agent to operate with persistent context, secure tool access, and production-grade reliability across long-running enterprise programs, with specific details on how the agents were built and customer outcomes achieved.

rss · AWS Machine Learning Blog · Jul 10, 15:23

**Background**: Amazon Bedrock AgentCore is AWS's platform for building, connecting, and optimizing AI agents at scale with security and reliability. The Strands Agents SDK is an open-source, model-driven framework for building AI agents with minimal code, offering a lightweight customizable agent loop for autonomous reasoning. Agentic AI differs from generative AI in that it can take autonomous actions based on reasoning rather than just generating content.

<details><summary>References</summary>
<ul>
<li><a href="https://aws.amazon.com/bedrock/">Amazon Bedrock – Build genAI applications and agents at production...</a></li>
<li><a href="https://grokipedia.com/page/Strands_Agents">Strands Agents</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-ai-vs-generative-ai">Agentic AI vs . Generative AI | IBM</a></li>

</ul>
</details>

**Tags**: `#agentic-ai`, `#amazon-bedrock`, `#sap`, `#enterprise-ai`, `#multi-agent-systems`

---

<a id="item-11"></a>
## [Disaggregated Prefill-Decode on SageMaker HyperPod](https://aws.amazon.com/blogs/machine-learning/disaggregated-prefill-and-decode-for-llm-inference-on-sagemaker-hyperpod/) ⭐️ 7.0/10

AWS published a technical guide on implementing disaggregated prefill and decode (DPD) with vLLM on Amazon SageMaker HyperPod using the HyperPod Inference Operator. This implementation is significant for ML infrastructure engineers deploying LLMs at scale, as DPD can significantly improve inference throughput and reduce latency by eliminating interference between prefill and decode phases. The guide details how to deploy disaggregated prefill and decode workers using vLLM on HyperPod, enabling each phase to focus on its specific optimization target: Time to First Token (TTFT) or Time Per Output Token (TPOT).

rss · AWS Machine Learning Blog · Jul 10, 15:20

**Background**: Disaggregated prefill and decode is an LLM inference optimization technique that separates the two phases of inference onto different compute devices. The prefill phase processes the input prompt and computes the KV cache, while the decode phase generates output tokens iteratively. These two phases have different computational characteristics—prefill is compute-bound while decode is memory-bound—and traditionally interfere with each other when run on the same device. vLLM is a high-throughput, memory-efficient open-source LLM inference serving engine originally developed at UC Berkeley, while SageMaker HyperPod is AWS's managed infrastructure for machine learning workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@thillaic/disaggregated-llm-inference-how-splitting-prefill-and-decode-changes-everything-7404d09d5ec2">Disaggregated LLM Inference : How Splitting Prefill and Decode ...</a></li>
<li><a href="https://github.com/vllm-project/vllm">vllm -project/ vllm : A high-throughput and memory-efficient inference ...</a></li>

</ul>
</details>

**Tags**: `#LLM-inference`, `#vLLM`, `#SageMaker-HyperPod`, `#machine-learning-infrastructure`, `#disaggregated-prefill-decode`

---

<a id="item-12"></a>
## [NVIDIA JAX Host Offloading for LLM Training](https://developer.nvidia.com/blog/reducing-high-bandwidth-memory-bottlenecks-in-jax-based-llm-training-with-host-offloading/) ⭐️ 7.0/10

NVIDIA推出了一种针对JAX大语言模型训练的host offloading技术，通过将选定的激活值移动到固定主机内存并在反向传播时流回，从而显著减轻高带宽内存（HBM）压力。 这一技术使得能够训练更大的模型或使用更大的批处理规模，而不会遇到GPU内存限制问题，解决了GPU内存限制阻止计算能力充分利用的常见瓶颈，对ML系统工程师具有重要实用价值。 该技术将激活值移动到pinned host memory（固定主机内存，而非标准系统RAM）并高效地流回，专门针对反向传播需要但消耗大量HBM的激活值进行优化。

rss · NVIDIA Developer Blog · Jul 10, 18:17

**Background**: 高带宽内存（HBM）是集成在GPU中的一种内存类型，比传统DDR内存提供更高的带宽但容量有限。JAX是Google开发的数值计算库，支持高效的多核CPU和GPU计算，广泛用于机器学习研究。Host offloading（主机卸载）是一种内存管理技术，通过在GPU内存和CPU内存之间移动数据来克服硬件资源限制。

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/reducing-high-bandwidth-memory-bottlenecks-in-jax-based-llm-training-with-host-offloading/">Reducing High-Bandwidth Memory Bottlenecks in JAX-Based LLM...</a></li>
<li><a href="https://blockchain.news/news/nvidia-jax-llm-training-host-offloading">NVIDIA Optimizes JAX LLM Training with Host Offloading</a></li>

</ul>
</details>

**Tags**: `#LLM Training`, `#JAX`, `#GPU Optimization`, `#Memory Management`, `#Machine Learning Systems`

---

<a id="item-13"></a>
## [NVIDIA CUDA Kernel Fusion: Optimizing Memory Traffic and Launch Overhead](https://developer.nvidia.com/blog/kernel-fusion-in-nvidia-cuda-optimizing-memory-traffic-and-launch-overhead/) ⭐️ 7.0/10

NVIDIA explains how kernel fusion combines multiple GPU kernels to improve memory bandwidth utilization and reduce kernel launch overhead for better CUDA performance. This optimization technique can significantly improve GPU performance by reducing memory traffic and kernel launch overhead, which is critical for memory-bound applications and can yield speedups of up to 3x. Kernel fusion reduces redundant off-chip memory accesses by retaining intermediate results on-chip, and eliminates the overhead of launching multiple separate kernels by merging operations into a single kernel.

rss · NVIDIA Developer Blog · Jul 10, 16:41

**Background**: A CUDA kernel is a function that runs in parallel on the GPU. Each kernel launch involves overhead from the host CPU, and reading/writing data between GPU global memory and on-chip memory is expensive in terms of bandwidth and latency. Kernel fusion addresses both issues by combining multiple sequential kernels into a single, larger kernel.

<details><summary>References</summary>
<ul>
<li><a href="https://stackoverflow.com/questions/53305830/cuda-how-does-kernel-fusion-improve-performance-on-memory-bound-applications-on">CUDA How Does Kernel Fusion Improve... - Stack Overflow</a></li>
<li><a href="https://www.peakinfer.com/blog/the-performance-wins-from-fusing-kernels">The Performance Wins from Fusing Kernels | PeakInfer Blog</a></li>
<li><a href="https://www.emergentmind.com/topics/kernel-fusion-and-arithmetic-intensity">Kernel Fusion and Arithmetic Intensity</a></li>

</ul>
</details>

**Tags**: `#CUDA`, `#GPU optimization`, `#kernel fusion`, `#performance optimization`, `#memory bandwidth`

---

<a id="item-14"></a>
## [Accelerating End-to-End Co-Folding with NVIDIA BioNeMo Agent Toolkit](https://developer.nvidia.com/blog/accelerating-end-to-end-co-folding-performance-with-nvidia-bionemo-agent-toolkit/) ⭐️ 7.0/10

NVIDIA demonstrates how to accelerate end-to-end protein co-folding with OpenFold3 using their BioNeMo Agent Toolkit for drug discovery applications, providing practical optimization guidance for computational biology workloads. This acceleration is significant for drug discovery pipelines as protein co-folding predictions help researchers understand how proteins interact with potential drug molecules, enabling faster identification of therapeutic candidates and reducing experimental costs. The optimization combines GPU acceleration techniques with the OpenFold3 co-folding model, which predicts the 3D structure of protein-molecule complexes including proteins bound to small-molecule drugs, antibodies, or nucleic acids.

rss · NVIDIA Developer Blog · Jul 10, 13:00

**Background**: Protein co-folding is a computational technique that predicts how two or more molecules interact and fold together in three-dimensional space, which is crucial for understanding drug binding mechanisms. OpenFold3 is a third-generation biomolecular foundation model capable of predicting structures of proteins, DNA, RNA, and ligands. The NVIDIA BioNeMo Agent Toolkit, announced in June 2026, provides AI agents with accelerated tools for biology, chemistry, genomics, and drug discovery research.

<details><summary>References</summary>
<ul>
<li><a href="https://build.nvidia.com/openfold/openfold3/preload">openfold 3 Model by Openfold | NVIDIA NIM</a></li>
<li><a href="https://www.sandboxaq.com/openfold3">OpenFold 3 | Fully Open-Source Cofolding AI for Drug... | SandboxAQ</a></li>
<li><a href="https://nvidianews.nvidia.com/news/nvidia-launches-bionemo-agent-toolkit-giving-ai-agents-the-tools-to-accelerate-scientific-discovery">NVIDIA Announces BioNeMo Agent Toolkit ... | NVIDIA Newsroom</a></li>
<li><a href="https://github.com/NVIDIA-BioNeMo/bionemo-agent-toolkit">GitHub - NVIDIA - BioNeMo / bionemo - agent - toolkit : Turn any agent ...</a></li>

</ul>
</details>

**Tags**: `#protein-folding`, `#drug-discovery`, `#gpu-computing`, `#computational-biology`, `#nvidia-bionemo`

---

<a id="item-15"></a>
## [Meta Removes Instagram AI Image Feature Over Privacy Concerns](https://www.theverge.com/tech/964416/meta-instagram-ai-muse-image-deepfakes) ⭐️ 7.0/10

Meta has removed an Instagram feature that allowed users to generate AI images of public account holders simply by tagging them, without the account owner's permission. The feature was announced earlier this week and was turned off following substantial backlash. This incident highlights growing tensions between AI innovation and user privacy rights, and signals increased regulatory scrutiny on how tech companies handle AI-generated content involving real people without consent. It demonstrates that public backlash can lead to rapid policy reversals. The feature used AI to generate images based on content from any public Instagram account, meaning account holders had no control over how their content was used in AI creations. The backlash centered on consent issues and the potential for misuse.

rss · The Verge AI · Jul 10, 23:49

**Background**: Deepfakes refer to AI-generated synthetic media that can manipulate or create realistic images, videos, or audio of people. The rapid advancement of AI image generation tools has raised significant concerns about privacy, consent, and the potential for abuse in creating non-consensual intimate imagery or misinformation. Meta's Instagram has been a platform where users share personal content, making it a rich source of data for AI training and generation.

**Discussion**: The backlash was substantial, focusing on the lack of consent mechanisms and the potential for privacy violations. Users and privacy advocates criticized the feature for enabling the creation of AI-generated images without the knowledge or permission of the account holders depicted.

**Tags**: `#AI policy`, `#Meta`, `#Instagram`, `#deepfakes`, `#privacy`

---

<a id="item-16"></a>
## [Kyutai Releases MuScriptor for Multi-Instrument Music Transcription](https://www.marktechpost.com/2026/07/10/kyutai-releases-muscriptor-an-open-weight-decoder-only-transformer-for-multi-instrument-music-transcription-to-midi/) ⭐️ 7.0/10

Kyutai has released MuScriptor, an open-weight decoder-only Transformer trained on 170k real recordings and 1.45M synthetic MIDIs for transcribing multi-instrument music into MIDI format with a three-stage pipeline. This open-weight release makes multi-instrument music transcription more accessible to researchers, offering a practical alternative to closed-source models with its substantial training data and benchmark performance against YourMT3+. The model features instrument conditioning that helps distinguish between different instrument sounds in a full mix. The decoder-only architecture follows the approach used in modern large language models, potentially allowing for efficient scaling.

rss · MarkTechPost · Jul 10, 20:21

**Background**: Music transcription converts audio recordings into symbolic music notation or MIDI files. Multi-instrument transcription is particularly challenging because it requires identifying and separating multiple instruments playing simultaneously. A decoder-only Transformer is an architecture that uses only the decoder portion of the original Transformer, similar to how GPT models work - it generates output sequentially based on previous predictions. MIDI (Musical Instrument Digital Interface) is a standard protocol for electronic musical instruments to communicate, storing note timing, pitch, and velocity rather than audio waveforms. YourMT3+ is a benchmark suite for multi-instrument music transcription that sets a standard for evaluating transcription quality.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2404.14462v2">Towards Smaller, Faster Decoder - Only Transformers : Architectural ...</a></li>
<li><a href="https://www.emergentmind.com/papers/2407.04822">YourMT 3+ : Enhanced Music Transcription</a></li>
<li><a href="https://arxiv.org/abs/1809.06127">[1809.06127] DeepDrum: An Adaptive Conditional Neural Network</a></li>

</ul>
</details>

**Tags**: `#music-ai`, `#transformers`, `#open-weights`, `#midi`, `#music-transcription`

---

<a id="item-17"></a>
## [Ant Group Releases LingBot-World-Infinity 14B Causal Video Model](https://www.marktechpost.com/2026/07/09/meet-lingbot-world-infinity-an-open-causal-world-model-with-an-agentic-harness/) ⭐️ 7.0/10

Ant Group's Robbyant unit released LingBot-World-Infinity (LingBot-World 2.0), a 14B parameter causal video generation model functioning as an interactive world simulator. It uses MoBA (Mixture of Bidirectional and Autoregressive) attention combined with distribution matching distillation over long self-rollout trajectories, wrapped in a Director-Pilot agentic harness where a VLM proposes events and a Diffusion Transformer renders them. This release directly targets long-horizon drift—the failure mode that smears textures and warps geometry in most interactive world models. It represents a significant open contribution for the embodied AI and video generation community, offering a 14B model addressing a fundamental limitation in world simulation. The model demonstrates a single 60-minute uninterrupted session covering 20 scenarios. However, the release is limited: one checkpoint, a 480P reference script, no deployment code, no quantitative benchmarks, and a non-commercial CC BY-NC-SA 4.0 license.

rss · MarkTechPost · Jul 10, 04:38

**Background**: World models are AI systems that simulate how the physical world works, crucial for training robots to perform tasks in real environments. Interactive world models allow users to interact with the environment through actions in real-time. Long-horizon drift is the degradation of model outputs over extended sessions. MoBA attention applies Mixture of Experts principles to attention mechanisms. Distribution Matching Distillation (DMD) compresses multi-step generative models into efficient one-step models. Diffusion Transformer (DiT) replaces convolutional U-Nets with transformer-based architectures.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MoonshotAI/MoBA">GitHub - MoonshotAI/ MoBA : MoBA : Mixture of Block Attention for...</a></li>
<li><a href="https://tianweiy.github.io/dmd2/dmd2.pdf">Improved Distribution Matching Distillation</a></li>
<li><a href="https://www.emergentmind.com/topics/88">Diffusion Transformer (DiT) Model</a></li>

</ul>
</details>

**Tags**: `#AI`, `#video-generation`, `#world-models`, `#machine-learning`, `#embodied-ai`

---

<a id="item-18"></a>
## [Apple Sues OpenAI Over Alleged Theft of Hardware Secrets](https://www.wired.com/story/apple-sues-openai-allegedly-stealing-ip-hardware/) ⭐️ 7.0/10

Apple has filed a lawsuit against OpenAI, alleging that the company encouraged employees it poached from Apple to steal confidential presentations, secret prototypes, and key supplier details. This lawsuit highlights growing tensions in the AI talent war between major tech companies. It could have industry-wide implications for how companies handle talent acquisition and protect their confidential information. The lawsuit claims OpenAI actively encouraged ex-Apple employees to bring over proprietary hardware information, including confidential presentations and supplier details. This marks another escalation in the ongoing legal disputes between major tech companies in the AI space.

rss · Hacker News - OpenAI / Anthropic / Gemini / DeepSeek · Jul 10, 21:00

**Background**: In the highly competitive AI landscape, talent acquisition has become crucial as companies race to develop advanced AI systems. Companies often recruit experienced engineers from rivals, which can lead to disputes over trade secrets and confidential information. This lawsuit reflects growing tensions in the tech industry over intellectual property protection and the boundaries of fair competition in hiring.

**Tags**: `#apple`, `#openai`, `#lawsuit`, `#ip-theft`, `#tech-industry`

---

<a id="item-19"></a>
## [Cactus v2 Launches as On-Device AI Platform with Cloud Fallback](https://news.ycombinator.com/item?id=48864459) ⭐️ 7.0/10

Cactus v2 launched as an on-device AI inference platform with cloud fallback, supporting Arm devices from iOS to Raspberry Pi with lossless 4-bit quantization and confidence-based routing. A Gemma 4 E2B model runs at 169 tok/sec on M5 Max, using only 2.7GB disk and 1.3GB RAM. This addresses a critical gap in on-device AI by enabling local models to handle 90% of workloads while seamlessly escalating complex inference to the cloud. It opens up production-ready AI for resource-constrained devices that previously couldn't run large models. The cloud fallback uses a probe trained into model weights that reads internal activations to emit a confidence signal, enabling routing inside the model rather than external classifiers. The runtime supports Python, Rust, React Native, Swift, and Kotlin bindings, with GPU acceleration starting with Apple Metal.

rss · Hacker News - Show HN · Jul 10, 19:57

**Background**: On-device AI inference refers to running ML models directly on edge devices rather than in data centers. 4-bit quantization compresses model weights from 16-bit floats to 4-bit representations, dramatically reducing memory and storage needs while maintaining accuracy. Arm processors power most mobile devices and embedded systems. DGX Spark is NVIDIA's personal AI supercomputer powered by Blackwell architecture. Apple Metal is Apple's low-level GPU API required for hardware-accelerated inference on Apple Silicon.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/4bit-transformers-bitsandbytes">Making LLMs even more accessible with bitsandbytes, 4 - bit ...</a></li>
<li><a href="https://www.runlocalai.co/learn/courses/local-ai-macos/chapter-4-metal-gpu-acceleration">Metal GPU Acceleration — Local AI on macOS (Chapter 4) | RunLocalAI</a></li>
<li><a href="https://www.nvidia.com/en-us/products/workstations/dgx-spark/">Personal AI Supercomputer Powered by Blackwell | NVIDIA DGX Spark</a></li>

</ul>
</details>

**Tags**: `#on-device-ai`, `#edge-computing`, `#inference-engine`, `#machine-learning`, `#arm`

---

<a id="item-20"></a>
## [Show HN: Spacemap.co – 3D Real-Scale Solar System Map](https://spacemap.co/b/399/Earth) ⭐️ 7.0/10

A developer launched Spacemap.co, a 3D real-time real-scale solar system map featuring 1.6 million objects including all known asteroids, comets, moons, planets, and spacecraft, with historical positions dating back to 1950, Wikipedia data integration, 11,000 3D models, and 12-language localization. This represents a significant advancement in accessible space visualization, offering unprecedented scale with 1.6 million objects and historical data since 1950. It democratizes space exploration for enthusiasts and developers by providing realistic lighting, search functionality, and the ability to zoom into detailed 3D models of spacecraft and asteroids. The project uses WebGL for 3D rendering and incorporates realistic lighting effects. Historical positions are calculated from 1950 to present, allowing users to view events like New Horizons' Pluto flyby in 2015 and Artemis 2's planned 2026 mission. The map includes deep links to specific objects like the Starlink constellation and Saturn's moons.

rss · Hacker News - Show HN · Jul 10, 20:17

**Background**: WebGL is a JavaScript API for rendering high-performance interactive 3D graphics in web browsers without plugins. Ephemerides are tables of computed positions for celestial bodies, essential for calculating orbital positions at specific times. This project combines these technologies to create a comprehensive solar system visualization that runs directly in the browser.

<details><summary>References</summary>
<ul>
<li><a href="https://www.khronos.org/webgl/">WebGL - Low-Level 3 D Graphics API Based on OpenGL ES</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ephemeris">Ephemeris - Wikipedia</a></li>
<li><a href="https://orbital-mechanics.space/reference/planetary-ephemeris.html">Planetary Ephemeris — Orbital Mechanics & Astrodynamics</a></li>

</ul>
</details>

**Tags**: `#space-exploration`, `#3d-visualization`, `#astronomy`, `#interactive-maps`, `#webgl`

---

<a id="item-21"></a>
## [chwire: High-Performance ClickHouse JavaScript Client with Native Format](https://github.com/maxjustus/chwire) ⭐️ 7.0/10

chwire is a new ClickHouse JavaScript client that uses the Native columnar binary format over HTTP/TCP, achieving 2-8x speed improvements over JSONEachRow for encoding/decoding 1M-row payloads, with ZSTD/LZ4 compression support. This matters because JavaScript developers working with ClickHouse at scale previously faced significant CPU overhead from gzip/deflate compression with the official client. chwire solves this real performance pain point by using the more efficient Native format, making high-volume inserts much more practical. The client supports all ClickHouse types including Variant, Dynamic, JSON, Nested, and Tuple at arbitrary nesting levels. It works in browsers via HTTP and in Node/Bun/Deno over HTTP or TCP. The implementation was aggressively fuzz-tested and includes a fully functional TCP client supporting ProfileEvents, logs, and progress.

rss · Hacker News - Show HN · Jul 10, 19:51

**Background**: ClickHouse is a columnar database known for analytical queries. The Native format is its most efficient format because it stores data in columnar binary without converting columns to rows, matching ClickHouse's internal representation. In contrast, JSONEachRow outputs each row as a separate JSON object, which is human-readable but less efficient for bulk operations.

<details><summary>References</summary>
<ul>
<li><a href="https://clickhouse.com/docs/integrations/data-formats/binary-native">Using native and binary formats in ClickHouse | ClickHouse Docs</a></li>
<li><a href="https://clickhouse.com/docs/interfaces/formats/JSONEachRow">JSONEachRow | ClickHouse Docs</a></li>
<li><a href="https://github.com/ClickHouse/ClickHouse/blob/master/docs/en/interfaces/formats/Native.md">ClickHouse /docs/en/interfaces/ formats / Native .md at master...</a></li>

</ul>
</details>

**Tags**: `#clickhouse`, `#javascript`, `#database-client`, `#performance-optimization`, `#columnar-databases`

---

<a id="item-22"></a>
## [9lives: Self-Healing Test Runner for Playwright](https://github.com/Quality-Max/9lives) ⭐️ 7.0/10

9lives is a self-healing test runner for Playwright that automatically fixes broken selectors in two tiers—Tier 1 uses offline deterministic healing via page snapshots (data-testid > id > aria-label > text > class priority), while Tier 2 leverages existing Claude/Codex CLI subscriptions for structural changes. 这解决了一个关键痛点：编码代理经常因微小的 UI 变化而导致 Playwright 测试失败，造成不必要的测试失败。最关键的是，9lives 拒绝修复失败的断言——将它们视为潜在的真正 bug，而不是用自动重写的测试来掩盖。 Tier 1 works offline without LLM or network, healing most selector drift in seconds for free—no baseline DOM from previous runs required (unlike Healenium). Tier 2 uses your existing CLI subscriptions. The tool also supports Cypress and Selenium/pytest, includes MCP server for Claude Code/Cursor integration, and provides a unified diff workflow for approval.

rss · Hacker News - Show HN · Jul 10, 18:01

**Background**: Self-healing test automation addresses 'selector drift'—when UI changes cause previously working element locators to fail. Tools like Healenium use baseline DOM from previous green runs to find alternative locators. In modern development, coding agents (like Claude Code, Cursor) frequently modify UI code and inadvertently break tests, making this a growing pain point for teams using Playwright or Selenium.

<details><summary>References</summary>
<ul>
<li><a href="https://healenium.io/">Self - healing plugins for Selenium-based tests</a></li>
<li><a href="https://www.testsprite.com/use-cases/en/ai-frontend-testing-tool">AI Frontend Testing Tool | TestSprite</a></li>

</ul>
</details>

**Tags**: `#testing`, `#playwright`, `#developer-tools`, `#automation`, `#self-healing`

---

<a id="item-23"></a>
## [从零开始预训练，蚂蚁灵波发布具身原生世界动作模型LingBot-VA 2.0](https://www.infoq.cn/article/aU7GMFKF8qZRhT8VMWvY?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Ant Group's Ling波 (LingBot) releases LingBot-VA 2.0, an embodied native world action model trained from scratch, representing a notable advancement in embodied AI from a major Chinese technology company.

rss · InfoQ 中文站 · Jul 10, 15:14

**Tags**: `#embodied-ai`, `#world-models`, `#ant-group`, `#robotics`, `#ai-research`

---

<a id="item-24"></a>
## [Claude Rewrites Bun Runtime Codebase in 11 Days](https://www.infoq.cn/article/uHkOoJ6Nfm6wNCsUryuO?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Anthropic's Claude AI successfully rewrote major portions of the Bun JavaScript runtime's codebase in just 11 days, representing a significant demonstration of AI's capability to handle complex production-level software rewriting. This milestone demonstrates AI's growing sophistication in software engineering tasks, potentially transforming how developers approach large-scale code refactoring and modernization projects. It highlights the rapidly evolving landscape of AI-assisted development tools and raises questions about the future role of human developers in code maintenance. The rewrite involved substantial portions of Bun's codebase, with the founder taking a month to prepare before disclosing the changes publicly. Bun uses Safari's JavaScriptCore as its JavaScript engine, unlike Node.js and Deno which run on Google's V8 engine.

rss · InfoQ 中文站 · Jul 10, 13:21

**Background**: Bun is an all-in-one JavaScript runtime, package manager, and test runner designed as a drop-in replacement for Node.js. It uses JavaScriptCore as its JavaScript engine and is known for its fast performance, shipping as a single executable. Claude Code is Anthropic's agentic coding tool designed to help developers understand codebases, edit files, and run commands.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Claude`, `#Bun`, `#Code Generation`, `#Developer Tools`, `#JavaScript Runtime`

---

<a id="item-25"></a>
## [vLLM Inference Optimization for Multimodal Models at AICon Shenzhen](https://www.infoq.cn/article/ItOOYNuWf6t9KtfgeH7F?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

vLLM presented its practical inference optimization techniques specifically designed for multimodal vision-language models at the AICon Shenzhen conference, sharing real-world optimization experience from practitioners. This is significant because vLLM is a leading open-source LLM inference engine and multimodal models represent a major research frontier. Efficient inference is critical for deploying vision-language models in production, and this talk addresses practical challenges faced by developers. The presentation focused on optimization techniques for vision-language models, building on vLLM's core technologies like PagedAttention. Multimodal models face unique challenges compared to text-only LLMs due to the need to process both visual and textual inputs simultaneously.

rss · InfoQ 中文站 · Jul 10, 10:00

**Background**: vLLM is an open-source high-performance inference engine for large language models, known for its PagedAttention mechanism that enables efficient memory management during inference. Vision-language models (VLMs) combine visual understanding with language capabilities, requiring different optimization approaches than text-only models. AICon is a technical conference series focused on AI engineering practices.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/paged_attention/">Paged Attention - vLLM</a></li>
<li><a href="https://www.emergentmind.com/topics/crossvla">CrossVLA: Cross-Paradigm VLA Optimization</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#multimodal-models`, `#inference-optimization`, `#AI-performance`, `#LLM-serving`

---

<a id="item-26"></a>
## [Long March 10B Achieves World's First Net-Based Sea Recovery](https://weibo.com/7340734455/R814of1Ki) ⭐️ 7.0/10

On July 10, 2026, China's Long March 10B rocket successfully launched from the Hainan Commercial Space Launch Site. Approximately 6 minutes after first and second stage separation, the first stage returned vertically and was successfully captured on a sea recovery platform using a net-based system, marking the world's first net-based rocket recovery. This achievement marks China's first successful controlled recovery of a launch vehicle first stage, making the Long March 10B China's first reusable launch vehicle. As the world's first net-based rocket recovery, it demonstrates an alternative approach to booster reusability that could reduce launch costs and advance sustainable space access. The net-based recovery technology works similarly to carrier-based aircraft arrestor systems, using a net to capture the descending rocket stage. The Long March 10B is the world's first 5-meter diameter launch vehicle to perform a first stage recovery mission, representing a significant engineering milestone for China's reusable launch vehicle program.

telegram · zaihuapd · Jul 10, 04:36

**Background**: Reusable launch vehicle technology aims to recover and reuse rocket boosters after launch, significantly reducing the cost of access to space. Traditional SpaceX-style recovery uses vertical propulsive landing, while net-based recovery offers an alternative approach. China's space program has been developing this capability as part of its broader push toward commercial space operations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.news.cn/20260710/ba0ac14f31dd492aaf918e7a86ac844a/c.html">长 征 十 号 乙 首飞成功 我国 运 载 火 箭 首次实现可控回收-新华网</a></li>
<li><a href="https://www.guancha.cn/politics/2026_07_10_823266.shtml">长 征 十 号 乙 运 载 火 箭 成功实现一子级可控回收</a></li>
<li><a href="https://www.spacechina.com/n25/n2014789/n2414549/c4647268/content.html">长十乙首飞成功 我国首次实现运载 火 箭 可控 回 收 _中国航天科 技 集团</a></li>

</ul>
</details>

**Tags**: `#space`, `#rockets`, `#China`, `#reusable launch vehicles`, `#aerospace`

---

<a id="item-27"></a>
## [China's Network Identity System Hits 40M Users After One Year](https://www.ithome.com/0/975/337.htm) ⭐️ 7.0/10

China's National Network Identity Authentication Public Service has completed one year of operation since July 15, 2025, with 40 million digital identity applications, 280 million authentication services provided, and over 530 apps, mini-programs, and websites integrated. This represents China's first nationwide digital identity infrastructure, creating a unified authentication system that could reshape how nearly 1.4 billion people verify their identity online. The 'available but not visible' mechanism addresses critical privacy concerns while enabling government oversight, potentially serving as a model for other nations exploring digital identity frameworks. Major platforms including WeChat, QQ, Taobao, JD.com, and Douyin support one-click login; the national government service platform and 17 provincial-level apps, six state-owned banks, and Peking Union Medical College Hospital have connected. The authentication app has been downloaded 90 million times, with future expansion planned for Railway 12306.

telegram · zaihuapd · Jul 10, 14:01

**Background**: The National Network Identity Authentication Public Service is a system that generates unique 'network numbers' (网号) and 'network certificates' (网证) based on法定身份证件信息. It allows users to verify their identity on internet platforms without exposing their real-name information, solving the 'real name not real person' problem through an 'available but not visible' mechanism.

<details><summary>References</summary>
<ul>
<li><a href="https://m.gmw.cn/2025-05/17/content_1304038900.htm">m.gmw.cn/2025-05/17/content_1304038900.htm</a></li>
<li><a href="https://xinwen.bjd.com.cn/content/s6827f356e4b0380e186c425a.html">网 购害怕隐私泄露？ “ 国 家 网 络 身 份 认 证 ”来救场</a></li>

</ul>
</details>

**Tags**: `#digital-identity`, `#china-technology`, `#government-services`, `#privacy-security`, `#infrastructure`

---

<a id="item-28"></a>
## [Meta Faces €120B EU Fine for Addictive Facebook/Instagram Design](https://www.theverge.com/policy/963872/meta-eu-addictive-design-200b-fine-risk-digital-services-act-dsa) ⭐️ 7.0/10

The EU Commission preliminarily found that Meta's Facebook and Instagram violate the Digital Services Act through addictive design patterns including infinite scroll, autoplay, and engagement-driven algorithms. The tech giant faces a potential fine of up to €120 billion (6% of global annual revenue) if the findings are upheld. This represents the first major enforcement action under the EU's Digital Services Act targeting addictive design patterns, potentially creating a precedent for holding platforms accountable for user welfare impacts. The fine magnitude signals regulators are willing to impose severe financial consequences for design choices that manipulate user behavior. The EU requires Meta to redesign its apps by defaulting off infinite scroll and autoplay, implementing effective screen time breaks, and reducing algorithmic emphasis on engagement. The time limits Meta currently provides were characterized as ineffective. This is a preliminary finding, with Meta having opportunity to respond before a final decision.

telegram · zaihuapd · Jul 10, 14:47

**Background**: The Digital Services Act (DSA) is an EU regulation that entered into force in 2022, establishing comprehensive rules for platform accountability, content moderation, and transparency. It applies to all digital intermediary services including social networks, with the most stringent requirements for Very Large Online Platforms (VLOPs) with over 45 million monthly active users in the EU. The DSA allows fines up to 6% of global annual turnover for violations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_Services_Act_Regulation">Digital Services Act Regulation</a></li>
<li><a href="https://digital-strategy.ec.europa.eu/en/policies/digital-services-act">The Digital Services Act | Shaping Europe ’s digital future</a></li>

</ul>
</details>

**Tags**: `#digital-regulation`, `#platform-design`, `#meta`, `#user-welfare`, `#digital-services-act`

---

<a id="item-29"></a>
## [SK Hynix ADR Jumps 14% on NASDAQ Debut, Raises $26.5B Record](https://www.aljazeera.com/economy/2026/7/10/south-koreas-sk-hynix-raises-26-5bn-in-record-breaking-us-ipo) ⭐️ 7.0/10

SK Hynix began trading on NASDAQ through American Depositary Receipts (ADRs) on July 10, 2026, pricing at $149 per share and raising approximately $26.5 billion through the sale of 177.9 million ADRs, making it the largest foreign company listing in US history. This IPO reflects the explosive demand for AI infrastructure, as SK Hynix is the world's largest manufacturer of High Bandwidth Memory (HBM) chips used in Nvidia and AMD AI GPUs. The oversubscribed offering (7x+ demand) signals strong market confidence in the AI semiconductor supply chain. The ADR opened at approximately $170, up about 14% from the $149 IPO price, with intraday gains reaching over 15%. The listing surpassed Alibaba's 2014 record of $25 billion and ranks second globally only to SpaceX's $85.7 billion raise.

telegram · zaihuapd · Jul 10, 16:02

**Background**: HBM (High Bandwidth Memory) is a next-generation DRAM technology using 3D stacking architecture and Through-Silicon Via (TSV) technology to achieve high-speed data transmission. HBM provides the massive bandwidth required for AI model training and inference, making it critical for data centers and AI accelerators.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bnext.com.tw/story/17/what-is-hbm">HBM 是 什 麼？3D完全圖解，帶你一次看懂「記憶體全村希望」</a></li>
<li><a href="https://www.cnblogs.com/wujianming-110117/p/19019556">从概念到架构：一文彻底读懂 HBM 技 术 本质 - 吴建明wujianming - 博客园</a></li>
<li><a href="https://www.21ic.com/a/985500.html">为什么 HBM 高 带 宽 内 存 很重要？ 看完你就懂了 - 21ic电子网</a></li>

</ul>
</details>

**Tags**: `#IPO`, `#半导体`, `#AI芯片`, `#SK海力士`, `#HBM`, `#纳斯达克`

---

<a id="item-30"></a>
## [FCC Approves Giant Mirror Satellite to Reflect Sunlight at Night](https://www.techspot.com/news/113068-fcc-approves-giant-mirror-satellite-designed-beam-sunlight.html) ⭐️ 7.0/10

The FCC approved Reflect Orbital's demonstration satellite Eärendil-1, which will deploy an 18×18 meter aluminumized polyester reflective mirror in a near-polar orbit at approximately 625 km altitude to test reflecting sunlight toward Earth with a moving 5-kilometer-wide beam. This represents a pioneering test of space-based solar energy infrastructure. If successful, it could enable solar farms to continue generating electricity after sunset, while also raising significant concerns about light pollution affecting astronomy, wildlife, and aviation safety. The satellite will test "on-demand sunlight" for sale to solar farms, with potential applications in emergency response, construction, and military uses. Astronomers warn that if thousands of such mirrors are deployed, they could become the brightest human-made objects in orbit, severely interfering with telescope observations. The first two satellites will launch on SpaceX Falcon 9 rockets.

telegram · zaihuapd · Jul 10, 16:47

**Background**: Space-based solar power has been researched for decades, as sunlight in orbit is more intense than on Earth's surface due to the absence of atmospheric absorption. The European Space Agency has also been studying the feasibility of collecting solar energy in orbit and transmitting it to ground receivers. This demo represents a novel approach to extending terrestrial solar power generation into nighttime hours.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reflectorbital.com/">Reflect Orbital</a></li>
<li><a href="https://www.securities.io/ja/turning-night-into-day-the-ambitious-gamble-of-reflect-orbital/">夜を昼に変える: Reflect Orbital の野心的な賭け – Securities.io</a></li>
<li><a href="https://m.ithome.com/html/612169.htm">欧空局正研究在 轨 道 收集 太 阳 能 并将其传送到地面使用的可行性 - IT之家</a></li>

</ul>
</details>

**Tags**: `#space-technology`, `#renewable-energy`, `#satellite`, `#light-pollution`, `#orbital-infrastructure`

---