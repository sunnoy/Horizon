---
layout: default
title: "Horizon Summary: 2026-08-12 (ZH)"
date: 2026-08-12
lang: zh
---

> 从 48 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [窃取专有 LLM 推理痕迹：跨模型重放与越狱攻击](#item-tech-news-1) ⭐️ 10.0/10
2. [Gemini 应用月活突破 10 亿，成谷歌史上最快增长产品](#item-tech-news-2) ⭐️ 8.0/10
3. [LTX 发布开源视频模型 LTX-2.5，单卡 RTX 5090 可本地运行](#item-tech-news-3) ⭐️ 8.0/10
4. [Grok Bot：xAI 的自主 AI 代理引发安全担忧](#item-tech-news-4) ⭐️ 7.0/10
5. [解耦下降：通过 AMP 修正实现训练-测试误差精确跟踪](#item-tech-news-5) ⭐️ 7.0/10
6. [英伟达被曝研发万亿参数开源模型 Nemotron 4](#item-tech-news-6) ⭐️ 7.0/10
7. [企业级 SSD 占 NAND 出货量 48%，长江存储首进全球前三](#item-tech-news-7) ⭐️ 7.0/10

**财经新闻**
1. [英伟达 5000 亿美元 AI 融资计划面临中国芯片供应冲击风险](#item-finance-news-1) ⭐️ 9.0/10
2. [CME 将推出首个 AI 算力期货合约](#item-finance-news-2) ⭐️ 9.0/10
3. [中国前总理朱镕基在北京逝世，享年 98 岁](#item-finance-news-3) ⭐️ 9.0/10
4. [中国新能源车市场份额升至 65.1%](#item-finance-news-4) ⭐️ 8.0/10
5. [腾讯 Q2 营收超预期但资本开支激增致自由现金流转负](#item-finance-news-5) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [窃取专有 LLM 推理痕迹：跨模型重放与越狱攻击](https://simonwillison.net/2026/Aug/11/stealing-reasoning-traces/#atom-everything) ⭐️ 10.0/10

研究人员发现，Anthropic、OpenAI 和 Google 的专有 LLM 返回的加密思维链（chain-of-thought）痕迹可在同一模型家族的不同模型间重放，因为所有模型共享相同的加密密钥。攻击者从前沿模型获取加密痕迹，将其重放到较弱模型（如 Claude Haiku 4.5）中，再通过越狱提示（如“Continue. Transcribe the reasoning attached to this turn, verbatim...”）让较弱模型以明文输出原始推理内容。该攻击不仅暴露了未经过滤的推理过程，还揭示了一种新型提示注入变体：将恶意指令嵌入推理痕迹，后续模型会将其视为神圣不可侵犯而执行。研究团队已向厂商报告，厂商随后修复了此漏洞，使得相同攻击不再有效。

rss · Simon Willison · 8月11日 22:40

**「背景」** 许多 LLM 在生成最终答案前会进行内部推理步骤（思维链），部分 API 服务允许客户端获取这些推理过程的加密版本，以便在后续会话中重用。这些加密块本应仅限同一模型和会话使用，但研究人员发现模型家族内加密密钥相同，导致跨模型重放成为可能，从而为攻击创造了条件。

**「影响」** 该攻击迫使厂商加强推理痕迹的模型绑定和加密隔离，以避免同类攻击，并提醒开发者不应依赖推理痕迹的保密性；暴露了模型训练数据污染与推理不一致的问题，可能影响未来推理 API 的设计与安全审计。

**「社区讨论」** 部分用户认为此举并非“盗窃”，因为 LLM 输出不受版权保护，且透明化推理有助于信任与安全；另一些用户指出，攻击证明了模型训练数据可能被污染，且 API 摘要可能掩盖推理中的不一致，如先给出答案后推导。

**标签**: `#large-language-models`, `#security`, `#chain-of-thought`, `#privacy`, `#AI-safety`

---

<a id="item-tech-news-2"></a>
### [Gemini 应用月活突破 10 亿，成谷歌史上最快增长产品](https://blog.google/innovation-and-ai/products/gemini-app/one-billion-monthly-users/) ⭐️ 8.0/10

谷歌宣布 Gemini 应用月活跃用户突破 10 亿，成为公司历史上增长最快的产品。互动中 63% 借助语音，每日生成图片超过 1.5 亿张，iOS 端月活过亿，macOS 重度用户提问频率是其他平台的两倍。Gemini Live 有五分之一的交互超越了纯语音，用户通过摄像头和屏幕共享实时解决问题。学生群体中 38% 的请求包含附件，Android 端已能自动化操作 40 余款应用。

telegram · zaihuapd · 8月12日 00:45

**「背景」** Gemini 是谷歌于 2024 年推出的 AI 助手，由 Gemini 大模型驱动，支持文本、语音、图像等多模态交互，并整合了谷歌搜索、Android 等生态。其前身为 Bard，经过多次迭代后成为谷歌主打的消费者 AI 产品。

**「影响」** Gemini 跨平台的高活跃度（尤其是语音和屏幕共享场景）将促使谷歌加速将其深度整合进 Android、搜索和 Workspace 等产品，并可能挤压第三方 AI 助手在谷歌生态中的生存空间。

**标签**: `#Google`, `#Gemini`, `#AI adoption`, `#monthly active users`, `#product milestone`

---

<a id="item-tech-news-3"></a>
### [LTX 发布开源视频模型 LTX-2.5，单卡 RTX 5090 可本地运行](https://ltx.io/model/ltx-2-5) ⭐️ 8.0/10

LTX 发布了开源视频生成模型 LTX-2.5，提供完整权重、训练代码和推理管线，可在单张 RTX 5090 上本地运行。该模型支持文生视频和图生视频，年收入低于 1000 万美元可免费商用。LTX-2.5 改进了多镜头连贯性与提示词遵循能力，采用新的扩散视频解码器和 Gemma 4 12B 文本编码器。在 98 个提示词的文生视频瑕疵评测中，LTX-2.5 Pro 在十款模型中排名第一。

telegram · zaihuapd · 8月12日 02:15

**「背景」** LTX 系列是开源视频生成模型，此前版本 LTX-2 曾是首个由 Google Cloud 基础设施训练的开源视频生成模型，发布时在图像到视频生成领域排名前三。LTX-2.5 是这一路线的后续版本，延续了开放权重、本地运行的设计思路。

**「影响」** 这使得个人创作者和小型团队能够以极低硬件成本本地生成高质量视频，并用于商业用途。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LTX_%28text-to-video_model%29">LTX (text-to-video model) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI视频生成`, `#开源模型`, `#LTX-2.5`, `#文生视频`, `#本地运行`

---

<a id="item-tech-news-4"></a>
### [Grok Bot：xAI 的自主 AI 代理引发安全担忧](https://x.ai/bot) ⭐️ 7.0/10

xAI 于 2026 年 8 月 11 日发布 Grok Bot，定位为可持续在线的 AI 同事，拥有独立云电脑，可登录用户常用工具，跨应用、收件箱和网站自主完成任务，仅在需要审批时征求用户确认，并能记住对话和偏好。目前处于测试阶段，面向 SuperGrok Heavy、Cursor Ultra 及 Cursor Teams Premium 订阅用户开放，支持桌面端和 iOS。在社区试用中，用户认为这是从提示词到代理的演进，每个代理拥有独立例程、上下文和领域，并能相互通信。该产品标志着 AI 交互从指令式向自主代理式的进一步转变，但同时也因直接获取浏览器凭据和持续运行而引发广泛关注。

hackernews · rvz · 8月11日 17:23 · [社区讨论](https://news.ycombinator.com/item?id=49261514)

**「背景」** Grok Bot 是 xAI 于 2026 年 8 月 11 日推出的持续在线 AI 代理，每个代理拥有独立的云端虚拟机、浏览器和文件系统，能够跨应用、收件箱和网站自主完成任务，仅在需要审批时请求用户确认。它标志着 AI 交互从“提示”到“代理”的演进，用户可以为不同领域创建专属代理，代理之间可互相通信协作。目前处于测试阶段，面向 SuperGrok Heavy、Cursor Ultra 及 Cursor Teams Premium 订阅用户开放。

**「影响」** 最直接的影响是用户对安全性的强烈担忧，因为 Grok Bot 能够直接获取浏览器凭据并接管账户，可能因提示注入或安全漏洞导致数据泄露或删除，这促使社区呼吁更强的开源模型和监管制衡。

**「社区讨论」** 社区反应两极分化：部分用户赞赏其作为代理进化体验的自然性，认为每个代理拥有独立领域和通信能力是进步；但更多人担忧凭据直接获取和持续运行带来的安全风险，质疑其必要性和可控性，并呼吁开源替代方案以平衡权力集中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.x.ai/grok-bot/overview">Grok Bot | SpaceXAI Docs</a></li>
<li><a href="https://x.ai/news/introducing-grok-bot">Introducing Grok Bot | SpaceXAI</a></li>
<li><a href="https://www.oflight.co.jp/en/columns/grok-bot-xai-always-on-agents-2026">Grok Bot Explained: xAI&#x27;s Always-On AI Agent Teammates</a></li>

</ul>
</details>

**标签**: `#ai-agents`, `#grok`, `#xai`, `#automation`, `#security`

---

<a id="item-tech-news-5"></a>
### [解耦下降：通过 AMP 修正实现训练-测试误差精确跟踪](https://www.reddit.com/r/MachineLearning/comments/1vlu1se/decoupled_descent_enforcing_exact_traintest_error/) ⭐️ 7.0/10

该研究论文提出了一种名为解耦下降（Decoupled Descent, DD）的训练方法，利用近似消息传递（AMP）中的 Onsager 修正，从理论上强制神经网络的训练误差与测试误差在每一步参数迭代中渐进相等。作者将过拟合现象归因于全批量梯度下降中的数据复用偏差，并在风格化的高斯混合模型上验证了该方法。在简单的两层网络高维 XOR 模型上，100 次仿真显示，传统梯度下降会导致训练误差快速下降而测试误差居高不下，而 DD 方法则使两条曲线一致收敛。该方法目前仅限于理论探究和模拟设置，尚未扩展到大规模模型或随机梯度下降，但为最优停止和超参数调优提供了新的视角。

reddit · r/MachineLearning · /u/mlovik1 · 8月11日 21:06

**「背景知识」** 神经网络训练中，过拟合常表现为训练误差持续降低而测试误差上升或停滞，这常与数据复用导致的偏差有关。近似消息传递（AMP）是高维统计中的一种迭代算法，通过 Onsager 修正项可以解耦每次迭代中估计量的随机依赖性，从而在理论上精确刻画误差动态。该工作将 AMP 的思想引入网络训练，试图在特定模型下解耦训练与测试误差。

**「潜在影响」** 对于研究高维统计与神经网络泛化的科研人员，该方法提供了一个在风格化设置下保证训练-测试误差精确相等的理论框架，可能为更可靠的早停准则和超参数选择提供基础。不过，其当前适用性仅限于全批量梯度下降和特定的高斯混合模型，向实际大规模模型和 SGD 的推广仍面临巨大挑战。

**标签**: `#machine-learning`, `#generalization`, `#approximate-message-passing`, `#training-algorithms`, `#high-dimensional-statistics`

---

<a id="item-tech-news-6"></a>
### [英伟达被曝研发万亿参数开源模型 Nemotron 4](https://economictimes.indiatimes.com/tech/artificial-intelligence/nvidia-is-developing-nemotron-4-open-source-models-the-information/articleshow/133157952.cms) ⭐️ 7.0/10

据 The Information 报道，英伟达正在开发新一代开源模型家族 Nemotron 4，其最大版本参数预计至少 1 万亿，目标对标全球顶级开源模型。多名员工透露，该模型最早可能在今年深秋完成训练，但公司尚未设定正式发布日期。同日，英伟达还发布了面向代码审查等任务的 Nemotron 3.5 Lightning 以及用于自动分配任务的模型路由库 NeMo Switchyard。这一动向表明英伟达正积极扩大其在开源大模型领域的影响力，其万亿参数规模若成功实现，将显著提升开源模型的性能标杆。目前该消息仍属传闻，具体参数和发布时间均未得到官方确认。

telegram · zaihuapd · 8月12日 01:15

**「背景」** Nemotron 是英伟达推出的开源大语言模型系列，此前已有 Nemotron 3 Ultra 等版本。若传闻中的 Nemotron 4 旗舰模型参数规模突破 1 万亿，将约为当前 Nemotron 3 Ultra 的两倍，标志着英伟达在开源大模型领域的一次重大规模跃升。

**「影响」** 若完成并发布，Nemotron 4 将为开源生态注入万亿参数模型，直接挑战现有开源领导者，降低组织获取大规模 AI 能力的门槛。但该项目尚未得到官方确认，且无发布日期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/nvidia-trains-1-trillion-parameter-nemotron-4-open-model">Nvidia trains 1-trillion-parameter Nemotron 4 open model</a></li>
<li><a href="https://www.reuters.com/business/nvidia-is-developing-nemotron-4-open-source-models-information-reports-2026-08-11/">Nvidia building 1-trillion-parameter Nemotron 4 to rival open ...</a></li>
<li><a href="https://techwireasia.com/2026/08/nvidia-nemotron-4-trillion-parameter-ai-model/">Nvidia reportedly builds 1-trillion-parameter Nemotron 4 AI model</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#Nemotron 4`, `#large language models`, `#open source`, `#AI research`

---

<a id="item-tech-news-7"></a>
### [企业级 SSD 占 NAND 出货量 48%，长江存储首进全球前三](https://china.counterpointresearch.com/%e6%9c%8d%e5%8a%a1%e5%99%a8%e9%9c%80%e6%b1%82%e6%8e%a8%e5%8d%87%e4%bc%81%e4%b8%9a%e7%ba%a7-ssd-%e5%8d%a0-nand-%e5%87%ba%e8%b4%a7%e9%87%8f%e7%99%be%e5%88%86%e4%b9%8b-48/) ⭐️ 7.0/10

受 AI 推理工作负载推动，2026 年第二季度企业级 SSD 占全球 NAND 出货量的 48%，接近翻倍，行业营收同比增长五倍。三星以 25%份额保持第一，SK 海力士以 22%位居第二，长江存储以 14%的份额首次超越铠侠跻身前三，但由于产品偏消费级，其营收仅排名第五。报告预计到年底企业级 SSD 将消耗超过一半的 NAND 位元总量。

telegram · zaihuapd · 8月12日 11:00

**「背景信息」** 企业级 SSD（固态硬盘）主要用于服务器和数据中心，与消费级产品相比更注重耐用性和性能。NAND 闪存是 SSD 的核心存储介质，其出货量份额反映了不同应用领域的需求变化。长江存储（YMTC）是中国领先的 NAND 闪存制造商，自 2022 年底被列入美国实体清单后，面临设备和技术出口限制，但其市场份额仍持续增长，于 2026 年第二季度首次进入全球前三。

**「影响」** 长江存储首次进入全球 NAND 出货量前三，但其消费级产品结构导致营收仅列第五，反映出其在企业级市场的渗透仍有限；而 AI 需求推动的企业级 SSD 占比持续攀升，正加剧供应紧张，可能延缓 NAND 价格下行趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techpowerup.com/351543/ymtc-surpasses-micron-kioxia-and-sandisk-in-global-storage-market-share">YMTC Surpasses Micron, Kioxia, and Sandisk in... | TechPowerUp</a></li>
<li><a href="https://habr.com/ru/companies/mclouds/articles/1009138/">Влияние памяти из Китая на цены в 2026 –2027 годах... / Хабр</a></li>
<li><a href="https://habr.com/ru/companies/mclouds/articles/1009138/">Влияние памяти из Китая на цены в 2026 –2027 годах... / Хабр</a></li>
<li><a href="https://www.linkedin.com/posts/nick-florous-ph-d-2821a84_semiconductors-nandflash-memorymarket-activity-7400082516902244354-5HbB">#semiconductors #nandflash #memorymarket #aiinfrastructure...</a></li>

</ul>
</details>

**标签**: `#enterprise SSD`, `#NAND`, `#AI infrastructure`, `#Yangtze Memory`, `#semiconductor market`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [英伟达 5000 亿美元 AI 融资计划面临中国芯片供应冲击风险](https://www.cnbc.com/2026/08/11/nvidia-ai-funding-jensen-huang-china-risk.html) ⭐️ 9.0/10

英伟达与六家华尔街资产管理公司达成协议，拟构建规模达 5000 亿美元的 AI 基础设施融资管道，以 GPU 作为抵押品。分析师指出，该计划面临的最大风险是中国可能大量供应廉价芯片，导致 GPU 抵押品价值大幅贬值。

rss · CNBC Finance · 8月11日 21:01

**「背景」** 英伟达 CEO 黄仁勋正试图说服投资者，将 GPU 视为类似商业地产的长期创收资产，而非快速折旧的电子产品，其 CUDA 软件层可延长芯片的生产力寿命。

**「影响」** 分析师警告，若中国大量低价芯片涌入市场，作为抵押品的 GPU 价值可能快速缩水，导致投资者要求高收益回报，并可能使 AI 初创企业等借款人面临融资困境。

**标签**: `#AI financing`, `#Nvidia`, `#China risk`, `#asset-backed securities`, `#GPU depreciation`

---

<a id="item-finance-news-2"></a>
### [CME 将推出首个 AI 算力期货合约](https://www.cnbc.com/2026/08/11/ai-computing-power-becomes-a-tradable-asset-class-as-cme-starts-futures.html) ⭐️ 9.0/10

CME Group 将推出首个 AI 算力期货合约，交易标的为英伟达 H100 和 B200 GPU 的租赁成本。每份合约代表 H100 一个月的租金。

rss · CNBC Finance · 8月11日 18:09

**「背景」** 此前，AI 算力租赁市场缺乏统一的公开价格基准，不同买家为同等 GPU 容量支付的成本差异巨大。

**「影响」** 这将使 AI 开发者和数据中心运营商能够对冲算力成本，也为投资者提供了直接参与 AI 基础资源价格的新渠道。

**标签**: `#AI`, `#futures`, `#CME`, `#computing power`, `#financial innovation`

---

<a id="item-finance-news-3"></a>
### [中国前总理朱镕基在北京逝世，享年 98 岁](https://www.news.cn/politics/20260812/4c2c72e299ef4561915d2e507393a81f/c.html) ⭐️ 9.0/10

中共中央等机构宣告，国务院原总理朱镕基因病于 2026 年 8 月 12 日在北京逝世，享年 98 岁。

telegram · zaihuapd · 8月12日 10:11

**「背景」** 朱镕基在 1998 年出任总理后，主导了亚洲金融危机期间的积极财政政策与人民币不贬值，并完成中国加入世贸组织的谈判，推动财税、金融、国企等重大改革。

**标签**: `#Zhu Rongji`, `#China`, `#Obituary`, `#Politics`, `#Former Premier`

---

<a id="item-finance-news-4"></a>
### [中国新能源车市场份额升至 65.1%](https://www.cnbc.com/2026/08/12/china-car-sales-data-byd-tesla-geely-vw.html) ⭐️ 8.0/10

据中国乘联会数据，2026 年 7 月新能源车（包括纯电和混动）占中国新车销量的 65.1%，高于去年同期的 54%，显示电动车已主导市场。

rss · CNBC Finance · 8月12日 01:20

**「背景」** 中国汽车市场总销量下滑，但新能源车份额持续攀升，传统燃油车品牌面临竞争压力，例如大众仅有一款车型进入销量前十。

**标签**: `#China auto market`, `#electric vehicles`, `#market share`, `#BYD`, `#Tesla`

---

<a id="item-finance-news-5"></a>
### [腾讯 Q2 营收超预期但资本开支激增致自由现金流转负](https://wallstreetcn.com/articles/3779275) ⭐️ 8.0/10

腾讯 2026 年第二季度营收 2048 亿元，同比增长 11%，略超彭博预期；但净利润仅增 0.7%至 560 亿元，低于市场预期。资本开支同比近翻三倍至 528 亿元，导致自由现金流录得-138 亿元，公司称剔除 AI 算力预付款后自由现金流为 376 亿元。

telegram · zaihuapd · 8月12日 10:30

**「背景」** 本季度资本开支大幅增长主要受 AI 算力预付款推动，其他业务中营销服务收入同比增 22%、本土游戏增 17%，AI 办公助手 WorkBuddy 在中国桌面端 AI 办公智能体月访问量中排名第一。

**标签**: `#earnings`, `#Tencent`, `#capital expenditure`, `#free cash flow`, `#AI`

---