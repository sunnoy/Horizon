---
layout: default
title: "Horizon Summary: 2026-08-15 (ZH)"
date: 2026-08-15
lang: zh
---

> 从 37 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [Qwen 3.8 27B 发布：推理与软件工程能力媲美 Gemma 4](#item-tech-news-1) ⭐️ 8.0/10
2. [Firefox 成为最后支持 uBlock Origin 的主流浏览器](#item-tech-news-2) ⭐️ 8.0/10
3. [将 Doom 渲染器编译为 21B 参数 Transformer](#item-tech-news-3) ⭐️ 8.0/10
4. [PostgreSQL 修复高危 to\_char 漏洞，攻击者可执行任意代码](#item-tech-news-4) ⭐️ 8.0/10
5. [Going Dark：执法部门转向黑客攻击的时代](#item-tech-news-5) ⭐️ 7.0/10
6. [RustDesk 实现 Wayland 下真正的无人值守远程访问](#item-tech-news-6) ⭐️ 7.0/10
7. [不必分类，大胆‘幻觉’：LLM 标记的新思路](#item-tech-news-7) ⭐️ 7.0/10
8. [BDH-CQ 模型：通过循环潜推理实现低成本上下文学习](#item-tech-news-8) ⭐️ 7.0/10
9. [苹果自研中国 AI 模型，阿里助获批](#item-tech-news-9) ⭐️ 7.0/10

**财经新闻**
1. [伯克希尔二季度净买入近 200 亿美元，Alphabet 成第三大重仓股](#item-finance-news-1) ⭐️ 8.0/10
2. [高盛从人工智能基础设施融资热潮中获利](#item-finance-news-2) ⭐️ 8.0/10
3. [中国拟解除 Manus 创始人出境限制，前投资者及管理层拟以约 20 亿美元估值回购](#item-finance-news-3) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Qwen 3.8 27B 发布：推理与软件工程能力媲美 Gemma 4](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 8.0/10

Qwen 3.8 27B 模型近期发布，在本地 LLM 评测中展现出与 Gemma 4 相当的推理与软件工程能力。社区私有基准测试中，该模型以 5 倍于 Gemma 4 的令牌量和 12 分 30 秒的推理时间正确完成了任务，且推理过程更为显式。软件工程方面，它能成功编写 JavaScript 待办应用并用 Rust 和 Tauri 重写，具备合格的开发能力。其思考链文本呈现出独特的省略风格，常省略“to”“we”等词，近似“电报体”。不过，该模型的显存效率低于 Gemma 4 和 Glimmer，在 32K 上下文长度下存在不足。

hackernews · erdaltoprak · 8月14日 15:00 · [社区讨论](https://news.ycombinator.com/item?id=49299605)

**「背景」** Qwen 3.8 27B 是 Qwen 在 2026 年 8 月 14 日发布的开源权重 27B 参数语言模型，作为 Qwen 3.8 系列中可在本地运行的中型版本，其上下文窗口为 262k token。该模型量化后可在约 17GB 显存的消费级硬件上运行，因此在本地 LLM 社区中备受关注。

**「影响」** 对于需要本地运行 LLM 的开发者，Qwen 3.8 27B 在推理和软件工程任务上提供了媲美 Gemma 4 的实用选择，但需付出更高的推理时间与令牌消耗代价。

**「社区讨论」** 社区普遍认可该模型的推理与软件工程能力，它成为继 Gemma 4 之后第二个通过私有基准测试的本地模型。同时，其推理速度慢、显存效率低，且思考链中独特的省略风格引发了关于训练数据处理的讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.yottalabs.ai/post/qwen-3-8-27b-specs-hardware-requirements-how-to-run-2026">Qwen 3.8 27B: Specs, Hardware Requirements, and How to Run It (2026) | Yotta Labs</a></li>
<li><a href="https://aireleasetracker.com/model/qwen/qwen3.8-27b">Qwen3.8-27B — Benchmarks, Specs &amp; Release Date</a></li>

</ul>
</details>

**标签**: `#Qwen`, `#local LLM`, `#model release`, `#reasoning`, `#software engineering`

---

<a id="item-tech-news-2"></a>
### [Firefox 成为最后支持 uBlock Origin 的主流浏览器](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 8.0/10

随着 Chrome 全面转向 Manifest V3 并限制 webRequest API，Edge、Brave 等基于 Chromium 的核心浏览器也相继削弱了广告拦截器的能力，唯有 Firefox 继续支持 Manifest V2，因此成为唯一能完整运行 uBlock Origin 的主流浏览器。该变化使 uBlock Origin 等依赖底层网络请求拦截的扩展在 Chrome 上无法完全发挥功能，而 Firefox 仍可为用户提供强大的去广告和隐私保护。此外，Firefox 对包括 uBlock Origin 在内的推荐扩展进行人工代码审查，以防范恶意代码注入。此事件凸显了浏览器扩展生态在开放性与控制权之间的关键分歧。

hackernews · DemiGuru · 8月14日 19:03 · [社区讨论](https://news.ycombinator.com/item?id=49303202)

**「背景」** uBlock Origin 是一款广泛使用的开源内容拦截扩展，能够屏蔽广告、跟踪器等。谷歌 Chrome 浏览器从 Manifest V2 迁移至 Manifest V3，新规范限制了扩展对网络请求的底层访问能力，导致全功能广告拦截器无法正常工作，而 Firefox 仍支持 Manifest V2，因此 uBlock Origin 得以继续完整运行。

**「对用户的影响」** Chrome 用户即将失去 uBlock Origin 支持，若要继续使用完整版扩展，必须迁移至 Firefox；否则只能接受 Manifest V3 下功能受限的替代方案，广告拦截能力将显著下降。

**「社区讨论」** 用户普遍批评 Manifest V3 限制了扩展自由，并担忧开放网络正在被封闭式应用取代。部分评论赞赏 Firefox 对 uBlock Origin 的主动代码审查，而其他用户则感叹大多数用户已经习惯了充斥着广告的网页。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">uBlock Origin - Wikipedia</a></li>
<li><a href="https://www.gamermarkt.com/blog/chrome-ad-blockers-manifest-v3-alternatives/">Chrome Ad Blockers Are Done: Manifest V 3 Explained</a></li>
<li><a href="https://techstory.in/the-end-of-ad-free-browsing-chrome-moves-toward-fully-phasing-out-ad-blockers-with-manifest-v3/">The End of Ad - Free Browsing: Chrome Moves Toward... - TechStory</a></li>

</ul>
</details>

**标签**: `#browsers`, `#privacy`, `#ad-blocking`, `#open-source`, `#Manifest V3`

---

<a id="item-tech-news-3"></a>
### [将 Doom 渲染器编译为 21B 参数 Transformer](https://www.reddit.com/r/MachineLearning/comments/1voazhm/i_compiled_dooms_renderer_into_a_21bparameter/) ⭐️ 8.0/10

一个名为 notforrob 的开发者将 Doom 的渲染算法编译到了一个 21B 参数的 Transformer 中，未经任何训练。他编写了一个自定义编译器，将计算图直接转换为标准 Transformer 权重，并移植了 Doom 渲染流程。最终生成的 checkpoint 可在 Hugging Face 上以标准方式加载，无需 trust\_remote\_code；输入表示场景的提示后，模型生成含像素绘制指令的 token 序列，机械执行这些指令即可获得 E1M1 帧画面。该方案在 B200 GPU 上生成一帧约需 40 分钟，相当于每秒约 35 帧/天，远低于原版 Doom 在 486 上的 35FPS，但展示了一种将算法直接嵌入 Transformer 权重的概念验证。

reddit · r/MachineLearning · /u/notforrob · 8月14日 15:50

**「背景」** 传统上，Transformer 模型通过训练学习数据中的模式，而非直接执行预先定义的算法。该项目通过编译计算图到注意力权重和 MLP 权重，使 Transformer 在推理时按计算图执行特定算法，无需训练。Doom 渲染器原本是运行在 CPU 上的软件光栅化程序，其逻辑被转换为计算图后，才能被编译器处理。

**「影响」** 该工作为可解释性研究和非传统模型用法提供了一种概念验证，表明大型 Transformer 能直接编译并执行复杂算法，但实际性能极低，不具备实用价值。

**标签**: `#transformers`, `#compiler`, `#doom`, `#computation-graphs`, `#novel-approach`

---

<a id="item-tech-news-4"></a>
### [PostgreSQL 修复高危 to\_char 漏洞，攻击者可执行任意代码](https://www.postgresql.org/support/security/CVE-2026-14669/) ⭐️ 8.0/10

PostgreSQL 全球开发组披露了高危漏洞 CVE-2026-14669，该漏洞存在于 to\_char\(timestamptz\) 函数对超长 POSIX 时区缩写的处理中，可导致堆缓冲区溢出。能够设置时区（例如通过会话）的低权限数据库用户可利用此漏洞，在 PostgreSQL 服务进程的操作系统权限下执行任意代码，CVSS 评分为 8.8。漏洞影响所有早于 18.5、17.11、16.15、15.19 和 14.24 的版本；由于 18.5 因回归问题未发布，18 系列用户应直接升级至 18.6，其他受支持的版本线需升级至对应的修复版本。这些修复作为小版本更新发布，只需更新程序文件并重启服务即可，无需转储数据库或运行 pg\_upgrade。

telegram · zaihuapd · 8月14日 14:35

**「背景」** to\_char 是 PostgreSQL 中用于将时间戳格式化为字符串的函数，支持 POSIX 时区缩写（如 EST、EDT）。用户可通过 SET 命令或连接参数设置会话时区，当格式化函数处理超长的时区缩写字符串时，内存拷贝操作可能引发堆缓冲区溢出。

**「影响」** 所有运行受影响 PostgreSQL 版本的数据库管理员应立即应用此次安全更新，因为低权限认证用户可能利用该漏洞完全控制数据库服务器。

**标签**: `#PostgreSQL`, `#security`, `#vulnerability`, `#CVE`, `#database`

---

<a id="item-tech-news-5"></a>
### [Going Dark：执法部门转向黑客攻击的时代](https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/) ⭐️ 7.0/10

随着端到端加密的普及，执法部门正大规模转向利用软件漏洞实施黑客攻击，以突破传统监控手段的“黑暗”地带。这篇分析指出，这种趋势可能引发漏洞市场膨胀、用户安全受损，并引发“漏洞军备竞赛”的可持续性争议。文章强调，尽管漏洞发现能力在提升，但软件复杂性增长可能抵消这一优势，最终使加密对抗陷入僵局。

hackernews · vslira · 8月14日 20:52 · [社区讨论](https://news.ycombinator.com/item?id=49304447)

**「背景」** 在“走向黑暗”的争论中，执法机构认为通信与设备的普遍加密阻碍了犯罪调查，而隐私倡导者和安全专家则强调削弱加密会为所有人制造漏洞。随着传统窃听手段效力下降，政府越来越多地转向利用软件漏洞（即黑客攻击）来获取数据，这实质上改变了监控与网络安全之间的边界。

**「影响」** 对于普通用户，执法部门对漏洞的依赖可能降低其设备安全性，因为未修补的漏洞或降级攻击威胁着所有人的隐私，而不仅仅是犯罪嫌疑人的。现有法律框架可能迫使嫌疑人使用生物特征解锁，暂时减缓完全加密的冲击。

**「社区讨论」** 有评论者认为，AI 编写代码将导致更多漏洞，因此漏洞供应不会见顶；另有人指出，政府可能转向强制生物特征解锁，但民主制度下无法完全避免加密带来的“黑暗”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/">Everything is about to “go dark”</a></li>

</ul>
</details>

**标签**: `#security`, `#cryptography`, `#law-enforcement`, `#privacy`, `#vulnerabilities`

---

<a id="item-tech-news-6"></a>
### [RustDesk 实现 Wayland 下真正的无人值守远程访问](https://rustdesk.com/blog/unattended-remote-access-wayland/) ⭐️ 7.0/10

RustDesk 开源远程桌面工具现已支持在 Wayland 显示服务器上实现真正的无人值守远程访问，解决了 Linux 用户长期面临的功能缺失。该功能允许在没有用户交互的情况下远程连接并控制桌面会话，填补了 Wayland 安全模型下远程管理的关键空白。这一改进使得 RustDesk 成为 Linux 远程桌面场景中更实用的选择，尤其适用于 headless 服务器或无人值守的工作站。

hackernews · rustdesk · 8月14日 16:12 · [社区讨论](https://news.ycombinator.com/item?id=49300759)

**「背景」** Wayland 作为 X11 的继任者，出于安全考虑限制了屏幕捕获和输入注入，导致传统远程桌面工具难以实现无人值守访问，通常需要用户手动授权。RustDesk 此前提供了部分支持，但此次更新通过新的技术方案彻底解决了 Wayland 下无人值守远程控制的难题。

**「影响」** 对于使用 Wayland 的 Linux 用户，RustDesk 现在无需用户在场即可远程访问桌面，显著提升了远程管理、技术支持和 headless 部署的便利性。

**「社区讨论」** 社区反馈总体积极，有用户称赞该修复及时解决了近期遇到的痛点；但也有评论指出 RustDesk 在自托管时仍不支持加密连接，并询问其与 VNC、Remmina、Sunshine/Moonlight 等替代方案的区别。

**标签**: `#remote-desktop`, `#open-source`, `#wayland`, `#linux`, `#rustdesk`

---

<a id="item-tech-news-7"></a>
### [不必分类，大胆‘幻觉’：LLM 标记的新思路](https://simonwillison.net/2026/Aug/14/dont-classify-hallucinate/) ⭐️ 7.0/10

Simon Willison 的博客介绍了 Doug Turnbull 提出的一种新颖的 LLM 标记技术：不再将庞大的标签词汇表直接喂给模型，而是让模型自由生成从未见过的新标签，然后通过向量嵌入计算这些‘幻觉’标签与现有标签库的相似度，匹配出最接近的真实标签。该方法的提示示例要求给出标签的格式样例，以帮助模型生成更贴合语境的候选标签。这一技巧避免了因词汇表过大而超出上下文窗口或增加推理成本，同时提升了标签与内容的语义匹配度，为信息检索和内容管理提供了实用的工程方案。

rss · Simon Willison · 8月14日 21:54

**「背景」** 当待选标签数量庞大时，直接将其全部放入 LLM 提示词会占用大量上下文窗口，导致成本上升、响应变慢，且模型可能难以精准挑选。利用向量嵌入进行语义匹配，可以在不依赖模型记忆全部标签的情况下，仅通过少量生成的候选标签，快速找到最相关的原始标签，从而绕过词汇表规模的限制。

**「影响」** 开发者可以借助这一模式，为拥有庞大标签体系的网站或应用构建轻量、高效的自动标记系统，无需手动精简词汇表，也能获得更贴近语义的标签结果。

**标签**: `#LLM`, `#tagging`, `#embeddings`, `#classification`, `#prompt-engineering`

---

<a id="item-tech-news-8"></a>
### [BDH-CQ 模型：通过循环潜推理实现低成本上下文学习](https://www.reddit.com/r/MachineLearning/comments/1vov5r5/bdhcq_incontext_learning_with_recurrent_latent/) ⭐️ 7.0/10

BDH-CQ 提出了一种将上下文学习与循环潜推理相结合的系统：在推理时，新任务的演示更新循环记忆，随后查询在隐空间中通过迭代计算求解，中间推理状态不解码为语言。该模型在训练阶段不接触任务标识或评估任务示例，推理时也不更新参数。一个 150M 参数的配置在 ARC-AGI-1 上达到 29.5% 的 pass@2，每次任务成本仅 $0.00070，突破了此前报告的成本-精度帕累托前沿。

reddit · r/MachineLearning · /u/moschles · 8月15日 06:18

**「背景」** ARC-AGI-1 是一个评估抽象推理能力的基准，要求模型在未见过任务上展现流体智力，而非依赖记忆或训练数据。此前，该基准上的成本-精度帕累托前沿界定了推理性能与计算开销之间的最优权衡。

**「影响」** 该模型以极低的每次任务成本（$0.00070）在 ARC-AGI-1 上达到 29.5% pass@2，证明了隐式循环推理在成本-精度权衡上的突破，为构建高效推理系统提供了新范式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/leaderboard">ARC Prize - Leaderboard</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#in-context learning`, `#reasoning`, `#ARC-AGI`, `#recurrent latent reasoning`

---

<a id="item-tech-news-9"></a>
### [苹果自研中国 AI 模型，阿里助获批](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 7.0/10

苹果已专门为中国市场训练了一款大语言模型，并获得阿里巴巴支持，一改此前依赖第三方模型的策略。该模型已通过中国网信办的生成式 AI 服务备案，搭载 Apple Intelligence 的 iOS 更新预计在未来数月内上线。这一自研模型将使苹果直接掌控在华 AI 体验，并可能使其成为首个获北京批准提供自有 AI 模型的外国公司。

telegram · zaihuapd · 8月14日 14:47

**「背景」** 苹果此前在中国市场依赖第三方大模型，曾与阿里巴巴合作将其通义千问（Qwen）模型整合进 Apple Intelligence 功能。中国对生成式 AI 服务实行备案制，网信办要求境外公司通常需与本地伙伴合作并将模型通过备案后方可向公众提供。苹果此次自研中国专属模型并由阿里巴巴支持，标志着其策略从依赖第三方转向自主开发，以更好地适应本地监管与用户体验需求。

**「影响」** 苹果将直接掌控中国市场的 AI 功能合规与体验，并有望成为首个在华获批部署自有 AI 模型的外国公司，为其 AI 服务本地化扫清关键障碍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/08/14/apple-trained-own-ai-model-for-china/">Apple Trained Own AI Model for China Market With Help From Alibaba - MacRumors</a></li>

</ul>
</details>

**标签**: `#Apple`, `#AI`, `#China`, `#LLM`, `#Alibaba`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [伯克希尔二季度净买入近 200 亿美元，Alphabet 成第三大重仓股](https://www.cnbc.com/2026/08/14/berkshire-hathaway-boosts-alphabet-to-a-top-three-holding-ups-delta-and-housing-bets.html) ⭐️ 8.0/10

伯克希尔哈撒韦第二季度 13F 文件显示，该季度净买入股票近 200 亿美元，结束了连续 14 个季度的净卖出；其中对 Alphabet 的持仓增加 83%，使其成为公司第三大美国上市股票持仓。

rss · CNBC Finance · 8月14日 21:06

**「背景」** 此前，伯克希尔连续 14 个季度为股票净卖出方，现金储备在今年一季度末曾创下 3974 亿美元的历史纪录。

**标签**: `#Berkshire Hathaway`, `#Alphabet`, `#Delta Air Lines`, `#homebuilders`, `#portfolio changes`

---

<a id="item-finance-news-2"></a>
### [高盛从人工智能基础设施融资热潮中获利](https://www.cnbc.com/2026/08/14/goldmans-latest-cash-cow-is-all-about-funding-the-ai-infrastructure-boom.html) ⭐️ 8.0/10

高盛正从人工智能基础设施融资中获利，参与英伟达 5000 亿美元融资计划，并担任英特尔（200 亿美元）和 Alphabet（850 亿美元）股票发行的联合账簿管理人。

rss · CNBC Finance · 8月14日 20:05

**「背景」** 人工智能热潮推动科技公司大规模融资，以建设数据中心和芯片制造能力，投资银行借此获得股权承销等业务机会。

**「影响」** 高盛全球银行与市场部门的费用收入因此增加，巩固了其作为大型科技公司融资首选合作伙伴的地位。

**标签**: `#Goldman Sachs`, `#AI infrastructure`, `#equity underwriting`, `#technology financing`, `#investment banking`

---

<a id="item-finance-news-3"></a>
### [中国拟解除 Manus 创始人出境限制，前投资者及管理层拟以约 20 亿美元估值回购](https://www.ft.com/content/fa479d50-7c79-4b6d-99c3-3830e37c1503?syn-25a6b1a6=1) ⭐️ 8.0/10

中国计划解除 AI 初创公司 Manus 创始人的出境限制，包括腾讯在内的前投资者及管理层拟以约 20 亿美元估值从 Meta 回购公司。交易仍需监管部门批准，完成后腾讯将成为最大股东但仅持少数股权，Manus 将继续在新加坡独立运营。

telegram · zaihuapd · 8月15日 08:05

**「背景」** 此前，中国国家发改委以“数据清洗”为由，命令 Meta 撤销对 Manus 母公司蝴蝶效应的收购，并禁止两位创始人出境。现拟解除该限制，并安排由腾讯等前投资者及管理层回购公司。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reuters.com/world/asia-pacific/china-blocks-foreign-acquisition-ai-startup-manus-2026-04-27/">China orders Meta to unwind $2 billion purchase of AI startup Manus | Reuters</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/manus-returns-independence-china-blocks-170145849.html">Manus returns to independence after China blocks Meta acquisition</a></li>

</ul>
</details>

**标签**: `#cross-border M&amp;A`, `#AI buyback`, `#Tencent`, `#Meta`, `#China travel restrictions`

---