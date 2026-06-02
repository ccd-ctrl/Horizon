---
layout: default
title: "Horizon Summary: 2026-06-02 (ZH)"
date: 2026-06-02
lang: zh
---

> 从 24 条内容中筛选出 18 条重要资讯。

---

1. [反向传播在一轮训练中破坏 V1 脑对齐](#item-1) ⭐️ 9.0/10
2. [Adafruit 收到 Flux.ai 律师函](#item-2) ⭐️ 8.0/10
3. [微软发布 MAI-Thinking-1 和 MAI-Code-1-Flash 大模型](#item-3) ⭐️ 8.0/10
4. [Minimax M3 未发现政治审查](#item-4) ⭐️ 8.0/10
5. [本地 Qwen3.6-27B 在多智能体系统中替代 Claude](#item-5) ⭐️ 8.0/10
6. [Bonsai Image 4B：1 比特和三值模型体积不到 1.3GB](#item-6) ⭐️ 8.0/10
7. [在 6GB RTX 4050 上对 20 个小语言模型进行基准测试](#item-7) ⭐️ 8.0/10
8. [CT 扫描揭示比亚迪垂直整合](#item-8) ⭐️ 7.0/10
9. [用户因侵入式 AI 功能离开 Gmail](#item-9) ⭐️ 7.0/10
10. [西雅图监控步行之旅揭示隐形网络](#item-10) ⭐️ 7.0/10
11. [特朗普签署缩水版人工智能行政令](#item-11) ⭐️ 7.0/10
12. [浏览器广告归因提案被批为大型科技公司卡特尔](#item-12) ⭐️ 7.0/10
13. [PapersWithCode 复活并支持 CVPR 2026 会议](#item-13) ⭐️ 7.0/10
14. [工人沦为不透明 AI 的“是/否”监督员](#item-14) ⭐️ 7.0/10
15. [花 200 英镑在游戏 PC 中安装 V100 数据中心 GPU](#item-15) ⭐️ 7.0/10
16. [LLM 编码基准测试：Step 3.7 对比 Qwen 系列](#item-16) ⭐️ 7.0/10
17. [llama.cpp PR 添加思考模式切换与推理努力级别](#item-17) ⭐️ 7.0/10
18. [Janet 语言：一个带有权衡的现代 Lisp](#item-18) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [反向传播在一轮训练中破坏 V1 脑对齐](https://www.reddit.com/r/MachineLearning/comments/1tupu9z/backpropagation_destroys_v1_brain_alignment_in/) ⭐️ 9.0/10

一项新研究表明，反向传播（BP）在 CIFAR-10 上仅训练一轮就破坏了 90%的 V1 脑对齐，而预测编码（PC）和 STDP 等局部学习规则则能更好地保持这种对齐。 这揭示了构建高层表征的全局误差信号与保留早期视觉表征之间的根本权衡，挑战了反向传播的生物学合理性，并支持局部学习规则更接近大脑。 该研究使用 RSA 对齐 THINGS 数据集的 fMRI 数据，对每种规则在 5 个随机种子上跟踪了 8 个检查点。BP 将 V1 对齐从 r=0.102 降至 0.011（p=0.031），而 PC 和 STDP 仅下降 25-31%并稳定，与 BP 相比 Cohen's d > 5。

reddit · r/MachineLearning · /u/ConfusionSpiritual19 · 6月2日 12:43

**背景**: 表征相似性分析（RSA）用于衡量神经网络内部表征与 fMRI 脑活动模式的匹配程度。反向传播使用全局误差信号更新权重，而预测编码和 STDP 依赖局部信息，因此更具生物学合理性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.brainvoyager.com/bv/doc/UsersGuide/RSA/RepresentationalSimilarityAnalysis.html">Representational Similarity Analysis (RSA)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Predictive_coding">Predictive coding - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Spike-timing-dependent_plasticity">Spike-timing-dependent plasticity - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Reddit 上的讨论内容充实，用户注意到不同随机种子之间结果的一致性，并讨论了其对生物学合理学习的意义。一些人质疑这种退化是否仅限于浅层架构，还是能推广到更深层的模型。

**标签**: `#neuroscience`, `#backpropagation`, `#predictive coding`, `#brain alignment`, `#learning rules`

---

<a id="item-2"></a>
## [Adafruit 收到 Flux.ai 律师函](https://blog.adafruit.com/) ⭐️ 8.0/10

开源硬件巨头 Adafruit 收到了代表云端 EDA 初创公司 Flux.ai 的 Fenwick 律师事务所发出的律师函。该函件很可能与 Adafruit 即将发布的关于 Flux.ai 的博文有关。 这场法律纠纷凸显了成熟的开源硬件社区与获得融资的初创公司之间的紧张关系，可能会抑制批评性评论。结果可能为公司在创客社区中如何应对负面报道树立先例。 Adafruit 创始人 Limor 'Ladyada' Fried 已联系 Flux.ai 首席执行官 Matthias Wagner，希望通过播客等方式友好解决此事。社区评论显示用户普遍对 Flux.ai 的产品质量和计费方式不满。

hackernews · semanser · 6月2日 10:00 · [社区讨论](https://news.ycombinator.com/item?id=48368121)

**背景**: Adafruit 是由 Limor Fried 创立的知名开源硬件公司，提供电子套件和教育内容。Flux.ai 是一款基于浏览器的云端 PCB 设计 EDA 工具，近期获得了 Bain Capital 的投资。律师函是一种正式的法律通知，常用于要求删除内容或威胁提起诉讼。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Adafruit_Industries">Adafruit Industries</a></li>
<li><a href="https://grokipedia.com/page/Comparison_of_KiCad_and_Fluxai">Comparison of KiCad and Flux.ai</a></li>

</ul>
</details>

**社区讨论**: 社区舆论强烈反对 Flux.ai，用户称其产品“极其糟糕”并指责其消耗代币。有人猜测 Flux.ai 的法律行动是为了在获得融资后压制负面报道。

**标签**: `#legal`, `#open-source hardware`, `#startup`, `#community`, `#electronics`

---

<a id="item-3"></a>
## [微软发布 MAI-Thinking-1 和 MAI-Code-1-Flash 大模型](https://simonwillison.net/2026/Jun/2/microsofts-new-models/#atom-everything) ⭐️ 8.0/10

微软宣布了两款新的小参数量大语言模型：MAI-Thinking-1（35B 活跃参数，约 1T 总参数，专注于推理）和 MAI-Code-1-Flash（5B 活跃参数，137B 总参数，专为代码生成设计）。两者均使用干净、商业许可的数据从头训练，未从第三方模型蒸馏。 这些模型表明，用更少的参数也能实现强大性能，有望降低推理成本并支持本地部署。MAI-Code-1-Flash 专为 GitHub Copilot 和 VS Code 打造，承诺为编码任务提供更低成本和高性能。 MAI-Thinking-1 采用稀疏混合专家架构，支持 128K 上下文窗口，在盲测中优于 Sonnet 4.6。MAI-Code-1-Flash 使用自适应解决方案长度控制，根据任务调整推理深度。两款模型目前尚未公开提供测试。

rss · Simon Willison · 6月2日 22:21

**背景**: 大语言模型通常以参数量衡量，像 GPT-4 这样的模型有数千亿参数。较小的模型（如 7B-35B）运行成本更低，但能力往往较弱。微软的新模型旨在通过使用干净数据和高效架构，以更少的参数实现有竞争力的性能，从而弥合这一差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://microsoft.ai/news/introducing-mai-thinking-1/">Introducing MAI-Thinking-1 | Microsoft AI</a></li>
<li><a href="https://microsoft.ai/news/introducingmai-code-1-flash/">Introducing MAI - Code - 1 - Flash | Microsoft AI</a></li>
<li><a href="https://www.neowin.net/news/microsoft-unveils-mai-thinking-1-reasoning-and-mai-code-1-coding-models/">Microsoft unveils MAI-Thinking-1 reasoning and MAI-Code-1 coding models - Neowin</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一：一些人欢迎竞争，但质疑小型云模型在严肃编码中的实际价值，指出 SWE-bench 等基准测试相比现有小模型提升有限。另一些人批评营销夸大其词，并指出总参数量（137B）并不像暗示的那么小。此外，对 GitHub Copilot 的定价变化也存在质疑。

**标签**: `#AI`, `#LLM`, `#Microsoft`, `#efficiency`, `#coding`

---

<a id="item-4"></a>
## [Minimax M3 未发现政治审查](https://www.reddit.com/r/LocalLLaMA/comments/1tuv1sv/minimax_m3_appears_to_have_no_political_censorship/) ⭐️ 8.0/10

一位正在开发中国/CCP AI 偏见基准测试的 Reddit 用户报告称，Minimax M3 在测试中未显示政治审查，这与其它中国大语言模型不同。 这一发现意义重大，因为它挑战了所有中国大语言模型都实施政治审查的普遍假设，可能影响 AI 偏见研究和更开放模型的开发。 该用户指出，所有其它 Minimax 模型都像典型的中国大语言模型一样受到审查，使得 M3 成为异常值。该基准测试仍在进行中，结果尚属初步。

reddit · r/LocalLLaMA · /u/DingyAtoll · 6月2日 15:52

**背景**: 许多中国大语言模型，如百度和阿里巴巴的模型，都包含政治审查以遵守政府规定。Minimax 是一家中国 AI 公司，本周早些时候发布了 M3，这是一个具有前沿编码能力和 1M 上下文长度的开放模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reddit.com/r/LocalLLaMA/comments/1ttdiq0/minimax_m3_coding_agentic_frontier_1m_context/">MiniMax M3 - Coding & Agentic Frontier, 1M Context, Multimodal</a></li>
<li><a href="https://arxiv.org/abs/2306.16244">[2306.16244] CBBQ: A Chinese Bias Benchmark Dataset Curated...</a></li>

</ul>
</details>

**社区讨论**: Reddit 社区表示惊讶和兴趣，一些人质疑基准测试的可靠性，另一些人希望这预示着中国 AI 模型审查减少的趋势。

**标签**: `#AI censorship`, `#LLM`, `#Chinese AI`, `#bias benchmark`, `#Minimax`

---

<a id="item-5"></a>
## [本地 Qwen3.6-27B 在多智能体系统中替代 Claude](https://www.reddit.com/r/LocalLLaMA/comments/1tunmam/replaced_claude_with_local_qwen3627b_in_my/) ⭐️ 8.0/10

一位开发者在其多智能体编排器 OpenYabby 中，用本地运行的 Qwen3.6-27B 模型（通过 Ollama 在单张 RTX 3090 上运行）替代了 Claude，并在 47 个多步骤编码工作流中进行了为期两周的测试。 该实验表明，本地模型可以作为多智能体系统中可行的推理层，可能减少对云 API 的依赖并降低成本，尽管它们在工具调用可靠性和复杂代码生成方面仍有差距。 Qwen3.6-27B 实现了约 95%的架构有效计划生成，并捕获了 Claude 审查中约 60%的 bug，但工具调用格式错误率为 12%（Claude 为 0.5%），且在超过约 14k token 后出现长上下文漂移。

reddit · r/LocalLLaMA · /u/Interesting-Sock3940 · 6月2日 11:05

**背景**: 多智能体编排器协调多个 AI 代理完成复杂任务，通常使用主导代理生成计划，子代理执行步骤。像 Qwen3.6-27B 这样的本地 LLM 提供隐私和成本优势，但通常上下文窗口较小，错误率高于 Claude 等云模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.6-27B">Qwen/Qwen3.6-27B · Hugging Face</a></li>
<li><a href="https://openrouter.ai/qwen/qwen3.6-27b">Qwen3.6 27B - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://github.com/ollama/ollama">GitHub - ollama/ollama: Get up and running with Kimi-K2.5, GLM-5, MiniMax, DeepSeek, gpt-oss, Qwen, Gemma and other models. · GitHub</a></li>

</ul>
</details>

**社区讨论**: Reddit 社区验证了这些发现，用户分享了使用本地模型的类似经验，并建议采用基于语法的采样等技术来减少工具调用错误。部分用户讨论了生产环境中本地模型与云模型之间的权衡。

**标签**: `#local-llm`, `#multi-agent`, `#qwen`, `#code-generation`, `#benchmark`

---

<a id="item-6"></a>
## [Bonsai Image 4B：1 比特和三值模型体积不到 1.3GB](https://www.reddit.com/r/LocalLLaMA/comments/1tusnh5/1bit_bonsai_image_4b_and_ternary_bonsai_image_4b/) ⭐️ 8.0/10

研究人员发布了 Bonsai Image 4B，这是一个用于图像生成的扩散变换器，有两个超紧凑版本：1 比特量化版仅 0.93GB，三值量化版仅 1.21GB。 这一突破使得在内存有限的本地设备（如智能手机和边缘硬件）上也能进行高质量图像生成，从而让生成式 AI 更加普及。 这些模型基于 40 亿参数的扩散变换器，通过 1 比特和三值量化实现极致的内存节省，同时保持合理的输出质量。

reddit · r/LocalLLaMA · /u/Addyad · 6月2日 14:28

**背景**: 量化将模型权重的精度从通常的 32 位浮点数降低到更低的位宽，如 1 比特（二进制）或三值（{-1,0,1}）。扩散变换器（DiT）用变换器架构取代了传统的 U-Net 主干网络，用于图像生成，具有更好的可扩展性。这种组合使得大型模型能够在资源受限的设备上运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2202.05292">[2202.05292] On One-Bit Quantization</a></li>
<li><a href="https://www.shadecoder.com/topics/1-bit-quantization-a-comprehensive-guide-for-2025">1-bit Quantization Guide - Efficient Models in 2025 | ShadeCoder</a></li>
<li><a href="https://www.emergentmind.com/topics/ternary-quantization">Ternary Quantization in Neural Networks</a></li>

</ul>
</details>

**社区讨论**: Reddit 社区对这些极小的模型体积表示兴奋，许多用户讨论了在移动设备上的潜在应用，并比较了压缩与图像质量之间的权衡。

**标签**: `#quantization`, `#image generation`, `#diffusion transformer`, `#local AI`, `#model compression`

---

<a id="item-7"></a>
## [在 6GB RTX 4050 上对 20 个小语言模型进行基准测试](https://www.reddit.com/r/LocalLLaMA/comments/1tuvs6l/benchmarks_of_20_small_llms_on_a_6gb_rtx_4050/) ⭐️ 8.0/10

一位用户在 6GB RTX 4050 笔记本 GPU 上对 20 个小量化语言模型进行了基准测试，测量了生成速度、VRAM 使用情况和定性任务性能，用于本地自动化。 这填补了 GPU 内存有限（6GB）用户的实际空白，提供了超越排行榜分数的真实性能数据，帮助用户为本地、私密、免费的自动化任务做出明智的模型选择。 基准测试包括来自 Granite、LFM、Gemma、Qwen 和 Nemotron 等系列的 20 个模型，在 1k、8k 和 32k 上下文长度下测试，生成速度从 28 到 207 tok/s 不等，VRAM 使用量从 1.9G 到 5.6G。

reddit · r/LocalLLaMA · /u/drfritz2 · 6月2日 16:16

**背景**: 量化通过降低模型精度（例如从 16 位降至 4 位）来将更大模型适配到有限 GPU 内存中，且质量损失极小。小语言模型（1-8B 参数）在消费级硬件上进行本地推理很受欢迎。排行榜分数通常使用全精度模型，而非用户实际运行的量化版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lmstudio.ai/models">Model Catalog - LM Studio</a></li>
<li><a href="https://developers.redhat.com/articles/2024/10/17/we-ran-over-half-million-evaluations-quantized-llms">We ran over half a million evaluations on quantized LLMs—here's what we found | Red Hat Developer</a></li>
<li><a href="https://medium.com/@kundansinghsorout/running-local-llms-on-a-6gb-gpu-laptop-what-actually-works-in-2026-and-what-doesnt-487fda2a604e">Running Local LLMs on a 6 GB GPU Laptop — What Actually... | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区称赞了针对 6GB GPU 的实用焦点和定性测试，许多人分享了类似经验，并请求更多模型或特定任务的评估。一些人讨论了模型选择以及量化对推理任务的影响。

**标签**: `#LLM`, `#benchmark`, `#local inference`, `#GPU`, `#small models`

---

<a id="item-8"></a>
## [CT 扫描揭示比亚迪垂直整合](https://www.lumafield.com/scan-of-the-month/byd) ⭐️ 7.0/10

Lumafield 发布了比亚迪汽车零部件的详细 CT 扫描图像，包括钥匙、制动卡钳和信息娱乐屏幕，展示了该公司的垂直整合和制造精度。 这项分析提供了罕见的非破坏性视角，深入了解比亚迪的工程设计和供应链策略，凸显垂直整合如何赋予比亚迪在电动汽车生产中的竞争优势。 CT 扫描显示，比亚迪约 75%的零部件为自产，而福特仅为 25%；钥匙设计包含一个可拔出的机械备用钥匙，而非最初描述的铰链式。

hackernews · viasfo · 6月2日 20:30 · [社区讨论](https://news.ycombinator.com/item?id=48375824)

**背景**: CT（计算机断层扫描）利用 X 射线创建物体的 3D 图像，无需拆解即可进行详细内部检查。比亚迪以其高度垂直整合而闻名，控制从锂矿开采到电池生产再到整车组装的全链条。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://evboosters.com/ev-charging-news/the-blueprint-of-an-ev-empire-how-byd-built-global-dominance-through-vertical-integration/">The blueprint of an EV empire: how BYD built global... | EVBoosters</a></li>
<li><a href="https://www.automotivemanufacturingsolutions.com/electrification/from-battery-maker-to-ev-leader-byds-strategic-rise/46813.article">BYD ’s strategy to overtake Tesla in EV production globally | Automotive...</a></li>
<li><a href="https://en.wikipedia.org/wiki/CT_scan">CT scan - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论纠正了钥匙的描述，指出机械钥匙是拔出而非铰链式。用户还引用了 Munroe Live 的相关拆解视频，并指出展示的方形电池并非刀片电池，澄清了一个常见误解。

**标签**: `#BYD`, `#EV`, `#manufacturing`, `#CT scan`, `#engineering`

---

<a id="item-9"></a>
## [用户因侵入式 AI 功能离开 Gmail](https://moddedbear.com/gmail-thinks-im-stupid-so-i-left) ⭐️ 7.0/10

一位用户公开宣布因对智能建议和弹窗等侵入式 AI 功能感到不满而离开 Gmail，并在 Hacker News 上引发了讨论。 这反映了对日常工具中激进 AI 集成的日益反弹，凸显了有用自动化与用户自主权之间的紧张关系。 该用户列举了具体烦恼，如 Gmail 的智能撰写建议和打断工作流程的弹窗，并选择切换到更简单的邮件服务商。

hackernews · speckx · 6月2日 19:27 · [社区讨论](https://news.ycombinator.com/item?id=48375016)

**背景**: Gmail 越来越多地集成 AI 功能，如智能撰写和智能回复，以帮助用户快速撰写邮件。虽然许多人觉得这些功能有用，但一些用户认为它们削弱了个人表达和对沟通的控制。

**社区讨论**: 评论者表达了复杂情绪：一些人同意 AI 写作建议感觉侵入且缺乏个性，而另一些人则为其辩护，认为对非母语者或快速回复有用。还有几人抱怨弹窗和垃圾邮件过滤问题。

**标签**: `#AI`, `#UX`, `#email`, `#privacy`, `#productivity`

---

<a id="item-10"></a>
## [西雅图监控步行之旅揭示隐形网络](https://coveillance.org/a-walking-tour-of-surveillance-infrastructure-in-seattle/) ⭐️ 7.0/10

2020 年发布了一次详细的西雅图监控基础设施步行之旅，记录了遍布全市的、通常不可见的摄像头和传感器网络。 这篇文章引发了关于隐私、警务和社会规范的批判性讨论，突显了监控技术在城市环境中如何变得常态化。 这次旅行涵盖了各种类型的监控设备，包括具有不同“观看方式”的摄像头，这些方式强制执行关于正常行为的社会协议。文章使用了学术语言，一些评论者认为难以理解。

hackernews · eustoria · 6月2日 13:24 · [社区讨论](https://news.ycombinator.com/item?id=48369980)

**背景**: 监控基础设施包括公共和私人摄像头、传感器以及数据收集系统，用于监控公共空间。在西雅图，这类系统迅速扩张，引发了隐私和公民自由的担忧。这次步行之旅旨在让公众看到这个隐形网络。

**社区讨论**: 评论者就安全与隐私之间的权衡进行了辩论，一些人认为在犯罪率高的环境中，视频证据对于起诉是必要的。其他人则批评文章的语言过于学术化，并质疑将监控视为固有压迫性的框架。

**标签**: `#surveillance`, `#privacy`, `#Seattle`, `#technology ethics`, `#civil liberties`

---

<a id="item-11"></a>
## [特朗普签署缩水版人工智能行政令](https://www.politico.com/news/2026/06/02/trump-signs-downsized-ai-order-00946389) ⭐️ 7.0/10

2026 年 6 月 2 日，特朗普总统签署了一项行政令，要求人工智能公司在公开发布前，自愿将强大的新模型提交给政府进行 30 天审查。 该行政令标志着从之前对 AI 监管的不干预态度转变，引发了关于平衡创新、国家安全以及对开源 AI 发展影响的讨论。 审查期限从早期草案的 90 天缩短为 30 天，这是行业反对的结果。该行政令还要求改善网络安全，并制定评估模型安全性的基准。

hackernews · _alternator_ · 6月2日 16:40 · [社区讨论](https://news.ycombinator.com/item?id=48372628)

**背景**: 该行政令是在数周的反复和关于如何在不扼杀创新的情况下监管 AI 的辩论之后出台的。它是全球政府探索对前沿 AI 模型进行监管这一更广泛趋势的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/06/02/technology/trump-executive-order-ai.html">Trump Signs Executive Order Seeking Oversight of A . I . Models</a></li>
<li><a href="https://www.theguardian.com/us-news/2026/jun/02/trump-executive-order-ai-voluntary-review">Trump signs executive order seeking early access to new AI releases</a></li>
<li><a href="https://www.whitehouse.gov/fact-sheets/2026/06/fact-sheet-president-donald-j-trump-promotes-advanced-artificial-intelligence-innovation-and-security/">Fact Sheet: President Donald J. Trump Promotes Advanced Artificial...</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了怀疑，一些人认为自愿审查是迈向强制性监管的一步，可能会限制开源模型。其他人指出该行政令缺乏实质内容，并质疑审查在实践中如何运作。

**标签**: `#AI regulation`, `#executive order`, `#policy`, `#open-source`, `#security`

---

<a id="item-12"></a>
## [浏览器广告归因提案被批为大型科技公司卡特尔](https://blog.zgp.org/the-advertising-cartel-coming-to-your-web-browser/) ⭐️ 7.0/10

一篇博客文章批评了一项基于浏览器的广告归因系统提案，认为它将巩固大型科技公司的追踪主导地位，同时损害小型广告网络和用户隐私。 该提案可能通过让浏览器供应商控制归因来重塑在线广告，可能减少竞争并削弱对用户的隐私保护。 该提案缺乏关于权限或同意的讨论，并创建了一个双轨系统，其中浏览器内置的追踪是选择退出，而第三方广告则面临更严格的隐私规则。

hackernews · speckx · 6月2日 19:39 · [社区讨论](https://news.ycombinator.com/item?id=48375175)

**背景**: 广告归因系统追踪哪些广告带来转化，但当前方法通常依赖跨站追踪。Google 和 Mozilla 等浏览器供应商提出了隐私保护替代方案，例如 Google 的 Privacy Sandbox 归因报告 API，旨在限制数据共享的同时仍能进行广告测量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.mozilla.org/en/mozilla/privacy-preserving-attribution-for-advertising/">Privacy Preserving Attribution for Advertising</a></li>
<li><a href="https://www.nextroll.com/blog/product/privacy-sandbox-attribution-reporting-api-explained">NextRoll - Google’s Privacy Sandbox APIs Explained: Attribution ...</a></li>

</ul>
</details>

**社区讨论**: 评论意见不一：一些人认为该提案对小型广告网络构成威胁，而另一些人则认为大型科技公司在隐私功能上达成一致是积极信号。一位评论者指责作者是广告商，将利润动机伪装成隐私担忧。

**标签**: `#privacy`, `#advertising`, `#web browsers`, `#tracking`, `#big tech`

---

<a id="item-13"></a>
## [PapersWithCode 复活并支持 CVPR 2026 会议](https://www.reddit.com/r/MachineLearning/comments/1tukrf4/browse_cvpr_2026_papers_on_paperswithcode_p/) ⭐️ 7.0/10

Hugging Face 的 Niels 宣布复活 PapersWithCode 为 paperswithcode.co，新增会议支持功能，可按任务浏览 CVPR 2026 论文，并附有代码、项目页面和 Hugging Face 工件的链接。 此次复活恢复了一个备受喜爱的跟踪 AI 前沿研究的平台，使研究人员和从业者更容易发现和复现 CVPR 2026 论文及其相关资源。 该平台索引了所有 CVPR 2026 论文及其 arXiv ID，按任务分类，并标记了 GitHub 链接、项目页面、Hugging Face 工件和评估结果；还支持浏览 Oral 和 Spotlight 论文。

reddit · r/MachineLearning · /u/NielsRogge · 6月2日 08:32

**背景**: PapersWithCode 是一个流行的网站，用于跟踪最新成果并将论文与代码实现关联。它于 2022 年被 Meta 收购，随后关闭。Hugging Face 的复活旨在通过会议浏览等新功能填补这一空白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/nielsr/paperswithcode-launch">Relaunching PapersWithCode with new features</a></li>
<li><a href="https://aiuntethered.com/news/hugging-face-revives-paperswithcode/">Hugging Face Revives PapersWithCode : New... | AiUntethered</a></li>
<li><a href="https://aiweekly.co/alerts/hugging-face-revives-paperswithcode-benchmark-tracker">Hugging Face Revives PapersWithCode Benchmark... | AI Weekly</a></li>

</ul>
</details>

**社区讨论**: Reddit 讨论氛围积极，用户对复活和新会议功能表示兴奋。一些用户询问与 Meta 原 PapersWithCode 的关系，创建者澄清这是一个独立项目。

**标签**: `#CVPR 2026`, `#PapersWithCode`, `#conference papers`, `#computer vision`, `#Hugging Face`

---

<a id="item-14"></a>
## [工人沦为不透明 AI 的“是/否”监督员](https://www.reddit.com/r/LocalLLaMA/comments/1tuth0k/i_have_become_george_jetson_my_job_is_now_yesno/) ⭐️ 7.0/10

一位 Reddit 用户报告称，他们的工作已沦为为一个他们不完全理解的 AI 系统提供“是/否”监督，这突显了人在环上监督的真实案例。 这说明了 AI 自动化的人力成本，工人被留下单调、低自主性的角色，可能降低工作满意度和技能运用，同时也引发了对不透明 AI 模型可靠性的担忧。 该用户描述其角色本质上是监控 AI 的输出并批准或拒绝，而不深入了解模型内部运作，这是一个典型的人在环上场景。

reddit · r/LocalLLaMA · /u/Helpful_Today7449 · 6月2日 14:58

**背景**: 人在环中（HITL）涉及人类主动训练或验证 AI 决策，而人在环上意味着监督性监督，仅在需要时干预。不透明 AI 模型是指其决策过程不易被人类解释的模型，这可能导致信任和安全问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://humansintheloop.org/">Humans in the Loop | Ethical AI with 99% Data Accuracy</a></li>
<li><a href="https://cloud.google.com/discover/human-in-the-loop">What Is Human In The Loop | Google Cloud</a></li>
<li><a href="https://www.abaka.ai/blog/hitl-ai-guide-2026">What Is Human - in - the - Loop AI ? How It Works, Examples... - Abaka AI</a></li>

</ul>
</details>

**社区讨论**: Reddit 讨论显示出复杂情绪：一些用户对失去有意义的工作表示同情，而另一些人则认为这种监督对安全是必要的，工人应该学习系统以重新获得自主权。少数人分享了类似经历，即沦为“人类验证层”。

**标签**: `#AI supervision`, `#human-in-the-loop`, `#automation`, `#job displacement`, `#opaque models`

---

<a id="item-15"></a>
## [花 200 英镑在游戏 PC 中安装 V100 数据中心 GPU](https://www.reddit.com/r/LocalLLaMA/comments/1tuxy5f/i_put_a_datacenter_gpu_in_my_gaming_pc_for_200/) ⭐️ 7.0/10

一位用户成功将二手 Nvidia Tesla V100 数据中心 GPU 安装到标准游戏 PC 中，花费约 200 英镑，从而以远低于消费级 GPU 的成本实现本地 LLM 推理。 这为本地 LLM 社区提供了一种极具成本效益的选择，因为 V100 拥有 16GB HBM2 内存和强大的计算性能，可运行大型模型，从而普及了高端 AI 硬件的使用。 V100 需要特定的电源连接器（8-pin EPS），并且可能需要支持 PCIe 分叉的主板或独立电源；用户可能使用了定制适配器和软件调整才能使其正常工作。

reddit · r/LocalLLaMA · /u/tymscar · 6月2日 17:29

**背景**: Nvidia Tesla V100 是一款基于 Volta 架构的数据中心 GPU，最初为 AI 和高性能计算工作负载设计，拥有 16GB HBM2 内存和 5,120 个 CUDA 核心。与消费级 GPU 不同，数据中心 GPU 通常没有显示输出，需要主动散热，因此 DIY 安装具有挑战性。本地 LLM 推理是指在个人硬件上运行大型语言模型，通常需要具有充足显存和计算能力的 GPU。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kitguru.net/components/graphic-cards/joao-silva/nvidia-releases-the-new-tesla-v100s-datacenter-graphics-card/">Nvidia releases the new Tesla V 100 s datacenter graphics ... | KitGuru</a></li>
<li><a href="https://tet.com.tr/product/tesla-v100-nvidia-gpu-computing-high-performace-computing">Nvidia Tesla V 100 | High Performace Computing | GPU Computing</a></li>
<li><a href="https://grokipedia.com/page/Running_Open-Source_LLMs_Locally">Running Open-Source LLMs Locally</a></li>

</ul>
</details>

**标签**: `#local LLM`, `#GPU`, `#V100`, `#hardware`, `#DIY`

---

<a id="item-16"></a>
## [LLM 编码基准测试：Step 3.7 对比 Qwen 系列](https://www.reddit.com/r/LocalLLaMA/comments/1tuxspu/a_simple_coding_benchmark_step_37_vs_qwen_35/) ⭐️ 7.0/10

一位 Reddit 用户发布了一项实用的编码基准测试，比较了 Step 3.7、Qwen 3.5 122B-A10B、Qwen 3.6 27B 和 Qwen 3.6 35B-A3B，提供了它们在编码任务上的直接性能对比。 这一对比帮助开发者和研究人员为编码任务选择最佳的开源 LLM，揭示了模型规模、效率和性能之间的权衡。 该基准测试可能涵盖多个编码挑战和指标，如通过率、延迟和资源使用。Step 3.7 和 Qwen 3.5 122B-A10B 是采用混合专家架构的新模型，而 Qwen 3.6 系列是较小的密集模型。

reddit · r/LocalLLaMA · /u/remeh · 6月2日 17:24

**背景**: 大型语言模型（LLM）越来越多地用于代码生成和辅助。此类基准测试帮助社区了解官方分数之外的真实性能。Step 3.7 是最近的开源模型，Qwen 3.5/3.6 来自阿里巴巴的 Qwen 系列，其中 122B-A10B 是一个 MoE 模型，每个 token 仅激活 10B 参数。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/qwen/qwen3.5-122b-a10b">Qwen 3 . 5 - 122 B - A 10 B - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://huggingface.co/unsloth/Qwen3.5-122B-A10B-GGUF">unsloth/ Qwen 3 . 5 - 122 B - A 10 B -GGUF · Hugging Face</a></li>
<li><a href="https://recipes.vllm.ai/Qwen/Qwen3.5-122B-A10B">Qwen / Qwen 3 . 5 - 122 B - A 10 B | vLLM Recipes</a></li>

</ul>
</details>

**标签**: `#LLM`, `#benchmark`, `#coding`, `#AI`, `#comparison`

---

<a id="item-17"></a>
## [llama.cpp PR 添加思考模式切换与推理努力级别](https://www.reddit.com/r/LocalLLaMA/comments/1turt87/ui_add_thinking_mode_toggle_with_reasoning_effort/) ⭐️ 7.0/10

allozaur 提交的新拉取请求 (#23434) 为 llama.cpp 引入了可配置推理努力级别（低、中、高）的思考模式切换开关，并改进了聊天表单的用户界面。 此功能让本地 LLM 用户能够精细控制模型的推理深度，对简单查询实现更快响应，对复杂任务进行更深入推理，类似于 GPT-5 和 Claude Opus 4.8 等商业模型的能力。 该切换开关允许启用、禁用或限制思考，努力级别可能映射到内部参数如 max_tokens 或 temperature。PR 还包括聊天表单添加操作按钮的 UI 改进。

reddit · r/LocalLLaMA · /u/jacek2023 · 6月2日 13:59

**背景**: LLM 中的思考模式指模型在生成最终答案前进行逐步推理的能力，通常会产生思维链 token。推理努力级别让用户在速度和彻底性之间取得平衡。llama.cpp 是一个流行的开源 C++ 实现，用于在消费级硬件上本地运行 LLM。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.besthub.dev/articles/how-to-turn-thinking-mode-on-or-off-for-qwen3-5-models-in-ollama-lm-studio-llama-cpp-and-vllm-e303d618cd77">How to Turn Thinking Mode On or Off for Qwen3.5 Model… | BestHub</a></li>
<li><a href="https://arsturn.com/blog/gpt-5-reasoning-effort-levels-explained">GPT-5 Reasoning Effort Levels Explained | A Complete Guide</a></li>
<li><a href="https://www.mindstudio.ai/blog/claude-opus-4-8-effort-levels-explained">Claude Opus 4.8 Effort Levels Explained: Low, Medium... | MindStudio</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#UI`, `#reasoning`, `#local-LLM`, `#open-source`

---

<a id="item-18"></a>
## [Janet 语言：一个带有权衡的现代 Lisp](https://ianthehenry.com/posts/why-janet/) ⭐️ 6.0/10

一篇题为《为什么选择 Janet？》的文章详细探讨了 Janet 编程语言的独特特性和权衡，强调了其最小化设置、可移植性和沙盒功能。 Janet 为寻求轻量级、可嵌入且具有线程和网络等现代特性的 Lisp 语言的开发者提供了一个有吸引力的选择，可能填补了 Scheme 和 Lua 之间的空白。 Janet 是一种具有一等函数、单一命名空间和词法作用域的指令式语言，但缺乏包版本管理和成熟的库生态系统。文章指出，Janet 中的 SETQ 实际上是更新现有绑定，而不是创建新绑定，这与常见误解相反。

hackernews · yacin · 6月2日 09:34 · [社区讨论](https://news.ycombinator.com/item?id=48367907)

**背景**: Janet 是一种现代 Lisp 方言，设计注重简单性和可嵌入性，编译为字节码并在小型 C 运行时上运行。它支持垃圾回收、闭包和事件循环等特性，适用于脚本编写和游戏开发。由于其最小的体积，该语言常被与 Lua 和 Scheme 进行比较。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://janet-lang.org/">Janet Programming Language</a></li>
<li><a href="https://ianthehenry.com/posts/why-janet/">Why Janet? - Ian Henry</a></li>

</ul>
</details>

**社区讨论**: 社区评论既表达了赞赏也提出了批评：一些人称赞 Janet 的可移植性和沙盒功能，而另一些人则对其缺乏包版本管理和库成熟度表示遗憾。还有用户指出文章中关于 SETQ 行为的事实错误，引发了关于语言语义的讨论。

**标签**: `#programming languages`, `#Janet`, `#Lisp`, `#software engineering`

---