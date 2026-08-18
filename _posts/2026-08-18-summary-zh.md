---
layout: default
title: "Horizon Summary: 2026-08-18 (ZH)"
date: 2026-08-18
lang: zh
---

> 从 43 条内容中筛选出 14 条重要资讯。

---

**科技新闻**
1. [DuckDB v2.0 预览版亮点](#item-tech-news-1) ⭐️ 9.0/10
2. [Linux 7.3 提升 VRAM 不足时的性能](#item-tech-news-2) ⭐️ 8.0/10
3. [谷歌购破产精神航空数据训练 AI](#item-tech-news-3) ⭐️ 8.0/10
4. [AI 生成的 Copilot 代码导致 Snowflake Jira 管道模板注入漏洞](#item-tech-news-4) ⭐️ 8.0/10
5. [Rust GPU 卸载系统：安全、可移植、快速](#item-tech-news-5) ⭐️ 8.0/10
6. [Qwen 3.8 27B 得分 52，媲美超大规模模型](#item-tech-news-6) ⭐️ 8.0/10
7. [Fairphone 6 主摄工作](#item-tech-news-7) ⭐️ 7.0/10
8. [AirTag 追踪证实稀有书籍流入亚马逊 AI 训练设施](#item-tech-news-8) ⭐️ 7.0/10
9. [macOS 26.7 代码曝光大陆 Apple 智能审查机制](#item-tech-news-9) ⭐️ 7.0/10
10. [企业微信 5.0.10 开放 CLI 与 MCP，接入 10 大办公模块](#item-tech-news-10) ⭐️ 7.0/10
11. [中国要求部分政府机构卸载定制版 Windows 10，停用计划提前](#item-tech-news-11) ⭐️ 7.0/10

**财经新闻**
1. [先买后付贷款扩展至生活必需品，2025 年美国借贷额达 1600 亿美元](#item-finance-news-1) ⭐️ 8.0/10
2. [预测市场显示派拉蒙收购华纳兄弟探索公司失败概率约四分之一](#item-finance-news-2) ⭐️ 7.0/10
3. [苹果美国 App Store 佣金收入下降 18%，用户消费额同比降 6%](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [DuckDB v2.0 预览版亮点](https://duckdb.org/2026/08/17/duckdb-20-highlights) ⭐️ 9.0/10

DuckDB 团队发布了 v2.0 预览版，揭开了这一广受喜爱的嵌入式分析数据库下一个重大版本的面纱。预览版中展示了 Quack 等新功能，并继续强化对超大文件处理、空间分析等场景的支持，社区反响热烈。值得注意的是，该版本在不到六个月时间内积累了超过 10,000 次提交，引发了社区对 AI 辅助开发加速的讨论。预览版旨在展示未来正式版方向，目前尚未提供完整特性列表。

hackernews · ibotty · 8月17日 13:46 · [社区讨论](https://news.ycombinator.com/item?id=49330781)

**「背景」** DuckDB 是一个流行的嵌入式分析型数据库，以高性能、轻量级和易用性著称，常被用于数据工程和分析场景。即将发布的 v2.0 是一次重大版本更新，预览版展示了包括服务器模式、触发器、VARIANT 类型、异步 I/O、新 SQL 解析器和存储格式等在内的多项重要特性。该版本预计于今年秋季正式推出。

**「影响」** 对于依赖 DuckDB 进行嵌入式分析的数据工程师与分析师，v2.0 预览版展示的 Quack 等新功能及大规模数据处理优化，有望进一步降低资源消耗并提升性能，但正式版特性尚未最终确定。

**「社区讨论」** 社区普遍表达了对 DuckDB v2.0 的强烈期待与喜爱，许多用户分享了在生产环境中处理实时分析、流事件等场景的积极经验。同时，有评论注意到预览版相关的大量提交，对 AI 工具在开发中的参与程度提出了疑问，但讨论仍以正面为主。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://duckdb.org/2026/08/17/duckdb-20-highlights">A Preview of DuckDB v2.0 – DuckDB</a></li>

</ul>
</details>

**标签**: `#duckdb`, `#databases`, `#analytics`, `#open-source`, `#release-preview`

---

<a id="item-tech-news-2"></a>
### [Linux 7.3 提升 VRAM 不足时的性能](https://pixelcluster.dev/VRAM-Overcommit/) ⭐️ 8.0/10

Linux 内核 7.3 版本将为 VRAM 引入过度提交（overcommit）逻辑，通过更智能的内存回收与分配策略，在 GPU 显存耗尽时提升系统性能并避免崩溃。该机制使内核能够根据应用需求灵活调配系统内存与显存，减少因显存不足导致的应用程序或桌面环境突然崩溃。这一改进对 AI 训练、游戏和图形密集型工作负载尤为关键，可在不增加硬件成本的情况下显著增强稳定性。具体的实现涉及内存压力下的页面回收和 GPU 调度优化，但内核仍依赖应用自身的显存使用提示来获得最佳效果。

hackernews · flaburgan · 8月18日 07:51 · [社区讨论](https://news.ycombinator.com/item?id=49342719)

**「背景」** 该文章作者此前为 AMD GPU 开发了显存管理改进，相关补丁已合并至 Linux 7.3 内核。此次新文章进一步讲解了内核的 VRAM 超量使用（overcommit）逻辑，旨在当物理显存耗尽时防止崩溃并提升性能。

**「影响」** 对于使用 Linux 的 GPU 加速应用（如游戏、AI 推理、桌面合成器）的用户，该改进将显著减少因显存耗尽导致的程序崩溃或系统冻结，提升日常使用和关键工作负载的可靠性。

**「社区讨论」** 社区普遍对 Linux 7.3 的 VRAM 改进表示期待，并分享了该问题在旧 NVIDIA 显卡上导致应用崩溃和桌面不稳定的实际体验。有评论指出，与 Windows 相比，Linux 在内存耗尽时的行为仍有改进空间，但此次内核更新向解决这类痛点迈出了重要一步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pixelcluster.dev/VRAM-Overcommit/">VRAM Management Part 2: Beyond the Limits of Physical VRAM | pixelcluster&#x27;s GPU blog</a></li>
<li><a href="http://pixelcluster.dev/VRAM-Mgmt-fixed/">Fixing AMDGPU&#x27;s VRAM management for low-end GPUs | pixelcluster&#x27;s GPU blog</a></li>

</ul>
</details>

**标签**: `#linux-kernel`, `#vram-overcommit`, `#gpu-memory`, `#performance`, `#memory-management`

---

<a id="item-tech-news-3"></a>
### [谷歌购破产精神航空数据训练 AI](https://www.theregister.com/ai-and-ml/2026/08/18/google-buys-crashed-airline-spirits-data-at-auction-because-ai/5288962) ⭐️ 8.0/10

谷歌在精神航空（Spirit Airlines）破产拍卖中购得逾 1 亿封邮件、5 亿条 Microsoft Teams 消息、超 3000 万通客服录音及大量其他企业数据，用于 AI 模型训练。该数据集涵盖客服聊天记录、ServiceNow 工单、营销邮箱地址和机上 Wi‑Fi 销售记录等，总规模达数百万条。尽管合同要求由第三方“去标识化”代理处理后再移交谷歌，但评论者普遍怀疑能否彻底剥离个人身份信息。此举引发对破产数据资产化、隐私合规及 AI 训练数据来源的伦理争议。

hackernews · pseudolus · 8月18日 10:13 · [社区讨论](https://news.ycombinator.com/item?id=49343559)

**「背景」** Spirit 航空在 2020 年新冠疫情冲击下持续亏损，最终于 2026 年 5 月永久停飞并进入破产清算。作为破产程序的一部分，其数据资产被公开拍卖，其中包含大量电子邮件、Teams 消息、客户服务录音等。此次拍卖竞争激烈，Google 以 500 万美元的出价胜出，竞争对手 Mercor 曾提出以 520 万至 700 万美元换取原始数据。

**「影响」** 谷歌因此获得丰富真实企业对话数据，有望加速其 AI 客服与协作助手的发展。但所涉数千万人的通信记录去标识化效果存疑，隐私风险未能消除。

**「社区讨论」** 社区广泛质疑第三方“去标识化”能否真正剥离个人身份，有评论指出含有大量可识别信息（如客服录音、邮件内容）无法彻底匿名化。此外，不少人认为破产企业出售内部通信记录本身就令人不安，反映数据资产化的极端案例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theregister.com/ai-and-ml/2026/08/18/google-buys-crashed-airline-spirits-data-at-auction-because-ai/5288962">Google buys crashed airline Spirit ’ s data at auction , because AI</a></li>
<li><a href="https://www.businessinsider.com/google-buys-spirit-airlines-data-ai-model-development-2026-8">Google Buys Spirit Airlines Data for AI Model... - Business Insider</a></li>

</ul>
</details>

**标签**: `#AI`, `#data-privacy`, `#training-data`, `#Google`, `#corporate-data`

---

<a id="item-tech-news-4"></a>
### [AI 生成的 Copilot 代码导致 Snowflake Jira 管道模板注入漏洞](https://www.wiz.io/blog/red-agent-snowflake-copilot-cicd-bug) ⭐️ 8.0/10

Snowflake 的 Jira CI/CD 管道中使用的 GitHub Actions 工作流被发现存在模板注入漏洞，安全研究人员将此漏洞归因于 GitHub Copilot“Autofix”功能生成的 AI 代码。该漏洞位于\`jira\_issue.yml\`工作流，通过\`echo\`命令扩展 Jira 议题标题或正文时未进行适当转义，导致攻击者可通过控制议题内容注入恶意命令。这一事件凸显了在关键自动化流程中依赖 AI 生成代码而缺乏严格静态分析的安全风险。

hackernews · galnagli · 8月17日 14:18 · [社区讨论](https://news.ycombinator.com/item?id=49331423)

**「GitHub Actions 模板注入漏洞背景」** GitHub Actions 工作流中如果在 \`run\` 步骤内直接使用 \`$\{\{ github.event.\* \}\}\` 表达式，会导致模板注入，攻击者可通过 Jira Issue 标题提交恶意命令。Snowflake 的 Jira 自动化流水线（jira\_issue.yml）在通过 PR \#1218 更新时引入了此漏洞，使研究人员能够模拟攻击其内部 Jira 实例。该 PR 同时包含了 Copilot Autofix 对 jira\_close.yml 的修复，但公开记录显示注入漏洞并非由 Copilot 直接生成。

**「影响」** 该漏洞可能允许对关联 Jira 议题有控制权的攻击者在 GitHub Actions 运行器中执行任意命令，从而威胁 Snowflake 的构建环境。

**「社区讨论」** 部分评论者指出，所关联的 Pull Request 中 Copilot 共同编写的提交与漏洞并无直接关系，对 AI 代码的直接归因提出质疑。多数讨论认为，在 CI/CD 工作流中缺乏类似 zizmor 的静态分析工具是严重疏忽，并强调了“LGTM”式代码审查无法有效发现 AI 生成代码中的隐蔽注入缺陷。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wiz.io/blog/red-agent-snowflake-copilot-cicd-bug">Red Agent Exploits Snowflake Vuln Missed by Github Copilot | Wiz Blog</a></li>
<li><a href="https://www.cyberkendra.com/2026/08/copilot-autofix-snowflake-jira-github-actions.html">Copilot Autofix Bug Exposed Snowflake&#x27;s Internal Jira - Cyber Kendra</a></li>
<li><a href="https://thehackernews.com/2026/08/snowflake-github-actions-flaw-lets_0330881554.html">Snowflake GitHub Actions Flaw Lets Crafted Issues Trigger Command Injection</a></li>

</ul>
</details>

**标签**: `#security`, `#AI`, `#GitHub Actions`, `#Copilot`, `#supply-chain`

---

<a id="item-tech-news-5"></a>
### [Rust GPU 卸载系统：安全、可移植、快速](https://arxiv.org/abs/2608.13759) ⭐️ 8.0/10

一项新研究提出了一种 Rust 的 GPU 卸载系统，可将 Rust 代码直接编译为 GPU 内核，旨在提供安全、可移植且高性能的 GPU 编程体验，无需手动编写 C/C++ 绑定。该系统自动处理主机与设备间的数据移动，并利用 Rust 的所有权模型实现内存安全，目前处于活跃开发阶段，计划上游合入 Rust 编译器。该方案有望让 Rust 开发者（尤其是 AI 和大语言模型推理领域）摆脱维护绑定的痛苦，在社区中引起了强烈兴趣。

hackernews · linggen · 8月17日 17:54 · [社区讨论](https://news.ycombinator.com/item?id=49334991)

**「背景」** Rust 语言通过严苛的所有权模型在编译期保障主机端代码的内存安全，但 GPU 编程长期以来依赖手动编写 CUDA 等 C/C++ 绑定，不仅破坏了安全保证，也带来了可移植性负担。该论文基于 LLVM Offload 框架，试图在 Rust 中实现一个安全、便携且足够高效的 GPU 编程接口，以填补 Rust 生态中缺少原生 GPU 内核方案的空白。

**「影响」** 若该系统成功上游并成熟，Rust 开发者将能够直接在 Rust 中编写 GPU 加速代码，从而消除维护脆弱的 C/C++ 绑定这一主要痛点，尤其在 AI/LLM 推理项目中。不过，该项目尚在早期开发阶段，尚未可用，其实质影响仍有待观察。

**「社区讨论」** Rust 开发者对消除 GPU 绑定的承诺表现出强烈兴趣，但也有声音质疑其依赖 LLVM 而非直接生成 PTX/HIP C 或通过 Vulkan/SPIR-V 等厂商中立方案实现。此外，社区指出论文尚未公开代码，并认为 Rust 的所有权模型天然适合 GPU 内存生命周期管理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.13759">[ 2608 . 13759 ] GPU Offload in Rust : Portable , Safe , and Fast</a></li>
<li><a href="https://xenospectrum.com/en/rust-gpu-offload-llvm-safe-kernels-performance/">A GPU kernel written in safe Rust matched... | XenoSpectrum</a></li>

</ul>
</details>

**标签**: `#Rust`, `#GPU`, `#compiler`, `#systems-programming`, `#open-source`

---

<a id="item-tech-news-6"></a>
### [Qwen 3.8 27B 得分 52，媲美超大规模模型](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 8.0/10

Qwen 3.8 27B 在 Artificial Analysis Intelligence Index 上取得 52 分，与 GPT-5.6 Luna（max）持平，仅比 753B 的 GLM-5.2（max）和 1.7T 参数的 DeepSeek V4 Pro 0813（max）落后一分。该成绩表明一个 27B 的小模型达到了与参数规模大 28 至 63 倍的模型相当的智能水平，直接挑战了以参数规模为核心驱动力的扩展假设。这一结果对追求高效部署的 AI 研究者和工程团队具有重要参考价值，显示了小模型在性能效率上的巨大潜力。

rss · Simon Willison · 8月17日 23:58

**「背景」** Artificial Analysis Intelligence Index 是一项综合评估大语言模型智能水平的基准指标，分数基于多个维度测试得出。GPT-5.6 Luna、GLM-5.2 和 DeepSeek V4 Pro 0813 均为当前领先的大语言模型，参数量在数百亿至数千亿级别，通常被视为性能与规模正相关的代表。

**「影响」** 对于需要本地部署或追求成本效益的开发者与企业，Qwen 3.8 27B 证明了在有限参数下也可获得接近顶尖闭源大模型的性能，有望显著降低推理所需的硬件门槛和运营成本。

**标签**: `#ai`, `#machine-learning`, `#llms`, `#benchmarks`, `#qwen`

---

<a id="item-tech-news-7"></a>
### [Fairphone 6 主摄工作](https://catcrafts.net/posts/fairphone-6-postmarketos-working-main-camera) ⭐️ 7.0/10

有开发者成功在 Fairphone 6 上运行 PostmarketOS 并驱动了主摄像头，这是移动 Linux 取得进展的重要一步。该工作涉及针对高通平台的摄像头栈移植，展示了主线内核在现代手机硬件支持上的进步。尽管主摄像头已可用，但内部扬声器和麦克风等关键组件仍无法工作，设备尚不适合日常使用。

hackernews · pizzaiolo · 8月17日 22:01 · [社区讨论](https://news.ycombinator.com/item?id=49338285)

**「背景」** Fairphone 6 搭载高通 SM7635 \(milos\) 平台，其摄像头硬件包含 TFE665、CSID665 和 CSIPHY v2.2.1 等 ISP 模块。此前，社区已基于主线内核分支为广角镜头提供了初步支持；本次工作在此基础上为后置主摄编写了驱动，实现了自动对焦与色彩校正。

**「影响」** Fairphone 6 的 PostmarketOS 用户现在可以使用主摄像头拍照，但缺少内部音频支持意味着该设备仍无法作为日常主力机使用。

**「社区讨论」** 社区对主摄像头驱动成功表示兴奋，同时也指出扬声器和麦克风缺失的问题，使得设备难以日常使用。讨论还涉及了完全开放手机生态的潜力，以及移植到其他设备时遇到的类似挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://catcrafts.net/posts/fairphone-6-postmarketos-working-main-camera">Fairphone 6 + PostmarketOS working main camera! — Catcrafts</a></li>
<li><a href="https://nondescriptpointer.com/articles/fairphone-6-wide-camera-linux/">Experimental Linux support for the Fairphone 6 wide camera · nondescriptpointer</a></li>

</ul>
</details>

**标签**: `#postmarketos`, `#fairphone`, `#linux-mobile`, `#camera-enablement`, `#open-source`

---

<a id="item-tech-news-8"></a>
### [AirTag 追踪证实稀有书籍流入亚马逊 AI 训练设施](https://simonwillison.net/2026/Aug/17/we-tracked-a-shipment-of-rare-books-it-ended-at-an-amazon-ai-tra/) ⭐️ 7.0/10

404 Media 将一个 Apple AirTag 放入一本通过 Biblio 平台订购的书籍中，该订单包含约 1000 本稀有书籍，并追踪到这批书最终被送至拉斯维加斯东北部的亚马逊 LAS8 设施，特别是 VGT3 区域，其入口处有一个恐龙抓书的标志。亚马逊员工在在线论坛上的讨论证实，VGT3 会对大量书籍进行破坏性扫描。该调查为人们长期以来的猜测——即 AI 公司通过大宗采购实体书来获取训练数据——提供了直接证据。

rss · Simon Willison · 8月17日 15:21

**「背景」** 此前，针对 Anthropic 的诉讼文件显示，该公司在 2024 年春季购买了数百万册新旧书籍并销毁以扫描用于 AI 训练。图书销售商长期怀疑，那些对价格不敏感、大量购入看似无关书籍的匿名买家实为 AI 公司。此次 404 Media 的追踪调查，通过 AirTag 将一箱稀有书籍的物流终点锁定在亚马逊的 AI 训练设施，为此类猜测提供了直接证据。

**「影响」** 此次调查揭示亚马逊批量采购稀有书籍后直接对其进行破坏性扫描以获取 AI 训练数据，迫使书商面临出售珍稀藏书可能使其毁于文化传承的伦理困境。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theatlantic.com/technology/2026/08/ai-companies-buying-used-books-for-data/688167/">Someone Is Mysteriously Snapping Up Used Books Around the World - The Atlantic</a></li>
<li><a href="https://www.eweek.com/news/amazon-books-ai-training-data/">Amazon Is Reportedly Buying and Destroying Books to Feed Its AI | eWeek</a></li>
<li><a href="https://www.ndtvprofit.com/technology/hidden-tracker-reveals-amazon-mass-scans-shred-books-just-to-feed-ai-report-11923001">Hidden Tracker &#x27;Reveals&#x27; Amazon Mass-Scans, Shred Books Just To Feed AI: Report</a></li>
<li><a href="https://arstechnica.com/tech-policy/2026/08/hidden-airtag-reveals-amazon-is-trashing-rare-books-to-train-ai/">Hidden Airtag reveals Amazon is trashing rare books to train AI - Ars Technica</a></li>

</ul>
</details>

**标签**: `#AI training data`, `#Amazon`, `#investigative reporting`, `#data sourcing`, `#AI ethics`

---

<a id="item-tech-news-9"></a>
### [macOS 26.7 代码曝光大陆 Apple 智能审查机制](https://www.macrumors.com/2026/08/17/macos-26-7-unreleased-apple-devices/) ⭐️ 7.0/10

macOS 26.7 代码揭示，苹果为中国大陆的 Apple Intelligence 写作工具内置了独立的内容安全过滤机制。系统会提示“需要进行内容安全更新”，并在自动更新完成后启用写作功能；对于无法编辑的文本，会引导用户尝试其他方式。若多次触发安全警报，写作工具将暂时受限，表明存在处罚性的使用限制。审查规则可通过云控远程下发，显示苹果在中国市场实施了动态、可远程调整的 AI 内容审查体系。

telegram · zaihuapd · 8月18日 02:16

**「背景」** Apple Intelligence 写作工具是苹果设备集成的 AI 辅助写作功能，能帮助用户改写、总结文本。在中国大陆，AI 服务需遵循内容安全法规，因此苹果必须为本地化版本加入合规机制，以过滤或限制可能违规的内容。

**「影响」** 中国大陆用户使用写作工具时将面临内容过滤和临时功能限制，敏感内容可能无法编辑，且多次触发安全警报后写作工具将暂时不可用。

**标签**: `#Apple Intelligence`, `#censorship`, `#China`, `#macOS`, `#content moderation`

---

<a id="item-tech-news-10"></a>
### [企业微信 5.0.10 开放 CLI 与 MCP，接入 10 大办公模块](https://mp.weixin.qq.com/s/uJf57P15-FQL_u6jLHiGYA) ⭐️ 7.0/10

企业微信 5.0.10 版本面向所有企业开放命令行接口（CLI）与模型上下文协议（MCP）能力，支持 WorkBuddy、DeepSeek Harness 及企业自建 AI 代理直接调用 10 大核心办公模块。安全方面，提供人员与 AI 权限隔离、关键操作人工审批、限时授权和完整审计日志。AI 代理还能读取文档和表格、分析数据，并生成提案 PPT 或经营看板，将自动化深度融入企业办公流程。

telegram · zaihuapd · 8月18日 06:22

**「背景」** CLI（命令行界面）和 MCP（模型上下文协议）是当前 AI 代理与外部工具、服务进行标准化交互的关键方式，其中 MCP 定义了统一的数据接入规范。企业微信此前主要面向内部办公，此次开放意味着外部 AI 代理可通过标准协议直接调用其审批、文档、数据分析等模块，降低企业自建智能工作流的集成门槛。

**「影响」** 企业微信成为 AI 代理触达企业协作场景的开放平台，开发者可据此构建安全可控的自动化办公应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol ( MCP )? - Model Context Protocol</a></li>

</ul>
</details>

**标签**: `#enterprise-software`, `#ai-agents`, `#mcp`, `#wechat-work`, `#api-integration`

---

<a id="item-tech-news-11"></a>
### [中国要求部分政府机构卸载定制版 Windows 10，停用计划提前](https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan) ⭐️ 7.0/10

中国国家安全部已要求部分政府相关机构卸载定制版 Windows 10，将原定于 2027 年 2 月的停用计划提前数月。该指令源于数据安全担忧，但未披露具体漏洞细节。微软表示，未发现影响该定制版产品的安全事件，且该产品仍在定期获得安全更新。此举凸显了中国对政府 IT 供应链安全的持续关注，可能加速国产操作系统在关键领域的替代进程。

telegram · zaihuapd · 8月18日 06:22

**「背景」** 中国曾为政府机构推出定制版 Windows 10，作为其减少对外国技术依赖战略的一部分。原计划于 2027 年 2 月停用该版本，但近期国家安全部以数据安全担忧为由，要求部分机构提前卸载。微软表示该定制版仍在定期获得安全更新，且未发现相关安全事件。

**「影响」** 受影响的中国政府机构将被迫提前放弃定制版 Windows 10，加速转向国产操作系统，直接利好麒麟信安、诚迈科技等国产 OS 厂商，并推动政务 IT 领域的信创替代进程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/software/operating-systems/china-reportedly-orders-state-agencies-to-uninstall-its-government-only-edition-of-windows-10">China reportedly orders state agencies to uninstall... | Tom&#x27;s Hardware</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan">China Removes Microsoft Windows at State Users Ahead of Plan</a></li>
<li><a href="https://windowsforum.com/windows-news.4/china-orders-some-groups-off-windows-10-government-edition.443067/">China Orders Some Groups Off Windows 10 Government Edition</a></li>
<li><a href="https://www.tomshardware.com/software/operating-systems/china-reportedly-orders-state-agencies-to-uninstall-its-government-only-edition-of-windows-10">China reportedly orders state agencies to uninstall its government-only edition of Windows 10 — Beijing accelerates planned retirement over data security concerns | Tom&#x27;s Hardware</a></li>

</ul>
</details>

**标签**: `#Windows`, `#China`, `#cybersecurity`, `#government IT`, `#software policy`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [先买后付贷款扩展至生活必需品，2025 年美国借贷额达 1600 亿美元](https://www.nytimes.com/2026/08/17/business/buy-now-pay-later.html) ⭐️ 8.0/10

美国“先买后付”贷款服务在 2025 年新增覆盖水电、房租等日常支出，全年消费者借款总额达 1600 亿美元，较 2023 年近乎翻倍。

telegram · zaihuapd · 8月18日 01:41

**「背景」** 此类贷款原本主要用于网购，现因机构将其扩展至基本生活开支，且 LendingTree 调查显示半数用户称没有这类贷款就难以维持收支，引发关注。

**「影响」** 消费者若过度依赖，可能因自动扣款导致银行透支费，并因多数贷款未纳入征信而难以管理债务，形成债务陷阱。

**标签**: `#BNPL`, `#consumer debt`, `#fintech lending`, `#household finance`, `#US economy`

---

<a id="item-finance-news-2"></a>
### [预测市场显示派拉蒙收购华纳兄弟探索公司失败概率约四分之一](https://www.cnbc.com/2026/08/17/pskys-wbd-bid-has-1-in-4-odds-of-falling-through-kalshi-traders-say.html) ⭐️ 7.0/10

预测市场交易员认为派拉蒙天舞影业在 2027 年 7 月前成功收购华纳兄弟探索公司的概率为 74%，而交易失败的概率为 22%。这一概率在 12 个州总检察长于 7 月 13 日提起诉讼后，从原先超过 80%的水平下降，并在派拉蒙宣布延期至 2027 年时一度跌至 66%。

rss · CNBC Finance · 8月17日 17:43

**「背景」** 预测市场平台如 Kalshi 和 Polymarket 允许交易员对并购等事件结果下注，反映市场对事件发生概率的集体判断。本次诉讼由加州等 12 个州的总检察长提起，旨在以反垄断为由阻止该媒体合并案，导致交易前景出现不确定性。

**「影响」** 诉讼为这笔大型媒体合并增添了司法障碍，加大了交易在 2027 年截止日前无法完成的风险，可能影响派拉蒙和华纳兄弟探索公司股东的回报预期。

**标签**: `#M&amp;A`, `#Media`, `#Prediction Markets`, `#Antitrust`, `#Warner Bros. Discovery`

---

<a id="item-finance-news-3"></a>
### [苹果美国 App Store 佣金收入下降 18%，用户消费额同比降 6%](https://www.macrumors.com/2026/08/18/apple-app-store-revenue-falling/) ⭐️ 7.0/10

Appfigures 数据显示，苹果美国 App Store 佣金收入自 2026 年初下降 18%；Sensor Tower 称，美国用户第二季度 App Store 消费额同比下降 6%，而去年同期增长 9%。苹果表示，监管变化已拖累服务业务增长。

telegram · zaihuapd · 8月18日 12:17

**「背景」** 苹果公司表示，近期针对应用商店的监管变化已开始拖累其服务业务增长，此前美国等地出台了限制应用商店佣金的新规。

**标签**: `#Apple`, `#App Store`, `#regulation`, `#services revenue`, `#consumer spending`

---