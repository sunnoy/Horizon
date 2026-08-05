---
layout: default
title: "Horizon Summary: 2026-08-05 (ZH)"
date: 2026-08-05
lang: zh
---

> 从 46 条内容中筛选出 18 条重要资讯。

---

**科技新闻**
1. [展示 HN：简单算法与色彩空间生成多样化肤色](#item-tech-news-1) ⭐️ 8.0/10
2. [生成式 AI 与软件工程的八大迷思](#item-tech-news-2) ⭐️ 8.0/10
3. [LLM 0.32 发布：新增推理轨迹、服务端工具与智能日志支持](#item-tech-news-3) ⭐️ 8.0/10
4. [llm-anthropic 0.26 发布：支持 Claude 5 模型与服务器端工具](#item-tech-news-4) ⭐️ 8.0/10
5. [白宫开源 AI 监管急转弯，硅谷分裂](#item-tech-news-5) ⭐️ 8.0/10
6. [ChainDrop 蠕虫攻陷逾 1300 个 npm 包](#item-tech-news-6) ⭐️ 8.0/10
7. [豆包上线原生音视频全双工模型](#item-tech-news-7) ⭐️ 8.0/10
8. [FFmpeg 9.0 发布，新增动画 WebP 支持](#item-tech-news-8) ⭐️ 8.0/10
9. [MiniMax-H3 模型移植至 MLX，可在 Apple Silicon 本地运行](#item-tech-news-9) ⭐️ 7.0/10
10. [SpaceX 将独家采用英伟达 Vera Rubin AI 架构](#item-tech-news-10) ⭐️ 7.0/10
11. [三星与 SK 海力士据报测试中微刻蚀设备对冲美管制](#item-tech-news-11) ⭐️ 7.0/10

**财经新闻**
1. [Polymarket 正洽谈估值超 200 亿美元融资轮](#item-finance-news-1) ⭐️ 8.0/10
2. [高盛股票交易收入创纪录 第二季度激增 72%](#item-finance-news-2) ⭐️ 8.0/10
3. [DeepSeek 重启第二轮融资，投前估值约 5000 亿元](#item-finance-news-3) ⭐️ 8.0/10
4. [宇树科技科创板 IPO 启动询价](#item-finance-news-4) ⭐️ 8.0/10
5. [城堡投资买入崩盘 AI 对冲基金资产，旗下基金 7 月回报创多年新高](#item-finance-news-5) ⭐️ 7.0/10
6. [费城联储主席保尔森对当前利率水平满意，但对政策调整持开放态度](#item-finance-news-6) ⭐️ 7.0/10
7. [贝索斯提交出售 41 亿美元亚马逊股票计划，股价下跌逾 2%](#item-finance-news-7) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [展示 HN：简单算法与色彩空间生成多样化肤色](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 8.0/10

作者在 Show HN 上展示了一个自定义色彩空间和简单算法，用于生成多样化且逼真的肤色，主要面向数字艺术和游戏开发。该工作包含色彩选择器、程序化生成工具和交互式演示，通过主成分分析（PCA）拟合二维函数，将肤色数据映射到新月形色彩空间，便于采样自然肤色。页面详细解释了方法原理、空间特性及未来改进方向，为需要多样化肤色的艺术家和开发者提供了实用工具。

hackernews · automatoney · 8月4日 15:16 · [社区讨论](https://news.ycombinator.com/item?id=49170165)

**「相关背景」** 皮肤色调的建模因光照、感知等复杂因素而极具挑战，现有工业参考如潘通肤色指南（Pantone SkinTone Guide）提供了 110 种标准色样\[cite:tool-1-2\]，而 Oklab 等感知均匀色彩空间则旨在改善色彩计算的视觉一致性\[cite:tool-2-1\]。该作品在此基础上提出了一种专用的色彩空间与算法，使生成多样的肤色变得简单。

**「影响」** 该工具为数字艺术家和游戏开发者提供了一种系统化生成多样化肤色的实用方法，有望减少手动配色偏见和提升效率，但作者承认底层方法仍有待完善。

**「社区讨论」** 社区普遍赞赏该工作的美观性、PCA 后函数拟合的巧妙设计以及肤色呈新月形分布。部分评论指出极端饱和时会出现绿、蓝、紫等异常色调，并提及了与 Pantone Skin Tones、Oklab 色彩空间等现有工作的对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pantone.com/articles/product-spotlight/skintone-guide-revealing-the-new-pantone-skintone-guide">Skintone Guide: Revealing the new PANTONE SkinTone™ Guide</a></li>
<li><a href="https://en.wikipedia.org/wiki/Oklab_color_space">Oklab color space - Wikipedia</a></li>

</ul>
</details>

**标签**: `#color-spaces`, `#skin-tones`, `#procedural-generation`, `#graphics`, `#game-dev`

---

<a id="item-tech-news-2"></a>
### [生成式 AI 与软件工程的八大迷思](https://queue.acm.org/detail.cfm?id=3807963) ⭐️ 8.0/10

这篇 ACM Queue 文章批判性地审视了生成式 AI 对软件工程影响的八大常见误解，并利用研究证据为开发者和研究人员提供基于事实的见解。文章驳斥了诸如 AI 智能体即将取代人类开发者、编程时间被过度高估以及 AI 工具能普遍提升生产力等迷思，指出开发者实际编写代码的时间仅占一小部分，且 AI 的引入可能带来意想不到的社会与心理影响，如对特定群体的“能力惩罚”。文章综合产业与学术研究，挑战了过于乐观或悲观的预期，强调 AI 工具虽能辅助，但无法替代软件工程中所需的深度思考与问题解决能力。

hackernews · tchalla · 8月4日 23:50 · [社区讨论](https://news.ycombinator.com/item?id=49176830)

**「背景」** 生成式 AI（GenAI）工具（如大型语言模型）正被广泛应用于软件开发，引发了关于开发者生产力、代码生成能力等大量乐观断言。但多项研究（包括微软等机构的调查）表明，开发者实际编写代码的时间仅占其工作量的约 14%，且自动化代码生成并不能直接等同于整体效率提升或创新加速。

**「影响」** 该分析促使开发者和工程领导者以更清晰的理解接纳生成式 AI 工具，避免对不切实际的全自主系统过度投资，并更加重视设计、调试和系统思维等人类核心技能。

**「社区讨论」** 社区讨论普遍认同“AI 即将取代研究者”一说不切实际，部分开发者指出 AI 工具将工作重心从编码转移到了指挥智能体，导致整体认知负荷未减，也有人报告了对代码库失去联系和兴趣丧失的副作用。此外，评论区对文章引用的 2025 年 METR 研究时效性及一项中国主导的“能力惩罚”研究的方法论提出质疑，反映出对证据质量的审慎态度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://explainx.ai/blog/eight-myths-software-engineering-genai-acm-queue-august-2026">8 GenAI Coding Myths Debunked ( ACM Queue 2026) | explainx.ai</a></li>

</ul>
</details>

**标签**: `#software engineering`, `#generative AI`, `#myths`, `#LLM`, `#developer productivity`

---

<a id="item-tech-news-3"></a>
### [LLM 0.32 发布：新增推理轨迹、服务端工具与智能日志支持](https://simonwillison.net/2026/Aug/4/new-release-of-llm/#atom-everything) ⭐️ 8.0/10

LLM 0.32 发布，这是项目自首次发布以来最重要的版本更新。新版本为推理模型增加了可见的推理轨迹（默认输出到标准错误，可通过 -R 隐藏），并支持从命令行调用服务端工具，如 OpenAI 的 CodeInterpreter 和 WebSearch，以及 Anthropic 的 WebSearch、WebFetch、CodeExecution 和 AnthropicMCP。默认模型升级为 GPT-5.6 Luna，同时新增 llm openai endpoint 命令可针对任意 OpenAI 兼容端点运行一次性提示。Python API 也得到改进，现在支持传入 messages 列表和 stream\_events\(\) 方法，以便处理混合了推理文本、工具调用和附件的响应。

rss · Simon Willison · 8月4日 23:58

**「背景」** LLM 是由 Simon Willison 开发的开源命令行工具，允许用户通过插件与多种大型语言模型提供商交互，并将对话记录在 SQLite 数据库中。它已成为开发者尝试和集成 AI 模型的常用工具，0.32 版本带来了多项面向高级工作流的功能。

**「影响」** 对于开发者而言，推理轨迹显示和服务端工具集成大幅简化了模型调试，并可直接在命令行中实现复杂的代理式工作流。

**标签**: `#LLM`, `#CLI`, `#open-source`, `#AI-tools`, `#OpenAI-API`

---

<a id="item-tech-news-4"></a>
### [llm-anthropic 0.26 发布：支持 Claude 5 模型与服务器端工具](https://simonwillison.net/2026/Aug/4/llm-anthropic/#atom-everything) ⭐️ 8.0/10

llm-anthropic 0.26 插件发布，升级至 LLM 0.32 及以上版本，新增对 Claude 5 系列模型的支持，包括 claude-fable-5、claude-sonnet-5 和 claude-opus-5。同时引入服务器端工具 WebSearch、WebFetch、CodeExecution 和 AnthropicMCP，可通过 LLM 的 -T 接口调用，旧有的 -o web\_search 选项已被移除。推理过程、工具调用及结果现在以类型化事件流式传输，CLI 中推理内容输出到标准错误，可通过 --hide-reasoning / -R 隐藏。扩展思考机制简化为 thinking 和 thinking\_effort（低、中、高、xhigh、max）参数，Claude 5 模型默认开启思考，Sonnet 5 和 Opus 5 可通过 -o thinking 0 禁用，Fable 5 始终思考，同时移除了 thinking\_budget 等旧参数。

rss · Simon Willison · 8月4日 22:00

**「背景」** LLM 是一个用于与大型语言模型交互的命令行工具，而 llm-anthropic 是提供 Anthropic Claude 模型访问的插件。本次更新适配 LLM 0.32 引入的工具和流式事件架构，并整合了 Anthropic 最新发布的 Claude 5 模型能力。

**「影响」** 开发者可立即通过命令行使用 Claude 5 模型及其服务器端工具，享受更灵活的推理控制与流式输出体验。

**标签**: `#llm`, `#anthropic`, `#claude-5`, `#cli-tools`, `#ai`

---

<a id="item-tech-news-5"></a>
### [白宫开源 AI 监管急转弯，硅谷分裂](https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html) ⭐️ 8.0/10

特朗普政府内部就限制中国开源 AI 模型出现剧烈摇摆，白宫幕僚长和财长等人一度考虑动用制裁、贸易黑名单甚至禁止美企与中国公司合作，但在硅谷强烈反对后转向聚焦提升美国 AI 竞争力，并于 8 月 4 日邀请科技公司商议新框架，拟在模型发布前引入网络安全审查。导火索是中国开源模型 Kimi 部分性能比肩 OpenAI 顶级模型，OpenAI 与 Anthropic 以国家安全为由推动限制，而 Nvidia、Meta 等则力挺开放生态，黄仁勋首次在 X 为开源辩护并组建逾 230 家成员的安全联盟。这一政策急转弯反映了美国在遏制中国 AI 与保持自身开源创新之间的深层矛盾。

telegram · zaihuapd · 8月4日 15:22

**「背景」** 开源 AI 模型允许开发者自由获取、修改和部署，近年来中国开源模型快速追赶，其中 Kimi 在部分基准测试中接近美国顶级闭源模型，引发美国国家安全担忧。美国科技界内部长期存在分歧：一方认为开放会加速对手技术扩散，另一方视开源为美国创新生态的核心优势，限制将削弱自身竞争力。

**「影响」** 拟议的网络安全审查框架可能使美国开源 AI 模型的发布流程增加合规成本与不确定性，直接波及 Meta、Nvidia 等依赖开放生态的巨头，并可能加剧中美 AI 技术脱钩，但最终政策走向仍取决于白宫内部角力。

**标签**: `#artificial intelligence`, `#open source`, `#regulation`, `#geopolitics`, `#technology industry`

---

<a id="item-tech-news-6"></a>
### [ChainDrop 蠕虫攻陷逾 1300 个 npm 包](https://www.bleepingcomputer.com/news/security/massive-chaindrop-npm-supply-chain-attack-infects-hundreds-of-packages/) ⭐️ 8.0/10

自我传播的 ChainDrop 蠕虫已感染 npm 仓库中超过 1300 个包，合计月下载量达 20 亿次，包括 Keyv、Cacheable 等热门缓存工具。攻击者通过攻破 Keyv 维护者的 GitHub 账号，利用正常的 GitHub Actions 工作流发布了带有合法来源证明的恶意版本，进而波及 Deliveroo、Qlik、ServiceTitan 等机构相关的包。安装后，包内的 setup.mjs 和 Math\_Symbol.js 脚本会自动执行，窃取 GitHub、npm、AWS、Kubernetes 等凭证，并感染其他维护者的包。安全公司建议将受影响系统视为已完全失陷，需重建环境、轮换所有令牌并检查日志，npm-cache\[.\]com 域名可作为失陷指标。攻击仍在持续扩散，受影响包数量预计进一步增加。

telegram · zaihuapd · 8月5日 03:04

**「背景」** npm 是 Node.js 的默认包管理器，拥有全球最大的开源软件注册表，依赖关系复杂，使其成为供应链攻击的高价值目标。蠕虫型供应链攻击不仅能通过受信任的包分发恶意代码，还能自动搜索并感染其他维护者的包，从而在开发者生态中快速传播。

**「影响」** 任何安装过受影响包版本的开发环境都可能已泄露 GitHub、npm、AWS 和 Kubernetes 凭证，必须立即视为已被攻破，并彻底重建系统、轮换所有密钥与令牌。

**标签**: `#supply-chain-attack`, `#npm`, `#malware`, `#security`, `#credentials-theft`

---

<a id="item-tech-news-7"></a>
### [豆包上线原生音视频全双工模型](https://seed.bytedance.com/zh/blog/seedrealtime-%E9%9F%B3%E8%A7%86%E9%A2%91%E5%85%A8%E5%8F%8C%E5%B7%A5%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%8F%91%E5%B8%83-%E8%B5%B0%E5%90%91%E5%85%A8%E6%A8%A1%E6%80%81%E8%87%AA%E7%84%B6%E4%BA%A4%E4%BA%92) ⭐️ 8.0/10

字节跳动于 8 月 5 日发布原生音视频全双工大模型 SeedRealtime，采用统一架构将音频、视频与文本的感知、理解、决策与表达融为同一端到端模型，无需外置语音活动检测（VAD）即可实现“边看、边听、边说”的全双工交互。相比传统级联系统依赖 ASR、VLM、TTS 多模块串联，该模型在端到端人工评测中使音视频对话节奏问题减少一半，显著降低了“话未说完被抢断”等卡壳现象。SeedRealtime 已全量部署于豆包 App，标志着实时多模态对话从模块拼接转向原生一体化处理。

telegram · zaihuapd · 8月5日 04:42

**「背景」** 传统的实时语音对话系统通常采用级联架构，将自动语音识别（ASR）、视觉语言模型（VLM）和语音合成（TTS）等多个模块串联，并依赖语音活动检测（VAD）来管理说话轮次，这容易引入延迟和信息损失。全双工模型则在一个端到端统一模型中同步进行感知、理解、决策与表达，支持“边看、边听、边说”的自然交互，SeedRealtime 正是基于这一思路设计的原生音视频全双工大模型。

**「影响」** 豆包 App 用户将直接受益于更流畅的实时音视频对话，对话中断或抢话现象减少约 50%。

**标签**: `#multimodal AI`, `#real-time interaction`, `#conversational AI`, `#full-duplex models`, `#audio-visual processing`

---

<a id="item-tech-news-8"></a>
### [FFmpeg 9.0 发布，新增动画 WebP 支持](https://news.ycombinator.com/item?id=49166202) ⭐️ 8.0/10

FFmpeg 9.0 正式发布，新增动画 WebP 解码器与分离器、v360\_vulkan 滤镜、Playdate 视频编码器与封装器、HE-AAC 960 解码（DAB+）、transpose\_cuda 滤镜、AMF 帧率转换器滤镜以及 ONNX Runtime DNN 后端等多项特性。作为广泛使用的基础多媒体工具，该版本扩展了编解码器和滤镜能力，对依赖 FFmpeg 的软件与 AI 系统具有重要意义。开发团队通过 Anthropic 的 Claude for Open Source 计划获得六个月免费 Claude Max，AI 主要用于协助查找缺失的向后移植，但社区成员对 AI 辅助开发的安全审查流程表达了关切。

telegram · zaihuapd · 8月5日 10:32

**「背景」** FFmpeg 是一个开源、跨平台的多媒体处理框架，支持几乎所有音视频格式的编解码、转码、滤镜和流化。版本 9.0 是其重大更新，引入了动画 WebP 解码、新的 Vulkan 和 CUDA 加速滤镜、以及 ONNX Runtime DNN 后端，并首次尝试利用 Claude AI 辅助代码向后移植。

**「影响」** FFmpeg 9.0 新增动画 WebP 解码、Vulkan/CUDA 硬件加速滤镜以及 ONNX Runtime DNN 后端，使开发者能够直接在多媒体管线中处理该类格式，并更高效地集成 AI 视频处理功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.phoronix.com/news/FFmpeg-9.0-Released">FFmpeg 9 . 0 Released With More Vulkan Acceleration, Animated ...</a></li>
<li><a href="https://ubuntuhandbook.org/index.php/2026/08/ffmpeg-9-0-new-decoders-ubuntu-ppa/">FFmpeg 9 . 0 Released with New GPU Accelerated... | UbuntuHandbook</a></li>
<li><a href="https://www.phoronix.com/news/FFmpeg-9.0-Released">FFmpeg 9.0 Released With More Vulkan Acceleration, Animated WebP &amp; More AMD AMF - Phoronix</a></li>
<li><a href="https://www.heise.de/en/news/FFmpeg-9-0-WebP-in-GIF-out-11398216.html">FFmpeg 9.0: WebP in, GIF out | heise online</a></li>

</ul>
</details>

**标签**: `#ffmpeg`, `#multimedia`, `#release`, `#open-source`, `#ai-assisted-development`

---

<a id="item-tech-news-9"></a>
### [MiniMax-H3 模型移植至 MLX，可在 Apple Silicon 本地运行](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 7.0/10

PipeNetwork 发布了 minimax-h3-mlx 包，将 MiniMax 两天前推出的全模态生成模型 MiniMax-H3 移植到 MLX，使 Apple Silicon 设备能够本地运行。该模型支持文本、图像、音频和视频输入，可生成最长 15 秒的带音频视频片段。Simon Willison 在 M5 Max MacBook Pro 上实测，下载约 115 GB 模型文件后，用 45 分钟生成了一段视频，但因未提供音频提示，生成的语音为无意义噪音。官方提供了详细的视频提示编写指南以改善生成效果。

rss · Simon Willison · 8月4日 19:10

**「背景」** MLX 是 Apple 推出的机器学习框架，专为 Apple Silicon 优化，便于在 Mac 上高效运行模型。MiniMax-H3 是 MiniMax 刚发布的通用全模态生成系统，能够跨多种模态理解和生成内容，其视频生成功能尤其引人关注。

**「影响」** 此举让拥有 Apple Silicon 设备的开发者首次能在本地运行 MiniMax-H3 进行视频生成实验，但模型体积庞大（115 GB）且生成耗时较长（45 分钟），实际应用仍需权衡硬件资源与速度。

**标签**: `#MLX`, `#multimodal`, `#video-generation`, `#MiniMax-H3`, `#Apple-Silicon`

---

<a id="item-tech-news-10"></a>
### [SpaceX 将独家采用英伟达 Vera Rubin AI 架构](https://wccftech.com/elon-musk-commits-spacex-exclusively-to-nvidia-gpus-citing-theyre-the-best/) ⭐️ 7.0/10

马斯克在 SpaceX 首次财报电话会上宣布，公司 AI 服务将独家基于英伟达系统，并称 Vera Rubin 架构为“最佳 AI 计算架构”。SpaceX 计划在全球地面数据中心和太空端部署英伟达 Vera Rubin NVL72 机架系统，预计今年底 AI 计算能力超过 2 吉瓦，2027 年底前接近 10 吉瓦。该架构还将用于“Starmind”卫星项目，明年开始发射卫星以构建轨道 AI 数据中心，英伟达已提供太空级 Space-1 Vera Rubin 模块支持在轨高性能推理。

telegram · zaihuapd · 8月5日 02:04

**「背景信息」** 英伟达 Vera Rubin 架构是继 Blackwell 之后的新一代 AI 计算平台，预计 2026 年推出，整合了 Rubin GPU 与 Vera CPU。SpaceX 的 Starmind 项目旨在通过低轨卫星部署轨道 AI 数据中心，每颗卫星将搭载该架构的机架系统，以实现太空中的高性能计算。

**「影响」** 此独家合作将推动 SpaceX 在轨 AI 计算能力大幅跃升，并可能加速轨道数据中心与卫星 AI 推理的部署进程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.blocktempo.com/spacex-exclusive-nvidia-ai-architecture-vera-rubin-space-data-center-starmind-2026/">SpaceX 独家锁定辉达 AI 架构，太空资料中心 Starmind 计划明年启动 | 动区动趋-最具影响力的区块链新闻媒体</a></li>
<li><a href="https://www.ndtvprofit.com/markets/the-best-ai-computer-spacex-picks-nvidia-as-exclusive-ai-compute-partner-amd-shares-fall-8-starmind-plans-11867119">&#x27;The Best AI Computer&#x27;: SpaceX Picks Nvidia As Exclusive AI Compute Partner; AMD Shares Fall 8%; Starmind Plans</a></li>
<li><a href="https://x.com/SpaceX/status/2084723854534951218">SpaceX is partnering with @Nvidia to design the Starmind AI1 ...</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#NVIDIA`, `#AI infrastructure`, `#Vera Rubin`, `#satellite computing`

---

<a id="item-tech-news-11"></a>
### [三星与 SK 海力士据报测试中微刻蚀设备对冲美管制](https://www.reuters.com/world/china/samsung-sk-hynix-test-chinese-chip-tools-hedge-against-us-risks-2026-08-05/) ⭐️ 7.0/10

路透社援引知情人士称，三星电子与 SK 海力士正在评估中国半导体设备商中微公司（AMEC）的刻蚀设备，考虑用于在华工厂，以对冲美国出口管制收紧的风险。两家公司约两年前已开始测试，但尚未决定是否大规模部署，三星声明否认相关测试，SK 海力士拒绝置评。美国 2025 年撤销了这两家韩企中国工厂的“经验证最终用户”待遇，改为年度许可，引发对现有西方设备维护可能受限的担忧。分析指出，中国设备价格通常低 20%至 30%，若获国际大厂认可将提供强力背书，德意志银行预计今年中国本土设备商或占据中国约 280 亿美元晶圆制造设备市场的 25%至 30%。

telegram · zaihuapd · 8月5日 04:32

**「背景」** 美国为限制中国半导体技术发展，对向中国出口先进芯片制造设备实施出口管制，并对在华工厂的境外企业实施许可审查。三星和 SK 海力士在华工厂之前享有“经验证最终用户”（VEU）待遇，可简化获得美国设备，但 2025 年被撤销，改为年度许可，增加了供应链不确定性。中微公司是中国领先的半导体刻蚀设备制造商，其设备被视为潜在替代方案。

**「影响」** 若三星和 SK 海力士最终采用中微设备，将为中国刻蚀设备获得国际认可提供关键背书，并可能削弱美国出口管制对韩企在华生产的约束力，同时压低设备采购成本。

**标签**: `#semiconductors`, `#export controls`, `#supply chain`, `#chip manufacturing`, `#geopolitics`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [Polymarket 正洽谈估值超 200 亿美元融资轮](https://www.cnbc.com/2026/08/04/polymarket-seeks-fundraising-round-at-more-than-20-billion-valuation.html) ⭐️ 8.0/10

据知情人士向 CNBC 透露，预测市场平台 Polymarket 正在洽谈一轮融资，其估值将超过 200 亿美元。

rss · CNBC Finance · 8月4日 13:31

**「背景」** 此前，该公司在 4 月刚刚完成了一轮估值 150 亿美元的融资，并于 5 月推出了受监管的美国交易所，其年化收入已超过 10 亿美元。

**标签**: `#Prediction markets`, `#Fundraising`, `#Valuation`, `#Polymarket`, `#Fintech`

---

<a id="item-finance-news-2"></a>
### [高盛股票交易收入创纪录 第二季度激增 72%](https://www.cnbc.com/2026/08/01/goldman-traders-are-on-pace-for-a-record-year-a-close-up-look-at-how-theyre-doing-it.html) ⭐️ 8.0/10

高盛第二季度股票交易收入同比飙升 72%，达到创纪录的 74.2 亿美元，成为该银行增长的最大驱动力。

rss · CNBC Finance · 8月4日 19:38

**「背景」** 高盛近年来通过整合投资银行、财富管理与股票交易业务，推动客户交叉使用服务，以提升整体业绩。

**标签**: `#Goldman Sachs`, `#equities trading`, `#earnings`, `#investment banking`, `#financial sector`

---

<a id="item-finance-news-3"></a>
### [DeepSeek 重启第二轮融资，投前估值约 5000 亿元](https://finance.sina.com.cn/wm/2026-08-05/doc-inimfmyv1554159.shtml) ⭐️ 8.0/10

据多名交易人士透露，DeepSeek 已重启第二轮融资，计划募资 500 亿元，投前估值约 5000 亿元，较首轮估值提升约 43%。

telegram · zaihuapd · 8月5日 02:46

**「背景」** DeepSeek 于今年 4 月开启首轮融资，6 月完成交割，金额 500 亿元、估值超 3500 亿元。本次重启的第二轮融资投前估值较首轮提升约 43%。

**标签**: `#DeepSeek`, `#AI funding`, `#valuation`, `#China tech`, `#private equity`

---

<a id="item-finance-news-4"></a>
### [宇树科技科创板 IPO 启动询价](https://m.jrj.com.cn/madapter/stock/2026/08/05141758022724.shtml) ⭐️ 8.0/10

宇树科技科创板 IPO 启动询价，拟募资 42 亿元，对应市值超 400 亿元，2025 年营收 16.99 亿元，净利润 2.78 亿元。

telegram · zaihuapd · 8月5日 07:40

**标签**: `#IPO`, `#科创板`, `#机器人`, `#企业融资`, `#财务数据`

---

<a id="item-finance-news-5"></a>
### [城堡投资买入崩盘 AI 对冲基金资产，旗下基金 7 月回报创多年新高](https://www.cnbc.com/2026/08/05/ken-griffins-citadel-posts-best-month-in-years-after-scooping-up-situational-awareness-stocks.html) ⭐️ 7.0/10

城堡投资旗舰惠灵顿基金 7 月回报 5.9%，创 2022 年以来最佳单月表现，这得益于其买入因 AI 交易逆转而崩盘的对冲基金 Situational Awareness 的折价资产。

rss · CNBC Finance · 8月5日 11:13

**「背景」** 前 OpenAI 研究员创立的 AI 对冲基金 Situational Awareness 因 AI 硬件股暴跌和软件股反弹而被迫平仓，城堡投资成为其折价资产的最大买家。

**「影响」** 此次强制平仓和城堡投资的接盘被交易员视为清算事件，促使空头获利了结，推动 Nebius 和美光等 AI 相关股票在月底反弹。

**标签**: `#hedge funds`, `#AI stocks`, `#forced liquidation`, `#Citadel`, `#market dislocation`

---

<a id="item-finance-news-6"></a>
### [费城联储主席保尔森对当前利率水平满意，但对政策调整持开放态度](https://www.cnbc.com/2026/08/04/philadelphia-fed-president-paulson-content-with-current-rates-but-keeping-an-open-mind.html) ⭐️ 7.0/10

费城联储主席保尔森表示，当前 3.5%-3.75%的联邦基金利率目标区间足以让通胀向 2%目标回落。但她补充，若其估算的剔除能源与关税等因素后的核心通胀（约 2.4%-2.8%）未能进一步下降，她将对调整利率持开放态度。

rss · CNBC Finance · 8月4日 17:49

**「背景」** 上周，美联储公开市场委员会以 9 票赞成、3 票反对决定维持利率不变，保尔森作为投票委员支持该决定；当前通胀仍高于 2%的目标。

**标签**: `#monetary policy`, `#federal reserve`, `#interest rates`, `#inflation`, `#FOMC`

---

<a id="item-finance-news-7"></a>
### [贝索斯提交出售 41 亿美元亚马逊股票计划，股价下跌逾 2%](https://www.cnbc.com/2026/08/04/jeff-bezos-just-filed-to-sell-4-billion-in-amazon-the-shares-are-falling.html) ⭐️ 7.0/10

杰夫·贝索斯提交了出售约 1500 万股亚马逊股票（价值约 41 亿美元）的计划。此前亚马逊股价因强劲业绩创下历史新高，消息披露后股价下跌逾 2%。

rss · CNBC Finance · 8月4日 16:14

**「背景」** 亚马逊股价此前因云计算业务强劲增长发布超预期财报而创下历史新高；此次出售依据一项预先安排的交易计划（10b5-1 计划）进行，该计划于 2025 年 11 月 14 日设立。

**标签**: `#insider-transactions`, `#Amazon`, `#Jeff-Bezos`, `#stock-market`, `#SEC-filing`

---