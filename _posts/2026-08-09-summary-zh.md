---
layout: default
title: "Horizon Summary: 2026-08-09 (ZH)"
date: 2026-08-09
lang: zh
---

> 从 36 条内容中筛选出 8 条重要资讯。

---

**科技新闻**
1. [全球最大单体 AI 算力设施在内蒙古乌兰察布投产](#item-tech-news-1) ⭐️ 9.0/10
2. [Shopify 用 MySQL 替换 Redis 实现库存预留，通过有界行池化扩展](#item-tech-news-2) ⭐️ 8.0/10
3. [语言模型首次生成可存活的全新噬菌体基因组](#item-tech-news-3) ⭐️ 8.0/10
4. [腾讯 WorkBuddy 成战略级办公智能体，国内居首](#item-tech-news-4) ⭐️ 7.0/10
5. [SpaceX 计划月球建厂制造 AI 卫星](#item-tech-news-5) ⭐️ 7.0/10
6. [MiniMax H3 团队 AMA 透露将开源 2K 模型与稀疏注意力](#item-tech-news-6) ⭐️ 7.0/10

**财经新闻**
1. [伯克希尔第二季度营业利润增长 16%，CEO Abel 开始动用巨额现金储备](#item-finance-news-1) ⭐️ 7.0/10
2. [美国法院批准药明康德初步禁令，暂停军方清单即时影响](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [全球最大单体 AI 算力设施在内蒙古乌兰察布投产](https://www.globaltimes.cn/page/202608/1367666.shtml) ⭐️ 9.0/10

8 月 6 日，远景科技集团宣布“远景乌兰察布星河基地”正式投产，成为全球最大的单体 AI 算力设施。该基地建筑面积 12 万平方米，支持百万 GPU 并行计算，规划总容量 2GW，是全球 Token 产出能力最强的单体 AI 数据中心，绿电占比超过 80%。乌兰察布是国家“东数西算”八大节点之一，距离北京约 240 公里，数据传输延迟仅 4.2 毫秒，数据中心电价较京津冀低约 50%，此前已有华为、阿里巴巴等企业在此布局。该基地是远景“戈壁使命”计划首个旗舰项目，旨在为国产算力集群提供可复制的建设方案。

telegram · zaihuapd · 8月9日 05:06

**「背景」** “东数西算”是中国将东部密集的算力需求有序引导到西部能源丰富地区的国家工程，旨在利用西部绿色能源和低成本优势建设大型数据中心。乌兰察布作为八大枢纽节点之一，凭借凉爽气候、靠近京津冀的地理位置和低廉电价，已成为多家科技企业算力基础设施的聚集地。

**「影响」** 该设施投产后，将为国内大模型训练和推理提供百万 GPU 级的并行计算能力，并结合超 80%的绿电和低电价，显著降低大规模 AI 算力成本，加速国产 AI 集群的规模化部署。

**标签**: `#AI infrastructure`, `#data center`, `#GPU computing`, `#green energy`, `#East Data West Computing`

---

<a id="item-tech-news-2"></a>
### [Shopify 用 MySQL 替换 Redis 实现库存预留，通过有界行池化扩展](https://shopify.engineering/scaling-inventory-reservations) ⭐️ 8.0/10

Shopify 工程团队公开了将库存预留系统从 Redis 迁移至 MySQL 的详细技术方案。他们采用每可售单元一行（而非数量列）的设计，并引入有界可用行池（每商品/地点组合最多 1,000 行）来避免高并发下的锁竞争和行数爆炸。预留操作直接消费池中的行，后台补充进程维持池大小，无需锁定即可安全处理并发请求。这一方案使 Shopify 在保证数据一致性的前提下，克服了 Redis 的局限性，实现了可扩展的库存预留。

hackernews · adletbalzhanov · 8月8日 22:32 · [社区讨论](https://news.ycombinator.com/item?id=49226536)

**「背景」** 在电子商务中，库存预留（inventory reservation）是为了防止超卖，在结账过程中临时为客户锁定商品。高并发的预留系统通常依赖 Redis 等内存数据库实现快速原子操作，因为传统关系型数据库在更新单行库存数量时容易产生锁竞争。Shopify 的工程师尝试用 MySQL 替代现有的 Redis 预留方案。

**「影响」** 对于面临类似高并发库存预留挑战的工程师，该实践证明了通过行级单元与有界池化设计，可以在 MySQL 上构建无锁、可扩展的预留系统，为用关系数据库替代键值存储提供了具体参考。

**「社区讨论」** 评论区中，有用户质疑博文为 LLM 生成，对 Shopify 工程师的可信度造成影响；另有用户提出更简单的方案（下单时直接扣减库存并维护进行中订单，超时后由后台归还），但未获回应，引发了对该设计选择合理性的讨论。

**标签**: `#inventory-systems`, `#mysql`, `#redis`, `#scalability`, `#concurrency`

---

<a id="item-tech-news-3"></a>
### [语言模型首次生成可存活的全新噬菌体基因组](https://www.reddit.com/r/MachineLearning/comments/1vjj4pr/r_generative_design_of_novel_bacteriophages_with/) ⭐️ 8.0/10

研究人员利用前沿基因组语言模型 Evo 1 与 Evo 2，以裂解性噬菌体 ΦX174 为模板，生成了具有合理基因组架构和目标宿主嗜性的全基因组序列。实验测试证实，16 个 AI 生成的基因组产生了可存活的噬菌体，且这些噬菌体呈现出显著的进化新颖性。该研究首次实现了生成式全基因组设计，并得到实验验证，展示了语言模型在从头设计复杂生物系统方面的巨大潜力。

reddit · r/MachineLearning · /u/moschles · 8月9日 07:11

**「研究背景」** 基因组语言模型（如 Evo 1 和 Evo 2）是将基因组序列当作语言来学习的深度学习模型，能够理解遗传规律并生成序列。噬菌体是感染细菌的病毒，ΦX174 是一种结构简单的裂解性噬菌体，常被用作合成生物学研究的设计模板。此前，人工智能能否生成完整且可存活的噬菌体基因组尚未得到实验验证。

**「影响」** 该研究首次证明了语言模型能从头设计可存活的全基因组，为合成生物学和噬菌体疗法等领域提供了可工程化的全新工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.biorxiv.org/content/10.1101/2025.09.12.675911v1">Generative design of novel bacteriophages with genome language models | bioRxiv</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#generative models`, `#synthetic biology`, `#genome language models`, `#bioinformatics`

---

<a id="item-tech-news-4"></a>
### [腾讯 WorkBuddy 成战略级办公智能体，国内居首](https://mp.weixin.qq.com/s/TRUjakoaprGFSYYQB301xw) ⭐️ 7.0/10

腾讯已将办公 AI 智能体 WorkBuddy 列为内部战略优先级最高的产品之一，内部视其为继 QQ、微信后的第三个战略级产品。根据易观报告，2026 年第二季度 WorkBuddy 的 PC 端月访问量达到 2097 万次，月活跃用户达 2000 万级别，日活百万，位居国内办公智能体平台首位。该产品已接入腾讯文档、企业微信、腾讯会议等核心生态，并支持混元、DeepSeek、GLM 等多种大模型；今年 7 月，腾讯还将 QClaw 相关业务调整至 WorkBuddy 所在部门以集中探索。目前 WorkBuddy 仍处于投入阶段，未设定商业化 KPI，年内重点放在扩大企业客户覆盖上。

telegram · zaihuapd · 8月8日 13:50

**「背景」** WorkBuddy 是腾讯于 2026 年推出的桌面级 AI 办公智能体，作为一个全场景 AI 助手，它能自主规划并执行多模态复杂任务，支持多 Agent 并行与 Skills 扩展（tool-1-1、tool-1-3）。该产品国内版支持无缝切换混元、DeepSeek、GLM 等多种大模型，并深度集成了腾讯文档、企业微信、腾讯会议等生态（tool-1-2）。这一定位使其成为腾讯在办公场景中继 QQ 和微信之后的战略级产品，同时也整合了 QClaw 相关业务，凸显了腾讯对 AI 办公赛道的集中投入。

**「影响」** WorkBuddy 的战略级定位和生态整合将加速腾讯在企业办公 AI 市场的渗透，对逾 2000 万月活用户及企业微信、腾讯文档等生态内的企业客户，带来更紧密的 AI 协作体验，并可能进一步巩固其在国内办公智能体领域的领先地位。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.codebuddy.cn/work/">WorkBuddy - AI Agent 办 公 新范式</a></li>
<li><a href="https://www.pai.com.cn/p/01kk8t0p3tf9tem36es6dy989p">腾 讯 旗下全场景AI 智 能 体 WorkBuddy 正式上线 - 电商派</a></li>
<li><a href="https://www.leavescn.com/Articles/Content/3875">WorkBuddy 是什么？ 腾 讯 版OpenClaw AI 办 公 助手全面解析</a></li>

</ul>
</details>

**标签**: `#AI products`, `#Tencent`, `#office agents`, `#Chinese tech`, `#enterprise AI`

---

<a id="item-tech-news-5"></a>
### [SpaceX 计划月球建厂制造 AI 卫星](https://finance.yahoo.com/technology/articles/pure-insanity-elon-musk-details-173635969.html) ⭐️ 7.0/10

在 SpaceX 首次上市公司财报电话会议上，马斯克公布了一项在月球建立自动化工厂的计划，拟通过星舰运送机器人设备，从月壤中提取铝、钛、硅等矿物，大规模生产 AI 计算卫星，并利用电磁弹射系统直接从月球表面发射入轨。尽管月球环境极端，前 SpaceX 高管 Jim Cantrell 称该计划“纯属疯狂”但认为能够实现，业界普遍认可其技术可行性，但指出马斯克的时间表通常过于乐观。SpaceX 当季营收 78 亿美元，太空部门因星舰投入录得 2.05 亿美元亏损。

telegram · zaihuapd · 8月9日 05:37

**「背景知识」** SpaceX 的 Starship 是一种可重复使用的超重型运载火箭，设计用于将大量货物和人员送往月球和火星。电磁质量驱动器（或称电磁弹射器）是一种利用电磁力将有效载荷加速至轨道速度的发射系统，可从月球表面直接部署卫星，无需化学火箭。

**「影响」** 该计划若成功，可大幅降低卫星制造与发射成本，加速 AI 卫星星座部署，但鉴于技术挑战和马斯克乐观的时间表，短期实际影响有限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eweek.com/news/spacex-robots-moon-factories/">SpaceX Envisions Robots Building AI Satellite Factories on... | eWeek</a></li>
<li><a href="https://www.futura-sciences.com/en/elon-musk-plans-a-moon-factory-with-an-electromagnetic-catapult-to-launch-ai-satellites_25836/">Elon Musk plans a Moon factory with an... - Futura-Sciences</a></li>

</ul>
</details>

**标签**: `#spacex`, `#lunar-factory`, `#ai-satellites`, `#robotics`, `#space-manufacturing`

---

<a id="item-tech-news-6"></a>
### [MiniMax H3 团队 AMA 透露将开源 2K 模型与稀疏注意力](https://www.reddit.com/r/StableDiffusion/s/fjM3d7AEV8) ⭐️ 7.0/10

MiniMax H3 团队在 Reddit r/StableDiffusion 社区 AMA 中宣布，将开源 H3-Regenerate-2K 模型，这是一个专用于高分辨率生成的潜空间 DiT 再生模型，但未给出具体发布日期。团队还计划近期发布稀疏注意力参考实现，目标是在不引入可感知画质损失的前提下提升效率。此外，官方正在考虑推出 4/8 步低步数推理版本，并计划基于 H3 模型谱系衍生独立图像生成模型。针对社区反馈的 Ref2VA 画质退化和纹理细节模糊等问题，团队表示已着手改进。

telegram · zaihuapd · 8月9日 08:28

**「背景」** MiniMax H3 是 MiniMax 公司于近期开源的一款视频生成模型，其初始开源版本暂未包含稀疏注意力机制，且仅输出 768p 视频。该模型采用专用的潜空间 DiT 架构，用于 2K 分辨率再生的 H3-Regenerate-2K 组件并非传统超分辨率模块，而为独立再生模型；稀疏注意力技术则旨在以可忽略的画质损失换取更低的计算开销。团队在本次 Reddit AMA 中透露了开源这些组件的计划，但尚未公布具体时间。

**「影响」** 视频生成社区将获得一个专门的高分辨率再生模型和稀疏注意力实现，但实际使用需等待代码放出，且暂无明确时间表。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minimax.io/news/minimax-h3-open-source">Open General Intelligence: MiniMax H3 Is Now Open Source - MiniMax News | MiniMax</a></li>

</ul>
</details>

**标签**: `#video generation`, `#open source`, `#sparse attention`, `#MiniMax`, `#AMA`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [伯克希尔第二季度营业利润增长 16%，CEO Abel 开始动用巨额现金储备](https://www.cnbc.com/2026/08/08/berkshire-hathaway-earnings-q2-2026.html) ⭐️ 7.0/10

伯克希尔·哈撒韦第二季度营业利润同比增长 16%至 129.8 亿美元，首席执行官 Greg Abel 通过约 45 亿美元的股票回购和近 200 亿美元的净股票购买，开始部署公司创纪录的现金储备。

rss · CNBC Finance · 8月8日 13:28

**「背景」** 前任 CEO 沃伦·巴菲特此前持续净卖出股票，积攒了近 4000 亿美元现金，但 Abel 今年初接任后，在第二季度扭转了此前连续 14 个季度的净卖出态势。

**标签**: `#Berkshire Hathaway`, `#earnings`, `#share buybacks`, `#Greg Abel`, `#equity purchases`

---

<a id="item-finance-news-2"></a>
### [美国法院批准药明康德初步禁令，暂停军方清单即时影响](https://np-info.eastmoney.com/wap/notice/?referrer=appShare&amp;amp;infocode=AN202608091827791183) ⭐️ 7.0/10

美国哥伦比亚特区联邦地区法院于 2026 年 8 月 7 日批准药明康德申请的初步禁令动议，该公司在挑战美国国防部“中国军工企业清单”（1260H 清单）认定的司法程序期间，将免受该认定带来的即时不利影响。

telegram · zaihuapd · 8月9日 10:13

**「背景」** 美国国防部于 2026 年 6 月 8 日将药明康德等十多家中国企业列入 1260H 清单，该清单虽非制裁，但禁止国防部与其签订合同，并计划从 2027 年起全面禁止通过第三方采购其产品或服务。

**标签**: `#biotech`, `#US-China`, `#legal`, `#trade-restrictions`, `#corporate`

---