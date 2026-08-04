---
layout: default
title: "Horizon Summary: 2026-08-04 (ZH)"
date: 2026-08-04
lang: zh
---

> 从 49 条内容中筛选出 19 条重要资讯。

---

**科技新闻**
1. [Waymo 在达拉斯向公众开放无人驾驶出租车服务](#item-tech-news-1) ⭐️ 8.0/10
2. [在单块 AMD MI300X 上运行 DeepSeek V4 Flash](#item-tech-news-2) ⭐️ 8.0/10
3. [Keyv 及依赖包遭 Shai-Hulud 供应链攻击](#item-tech-news-3) ⭐️ 8.0/10
4. [MiniMax-H3 MLX 端口支持本地音视频生成](#item-tech-news-4) ⭐️ 8.0/10
5. [Cloudflare 用 AI 每月 58 美元处理漏洞赏金](#item-tech-news-5) ⭐️ 8.0/10
6. [首部 L3/L4 自动驾驶强制国标发布，2027 年 7 月实施](#item-tech-news-6) ⭐️ 8.0/10
7. [白宫对开源 AI 监管急转弯，硅谷内部分裂加剧](#item-tech-news-7) ⭐️ 8.0/10
8. [Mistral 发布 Shieldstral：3B 参数开源多模态审核模型](#item-tech-news-8) ⭐️ 7.0/10
9. [生成多样化肤色的算法与色彩空间](#item-tech-news-9) ⭐️ 7.0/10
10. [FedEx 等企业邮件形似钓鱼，训练用户忽视安全警告](#item-tech-news-10) ⭐️ 7.0/10
11. [苹果指控更多前员工向 OpenAI 泄露机密数据](#item-tech-news-11) ⭐️ 7.0/10
12. [Harness 工程：AI 自我改进的工程实践](#item-tech-news-12) ⭐️ 7.0/10
13. [白宫完成 AI 评估框架，细节不公开](#item-tech-news-13) ⭐️ 7.0/10
14. [iPhone 与 Win 剪贴板共享将随 iOS 28 登陆欧盟](#item-tech-news-14) ⭐️ 7.0/10
15. [华为首席科学家警告英伟达芯片将触及物理极限](#item-tech-news-15) ⭐️ 7.0/10
16. [美国拟起草禁令禁止进口中国光模块](#item-tech-news-16) ⭐️ 7.0/10

**财经新闻**
1. [谷歌为 Anthropic 搭建 2000 亿美元 AI 融资架构](#item-finance-news-1) ⭐️ 9.0/10
2. [Polymarket 洽谈估值逾 200 亿美元融资](#item-finance-news-2) ⭐️ 8.0/10
3. [国家邮政局对申通快递立案调查](#item-finance-news-3) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Waymo 在达拉斯向公众开放无人驾驶出租车服务](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 8.0/10

Waymo 已将其自动驾驶出租车服务向达拉斯公众全面开放，这是其在美国前五大都市圈之一的重要扩张。达拉斯-沃斯堡地区以低密度、高度依赖汽车且公共交通有限而闻名，因此该服务填补了当地出行选择的空白。社区评论认为，无人驾驶汽车可通过减少停车需求及相关成本，成为一种有效的可负担住房政策工具，同时其可预测的驾驶行为也有助于提升交通安全性。服务覆盖区域的具体细节可通过官方支持页面获取，但未提供精确的启动日期。

hackernews · xnx · 8月4日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=49172836)

**「背景」** Waymo 是 Alphabet 旗下的自动驾驶技术公司，前身为谷歌自动驾驶汽车项目，在美国多个城市提供机器人出租车服务。

**「影响」** 达拉斯居民和游客现在可以使用无安全驾驶员的自动驾驶出租车，这为高汽车依赖型城市提供了更安全、可预测的出行替代方案，并可能降低事故率。

**「社区讨论」** 评论者普遍认为无人驾驶出租车是有效的可负担住房政策，通过减少停车空间需求来降低住房成本；同时，根据在洛杉矶等地的实际体验，Waymo 车辆比人类司机更可预测且引发的事故更少，尽管偶尔会出现短暂卡顿，但已逐渐被当地居民接受。有人对这项技术得到的低调宣传感到意外。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.m.wikipedia.org/wiki/Waymo">Waymo - Wikipedia</a></li>

</ul>
</details>

**标签**: `#autonomous-vehicles`, `#robotaxi`, `#urban-mobility`, `#Waymo`, `#Dallas`

---

<a id="item-tech-news-2"></a>
### [在单块 AMD MI300X 上运行 DeepSeek V4 Flash](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 8.0/10

一份实用指南展示了如何在单块 AMD MI300X GPU 上运行 DeepSeek V4 Flash，完整保留了推理权重和模型质量。该配置实现了超过 150 token/秒的吞吐量，但上下文窗口从原生的 1M token 缩减至 256k。这一折衷方案仍具有实用性，因为 Codex 等模型也在此范围内。这凸显了高 HBM 内存 GPU 在自托管大型 MoE 模型方面的可行性，为 AI 基础设施工程师提供了及时见解。

hackernews · zhoutong · 8月4日 10:00 · [社区讨论](https://news.ycombinator.com/item?id=49166386)

**「背景」** DeepSeek 是一家专注于通用人工智能的中国公司（来源：tool-1-1），其推出的 DeepSeek V4 Flash 是一个混合专家（MoE）语言模型，推理时需要大量显存。AMD Instinct MI300X 是 AMD 的旗舰 AI 加速器，拥有 192 GB HBM3 内存，远高于常见 GPU，非常适合单卡部署此类大模型。

**「影响」** 对于 AI 基础设施工程师，此举证明了在单块高 HBM GPU 上自托管完整权重大型 MoE 模型的可行性，可能推动本地部署方案的普及。

**「社区讨论」** 社区评论普遍认可该指南的实用性，强调高 HBM 内存对运行 MoE 模型的关键作用，但指出 MI300X 作为 OAM 模块难以单买，并建议考虑 MI350P 或 DwarfStar 等替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AMD MI300X`, `#DeepSeek V4`, `#LLM inference`, `#MoE`, `#GPU`

---

<a id="item-tech-news-3"></a>
### [Keyv 及依赖包遭 Shai-Hulud 供应链攻击](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 8.0/10

npm 包 Keyv 及其部分依赖项遭遇名为 Shai-Hulud 的供应链攻击，攻击者通过植入恶意 pre-install 钩子在安装时自动执行任意代码，窃取凭据或植入后门。该攻击影响了多个流行包，对 JavaScript 生态构成严重威胁。由于 npm 缺乏对 pre-install 脚本的默认限制，此类攻击极易得手，开发者应立即检查项目依赖并等待官方修复。

hackernews · cimi\_ · 8月4日 11:01 · [社区讨论](https://news.ycombinator.com/item?id=49166874)

**「背景」** Keyv 是一个拥有约 1.27 亿周下载量的 Node.js 键值存储库。npm 包可通过 preinstall 等生命周期脚本在安装时自动执行任意代码，这常被用于供应链攻击，即攻击者通过入侵维护者账户或依赖项来植入恶意代码。

**「影响」** 所有使用 Keyv 或相关受影响包的 JavaScript 项目，若在近期安装了受感染版本，均可能面临凭据泄露或远程代码执行风险。该攻击已处于活跃利用状态，应立即采取缓解措施。

**「社区讨论」** 社区普遍呼吁彻底禁用 pre-install 和 post-install 钩子，认为 npm 依赖链的脆弱性是此类攻击的根源。多名开发者建议在 ~/.npmrc 中设置 min-release-age=5 以延迟升级，并分享了用于检测受感染包的命令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack">Keyv and friends compromised in npm supply chain attack</a></li>

</ul>
</details>

**标签**: `#supply-chain-attack`, `#npm`, `#security`, `#open-source`, `#malware`

---

<a id="item-tech-news-4"></a>
### [MiniMax-H3 MLX 端口支持本地音视频生成](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 8.0/10

MiniMax 近日发布了全模态生成模型 MiniMax-H3，支持文本、图像、音频、视频输入并生成带音频的 15 秒视频。社区贡献者 PipeNetwork 迅速将其移植到 MLX 框架，使模型能在 Apple Silicon 设备上本地运行。Simon Willison 在 M5 Max MacBook Pro 上成功运行，模型下载量约 115GB，生成一段视频耗时近 45 分钟。由于未使用音频提示，生成的音频为无意义语音，但视频效果良好，且官方提供了详细的提示编写指南。

rss · Simon Willison · 8月4日 19:10

**「背景知识」** MiniMax H3 是 MiniMax 近日发布的全能型多模态生成模型，能够统一理解文本、图像、音频和视频，并生成最长 15 秒、带原生立体声音频的视频。MLX 是苹果公司为 Apple Silicon 芯片优化的机器学习框架，PipeNetwork 的移植将 MiniMax H3 模型转换为 MLX 格式，使其能在 Mac 上本地运行。

**「影响」** 现在，苹果芯片 Mac 用户可通过 MLX 在本地运行 MiniMax-H3，生成带音频的视频，但需准备约 115GB 存储空间并接受约 45 分钟的生成时间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H 3 : An Open Model Breaking the Boundaries Between Tasks...</a></li>
<li><a href="https://huggingface.co/MiniMaxAI/MiniMax-H3">MiniMaxAI/ MiniMax - H 3 · Hugging Face</a></li>

</ul>
</details>

**标签**: `#machine-learning`, `#multimodal-models`, `#video-generation`, `#apple-silicon`, `#mlx`

---

<a id="item-tech-news-5"></a>
### [Cloudflare 用 AI 每月 58 美元处理漏洞赏金](https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600) ⭐️ 8.0/10

Cloudflare 首席安全官 Grant Bourzikas 透露，公司已采用 Anthropic 的 Claude Sonnet 模型自动处理漏洞赏金报告，负责去重与价值评估，每月成本仅 58 美元，而换用安全专用模型 Mythos 同一工作每月需花费约 20 万美元，节省 99.97% 开支。同时，Cloudflare 已构建 200 多个自主安全代理，几乎弃用全部第三方安全工具，转而使用部分由 AI 辅助编写的自研应用。Bourzikas 建议其他企业不要效仿，强调 Cloudflare 具备自研安全软件的能力，并非每家银行都应自行开发所有软件。首席战略官 Stephanie Cohen 还将公司此前裁员 1100 人归因于 AI 带来的自动化变革，并透露 Cloudflare 正计划充当 AI 公司与出版商之间的中介，通过微支付让 AI 公司付费获取内容。

telegram · zaihuapd · 8月4日 09:24

**「背景」** 漏洞赏金计划由企业向外部安全研究人员征求漏洞报告，通常需人工去重、评估危害并分配奖金，成本高昂且耗时。Cloudflare 作为大型互联网服务商，每日接收大量报告，传统上依赖第三方安全工具或专用模型管理该流程。

**「影响」** 该案例为具备自研能力的安全团队提供了可量化的 AI 自动化降本参考，但 Cloudflare 强调其模式不可复制，普通企业仍需谨慎评估自身开发能力。

**标签**: `#AI 安全`, `#漏洞赏金自动化`, `#Cloudflare`, `#安全工程`, `#成本优化`

---

<a id="item-tech-news-6"></a>
### [首部 L3/L4 自动驾驶强制国标发布，2027 年 7 月实施](https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html) ⭐️ 8.0/10

工业和信息化部组织制定的《智能网联汽车 自动驾驶系统安全要求》（GB 44721—2026）强制性国家标准正式获批，将于 2027 年 7 月 1 日起实施。这是我国首部针对 L3 级有条件自动驾驶和 L4 级高度自动驾驶系统的强制性国标，适用于 M 类（载客）和 N 类（载货）车辆，但不包括自动泊车系统。该标准从 2024 年的推荐性国标升级为强制性，要求自动驾驶系统安全水平至少达到合格且专注驾驶人的水平，从企业全生命周期安全保障、系统动态驾驶能力、人机交互与用户告知、多维度检验检测四个维度构建安全要求体系。

telegram · zaihuapd · 8月4日 13:06

**「背景」** L3 级有条件自动驾驶指系统可在特定条件下执行全部驾驶任务，但驾驶人需随时准备接管；L4 级高度自动驾驶则在限定场景下无需驾驶人接管。此前，我国于 2024 年发布了推荐性国标，此次为首次将其升级为强制性要求，以强化自动驾驶系统的安全底线。

**「影响」** 该标准将强制规范国内 L3/L4 自动驾驶车辆的开发与上市，要求车企在 2027 年 7 月 1 日前确保相关系统符合安全要求，否则可能无法通过认证。

**标签**: `#autonomous driving`, `#China`, `#regulations`, `#safety standards`, `#L3/L4`

---

<a id="item-tech-news-7"></a>
### [白宫对开源 AI 监管急转弯，硅谷内部分裂加剧](https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html) ⭐️ 8.0/10

特朗普政府内部曾考虑动用制裁、贸易黑名单甚至禁止美企与中国公司合作，以限制中国开源 AI 模型，但在硅谷强烈反对后，白宫于 8 月 4 日转而邀请科技公司商议新框架，拟在模型发布前审查网络安全。这次政策急转弯的导火索是中国开源模型 Kimi 部分性能比肩 OpenAI 顶级模型，凸显了开源 AI 的快速追赶能力。OpenAI 与 Anthropic 以国家安全为由推动限制中国对手，而 Nvidia、Meta 等则力挺开放生态，黄仁勋首次在 X 发帖为开源辩护，并组建了逾 230 家成员的安全联盟。政府最终聚焦于提升美国 AI 竞争力，而非直接封锁，但硅谷内部的分裂已公开化。

telegram · zaihuapd · 8月4日 15:22

**「背景」** 美国 AI 监管政策在国家安全与产业创新之间长期摇摆，而开源 AI 模型因其可自由获取的特性，削弱了闭源公司的技术壁垒，导致硅谷巨头间利益分化。随着中国开源模型在某些基准上逼近甚至追平美国顶尖闭源模型，围绕是否限制中国开源模型的讨论激化了这一内部分歧。

**「影响」** 此次逆转可能使针对中国开源模型的直接制裁暂时搁置，但新的发布前安全审查框架将给开源 AI 的协作与部署节奏带来不确定性，并可能加剧中美在 AI 标准与供应链上的制度性分歧。

**标签**: `#AI regulation`, `#open-source AI`, `#Silicon Valley`, `#Chinese AI models`, `#technology policy`

---

<a id="item-tech-news-8"></a>
### [Mistral 发布 Shieldstral：3B 参数开源多模态审核模型](https://mistral.ai/news/shieldstral/) ⭐️ 7.0/10

Mistral 发布了 Shieldstral，一个 30 亿参数的开源权重多模态内容审核模型，能够对文本和图像回答单一的是/否问题（例如“此内容是否宣扬暴力”）。该模型的开源特性使开发者能够集成和定制安全审查，无需依赖闭源 API，适用于作为 AI 应用的第一道防线。尽管其非确定性输出可能要求人工复核，但这一发布为日益需要的透明、可控审核工具提供了实用选择。

hackernews · riadsila · 8月4日 16:36 · [社区讨论](https://news.ycombinator.com/item?id=49171268)

**「背景」** Shieldstral 将内容审核重新定义为一种策略自适应的问答任务：模型接收文本或图像内容，并回答一个具体的 yes/no 问题（如“该内容是否宣扬暴力？”），从而判断安全性。这种设计允许开发者在不重新训练的情况下调整审核规则，且该 3B 参数模型仅需单张 16GB GPU 即可运行，效率远超多数大模型。

**「影响」** 对于需要内嵌内容安全机制的开发者，Shieldstral 提供了一个可直接集成、参数规模仅 3B 的开源选项，有望减少对第三方闭源审核 API 的依赖，但其非确定性意味着在关键决策中仍需人工监督。

**「社区讨论」** 社区评论质疑该模型能否支持任意规则集，还是仅局限于预设审查风格；同时讨论了其与 OpenAI Omni-moderation 的性能对比，以及非确定性在宗教文本等争议内容上的适用性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral. | Mistral AI</a></li>

</ul>
</details>

**标签**: `#moderation`, `#multimodal`, `#open-weights`, `#AI safety`, `#Mistral`

---

<a id="item-tech-news-9"></a>
### [生成多样化肤色的算法与色彩空间](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 7.0/10

Toney Alexander 开发了一个用于生成多样化肤色的色彩空间和算法，包含颜色选择器和程序化生成功能，旨在帮助数字艺术和游戏开发。该空间的核心思路是：对肤色数据进行 PCA 降维，将三维颜色映射到二维平面，再通过手动函数拟合生成逼真的肤色。页面提供了交互式演示和详细说明，展示了方法的实用性和局限性。

hackernews · automatoney · 8月4日 15:16 · [社区讨论](https://news.ycombinator.com/item?id=49170165)

**「背景」** 色彩空间是组织和表示颜色的数学模型；常见的 RGB 空间在描述不同光照条件下的人类肤色感知时不够理想。主成分分析（PCA）是一种降维技术，可用于从肤色数据集中提取最具代表性的颜色变化轴，从而帮助构建更贴合肤色自然分布的空间。

**「影响」** 对于数字艺术家和游戏开发者，该工具提供了一种无需手动调配即可快速生成可信且多样化肤色的方法。

**「社区讨论」** 社区普遍赞赏该工作，尤其肯定函数拟合方法巧妙，但有人指出部分生成颜色可能偏绿或偏紫，并建议参考 Pantone 肤色色卡等现有标准以提升准确性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://digitalcommons.imsa.edu/sir_presentations/2026/session1/49/">DigitalCommons@IMSA - IMSAloquium Student Investigation...</a></li>

</ul>
</details>

**标签**: `#color-science`, `#algorithm`, `#computer-graphics`, `#generative-art`, `#skin-tone`

---

<a id="item-tech-news-10"></a>
### [FedEx 等企业邮件形似钓鱼，训练用户忽视安全警告](https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/) ⭐️ 7.0/10

安全研究员 Troy Hunt 在 2024 年撰文指出，FedEx 等企业长期使用类似钓鱼邮件的做法（如发件人为个人邮箱、附带 PDF、链接使用短域名等），持续训练用户忽略安全警告，加剧了钓鱼攻击的危害。这些合法邮件与诈骗信息边界模糊，使用户难以区分，甚至对安全提示产生麻木。文章强调，企业邮件实践中的短域名（如 c.gle）、新通用顶级域（如.xyz）的泛滥，正在系统性削弱用户的安全意识，使反钓鱼努力事倍功半。

hackernews · stymaar · 8月4日 21:09 · [社区讨论](https://news.ycombinator.com/item?id=49175192)

**「背景：企业邮件为何助长钓鱼攻击」** 安全研究员 Troy Hunt 在 2024 年 2 月 24 日的博文中揭露，FedEx 等公司发送的官方邮件常带有拼写错误、怪异发件人地址等明显的钓鱼特征。这些看似“可疑”的合法邮件反复出现在用户收件箱中，实际上在训练用户忽略警告信号，导致他们难以区分真正的欺诈邮件，从而加剧了钓鱼攻击的泛滥。

**「影响」** 用户因长期接触形似钓鱼的合法邮件，对安全警告的敏感度降低，导致实际钓鱼攻击的成功率上升，个人和企业数据泄露风险加剧。

**「社区讨论」** 评论者普遍认同企业邮件实践模糊了合法与诈骗的界限，并分享了 FedEx 海关通知、Google 使用 c.gle 短链接、IRS 语音系统与诈骗电话相似等亲身经历，认为这些做法使普通用户更难防范钓鱼，是系统性问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/">Troy Hunt: Thanks FedEx, This is Why we Keep Getting Phished</a></li>

</ul>
</details>

**标签**: `#phishing`, `#cybersecurity`, `#social engineering`, `#email security`, `#corporate practices`

---

<a id="item-tech-news-11"></a>
### [苹果指控更多前员工向 OpenAI 泄露机密数据](https://techcrunch.com/2026/08/04/apple-says-more-ex-employees-may-have-taken-confidential-data-to-openai/) ⭐️ 7.0/10

苹果公司在一场与 OpenAI 的硬件商业秘密诉讼中扩大指控，声称可能有更多前员工将机密数据带到 OpenAI。此案最初围绕苹果前员工涉嫌窃取硬件设计机密，而新指控指出这些员工可能通过截图和利用认证漏洞获取了至少 37 份高度敏感的技术文件。这一进展加剧了这起科技行业法律纠纷，可能影响 OpenAI 自研 AI 芯片等硬件计划。

hackernews · thewebguyd · 8月4日 15:37 · [社区讨论](https://news.ycombinator.com/item?id=49170479)

**「背景」** 苹果公司此前已对 OpenAI 提起商业秘密诉讼，指控其非法获取了苹果的硬件机密数据。现在，苹果在最新法庭文件中表示，调查范围扩大，可能涉及更多前员工在离职后保留或访问了苹果的机密信息，并可能将其带至 OpenAI。

**「影响」** 若指控成立，可能迫使 OpenAI 搁置或调整其硬件研发方向，并加剧科技公司对员工流动中知识产权保护的担忧。

**「社区讨论」** 社区评论中，部分人认为这是苹果惯用的恐吓策略，也有人指出指控涉及截图等具体证据而非仅凭记忆；还有评论认为 OpenAI 的硬件项目是 Sam Altman 的虚荣之举，诉讼可能反而对其有利。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/08/04/apple-says-more-ex-employees-may-have-taken-confidential-data-to-openai/">Apple says more ex - employees may have taken confidential data ...</a></li>

</ul>
</details>

**标签**: `#apple`, `#openai`, `#legal`, `#data-theft`, `#hardware`

---

<a id="item-tech-news-12"></a>
### [Harness 工程：AI 自我改进的工程实践](https://lilianweng.github.io/posts/2026-07-04-harness/) ⭐️ 7.0/10

Lilian Weng 的博客文章探讨了用于 AI 自我改进的“harness”工程，即通过优化代理的提示词、工具和代码来提升其性能、质量和成本效率。文章引发了社区对如何在大型代码库中实施这一理念的讨论，核心在于定义明确的质量指标，并构建可靠的适应度函数。评论者分享了自动研究 harness 的实际经验，发现通过分析生产轨迹来发现问题、让代理自行编写工具能显著降低 token 消耗。这一方法表明，优化代理周围的“harness”可能比单纯扩大模型规模更具样本效率。

hackernews · tosh · 8月4日 06:17 · [社区讨论](https://news.ycombinator.com/item?id=49164896)

**「背景知识」** 在 AI 自改进的语境中，“harness”指围绕 AI agent 构建的工程支架，包含工具、技能、提示词和评估函数等，使 agent 能够通过分析自身运行轨迹来优化性能、质量或成本，而无需修改模型权重。自改进指 agent 自动迭代其使用的外部组件，如生成更高效的专用工具或调整提示词，以实现闭环优化。Lilian Weng 的博文系统阐述了这一工程化方法，并激发了关于如何在组织层面实现此类自改进系统的讨论。

**「影响」** 对于构建 AI 代理的工程师而言，harness 工程可能成为提升代理性能的关键杠杆，通过自动优化工具、提示和上下文管理，能直接改善代理在实际任务中的表现。

**「社区讨论」** 社区讨论中，实践经验表明让代理分析生产轨迹并自行编写工具可大幅减少 token 消耗，但定义可靠的质量函数仍是关键挑战。此外，有评论者展望 harness 未来可能自行生成 RLHF 训练集并微调底层模型。

**标签**: `#ai`, `#self-improvement`, `#harness-engineering`, `#software-engineering`, `#llm`

---

<a id="item-tech-news-13"></a>
### [白宫完成 AI 评估框架，细节不公开](https://www.axios.com/2026/08/03/white-house-finalizes-ai-framework-behind-closed-doors) ⭐️ 7.0/10

白宫于 8 月 3 日宣布已按期完成先进 AI 模型的自愿评估框架，但拒绝公开框架内容、审阅者名单及启用时间表。该框架规定企业在模型公开发布前最多 30 天内向政府开放访问，并明确保密、网络安全、知识产权保护及保密协议等要求，同时列出可提前接触模型的“可信伙伴”。网络能力基准测试及适用门槛被列为机密。白宫已邀请 OpenAI、谷歌、Anthropic 等公司于周二参加闭门审阅，并称正与更多业界伙伴讨论后续步骤。

telegram · zaihuapd · 8月4日 02:31

**「背景」** 该框架源于 6 月 2 日签署的行政令，要求建立对先进 AI 模型的自愿评估机制，以在模型发布前确保政府能够提前审查潜在风险。该行政令将模型网络能力基准测试等技术细节列为机密，并设定了 8 月初的完成期限。

**「影响」** 该自愿框架将迫使 AI 实验室在模型发布前调整内部流程，提前至少 30 天向政府开放访问，并承担保密和知识产权保护义务，可能延缓公开发布节奏。

**标签**: `#AI regulation`, `#government policy`, `#model evaluation`, `#voluntary framework`, `#AI safety`

---

<a id="item-tech-news-14"></a>
### [iPhone 与 Win 剪贴板共享将随 iOS 28 登陆欧盟](https://appleinsider.com/articles/26/08/04/iphone-to-windows-clipboard-sharing-coming-to-ios-28-in-the-eu) ⭐️ 7.0/10

苹果已批准微软依据欧盟《数字市场法案》（DMA）提交的互操作性请求，将开发 iPhone 与 Windows PC 之间的跨设备剪贴板共享功能。该功能预计在 2027 年秋季随 iOS 28 的某个版本向欧盟用户推出，支持在 iPhone 上复制、在 Windows 上粘贴，反之亦然，无需第三方应用和反复授权。微软于 2026 年 3 月 25 日提交请求，同年 6 月 26 日获批；实现方案类似 iOS 26.5 中的配件通知框架，开发者需通过 AccessorySetupKit 进行一次配对授权。该功能目前仅面向欧盟开发，苹果未排除未来推广至全球的可能性，但能否赶上 iOS 28 首个正式版尚不确定。

telegram · zaihuapd · 8月4日 03:15

**「背景」** 欧盟《数字市场法案》（DMA）要求苹果等被认定为“守门人”的平台向第三方开放互操作性，此次微软正是根据该机制提交了跨设备剪贴板共享的请求。苹果批准这一请求，标志着 DMA 推动下的又一项跨平台互操作功能落地，与此前开放的配件通知框架等路径类似。

**「对欧盟用户的影响」** 欧盟的 iPhone 用户预计在 2027 年秋季随 iOS 28 获得系统级 iPhone 与 Windows 跨设备剪贴板共享，无需第三方应用并仅需一次配对授权，从而消除了当前 iOS 对剪贴板后台同步的限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://appleinsider.com/articles/26/08/04/iphone-to-windows-clipboard-sharing-coming-to-ios-28-in-the-eu">iPhone to Windows clipboard sharing coming to iOS 28 in the EU</a></li>
<li><a href="https://www.hngn.com/articles/272564/20260804/apple-bring-iphone-windows-clipboard-sharing-eu-users-under-microsofts-dma-request.htm">Apple To Bring iPhone-Windows Clipboard Sharing To EU Users Under Microsoft&#x27;s DMA Request</a></li>

</ul>
</details>

**标签**: `#cross-platform`, `#interoperability`, `#clipboard`, `#iOS`, `#DMA`

---

<a id="item-tech-news-15"></a>
### [华为首席科学家警告英伟达芯片将触及物理极限](https://www.bloomberg.com/news/articles/2026-08-04/huawei-s-top-scientist-warns-of-chip-limit-nvidia-will-soon-face) ⭐️ 7.0/10

华为首席半导体科学家廖恒在 7 月底的一次公开采访中警告，英伟达等厂商通过堆叠计算芯片与高带宽内存来扩展性能的做法终将遭遇物理极限，跨越极限后将出现“雪崩”式衰退。他提出以“韬定律”为替代路径，并宣布首款采用“LogicFolding”技术框架的手机芯片将于今年晚些时候亮相。廖恒还指出，中美半导体产业正分化为两个独立生态系统，各方必须构建完整的制造与供应能力才能生存。

telegram · zaihuapd · 8月4日 08:04

**「背景」** 长期以来，AI 芯片性能提升主要依赖增大芯片面积、提高晶体管密度和增加高带宽内存（HBM），但这些方式正逼近物理极限，面临能效和散热瓶颈\[1\]。华为首席科学家廖恒在近期公开采访中提出‘韬定律’和‘LogicFolding’技术框架作为替代路径，并透露首款采用该技术的手机芯片将于今年晚些时候推出。

**「影响」** 若华为年内推出的 LogicFolding 手机芯片得以验证，将在移动端提供一条绕开传统缩放限制的新路径，并可能加剧中美半导体生态的分离趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://theunum.io/en/news/read/huawei-scientist-liao-heng-announced-the-physical-scaling-limits-of-nvidia-chips">Huawei scientist Liao Heng announced the physical scaling limits of...</a></li>

</ul>
</details>

**标签**: `#semiconductor physics`, `#AI hardware`, `#chip scaling`, `#NVIDIA`, `#Huawei`

---

<a id="item-tech-news-16"></a>
### [美国拟起草禁令禁止进口中国光模块](https://www.reuters.com/world/trump-administration-drafting-ban-chinese-data-center-devices-sources-say-2026-08-04/) ⭐️ 7.0/10

据路透社援引知情人士报道，特朗普政府正在起草一项禁令，拟禁止进口用于数据中心的中国新型光模块，由美国联邦通信委员会（FCC）推进，目标是在今年内发布并生效。此举旨在保护支撑人工智能热潮的关键基础设施，防止所谓的数据窃取、恶意软件植入或服务中断。若禁令实施，将冲击全球市场份额第一（27%）的中国光模块厂商中际旭创。目前该禁令仍处于草案阶段，可能修改或搁置，中国驻美使馆表示将对损害中国利益的行为采取一切必要措施。

telegram · zaihuapd · 8月4日 11:29

**「背景」** 光模块是数据中心内部实现高速光互联的关键器件，对人工智能训练和推理网络至关重要。中国厂商在全球光模块市场占据主导地位，中际旭创等企业是主要供应商。美国联邦通信委员会（FCC）此前已以国家安全为由，陆续对中国无人机、路由器、机器人和逆变器实施进口限制，此次禁令是这一趋势的延续。

**「影响」** 若禁令生效，依赖中国光模块的美国数据中心和 AI 基础设施运营商将面临供应链中断和成本上升，而中际旭创等主要供应商可能失去重要市场。不过，由于禁令仍在起草阶段，具体范围和实施时间尚不确定。

**标签**: `#technology policy`, `#optical modules`, `#data centers`, `#AI infrastructure`, `#supply chain`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [谷歌为 Anthropic 搭建 2000 亿美元 AI 融资架构](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 9.0/10

谷歌已为 AI 公司 Anthropic 搭建总额约 2000 亿美元的融资架构，其中超 1500 亿美元用于交付 AI 芯片；首批交易通过特殊目的载体购入约 350 亿美元硬件，约合 1 吉瓦算力与 100 万颗 TPU。

telegram · zaihuapd · 8月4日 10:52

**「背景」** 由于 Anthropic 无信用评级，该架构借鉴厂商融资模式，让博通、阿波罗、黑石、摩根士丹利等参与方分担风险，谷歌担保数据中心，出资方购买硬件后回租给 Anthropic。

**标签**: `#AI`, `#Infrastructure Financing`, `#Semiconductors`, `#Anthropic`, `#Google`

---

<a id="item-finance-news-2"></a>
### [Polymarket 洽谈估值逾 200 亿美元融资](https://www.cnbc.com/2026/08/04/polymarket-seeks-fundraising-round-at-more-than-20-billion-valuation.html) ⭐️ 8.0/10

据知情人士透露，预测市场平台 Polymarket 正就新一轮融资进行谈判，估值目标超过 200 亿美元；此前该公司表示其年化收入已远超 10 亿美元。

rss · CNBC Finance · 8月4日 13:31

**「背景」** Polymarket 今年 4 月刚完成一轮融资，估值 150 亿美元；其竞争对手 Kalshi 在 5 月的融资估值达 220 亿美元，并计划寻求更高估值。

**标签**: `#prediction markets`, `#Polymarket`, `#fundraising`, `#valuation`, `#fintech`

---

<a id="item-finance-news-3"></a>
### [国家邮政局对申通快递立案调查](https://www.spb.gov.cn/gjyzj/c100015/c100016/202608/c4467c234e1c4db0a6e393cff2e64902.shtml) ⭐️ 8.0/10

国家邮政局于 8 月 4 日宣布，因申通快递有限公司对使用其商标的快递企业安全生产管理缺位、未按规定实行统一管理，导致 2026 年以来多发生产安全事故，依法对该公司立案调查。

telegram · zaihuapd · 8月4日 12:07

**「背景」** 申通快递是国内主要快递企业，其品牌授权网点多次被监管部门查出安全隐患，但公司未能对加盟商的安全保障进行统一管理，触发了监管机构的正式调查。

**标签**: `#regulatory investigation`, `#logistics`, `#Shentong Express`, `#production safety`, `#listed company`

---