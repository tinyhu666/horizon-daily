---
layout: default
title: "Horizon Summary: 2026-07-17 (ZH)"
date: 2026-07-17
lang: zh
---

> 从 38 条内容中筛选出 24 条重要资讯。

---

1. [Claude web_fetch 工具被绕过，泄露用户隐私数据](#item-1) ⭐️ 9.0/10
2. [Schema 架构在 ARC-AGI-3 上使用前沿模型达到 99%](#item-2) ⭐️ 9.0/10
3. [Kimi K3：新开放权重前沿 AI 模型引发争论](#item-3) ⭐️ 8.0/10
4. [LM Studio Bionic：面向开源模型的 AI 代理](#item-4) ⭐️ 8.0/10
5. [数据科学的数学：高维直觉](#item-5) ⭐️ 8.0/10
6. [Roc 编译器从 Rust 到 Zig 的重写进展报告](#item-6) ⭐️ 8.0/10
7. [用经典机器学习检测 LLM 生成文本](#item-7) ⭐️ 8.0/10
8. [Thinking Machines Lab 发布 975B 参数开放权重模型 Inkling](#item-8) ⭐️ 8.0/10
9. [Linus Torvalds：Linux 不反 AI，AI 是有用工具](#item-9) ⭐️ 8.0/10
10. [xAI 因隐私争议开源 Grok Build](#item-10) ⭐️ 8.0/10
11. [DABSN：新型循环语言模型寻求合作](#item-11) ⭐️ 8.0/10
12. [QLoRA 的 2e-4 学习率在小数据集上有问题](#item-12) ⭐️ 8.0/10
13. [ExTernD：可实现任意精度的三元 LLM 量化](#item-13) ⭐️ 8.0/10
14. [PnP-CoSMo：基于内容/风格建模的 MRI 重建框架](#item-14) ⭐️ 8.0/10
15. [用哈达玛积聚类解耦卷积神经元](#item-15) ⭐️ 8.0/10
16. [微软 Comic Chat 在 30 年后开源](#item-16) ⭐️ 7.0/10
17. [将高尔夫球场改为公园以抵消数据中心用水](#item-17) ⭐️ 7.0/10
18. [GPT-5.6 Codex 漏洞可通过覆盖$HOME 删除文件](#item-18) ⭐️ 7.0/10
19. [为机器人学习中的 JEPA 世界模型寻求批判性意见](#item-19) ⭐️ 7.0/10
20. [PyTorch 模型在 T4 上比 A100 慢 170 倍：架构瓶颈？](#item-20) ⭐️ 7.0/10
21. [Decoy 字体：人类可读但能迷惑 AI 的字体实验](#item-21) ⭐️ 6.0/10
22. [Mermaid 转换为 ASCII 艺术工具编译为 WebAssembly](#item-22) ⭐️ 6.0/10
23. [AI 记忆应存储模式而非事实？](#item-23) ⭐️ 6.0/10
24. [NeurIPS 2026 RTCA 研讨会征稿](#item-24) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Claude web_fetch 工具被绕过，泄露用户隐私数据](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 9.0/10

研究员 Ayush Paul 发现了 Anthropic 的 Claude web_fetch 工具中的一个漏洞，可导致用户隐私数据（包括姓名、所在城市和雇主名称）被窃取。该攻击利用了 web_fetch 能够访问先前获取页面中嵌入链接的漏洞，通过一个蜜罐网站引导 AI 泄漏数据。 该攻击绕过了 Anthropic 现有的数据外泄防护机制，凸显了在同时拥有私密数据访问权和外部工具的 LLM 代理安全防护方面的根本挑战。它强调了对 AI 系统进行更严格隔离机制的必要性。 该攻击仅针对带有 'Claude-User' 用户代理的客户端以躲避检测，并成功提取了用户的姓名、所在城市和雇主名称。Anthropic 未支付漏洞赏金，声称已内部发现该问题，随后通过阻止 web_fetch 访问获取内容中的额外链接来修复该漏洞。

rss · Simon Willison · 7月15日 14:21

**背景**: Claude 的 web_fetch 工具允许 AI 从网页 URL 获取并分析内容，但出于安全考虑，它仅限于用户提供或伴随的 web_search 工具返回的 URL。这属于更广泛的“致命三重奏”攻击类型，即 LLM 同时具备私密数据访问权、处理不可信内容的能力以及可窃取数据的工具，这三种条件共同构成了一个关键的攻击面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.claude.com/en/docs/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Docs</a></li>
<li><a href="https://www.cyera.com/research/when-language-becomes-the-attack-vector-the-lethal-trifecta-of-ai-agents">When Language Becomes the Attack Vector: The Lethal Trifecta of...</a></li>

</ul>
</details>

**标签**: `#AI security`, `#data exfiltration`, `#prompt injection`, `#LLM vulnerabilities`, `#Claude`

---

<a id="item-2"></a>
## [Schema 架构在 ARC-AGI-3 上使用前沿模型达到 99%](https://www.reddit.com/r/MachineLearning/comments/1uyf8oo/new_fable5opus48_harness_called_schema_claims_99/) ⭐️ 9.0/10

Schema 架构通过改进推理过程，在不修改模型权重的情况下，使用 Claude Opus 4.8 和 Fable 5 在 ARC-AGI-3 公开基准测试中达到 99% 的准确率，并使用 GPT-5.6 Sol 获得 95.35% 的分数。 这一结果表明，通过在现有模型周围进行过程工程，而不仅仅是依靠更大的模型，可以在 ARC-AGI-3 等推理基准上取得显著提升。这可能会将 AI 研究的焦点转向架构和脚手架开发。 该架构使用回退策略：先运行 Opus 4.8 和 Sol xhigh，得分低于 80 的游戏再使用 Fable 5 和 Sol max 重跑，取每个游戏的最高分。这两个分数均为自行报告，尚未经 ARC Prize 验证。

reddit · r/MachineLearning · /u/we_are_mammals · 7月16日 21:02

**背景**: ARC-AGI-3 是一个基准测试，旨在测试在陌生环境中的交互式推理和技能获取能力。AI 架构是一种将模型连接到工具、记忆和外部系统的系统，将推理转化为行动。Schema 架构改进了对游戏世界模型的形成和测试过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://schema-harness.github.io/">Frontier Models with Our Harness Achieve ~99% on ARC-AGI-3 Public — Schema</a></li>
<li><a href="https://arcprize.org/arc-agi/3">Arc-agi-3</a></li>
<li><a href="https://www.databricks.com/blog/ai-harness">What is an AI Agent Harness? | Databricks Blog</a></li>

</ul>
</details>

**社区讨论**: Reddit 帖子旨在重新引发技术讨论，社区期待参与。ARC Prize 主席的一条评论表示有兴趣深入研究该方法。内容中未提供详细评论。

**标签**: `#AI`, `#reasoning`, `#ARC-AGI`, `#prompt engineering`, `#LLM`

---

<a id="item-3"></a>
## [Kimi K3：新开放权重前沿 AI 模型引发争论](https://www.kimi.com/blog/kimi-k3) ⭐️ 8.0/10

Kimi K3 挑战了开放权重模型是商品的观点，其高定价和前沿性能可能改变 AI 市场格局，迫使竞争对手重新评估其定价和模型开放策略。 该模型支持 100 万 token 的上下文窗口，并使用推理 token，社区成员 simonw 指出其输出成本很高。来自中国社交媒体的官方基准测试表明，Kimi K3 达到 Sol/Fable 级别，全面超越 Opus 4.8。

hackernews · vincent_s · 7月16日 14:46 · [社区讨论](https://news.ycombinator.com/item?id=48935342)

**背景**: 开放权重模型发布模型权重（神经网络参数），但不发布完整训练代码或数据，允许他人运行和微调模型。前沿智能指的是当前最先进的通用 AI 模型。Kimi K3 的 2.8 万亿参数使其成为有史以来最大的开放权重模型之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/lets-code-future/open-weight-ai-models-what-they-are-and-why-openais-next-move-matters-f86fe481973a">Open - Weight AI Models : What They Are, and Why... | Medium</a></li>
<li><a href="https://www.crowdstrike.com/en-us/cybersecurity-101/artificial-intelligence/frontier-ai/">Frontier AI Explained: Key Models, Players, and Business Impact</a></li>

</ul>
</details>

**社区讨论**: 社区对该模型的性能感到兴奋，但也对其高定价表示担忧。一些用户争论中国实验室是否在将智能商品化，而其他人指出，如果性能确实如此，其成本与 Anthropic 的 Sonnet 系列一致，因此定价合理。

**标签**: `#AI`, `#open-weight model`, `#frontier intelligence`, `#AI pricing`, `#machine learning`

---

<a id="item-4"></a>
## [LM Studio Bionic：面向开源模型的 AI 代理](https://lmstudio.ai/blog/introducing-lm-studio-bionic) ⭐️ 8.0/10

LM Studio 发布了 Bionic，一款面向开源模型的新 AI 代理应用，支持编码、研究和文档操作，并具备自动检查点功能。 这使得 LM Studio 从聊天界面扩展到完整的代理框架，为开发者和企业提供本地、私密的 AI 驱动任务自动化。它在保持数据本地化的同时，与云端代理竞争。 Bionic 支持“代码”和“工作”两种项目类型，在工作项目中具有自动检查点功能，可保存每次更改。目前代理锁定到每个项目的单个目录，不包含 SSH 或本地网络搜索功能。

hackernews · minimaxir · 7月16日 20:18 · [社区讨论](https://news.ycombinator.com/item?id=48939662)

**背景**: LM Studio 是一款流行的本地大语言模型运行时，允许用户在没有网络依赖的情况下在自己的机器上运行开源模型。Bionic 是其首个代理功能，从简单的聊天扩展到自主任务执行，如代码生成和文档编辑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lmstudio.ai/">LM Studio Bionic - Agent for Open Models</a></li>
<li><a href="https://9to5mac.com/2026/07/16/lm-studio-expands-beyond-chat-with-bionic-a-new-ai-agent-app-for-open-models/">LM Studio launches Bionic, a new AI agent app for open models - 9to5Mac</a></li>

</ul>
</details>

**社区讨论**: 社区成员分享了积极的初步印象，指出与 Codex 的相似性，但要求改进，如系统级访问、本地网络搜索、SSH 集成和加载进度条。创始人 Yagil 为使用 GLM 5.2 和 Kimi K2.6 等特定模型进行测试的用户提供了免费积分。

**标签**: `#LM Studio`, `#AI agent`, `#local LLM`, `#open-source models`, `#coding agent`

---

<a id="item-5"></a>
## [数据科学的数学：高维直觉](https://arxiv.org/abs/2607.11938) ⭐️ 8.0/10

一本名为《数据科学的数学》的新书介绍了基础数学概念，重点强调高维直觉及其对模型训练和优化的影响。 理解高维几何对现代数据科学至关重要，这本书提供了直观的解释，帮助从业者避免模型训练和优化中的常见陷阱。 该书从解释人类直觉在高维空间中的失效（如尖峰性、测度集中）入手，并将这些概念与随机梯度下降和高维模型拟合中的实际挑战联系起来。

hackernews · Anon84 · 7月16日 20:38 · [社区讨论](https://news.ycombinator.com/item?id=48939896)

**背景**: 在高维空间中，许多来自二维和三维的常见直觉会失效。例如，测度集中现象表明，高维球体的大部分质量集中在赤道附近，而不是两极。这使得许多机器学习算法的行为出乎意料。这本书涵盖了这些概念，帮助数据科学家建立正确的直觉。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Concentration_of_measure">Concentration of measure</a></li>
<li><a href="https://mark.reid.name/blog/warning-high-dimensions.html">Warning! High Dimensions Ahead Inductio Ex Machina Mark Reid</a></li>

</ul>
</details>

**社区讨论**: 社区评论者热情洋溢，赞扬该书对高维直觉的关注。有评论者指出，统计学是当今数据科学家最重要的技能，这本书有助于建立必要的判断力。另一位评论者提到，数据科学角色已演变，优先考虑扎实的基础和良好的判断力，这正是该书所支持的。

**标签**: `#data-science`, `#mathematics`, `#high-dimensional`, `#statistics`, `#intuition`

---

<a id="item-6"></a>
## [Roc 编译器从 Rust 到 Zig 的重写进展报告](https://rtfeldman.com/rust-to-zig) ⭐️ 8.0/10

Richard Feldman 发布了一篇博客文章，详细介绍了将 Roc 编译器从 Rust 重写为 Zig 的进展和动机，理由是更好的内存控制以及增量构建性能。 这次重写为系统编程中 Rust 与 Zig 的比较提供了一个实际案例，特别是在编译器开发领域，并引发了关于性能关键代码中内存安全权衡的讨论。 博文强调，生成机器码本质上涉及内存不安全操作，尽管一些社区成员持不同意见。Zig 的 ReleaseSafe 模式可以在运行时捕获释放后使用错误，但其有效性存在争议。

hackernews · jorangreef · 7月16日 11:39 · [社区讨论](https://news.ycombinator.com/item?id=48933149)

**背景**: Roc 是一种函数式编程语言，其编译器最初用 Rust 编写。Zig 是一种系统编程语言，专注于简洁性和手动内存控制，旨在作为 C 语言的改进。重写旨在利用 Zig 的增量编译速度和更底层的控制能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rust_(programming_language)">Rust (programming language) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://www.roc-lang.org/">The Roc Programming Language</a></li>

</ul>
</details>

**社区讨论**: steveklabnik 评论称，对于普通的编译输出，内存不安全操作并不像所声称的那样必要。landr0id 质疑 Zig 检测释放后使用错误的能力，而 onlyrealcuzzo 则称赞 Zig 的增量构建功能是一个杀手锏优势。

**标签**: `#Rust`, `#Zig`, `#compiler`, `#systems programming`, `#performance`

---

<a id="item-7"></a>
## [用经典机器学习检测 LLM 生成文本](https://blog.lyc8503.net/en/post/llm-classifier/) ⭐️ 8.0/10

一篇博客文章探讨了使用逻辑回归和支持向量机等经典机器学习模型检测大型语言模型生成的文本，其准确率可与复杂神经网络检测器相媲美。 随着 LLM 生成的内容充斥互联网，轻量级且透明的检测方法至关重要。经典机器学习提供了一种低成本、可解释的替代方案，可部署在浏览器或工具中，但评论者指出了军备竞赛和固有的局限性。 该方法依赖于诸如词频和句子模式等统计特征来区分人类与 AI 写作。在受控测试中准确率很高，但检测器可能被改写或使用不同模型所欺骗。

hackernews · uneven9434 · 7月16日 16:41 · [社区讨论](https://news.ycombinator.com/item?id=48936880)

**背景**: 大型语言模型（如 GPT-4 和 Claude）生成的文本存在细微的统计偏差，例如过度使用某些词语或句子结构。经典机器学习模型可以通过训练诸如 unigram 频率、词性比例和可读性分数等特征来利用这些偏差。这些模型比深度学习分类器更快、更透明，且计算需求更低，因此适合实时或客户端检测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://biodivert.com/ai-tooling/detecting-llm-generated-texts-with-classical-machine-learning/">Detecting LLM - Generated Texts With “ Classical ” Machine Learning</a></li>
<li><a href="https://dev.to/tamizuddin/detecting-llm-generated-text-with-classical-machine-learning-bridging-the-gap-between-old-and-new-464l">Detecting LLM - Generated Text with Classical Machine Learning ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing">Wikipedia:Signs of AI writing - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：有人认为由于信息密度低且 LLM 会适应检测器，检测是“一场必败之战”（akersten、gdiamos）。其他人则提出关注努力度量指标，或指出人类仍是最好的检测器（moxza）。有人对浏览器扩展感兴趣（Krssst），也有人对可靠性持怀疑态度。

**标签**: `#LLM`, `#machine learning`, `#text classification`, `#AI detection`, `#classical ML`

---

<a id="item-8"></a>
## [Thinking Machines Lab 发布 975B 参数开放权重模型 Inkling](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

由 Mira Murati 领导的 Thinking Machines Lab 发布了 Inkling 模型，这是一个 975B 参数的混合专家多模态模型，活跃参数为 41B，采用 Apache-2.0 许可，基于 45 万亿 token 的文本、图像、音频和视频数据训练。 Inkling 增强了美国开放权重 AI 生态系统，为微调提供了与 NVIDIA Nemotron 和 Gemma 4 等模型竞争的坚实基础。其多模态能力和 Apache-2.0 许可使其易于定制，可能降低 AI 研究和开发的门槛。 Inkling 并非前沿模型，而是一个适合通过 Tinker 平台进行微调的强大基础模型。较小的变体 Inkling-Small（276B 参数，12B 活跃）仍在测试中。其模型卡和训练数据文档内容较少，关于数据来源的细节有限。

rss · Simon Willison · 7月16日 15:35

**背景**: 混合专家（MoE）架构每次输入只激活部分参数，提升了效率和规模。开放权重模型以宽松许可发布训练后的参数，但与开源不同，它们通常缺乏训练数据的完整透明度和可复现性。此次发布顺应了美国和中国实验室日益增多的大规模开放权重模型的趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/mixture-experts-moearchitecture-padmashri-suresh-o5nqc">Mixture of Experts ( MoE ) architecture</a></li>
<li><a href="https://deasadiqbal.medium.com/understanding-open-weights-vs-open-source-models-988b50ce64d7">Understanding Open Weights vs. Open Source Models | by Asad Iqbal | Medium</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told – Open Source Initiative</a></li>

</ul>
</details>

**社区讨论**: 通过 API 测试 Inkling 的 Simon Willison 称赞其 Apache-2.0 许可，并认为它与中国开放权重模型具有竞争力。但他批评文档过于简略，称模型卡和训练数据文档远短于对美国 AI 实验室的预期。

**标签**: `#AI`, `#open-weights`, `#multimodal`, `#Mixture-of-Experts`, `#machine learning`

---

<a id="item-9"></a>
## [Linus Torvalds：Linux 不反 AI，AI 是有用工具](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linux 内核维护者 Linus Torvalds 明确表示，Linux 并非反 AI 项目，AI 是一款明显有用的工具，并挑战持反对意见者要么分叉要么离开。 Linux 顶级维护者的这一权威声明可能塑造社区规范，解决关于 AI 在开源开发中角色的持续辩论，标志着官方对 AI 工具的认可。 Torvalds 在 Linux 媒体邮件列表中发表了上述言论，强调虽然 AI 存在经济方面的开放性问题，但其有用性对真正使用过的人来说已毋庸置疑。

rss · Simon Willison · 7月16日 13:26

**背景**: Linus Torvalds 是 Linux 内核的创始人和主要维护者，Linux 内核是全球使用的 Linux 操作系统的核心。开源社区内部一直存在关于是否应接受 AI 生成代码的争议，有些项目明确禁止 AI 贡献。作为顶级维护者，Torvalds 的立场对制定项目政策具有重要影响力。

**标签**: `#Linux`, `#AI`, `#Linus Torvalds`, `#Open Source`, `#Kernel Development`

---

<a id="item-10"></a>
## [xAI 因隐私争议开源 Grok Build](https://simonwillison.net/2026/Jul/15/grok-build/#atom-everything) ⭐️ 8.0/10

xAI 因其 grok CLI 工具被曝上传整个用户目录到云端而面临强烈批评；作为回应，xAI 禁用了该功能，删除了已保留的数据，并以 Apache 2.0 许可证开源了整个 Grok Build 代码库。 这一事件凸显了 AI 编码工具中严重的隐私风险，激进的数据收集可能危及敏感用户数据。通过开源代码库，xAI 旨在重建信任，但信任的破裂可能对用户采用基于云的 AI 开发者工具产生持久影响。 Grok Build 代码库包含 844,530 行 Rust 代码，仅以一个初始提交发布，没有提交历史。调查显示，该工具默认上传了完整的 Git 仓库，包括未读取的文件、完整提交历史和未脱敏的 .env 密钥。

rss · Simon Willison · 7月15日 23:59

**背景**: Grok Build 是 xAI 用于开发工作流的编码代理框架和 TUI。作为一款基于云的工具，它将代码上传到 xAI 的服务器进行分析，但一个隐私漏洞导致它在未经用户明确同意的情况下上传了整个目录——包括 SSH 密钥和密码数据库——引发了广泛抗议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/xai-org/grok-build">GitHub - xai-org/grok-build: SpaceXAI's coding agent harness and TUI. Fullscreen, mouse interactive, extensible. · GitHub</a></li>
<li><a href="https://thehackernews.com/2026/07/grok-build-uploads-entire-git.html">Grok Build Uploaded Entire Git Repositories to xAI Storage, Not Just Files It Read</a></li>
<li><a href="https://hivesecurity.gitlab.io/blog/grok-build-repository-upload-2026/">Grok Build Uploaded Entire Git Repositories: What the Wire Capture Proved — Hive Security</a></li>

</ul>
</details>

**社区讨论**: 社区表达了愤怒和不信任，一名用户报告称在其主目录中运行该工具导致 SSH 密钥和密码管理器数据库被上传。一些人欢迎开源发布，认为这是迈向透明的一步，但许多人仍对 xAI 的数据处理做法及补救措施的有效性持怀疑态度。

**标签**: `#privacy`, `#security`, `#xAI`, `#open source`, `#CLI tool`

---

<a id="item-11"></a>
## [DABSN：新型循环语言模型寻求合作](https://www.reddit.com/r/MachineLearning/comments/1uycffg/seeking_collaborators_for_scaling_and_independent/) ⭐️ 8.0/10

一位研究人员发布了名为 DABSN（动态自适应偏置状态网络）的新型循环架构的预印本和开源代码，并寻求合作者进行扩展和独立评估。使用 GPT-2 tokenizer 在 1B token 上训练的 24M 参数模型的初步实验在推理和长上下文基准测试中显示出有前景的结果。 这可能为基于 transformer 的语言模型提供有竞争力的替代方案，有望提高效率和长上下文处理能力。开放合作可能加速该架构的开发和验证，使更广泛的 AI 研究社区受益。 该架构包含 PyTorch、C++ 和 Triton 实现。研究人员正在准备第二篇专注于语言建模和扩展的论文，并邀请帮助进行独立复现、设计更强的基线或提供更大的 GPU 集群访问权限。

reddit · r/MachineLearning · /u/BleedingXiko · 7月16日 19:17

**背景**: 像 LSTM 这样的循环架构逐步处理序列，但由于并行化和可扩展性，它们在 NLP 领域基本被 transformer 取代。新的循环变体如 Mamba 和 RWKV 旨在将循环的效率与强大性能结合起来，而 DABSN 是这一研究路线的最新成员。像 MQAR 这样的基准测试模型执行多次关联键值查找的能力，这对推理和记忆任务至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/multi-query-associative-recall-mqar">MQAR: Multi-Query Associative Recall</a></li>
<li><a href="https://wandb.ai/stud76/zoology/reports/MQAR-and-data-driven-expansion-of-state--Vmlldzo3NDUwMzI2">MQAR and data-driven expansion of state | zoology – Weights & Biases</a></li>

</ul>
</details>

**标签**: `#recurrent architecture`, `#language models`, `#open-source`, `#preprint`, `#scaling`

---

<a id="item-12"></a>
## [QLoRA 的 2e-4 学习率在小数据集上有问题](https://www.reddit.com/r/MachineLearning/comments/1uy1z8b/the_qlora_2e4_default_is_wrong_under_10k_samples/) ⭐️ 8.0/10

作者指出，QLoRA 微调中标准的 2e-4 学习率对于少于 1 万样本的数据集过高，会导致过拟合，建议改用 1e-4 学习率并增加训练轮次。 这一见解挑战了广泛使用的默认值，可节省实践者数周的调试和数据清理时间，强调了根据数据集大小调整超参数的必要性。 作者发现将学习率从 2e-4 降至 1e-4 并将轮次从 3 增加到 5，显著提升了评估指标；建议对少于 1 万样本的数据集使用 1e-4 或更低的学习率，对于更大数据集则需调整。

reddit · r/MachineLearning · /u/Pretty-Ad774 · 7月16日 12:50

**背景**: QLoRA 是一种内存高效的微调方法，结合了量化和 LoRA（低秩自适应），可在单个 GPU 上微调大型语言模型。默认学习率 2e-4 源自 Alpaca 数据集（5.2 万样本），而小数据集可能需要不同设置以避免过拟合。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2305.14314">[2305.14314] QLoRA: Efficient Finetuning of Quantized LLMs</a></li>
<li><a href="https://medium.com/@dsh.2065/fine-tuning-llms-with-lora-and-qlora-from-confusion-to-kinda-working-results-89b348bcce71">Fine-Tuning LLMs with LoRA and QLoRA: From Confusion to (Kinda) Working Results | by Deepesh Sharma | Medium</a></li>

</ul>
</details>

**标签**: `#QLoRA`, `#fine-tuning`, `#learning rate`, `#overfitting`, `#LLM`

---

<a id="item-13"></a>
## [ExTernD：可实现任意精度的三元 LLM 量化](https://www.reddit.com/r/MachineLearning/comments/1uy2zb3/externd_expandedrank_ternary_decomposition/) ⭐️ 8.0/10

ExTernD 提出了用于 LLM 后训练量化的扩阶三元分解，将权重矩阵分解为两个三元矩阵和一个对角缩放矩阵，使得精度可以接近任意目标水平，而 VRAM 仅小幅增加。 该方法通过允许内部秩任意扩展，解决了三元量化的根本限制——固定矩阵大小导致精度损失，可能使三元 LLM 在部署时兼具实用性和高精度，从而大幅减小模型尺寸和功耗。 该分解使用两个三元矩阵（取值{-1,0,1}）和一个内部对角缩放矩阵；内部秩可增加以在 VRAM 和精度之间权衡，且该方法相比传统三元量化仅需略多的 VRAM。

reddit · r/MachineLearning · /u/LMTLS5 · 7月16日 13:31

**背景**: 后训练量化（PTQ）在训练后将神经网络权重精度降低到较低比特宽度（如三元值{-1,0,1}），旨在减小模型大小并加速推理。然而，三元 PTQ 常因固定矩阵大小的三元表示表达能力有限而导致显著的精度损失。ExTernD 通过将权重矩阵分解为两个三元矩阵，并引入可调的内部维度，有效增加了表示能力，而无需使用更高比特的量化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2607.13511">[2607.13511] ExTernD: Expanded - Rank Ternary Decomposition ...</a></li>
<li><a href="https://arxiv.org/html/2607.13511">ExTernD: Expanded - Rank Ternary Decomposition Ternary LLM...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#quantization`, `#ternary`, `#post-training quantization`, `#efficiency`

---

<a id="item-14"></a>
## [PnP-CoSMo：基于内容/风格建模的 MRI 重建框架](https://www.reddit.com/r/MachineLearning/comments/1uy2h66/pnpcosmo_a_multicontrast_mri_reconstruction/) ⭐️ 8.0/10

PnP-CoSMo 提出了一种即插即用的多对比度 MRI 重建框架，该框架仅从图像域数据学习内容/风格模型，无需原始 k 空间训练数据。 该方法克服了基于学习的 MRI 重建中的一个主要瓶颈——原始 k 空间数据稀缺性，并且能够跨不同对比度和前向算子进行泛化，使其在临床部署中具有很高的实用性。 该框架分两个阶段运行：首先从未配对图像数据集学习内容/风格模型；然后冻结该模型，将其作为迭代重建中的先验，兼容任何前向算子。

reddit · r/MachineLearning · /u/void_gear · 7月16日 13:10

**背景**: 多对比度 MRI 通过获取不同组织对比度的图像来辅助诊断。传统重建方法需要完整的 k 空间数据，而基于学习的方法通常需要大量配对数据集。即插即用框架将先验学习与重建算法分离，允许灵活集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2409.13477v2">A Plug-and-Play Method for Guided Multi-contrast MRI Reconstruction based on Content/Style Modeling</a></li>
<li><a href="https://arxiv.org/abs/2409.13477">[2409.13477] A Plug-and-Play Method for Guided Multi-contrast MRI Reconstruction based on Content/Style Modeling</a></li>

</ul>
</details>

**标签**: `#MRI reconstruction`, `#machine learning`, `#medical imaging`, `#plug-and-play`, `#content/style modeling`

---

<a id="item-15"></a>
## [用哈达玛积聚类解耦卷积神经元](https://www.reddit.com/r/MachineLearning/comments/1uwya70/mechanistic_interpretability_a_first_paper_on/) ⭐️ 8.0/10

一项新技术利用神经元感受野与权重的哈达玛积对检测到的模式进行聚类，在 Inception v1 的 mixed4e 层中揭示了单语义聚类。 这项工作为机制可解释性提供了具体方法，能够将多语义神经元分解为可理解的单语义概念，有助于理解神经网络内部机制。 应用于 Inception v1 的 1x1 卷积时，该方法产生了对汽车、猫、狗的清晰聚类，以及对字母和人脸的低激活聚类，并表明梯度下降有意将模式置于噪声范围内。

reddit · r/MachineLearning · /u/narang_27 · 7月15日 06:59

**背景**: 机制可解释性旨在通过理解单个神经元和电路来逆向工程神经网络。多语义神经元对多个不相关概念做出响应，而单语义神经元仅对一个概念做出响应。哈达玛积是矩阵的元素级乘法，此处用于将感受野激活与权重调制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1uwya70/mechanistic_interpretability_a_first_paper_on/">a first paper on disentangling a convolutional neuron [R] - Reddit</a></li>
<li><a href="https://openaccess.thecvf.com/content/CVPR2025W/MIV/papers/Hesse_Disentangling_Polysemantic_Channels_in_Convolutional_Neural_Networks_CVPRW_2025_paper.pdf">[PDF] Disentangling Polysemantic Channels in Convolutional Neural Networks</a></li>
<li><a href="https://www.lesswrong.com/posts/eDicGjD9yte6FLSie/interpreting-neural-networks-through-the-polytope-lens?ref=upstract.com">Interpreting Neural Networks through the Polytope Lens - LessWrong</a></li>

</ul>
</details>

**标签**: `#mechanistic interpretability`, `#convolutional neural networks`, `#neuron disentanglement`, `#Inception v1`

---

<a id="item-16"></a>
## [微软 Comic Chat 在 30 年后开源](https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/) ⭐️ 7.0/10

微软于 2026 年 7 月 16 日在 GitHub 上发布了其 1996 年经典图形化 IRC 客户端 Comic Chat 的源代码。 此次发布保留了一段独特的互联网历史，使开发者、历史爱好者和爱好者能够研究、修改和运行这个曾经流行的聊天客户端，彰显了早期网络的实验精神。 开源代码位于 GitHub 的 Microsoft 组织下，此次发布恰逢该软件诞生 30 周年；原始开发者是 David Kurlander，但 Robert Standefer 和 Scott Hanselman 推动了开源。

hackernews · jervant · 7月16日 16:06 · [社区讨论](https://news.ycombinator.com/item?id=48936426)

**背景**: Microsoft Comic Chat（后更名为 Microsoft Chat）是一款图形化 IRC 客户端，可自动将文本对话渲染为带有卡通头像和气泡的连环漫画。它于 1996 年随 Internet Explorer 3.0 首次发布，并捆绑在 Windows 98 中，帮助推广了 Comic Sans 字体。该客户端扩展了 IRC 协议，增加了控制角色外观和表情的命令，这招致了一些传统主义者的批评。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microsoft_Comic_Chat">Microsoft Comic Chat</a></li>
<li><a href="https://github.com/microsoft/comic-chat">microsoft/ comic - chat : Source code for the ComicChat IRC client ...</a></li>
<li><a href="https://www.windowscentral.com/microsoft/windows-11/microsoft-comic-chat-an-irc-client-from-30-years-ago-that-helped-popularize-comic-sans-is-going-open-source">Microsoft Comic Chat , an IRC client from 30 years... | Windows Central</a></li>

</ul>
</details>

**社区讨论**: 社区反应极为积极且充满怀旧情怀，许多人分享了 Comic Chat 如何激发他们自己的项目或定义了他们早期的互联网体验。一些评论者注意到了技术细节，比如对 IRC 协议的扩展，而另一些人则对微软保留如此具有实验性的软件表示赞赏。

**标签**: `#open source`, `#microsoft`, `#comic chat`, `#irc`, `#nostalgia`

---

<a id="item-17"></a>
## [将高尔夫球场改为公园以抵消数据中心用水](https://simonwillison.net/2026/Jul/17/spot-birds-not-golf/#atom-everything) ⭐️ 7.0/10

Simon Willison 提议，像 Google 这样的超大规模云服务商可以通过购买并将高尔夫球场改造成公共观鸟公园来抵消其数据中心用水，并指出 40 个高尔夫球场即可平衡 Google 的每日用水量。 这一引人深思的提议突显了人工智能数据中心的巨大水足迹，并提供了一种对社区有益的创造性替代方案，可能改变科技公司应对可持续发展的方式。 Google 的 2025 年环境报告显示其用水量为 109 亿加仑，每天约 3000 万加仑。在科切拉谷，120 个高尔夫球场每个每天约用水 75 万加仑，因此收购 40 个球场（三分之一）理论上可抵消 Google 的用水量。

rss · Simon Willison · 7月17日 02:58

**背景**: 超大规模云服务商是像 Google、Amazon 和 Microsoft 这样的大型云服务提供商，它们运营着需要大量冷却用水的大型数据中心。数据中心用水是一个日益增长的环境问题，尤其是在水资源匮乏的地区。高尔夫球场以高耗水著称，每天灌溉用水常达数百万加仑。该提议创造性地将两个高耗水行业联系起来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hyperscale_computing">Hyperscale computing - Wikipedia</a></li>
<li><a href="https://www.redhat.com/en/topics/cloud-computing/what-is-a-hyperscaler">What is a hyperscaler?</a></li>
<li><a href="https://www.eesi.org/articles/view/data-centers-and-water-consumption">Data Centers and Water Consumption | Article | EESI</a></li>

</ul>
</details>

**标签**: `#ai-energy-usage`, `#sustainability`, `#water-usage`, `#data-centers`

---

<a id="item-18"></a>
## [GPT-5.6 Codex 漏洞可通过覆盖$HOME 删除文件](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 7.0/10

Thibault Sottiaux 报告称，GPT-5.6 的 Codex 在全访问模式且无沙箱保护时，由于模型错误地覆盖并删除了$HOME 环境变量，可能导致文件删除。 这是一个严重的 AI 安全问题，影响使用 Codex 等编码代理的开发者，可能导致不可逆的数据丢失。它凸显了 AI 编码工具中沙箱保护和自动审核功能的重要性。 该漏洞发生在启用全访问模式、禁用沙箱保护（包括自动审核）且模型尝试覆盖$HOME 以定义临时目录时，错误地删除了$HOME 本身。

rss · Simon Willison · 7月16日 17:45

**背景**: Codex 是 OpenAI 开发的 AI 编码代理，可在用户本地机器上运行代码。沙箱是一种隔离技术，限制代理的访问权限，防止对系统造成损害。自动审核功能使用单独的审核代理替代手动审批。如果没有这些保护，代理可能执行破坏性命令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-codex/">Introducing Codex | OpenAI</a></li>
<li><a href="https://northflank.com/blog/how-to-sandbox-ai-agents">How to sandbox AI agents in 2026: MicroVMs, gVisor & isolation strategies | Blog — Northflank</a></li>
<li><a href="https://alignment.openai.com/auto-review/">Auto-review of agent actions without synchronous human oversight</a></li>

</ul>
</details>

**标签**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#bug`

---

<a id="item-19"></a>
## [为机器人学习中的 JEPA 世界模型寻求批判性意见](https://www.reddit.com/r/MachineLearning/comments/1uxcryc/looking_for_jepa_devil_advocates_r/) ⭐️ 7.0/10

一名研究人员在 Reddit 上发帖，请求社区扮演唱反调的角色，指出 Yann LeCun 提出的用于世界模型的 JEPA 模型（尤其是在机器人学习领域）中可能存在的警示信号。 JEPA 是一种重要的自监督学习方法，LeCun 将其吹捧为 LLM 和 RL 的潜在替代方案，因此批判性审视有助于研究人员避免过度炒作并识别实际局限性。 帖子指出 LeCun 贬低 LLM、RL 等方法，引发了对潜在偏见的担忧。评论者可能讨论可扩展性、样本效率以及与控制的集成等问题。

reddit · r/MachineLearning · /u/Amazing-Coat5160 · 7月15日 17:34

**背景**: JEPA 代表联合嵌入预测架构（Joint Embedding Predictive Architecture），是一种自监督方法，通过预测潜在空间中的表示而非重建原始像素来学习。它由 Meta AI 于 2023 年针对图像任务（I-JEPA）提出，后来扩展到视频和机器人领域。LeCun 一直倡导将 JEPA 作为自主 AI 世界模型的核心组件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.turingpost.com/p/jepa">What is Joint Embedding Predictive Architecture (JEPA)?</a></li>
<li><a href="https://arxiv.org/abs/2301.08243">[2301.08243] Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture</a></li>

</ul>
</details>

**标签**: `#JEPA`, `#world models`, `#robot learning`, `#machine learning`, `#critiques`

---

<a id="item-20"></a>
## [PyTorch 模型在 T4 上比 A100 慢 170 倍：架构瓶颈？](https://www.reddit.com/r/MachineLearning/comments/1ux6a9x/pytorch_model_running_170x_slower_on_t4_vs_a100/) ⭐️ 7.0/10

有用户报告，一个使用 4D 相关体积和 Transformer 的 PyTorch 点追踪模型在 NVIDIA T4 GPU 上运行需要 85 秒，而在 A100 上仅需 0.5 秒，慢了 170 倍，且观察到纯 FP32 执行和 99%的 GPU 利用率。 这种极端差异远超 T4 与 A100 之间 2.4 倍的 FP32 TFLOPS 差距，表明存在严重的软件或算法级别瓶颈，可能影响许多在 T4 硬件上部署模型的机器学习从业者。 该模型构建用于帧间密集匹配的 4D 相关体积，这是一项内存密集型操作；使用纯 FP32 禁用了 T4 上的张量核心加速，而 A100 可以利用 TF32 张量核心实现更快的类 FP32 性能。

reddit · r/MachineLearning · /u/Future-Structure-296 · 7月15日 13:44

**背景**: NVIDIA T4（图灵架构，8.1 TFLOPS FP32，320 GB/s）和 A100（安培架构，19.5 TFLOPS FP32，1555 GB/s）在架构和内存带宽上存在差异。4D 相关体积通过比较图像之间所有点对来构建成本体积，这需要高内存带宽和高效的内核执行。170 倍的差距表明 T4 可能遭遇严重的内存瓶颈，或者缺乏针对此类操作的优化库支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.server-parts.eu/post/nvidia-t4-vs-a100-gpu-comparison-ai-deep-learning-data-centers">NVIDIA T4 vs. NVIDIA A100 Comparison: Which GPU Should You Choose for AI and Data Center Workloads?</a></li>
<li><a href="https://gpuperhour.com/compare/t4-vs-a100">T4 vs A100: 38.5x FP16 Gap, 80GB vs 16GB | GPUPerHour</a></li>

</ul>
</details>

**标签**: `#PyTorch`, `#GPU performance`, `#model optimization`, `#troubleshooting`, `#hardware comparison`

---

<a id="item-21"></a>
## [Decoy 字体：人类可读但能迷惑 AI 的字体实验](https://www.mixfont.com/experiments/decoy-font) ⭐️ 6.0/10

开发者 Eric Lu 创造了 Decoy 字体，这是一种设计成人类易读但会误导 AI 文本识别系统的字体。该字体利用多层空间频率嵌入隐藏信息，人类能看到隐藏文字，而 GPT、Gemini 等 AI 模型则会读出完全不同的内容。 这一实验凸显了 AI 视觉模型面对对抗性输入时的脆弱性，并引发了关于保护个人文本免受自动监视的讨论。它也展示了对抗性示例在排版领域的实际应用，可能激发隐私保护设计的新思路。 该字体通过叠加两组字符实现：一组是高空间频率（清晰）的文本，另一组是低空间频率（模糊）的文本。人类在眯眼或从远处观看时能感知到低频文字，而 AI OCR 系统倾向于读取高频文字。

hackernews · ray__ · 7月16日 16:18 · [社区讨论](https://news.ycombinator.com/item?id=48936584)

**背景**: 对抗性示例是专门设计来让机器学习模型出错的输入，通常通过在图像上添加人眼无法察觉的扰动来实现。在计算机视觉领域，已有针对 OCR 系统的此类攻击，而 Decoy 字体将类似原理应用于排版。其概念源于混合图像——在不同空间频率下呈现不同画面，例如著名的爱因斯坦-梦露错觉。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mixfont.com/experiments/decoy-font">Decoy Font: A TTF font that hides what you type</a></li>
<li><a href="https://www.ndtv.com/feature/this-ghost-font-can-only-be-read-by-humans-leaves-top-ai-models-stumped-11773990">This 'Ghost Font' Can Only Be Read by Humans, Leaves Top AI Models Stumped</a></li>

</ul>
</details>

**社区讨论**: 社区评论呈现出混合但好奇的反应。用户证实 GPT、Gemini 和 Claude 都无法准确检测隐藏文字，不过不同模型和提示词下结果各异。有人指出调整图像大小会改变读取的文本，还有人称可以通过简单的脚本修复来抵消该字体的效果。

**标签**: `#font`, `#anti-AI`, `#typography`, `#adversarial`, `#computer vision`

---

<a id="item-22"></a>
## [Mermaid 转换为 ASCII 艺术工具编译为 WebAssembly](https://simonwillison.net/2026/Jul/16/mermaid-ascii/#atom-everything) ⭐️ 6.0/10

Simon Willison 创建了一个网页工具，将 AlexanderGrooff/mermaid-ascii Go 库编译为 WebAssembly，从而在浏览器中直接实现将 Mermaid 图表转换为彩色 ASCII 艺术。 该工具使 Mermaid 图表在纯文本环境（如终端或代码注释）中可用，且支持颜色以增强可读性。它展示了 WebAssembly 在将现有 Go 库移植到基于浏览器的应用程序中的强大能力。 该工具支持类似 ANSI 的颜色，并提供填充和框尺寸的选项。它是通过使用 Claude Fable 5 将 Go 库编译为 WebAssembly 而构建的。

rss · Simon Willison · 7月16日 14:57

**背景**: Mermaid 是一种流行的图表工具，使用基于文本的语法生成图表。ASCII 艺术表示对于在纯文本环境（如电子邮件、文档或终端输出）中嵌入图表非常有用。WebAssembly 允许在网页浏览器中高效运行编译后的代码（如 Go），从而实现无需服务器的转换。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/AlexanderGrooff/mermaid-ascii">GitHub - AlexanderGrooff/mermaid-ascii: Render Mermaid graphs inside your terminal · GitHub</a></li>

</ul>
</details>

**标签**: `#mermaid`, `#ascii-art`, `#webassembly`, `#developer-tools`, `#go`

---

<a id="item-23"></a>
## [AI 记忆应存储模式而非事实？](https://www.reddit.com/r/MachineLearning/comments/1uy6yht/are_current_ai_memory_architectures_optimizing/) ⭐️ 6.0/10

Reddit 上的一篇帖子质疑当前 AI 记忆系统是否应从存储描述性事实（如用户偏好）转向推断更高级的推理模式（如解释框架和推理风格）。这一概念性探索设想未来的持久上下文更像一个演化中的用户理解问题模型。 如果实现，这一转变将使 AI 助手更加个性化和自适应，超越简单的事实回忆，深入到与用户认知风格的深度对齐。它挑战了当前基于检索增强生成和摘要的记忆架构，可能为 AI 记忆和认知架构研究开辟新方向。 帖子对比了当前描述性记忆（“用户对经济学感兴趣”）与一个推断解释倾向的模型（“用户倾向于通过激励和制度约束解释经济结果”）。但指出这种表示可能需要与当前记忆、检索和摘要方法根本不同的架构，并且没有提供实现细节或实证验证。

reddit · r/MachineLearning · /u/Boris_Ljevar · 7月16日 16:00

**背景**: 当前的 AI 记忆系统通过保存的记忆、对话摘要和用户偏好等机制存储持久上下文，通常依赖检索增强生成（RAG）将相关事实拉入上下文窗口。认知架构是构建智能体的蓝图，它将 LLM 与符号推理和记忆检索相结合，以模拟类人推理。该帖子提出从存储描述性事实转向推断更高级认知模式的假设性转变，这可能与认知架构研究一致，但目前缺乏具体的架构或实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cognitive_architecture">Cognitive architecture - Wikipedia</a></li>
<li><a href="https://www.mindstudio.ai/blog/ai-memory-system-persistent-context-agents">What Is an AI Memory System? How to Build Persistent Context for Your Agents | MindStudio</a></li>
<li><a href="https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents">Effective context engineering for AI agents \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI memory`, `#persistent context`, `#cognitive architectures`, `#ML systems`

---

<a id="item-24"></a>
## [NeurIPS 2026 RTCA 研讨会征稿](https://www.reddit.com/r/MachineLearning/comments/1uy8e0v/cfp_rtca_neurips_2026_r/) ⭐️ 6.0/10

首届 RTCA 研讨会将在 NeurIPS 2026 上举办，现已发布论文和演示征稿通知，专注于实时多模态对话代理。 该研讨会致力于解决让对话 AI 实时自然交互的关键挑战，这是超越当前离线系统的一个前沿领域。 投稿类型包括完整论文（最多 8 页）、短论文（最多 4 页）和演示论文（最多 2 页），提交截止日期为 2026 年 8 月 29 日。

reddit · r/MachineLearning · /u/Few-Ferret9700 · 7月16日 16:51

**背景**: 实时对话代理需要全双工通信，即双方可以同时说话，不同于传统的轮流说话系统。回馈（如“嗯”或点头）是表示持续注意的语言和非语言回应，对于自然交互至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sesame.com/blog/crossing-the-uncanny-valley-of-voice">Crossing the uncanny valley of conversational voice | Sesame</a></li>
<li><a href="https://en.wikipedia.org/wiki/Backchannel_(linguistics)">Backchannel (linguistics) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#real-time conversational agents`, `#multimodal interaction`, `#NeurIPS workshop`, `#call for papers`

---