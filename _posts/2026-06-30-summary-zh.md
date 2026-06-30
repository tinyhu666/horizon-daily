---
layout: default
title: "Horizon Summary: 2026-06-30 (ZH)"
date: 2026-06-30
lang: zh
---

> 从 28 条内容中筛选出 17 条重要资讯。

---

1. [最高法院：地理围栏搜查令需宪法保障](#item-1) ⭐️ 9.0/10
2. [Google 的智能 AI 审稿人处理 1 万篇论文](#item-2) ⭐️ 9.0/10
3. [火箭实验室收购铱星公司，达成历史性交易](#item-3) ⭐️ 8.0/10
4. [大麻店身份证系统泄露百万护照](#item-4) ⭐️ 8.0/10
5. [Ornith-1.0：用于代理编程的开源 LLM 达到 SOTA](#item-5) ⭐️ 8.0/10
6. [Cerebras 与 OpenAI 交易致初创公司等待名单无限延长](#item-6) ⭐️ 8.0/10
7. [微型 Transformer 可视化，权重可实时编辑](#item-7) ⭐️ 8.0/10
8. [Qwen 3.6 27B：本地开发的甜点？高成本引争议](#item-8) ⭐️ 7.0/10
9. [新顶级域名 .self 旨在支持自托管](#item-9) ⭐️ 7.0/10
10. [为 SSH 添加原生图形化 Shell 的提议](#item-10) ⭐️ 7.0/10
11. [乔恩·尤德尔：将 AI 代理视为队友，而非循环](#item-11) ⭐️ 7.0/10
12. [EML 树被证明是通用逼近器](#item-12) ⭐️ 7.0/10
13. [HEMA 从业者创建开源数据集以促进 AI 剑术追踪](#item-13) ⭐️ 7.0/10
14. [人格与价值观测验助你找到最契合的 LLM](#item-14) ⭐️ 7.0/10
15. [因藏匿杂志被判 30 年引发言论自由担忧](#item-15) ⭐️ 6.0/10
16. [Simon Willison 发布 HTML 表格提取工具](#item-16) ⭐️ 6.0/10
17. [Hack Your Summer：免费学生生产冲刺](#item-17) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [最高法院：地理围栏搜查令需宪法保障](https://www.theguardian.com/us-news/2026/jun/29/supreme-court-geofence-warrants-case-decision) ⭐️ 9.0/10

美国最高法院于 2026 年 6 月 29 日裁定，地理围栏搜查令属于第四修正案规定的搜查行为，必须符合宪法保护要求，如具备可能原因和具体描述。 这一里程碑式的裁决极大地限制了执法机构在缺乏司法监督的情况下使用地理围栏搜查令的能力，强化了数百万美国人的数字隐私权。 大法官埃琳娜·卡根撰写了多数意见，认为个人对其聚合位置数据享有合理的隐私期待，即使这些数据是从谷歌等第三方收集而来的。

hackernews · cdrnsf · 6月29日 15:54 · [社区讨论](https://news.ycombinator.com/item?id=48720924)

**背景**: 地理围栏搜查令（或称反向位置搜查令）允许执法机构要求谷歌等科技公司提供犯罪现场虚拟边界内所有设备的数据。在此裁决之前，下级法院对此类搜查令是否违反第四修正案禁止不合理搜查的规定存在分歧。第四修正案要求搜查令必须基于可能原因，并具体描述搜查地点或逮捕对象。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Geofence_warrant">Geofence warrant</a></li>
<li><a href="https://www.theguardian.com/us-news/2026/jun/29/supreme-court-geofence-warrants-case-decision">US supreme court rules geofence warrants require constitutional privacy protections | US supreme court | The Guardian</a></li>
<li><a href="https://www.congress.gov/crs-product/LSB11274">Geofence Warrants and the Fourth Amendment | Congress.gov | Library of Congress</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了此案的广泛影响，一些人注意到法院引用了 Riley 诉 California 案等历史先例，而另一些人则质疑类似的推理是否适用于 Flock 摄像头等监控技术。还有用户提供了一个例子，说明即使没有地理围栏搜查令，位置数据也可用于识别嫌疑人。

**标签**: `#privacy`, `#surveillance`, `#supreme court`, `#digital rights`, `#law enforcement`

---

<a id="item-2"></a>
## [Google 的智能 AI 审稿人处理 1 万篇论文](https://www.reddit.com/r/MachineLearning/comments/1uio9rb/googles_agentic_peerreviewer_handled_10k_papers/) ⭐️ 9.0/10

Google 在顶级计算机科学会议 ICML 和 STOC 上部署了智能 AI 审稿人，以每篇 30 分钟的速度处理了约 1 万篇论文，正式研究论文表明，它比零样本提示多检测出 34%的数学错误。 这展示了人工智能在自动化学术同行评审中的首次大规模部署，为减少评审者工作量和提高错误检测准确性树立了先例。它可能改变会议处理论文评估的方式，但公平性和可靠性问题仍然存在。 该系统是一种“智能型”AI，能够自主感知、推理和行动以完成任务。与零样本提示基线相比，它在捕捉数学错误方面提高了 34%，凸显了多步推理相较于单次提示的优势。

reddit · r/MachineLearning · /u/Justgototheeffinmoon · 6月29日 10:05

**背景**: 智能型 AI 指的是能够独立设定目标、做出决策并采取行动以达成用户定义目标的系统，而非简单的聊天机器人式回应。传统的 AI 同行评审工具通常依赖零样本提示，即模型在无迭代推理的情况下仅接受单一指令，这可能会遗漏细微错误。该系统采用更自主的工作流程，能够捕捉数学证明和方程中更隐蔽的错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.relativity.com/blog/agentic-ai-is-in-the-air/">Agentic AI is in the aiR | Relativity Blog</a></li>
<li><a href="https://www.fastcompany.com/91246740/true-ai-agents-are-agentic-ai-not-just-dressed-up-rag">True AI agents are agentic AI , not just dressed-up RAG</a></li>

</ul>
</details>

**社区讨论**: 新闻条目中未提供社区评论，因此无法总结观点。但根据高分和新颖性，Reddit 社区可能对规模和方法表示兴奋，同时也提出了对 AI 偏见和可能取代人类评审者的担忧。

**标签**: `#AI`, `#peer review`, `#research automation`, `#machine learning`, `#Google`

---

<a id="item-3"></a>
## [火箭实验室收购铱星公司，达成历史性交易](https://investors.rocketlabcorp.com/news-releases/news-release-details/rocket-lab-acquire-iridium-historic-deal-creating-fully) ⭐️ 8.0/10

火箭实验室宣布收购铱星通信公司，打造一家完全整合的太空通信企业。该交易将火箭实验室的发射能力与铱星的卫星星座及服务相结合。 此次收购使火箭实验室成为航天领域垂直整合的参与者，可能颠覆卫星通信市场。它为火箭实验室提供了稳定的发射需求，并获取了铱星宝贵的频谱资源和客户基础。 收购包括铱星在轨运行的 66 颗低轨卫星星座及其频谱许可证。火箭实验室计划利用其 Electron 火箭和未来的 Neutron 火箭为铱星提供下一代卫星替换服务。

hackernews · everfrustrated · 6月29日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=48719485)

**背景**: 火箭实验室是一家美国航空航天公司，以其 Electron 小型卫星运载火箭知名。铱星通信公司运营全球卫星网络，提供语音和数据服务，主要用于卫星电话和物联网连接。这笔交易类似于 SpaceX 利用 Starlink 稳定发射需求的策略，但规模较小。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Iridium_satellite_constellation">Iridium satellite constellation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rocket_Lab_Electron">Rocket Lab Electron - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论中有人担忧发射更多卫星会增加太空垃圾，但也有人注意到这与 SpaceX 的 Starlink 模式有战略相似之处。一些人认为这是火箭实验室确保基础发射需求并增加内部卫星制造的明智之举。还有关于火箭实验室从新西兰起源转向成为美国实体的讨论。

**标签**: `#aerospace`, `#satellite`, `#acquisition`, `#RocketLab`, `#Iridium`

---

<a id="item-4"></a>
## [大麻店身份证系统泄露百万护照](https://www.theverge.com/tech/947157/passports-data-breach-cannabis-club-systems-nefos-puffpal) ⭐️ 8.0/10

用于大麻店应用 PuffPal 的身份验证系统 Nefos 发生数据泄露，超过一百万张用于年龄验证的护照扫描件被泄露。泄露内容包括高分辨率护照图像和用户个人信息。 此次泄露凸显了在低安全性系统中使用护照等高价值凭证的危险，可能导致大规模身份盗窃。它强调了在辅助验证系统中需要更好的安全实践和最小化数据保留。 研究人员 Azdoufal 发现 Nefos 系统没有有效的安全措施，数据无需身份验证即可访问。泄露还显示护照数据在验证后被保留，违反了数据最小化原则。

hackernews · jruohonen · 6月28日 11:22 · [社区讨论](https://news.ycombinator.com/item?id=48706389)

**背景**: 许多大麻店使用第三方年龄验证系统以符合法律要求。这些系统通常收集和存储敏感身份证件，但可能缺乏强大的安全保护。PuffPal 是一款使用 Cannabis Club Systems 软件连接用户与大麻俱乐部的应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.resetera.com/threads/a-million-passports-for-online-age-verification-have-been-hacked-leaked.1563271/">A million passports for online age verification have been... | ResetEra</a></li>
<li><a href="https://daringfireball.net/linked/2026/06/28/puffpal-passport-leak">Daring Fireball: PuffPal , an App for Accessing Cannabis Clubs...</a></li>
<li><a href="https://puffpal.app/">PuffPal app - Discover, Connect, Elevate - Puffpal</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了类似护照泄露的经历，例如来自旅游 CRM 系统和未受保护的 S3 存储桶，质疑系统为何在验证后保留数据。有人指出护照复印件常被酒店存储，引发对广泛身份盗窃风险的担忧。

**标签**: `#data breach`, `#cybersecurity`, `#passport`, `#privacy`, `#identity theft`

---

<a id="item-5"></a>
## [Ornith-1.0：用于代理编程的开源 LLM 达到 SOTA](https://simonwillison.net/2026/Jun/29/ornith/#atom-everything) ⭐️ 8.0/10

DeepReinforce 发布了 Ornith-1.0，这是一系列基于 Gemma 4 和 Qwen 3.5 的开源权重、MIT 许可的 LLM（9B、31B、35B MoE、397B MoE），在同等规模的开源模型中，于编程基准测试上取得了最先进的性能。 该发布为代理编程任务提供了强大的开源替代方案，可能降低开发者对本地高性能代码生成模型的需求门槛。其自脚手架能力有望在不依赖外部工具的情况下提升多步推理表现。 Ornith-1.0 采用了一种“自脚手架”强化学习方法，模型自行生成脚手架以改进迭代代码生成。35B MoE 变体可通过 GGUF 在消费级硬件上本地运行，图像生成速度达到 103 token/秒，并且由于思维链更短，速度明显快于 Qwen 3.6 35B。

rss · Simon Willison · 6月29日 16:17

**背景**: 代理编程是指利用 LLM 和 AI 代理自主执行多步软件开发任务。自脚手架是一种通过强化学习让 LLM 迭代优化自身输出的技术，生成“脚手架”以指导后续步骤。混合专家（MoE）架构每次只激活部分参数，平衡了性能与效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/data-science-in-your-pocket/ornith-1-0-self-learning-llm-for-coding-318c9a830bfc">Ornith 1.0 : Self Learning LLM for Coding | by Mehul Gupta | Medium</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agentic_coding">Agentic coding</a></li>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts">A Visual Guide to Mixture of Experts (MoE)</a></li>

</ul>
</details>

**社区讨论**: 早期用户报告 Ornith-1.0 35B 在编程任务中优于 Qwen 3.6 35B，且由于思维链更短，速度快达 3 倍。但也有用户指出其在无工具聊天时表现欠佳且易产生幻觉，此外对 DeepReinforce 的背景以及自脚手架的具体工作原理仍存疑问。

**标签**: `#LLM`, `#open-source`, `#code generation`, `#agentic coding`, `#machine learning`

---

<a id="item-6"></a>
## [Cerebras 与 OpenAI 交易致初创公司等待名单无限延长](https://www.reddit.com/r/MachineLearning/comments/1uiqhiv/cerebras_openai_deal_capacity_has_effectively/) ⭐️ 8.0/10

一名 Reddit 用户报告称，Cerebras 与 OpenAI 的协议（据报道价值 200 亿美元）已将 Cerebras 近期几乎所有的推理能力预留给 OpenAI，使得其他用户——特别是小型初创公司——的 API 等待名单实际上无限延长。 这种 AI 计算能力的集中威胁到了依赖专用高吞吐量推理硬件的初创公司的生存，加剧了 AI 生态系统中计算资源垄断的风险。 该交易涉及 OpenAI 购买价值 200 亿美元的 Cerebras 芯片，这些芯片是为高吞吐量推理设计的晶圆级 ASIC；该用户的初创公司需要每秒 1-2 千 token 的持续吞吐量以及严格的 p95 延迟。

reddit · r/MachineLearning · /u/Kortopi-98 · 6月29日 12:00

**背景**: Cerebras 生产晶圆级引擎（WSE-3），这是有史以来最大的芯片，专为细粒度并行性和高吞吐量推理而设计。与通用 GPU 不同，像 Cerebras 这样的专用 ASIC 可以在特定工作负载上实现更高的效率。P95 延迟是一个指标，表示 95%请求的响应时间阈值，对于实时应用至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cerebras.ai/chip">Product - Chip - Cerebras</a></li>
<li><a href="https://nexaninsights.beehiiv.com/p/ai-chips-nvidia-and-a-game-of-inference">ASIC vs GPU in a Clown Car</a></li>
<li><a href="https://redis.io/blog/p95-latency/">P 95 Latency : What It Is & Why It Matters</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#Cerebras`, `#OpenAI`, `#inference`, `#startup challenges`

---

<a id="item-7"></a>
## [微型 Transformer 可视化，权重可实时编辑](https://www.reddit.com/r/MachineLearning/comments/1uhw7fu/i_shrank_a_transformer_until_every_number_fitted/) ⭐️ 8.0/10

一位软件工程师创建了一个单文件 HTML 页面，可视化了一个完整但微型的 Transformer（6 个词的词汇表，3 维嵌入），其中每个权重和向量都可编辑，前向传播会实时重新计算。 该工具让学习者能够直观地理解 Transformer 的内部机制，无需任何库即可动手实验 QKV 注意力、因果掩码和前馈网络。 该 Transformer 只有一个注意力头和一个块，使用随机未训练的权重，并故意省略了反向传播。它作为一个独立的 HTML 文件，没有外部依赖。

reddit · r/MachineLearning · /u/DanielMoGo · 6月28日 12:35

**背景**: Transformer 是现代大型语言模型的基础；它们使用包含查询、键和值的自注意力机制，以及因果掩码来防止关注未来的词元。这个交互工具通过将模型缩小到最小但可工作的规模，简化了这些概念。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://machinelearningmastery.com/a-gentle-introduction-to-attention-masking-in-transformer-models/">A Gentle Introduction to Attention Masking in Transformer Models - MachineLearningMastery.com</a></li>
<li><a href="https://www.anthonychiu.xyz/blog/attention-mechanism">Attention Mechanism - What are Query , Key , and Value ?</a></li>

</ul>
</details>

**标签**: `#transformer`, `#visualization`, `#education`, `#interactive`, `#machine learning`

---

<a id="item-8"></a>
## [Qwen 3.6 27B：本地开发的甜点？高成本引争议](https://quesma.com/blog/qwen-36-is-awesome/) ⭐️ 7.0/10

Qwen 3.6 27B 是阿里巴巴于 2026 年 4 月发布的稠密 270 亿参数语言模型，因其大小与性能的平衡而被誉为本地开发的理想选择。然而，社区评论揭示了在本地运行该模型时巨大的硬件成本与性能权衡。 这场辩论凸显了本地 AI 部署的优势（隐私、离线访问）与运行高性能模型所需的高昂硬件投资之间的持续矛盾。它影响着开发者决定是投资昂贵的本地设备，还是依赖像 OpenRouter 这样廉价的云 API 服务。 Qwen 3.6 27B 模型拥有 262,144 个 token 的上下文窗口，支持多 token 预测（MTP），采用 Apache-2.0 许可证。要在本地以不错的速度运行，建议至少需要 16GB VRAM（量化后）或 64GB 统一内存；一台 128GB 内存的 MacBook Pro 起售价为 6,699 美元。

hackernews · stared · 6月29日 17:05 · [社区讨论](https://news.ycombinator.com/item?id=48721903)

**背景**: 在本地运行大型语言模型需要大量硬件资源，尤其是内存（VRAM 或统一内存）。一个粗略的经验法则是：4 位量化的 7B 模型需要约 4-6GB，而 27B 模型 4 位量化需要约 14-16GB。云 API 提供更便宜的替代方案，按 token 收费，但牺牲了隐私和离线能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/qwen/qwen3.6-27b">Qwen 3 . 6 27 B - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://www.runlocalai.co/models/qwen-3-6-27b-mtp">Qwen 3 . 6 27 B (MTP) — local inference guide | RunLocalAI</a></li>
<li><a href="https://www.geeksforgeeks.org/deep-learning/recommended-hardware-for-running-llms-locally/">Recommended Hardware for Running LLMs Locally - GeeksforGeeks</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂：部分用户认可模型性能，但警告不要为本地 LLM 工作购买昂贵的 MacBook Pro，指出其散热和噪音问题。其他人则认为像 OpenRouter 这样的云 API 性价比更高，10 美元就能使用像 DeepSeek V4 Flash 这样的更大模型。少数用户质疑本地模型在实际编码任务中的实用价值，指出零样本新项目例子并不具有代表性。

**标签**: `#LLM`, `#local development`, `#Qwen`, `#hardware`, `#AI deployment`

---

<a id="item-9"></a>
## [新顶级域名 .self 旨在支持自托管](https://hccf.onmy.cloud/2026/06/21/reclaiming-our-digital-selves-hccfs-vision-for-a-human-centered-top-level-domain/) ⭐️ 7.0/10

HCCF 提出了一项新顶级域名 '.self' 的提案，为每人提供一个免费域名，以促进自托管。该计划包括禁止停放、抢注和转售的规定。 该顶级域名可通过赋予个人对其在线身份的控制权、不依赖商业注册商，从而使网络托管民主化。然而，其成功取决于解决曾困扰类似免费域名计划的滥用和身份验证挑战。 .self 顶级域名需要经过密码学身份验证流程以防止抢注，闲置域名可能在宽限期后被收回。域名的运营资金尚未明确，引发了可持续性方面的质疑。

hackernews · HumanCCF · 6月29日 19:49 · [社区讨论](https://news.ycombinator.com/item?id=48724230)

**背景**: 顶级域名是域名最后一部分，例如 .com 或 .org。自托管是指运行自己的网络服务器，而非使用托管服务。过去的免费顶级域名计划（如 .tk）曾遭遇广泛滥用，并最终被安全软件列入黑名单。

**社区讨论**: 社区成员表达了怀疑，指出之前的免费顶级域名（如 .tk）因滥用而失败。一些人建议使用声誉系统或挑战闲置域名作为对抗性删除的替代方案。

**标签**: `#TLD`, `#self-hosting`, `#domain names`, `#internet governance`

---

<a id="item-10"></a>
## [为 SSH 添加原生图形化 Shell 的提议](https://probablymarcus.com/blocks/2026/06/28/native-graphical-shell-for-SSH.html) ⭐️ 7.0/10

Marcus Lewis 提议扩展 SSH 以支持原生图形化 Shell，并发布了实现这一概念的开源工具 Outer Shell。 这挑战了 SSH 仅服务于文本界面的长期假设，有望在不依赖 X11 转发或基于 Web 的解决方案的情况下，实现更丰富的远程桌面体验。 Outer Shell 作为一个 SSH 浏览器工作，转发图形显示层而不仅仅是 PTY，并且是开源的。批评者指出，现有的 X11 转发和 HTML5 Web 应用已经满足了类似需求。

hackernews · mrcslws · 6月29日 15:42 · [社区讨论](https://news.ycombinator.com/item?id=48720758)

**背景**: SSH 是一种安全远程访问协议，传统上通过伪终端（PTY）提供命令行（TUI）访问。文本用户界面（TUI）依赖终端能力，而图形用户界面（GUI）需要像 X11 或 Wayland 这样的显示服务器。该提议设想一种原生图形化 Shell，可无缝集成到 SSH 中，超越纯 TUI 模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Text-based_user_interface">Text-based user interface - Wikipedia</a></li>
<li><a href="https://probablymarcus.com/blocks/2026/06/28/native-graphical-shell-for-SSH.html">A native graphical shell for SSH | Marcus Lewis</a></li>
<li><a href="https://news.ycombinator.com/item?id=48720758">A native graphical shell for SSH | Hacker News</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论呈现分歧：一些人认为这是对现有方案（如 X11 转发）的重复发明，而另一些人则认为 TUI 并非天生优越，SSH 应原生支持 GUI 显示层。多位用户提到了 webtop 容器和 WebDAV 等图形化远程访问的替代方案。

**标签**: `#SSH`, `#GUI`, `#Terminal`, `#Remote Access`, `#User Interface`

---

<a id="item-11"></a>
## [乔恩·尤德尔：将 AI 代理视为队友，而非循环](https://simonwillison.net/2026/Jun/28/jon-udell/#atom-everything) ⭐️ 7.0/10

乔恩·尤德尔认为，“人在循环中”这一说法将权威让给了机器，并提出将 AI 代理视为软件开发中受邀的队友。他强调，代理辅助过程不应是黑箱，而应是透明的协作。 这种重新定义将叙事从人类监督转向人机伙伴关系，可能影响开发者如何看待和采用 AI 编码代理。它鼓励在代理驱动的开发工作流程中建立透明度和信任。 尤德尔的论点是对代理生成不可审查的拉取请求这一担忧的回应。他主张将代理邀请到现有的人类工作流程中，而不是创建一个单独的循环。

rss · Simon Willison · 6月28日 21:57

**背景**: AI 代理是可以执行代码生成和测试等任务的自主软件程序。“人在循环中”的概念通常将人类作为 AI 行动的监督者，但批评者认为这可能会削弱人的主体性。代理驱动型软件开发将 AI 代理整合到软件开发生命周期中，引发了关于控制与协作的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/ai-agents">What Are AI Agents ? | IBM</a></li>
<li><a href="https://www.ness.com/blog/what-is-agentic-software-development/">Agentic Software Development : Beyond Metrics and Speed</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#software development`, `#human-in-the-loop`, `#developer tools`

---

<a id="item-12"></a>
## [EML 树被证明是通用逼近器](https://www.reddit.com/r/MachineLearning/comments/1uipl1t/eml_trees_are_universal_approximators_r/) ⭐️ 7.0/10

一篇新论文证明，EML 树（一种初等函数的组合表示）是通用逼近器，能够以任意精度逼近任何连续函数。 这一理论结果连接了符号函数表示与神经网络通用逼近，可能为机器学习中的新型混合架构或理论见解提供启发。 证明显式构造了二元运算、多项式、双曲正切和近似单位划分的 EML 表示，将其作为积木块。它还通过基于符号的分解和仿射映射处理了自然对数对非正输入的定义不良问题。

reddit · r/MachineLearning · /u/JoeGermany · 6月29日 11:16

**背景**: 通用逼近定理指出，某些函数族（如神经网络）可以任意好地逼近任何连续函数。EML 函数是一种单一的二元运算，可以通过组合表示所有初等函数。本文扩展了这一思想，证明了 EML 运算构成的树也是通用逼近器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2606.23179">EML Trees Are Universal Approximators</a></li>
<li><a href="https://en.wikipedia.org/wiki/Universal_approximation_theorem">Universal approximation theorem - Wikipedia</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#universal approximation`, `#function approximation`, `#EML trees`, `#theoretical ML`

---

<a id="item-13"></a>
## [HEMA 从业者创建开源数据集以促进 AI 剑术追踪](https://www.reddit.com/r/MachineLearning/comments/1uivddx/i_do_historical_swordfighting_and_noticed_ai/) ⭐️ 7.0/10

一名历史欧洲武术（HEMA）从业者正在构建一个开源的剑术多视角数据集，旨在帮助计算机视觉模型追踪快速移动的细长物体，如钢剑。 该数据集针对细长物体追踪和运动模糊等计算机视觉难题，对于弥合具身 AI 中的模拟到现实差距至关重要，还可能促成 HEMA 比赛的自动计分系统。 该数据集将包含 100 个超精简片段，以 120/240 帧每秒的多角度同步拍摄，标注了生物力学、遮挡等级以及剑和击剑手的 2D 关键点。

reddit · r/MachineLearning · /u/fonssagrives · 6月29日 15:16

**背景**: 模拟到现实差距（Sim2Real gap）指 AI 模型在虚拟环境中训练后难以适应混乱现实条件（如变化的光照和遮挡）的问题。细长物体追踪尤其困难，因为剑之类的细长物体常降至像素分辨率以下或产生运动模糊。HEMA 涉及使用钢制武器进行的快速复杂动作，是计算机视觉的理想测试平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://underline.io/lecture/9042-exploring-the-sim-2-real-gap-in-vision-and-language-navigation">Exploring the Sim - 2 - Real Gap in Vision-and-Language Navigation</a></li>
<li><a href="https://sertiscorp.medium.com/an-overview-of-object-tracking-use-cases-challenges-and-applications-f5689794c3ba">An Overview of Object Tracking : Use Cases, Challenges... | Medium</a></li>

</ul>
</details>

**标签**: `#computer vision`, `#dataset`, `#embodied AI`, `#tracking`, `#HEMA`

---

<a id="item-14"></a>
## [人格与价值观测验助你找到最契合的 LLM](https://www.reddit.com/r/MachineLearning/comments/1uin5ad/i_made_a_quiz_that_tells_you_which_llm_you_align/) ⭐️ 7.0/10

该工具提供了一种理解 LLM 之间价值观差异的新颖方式，这对 AI 对齐和负责任部署至关重要。它揭示了尽管 LLM 基于相似数据训练，但展现出不同的道德立场，这可能影响其实际应用。 该测验使用了 117 个无上下文、无状态的问题，每个问题至少询问 5 次（最多 50 次）以确保可靠性。模型在包括大五人格、道德基础理论和 HEXACO 等人格框架上进行了测试。值得注意：Grok 4.3 是唯一反对对亿万富翁征税的模型，GPT-4o 独树一帜地认为回形针行动在道德上合理。

reddit · r/MachineLearning · /u/DarkyPaky · 6月29日 09:00

**背景**: 回形针行动是美国在二战后秘密招募超过 1600 名来自纳粹德国的科学家的计划，其中许多人具有纳粹背景，引发了伦理争议。该测验通过比较 LLM 对此类道德困境的回答来评估价值观对齐。数据集和详细的模型档案已在网站上公开。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Operation_Paperclip">Operation Paperclip</a></li>
<li><a href="https://runware.ai/models/xai-grok-4-3">Grok 4 . 3 AI Text Generator | Runware</a></li>

</ul>
</details>

**标签**: `#LLM`, `#personality`, `#values`, `#quiz`, `#AI alignment`

---

<a id="item-15"></a>
## [因藏匿杂志被判 30 年引发言论自由担忧](https://theintercept.com/2026/06/26/daniel-sanchez-estrada-zines-prairieland-free-speech/) ⭐️ 6.0/10

一名联邦法官因丹尼尔·桑切斯-埃斯特拉达隐藏联邦搜查令追寻的杂志而判处其 30 年监禁，引发对言论自由侵犯的愤怒。 这一异常严厉的判决为持有或分发争议出版物的人树立了令人不寒而栗的先例，可能将普通的政治表达定为犯罪。 30 年刑期是因为藏匿文件，而非任何暴力行为；原定罪行估计为 75 年，而桑切斯-埃斯特拉达并非抗议活动中射伤联邦特工的枪手。

hackernews · xrd · 6月28日 21:42 · [社区讨论](https://news.ycombinator.com/item?id=48711981)

**背景**: Zines（发音为'zeens'）是非商业性、通常自制的出版物，关注小众或非常规主题，历史上被政治和反文化运动广泛使用。该案涉及针对反法西斯活动人士的联邦搜查令，引发了对政府越权以及如何处理与表达性材料相关证据的质疑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zine">Zine - Wikipedia</a></li>
<li><a href="https://mixam.com/blog/education/what-is-a-zine">What is a Zine ? | Defining Zines | History & Impact | Mixam</a></li>
<li><a href="https://fliplink.me/blog/what-is-a-zine">What Is a Zine ? Definition , History, and Modern Examples | FlipLink</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为 30 年刑期过于严厉，有人指出司法系统固有的偏见以及对言论自由的潜在寒蝉效应。也有人指出，根据搜查令隐藏证据构成妨碍司法，但极端刑期表明司法保护出现了裂痕。

**标签**: `#free speech`, `#legal`, `#hackernews`, `#civil liberties`, `#sentencing`

---

<a id="item-16"></a>
## [Simon Willison 发布 HTML 表格提取工具](https://simonwillison.net/2026/Jun/29/html-table-extractor/#atom-everything) ⭐️ 6.0/10

Simon Willison 发布了一个名为 HTML Table Extractor 的新粘贴转换工具，它能接受嵌入 HTML 表格的富文本，并将其转换为 HTML、Markdown、CSV、TSV 或 JSON 格式。 该工具为开发者和数据分析师简化了从网页提取数据的过程，提供多种输出格式以实现灵活使用，并展示了与 Wikipedia 的 CORS API 的实用集成。 该工具可以利用 Wikipedia 开放的 CORS API 自动获取页面中的表格，界面以带复制按钮的标签面板显示结果。

rss · Simon Willison · 6月29日 23:38

**背景**: 粘贴转换工具允许用户从浏览器复制富内容，并将其转换为结构化格式而无需编写代码。HTML 表格是网页上常见的表格数据形式，但将其提取为 CSV 或 JSON 等可复用格式通常需要手动操作或编写脚本。

**标签**: `#tool`, `#html`, `#table`, `#csv`, `#conversion`

---

<a id="item-17"></a>
## [Hack Your Summer：免费学生生产冲刺](https://simonwillison.net/2026/Jun/28/hack-your-summer/#atom-everything) ⭐️ 6.0/10

Hack Your Summer 是一项为期 4 周的免费夏季生产冲刺活动，面向本科生、研究生和应届毕业生，是对当前实习短缺危机的回应。第二期将于 7 月 13 日开始，申请截止日期为 7 月 8 日。 该计划为未能获得有限实习机会的学生提供了替代途径，帮助他们构建真实项目并获得经验。它解决了当前学生就业市场中的一个关键缺口。 参与者将在导师和同伴的支持下，学习识别项目、稳步推进，并创作出可用于展示的公开作品。该项目对学生免费，同时也在招募志愿者担任导师。

rss · Simon Willison · 6月28日 19:26

**背景**: 由于经济压力，许多美国公司减少了实习项目，导致学生获得实践经验的机会减少。Hack Your Summer 旨在通过提供结构化的、有导师支持的生产冲刺活动来填补这一空白，学生可以在此构建真实项目以展示给雇主。

**标签**: `#education`, `#internships`, `#student programs`, `#summer sprint`

---