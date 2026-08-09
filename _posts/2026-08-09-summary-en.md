---
layout: default
title: "Horizon Summary: 2026-08-09 (EN)"
date: 2026-08-09
lang: en
---

> From 36 items, 8 important content pieces were selected

---

**Technology News**
1. [World&\#x27;s largest single-building AI compute facility launches in Inner Mongolia](#item-tech-news-1) ⭐️ 9.0/10
2. [Shopify replaced Redis with MySQL for inventory reservations–and it scaled](#item-tech-news-2) ⭐️ 8.0/10
3. [Generative AI Designs First Viable Novel Bacteriophages](#item-tech-news-3) ⭐️ 8.0/10
4. [Tencent&\#x27;s WorkBuddy AI Agent Becomes Strategic Priority, Tops Rivals](#item-tech-news-4) ⭐️ 7.0/10
5. [Elon Musk Unveils SpaceX Lunar Factory Plan for AI Satellites](#item-tech-news-5) ⭐️ 7.0/10
6. [MiniMax H3 Team Reveals Plans to Open-Source 2K Model and Sparse Attention](#item-tech-news-6) ⭐️ 7.0/10

**Financial News**
1. [Berkshire Hathaway Q2 earnings up 16%, new CEO Abel starts deploying cash](#item-finance-news-1) ⭐️ 7.0/10
2. [US Court Temporarily Blocks Pentagon Blacklist of WuXi AppTec](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [World&\#x27;s largest single-building AI compute facility launches in Inner Mongolia](https://www.globaltimes.cn/page/202608/1367666.shtml) ⭐️ 9.0/10

On August 6, Envision Group announced the launch of its &quot;Envision Ulanqab Nebula Base&quot; in Inner Mongolia, the world&\#x27;s largest single-building AI computing facility. The 12,000-square-meter site supports million-GPU parallel computing with a planned total capacity of 2GW, making it the highest token-output single-building AI data center globally. Over 80% of its electricity comes from green sources, and it leverages Ulanqab&\#x27;s status as a national &quot;East Data West Computing&quot; hub with 4.2ms data transmission latency to Beijing and electricity costs roughly 50% lower than the Beijing-Tianjin-Hebei region. The facility is the first flagship project under Envision&\#x27;s &quot;Gobi Mission&quot; initiative, intended to deliver a replicable model for domestic computing clusters.

telegram · zaihuapd · Aug 9, 05:06

**「Background」** China&\#x27;s &quot;East Data West Computing&quot; policy aims to relocate data processing to energy-rich western regions like Inner Mongolia to balance latency, cost, and sustainability. Ulanqab is one of eight national computing hubs, already hosting facilities from companies such as Huawei, Alibaba, Apple, and Kuaishou.

**「Impact」** The launch provides a massive, green-powered compute resource that could accelerate domestic AI model training and deployment, while serving as a replicable blueprint for future large-scale AI infrastructure in China.

**Tags**: `#AI infrastructure`, `#data center`, `#GPU computing`, `#green energy`, `#East Data West Computing`

---

<a id="item-tech-news-2"></a>
### [Shopify replaced Redis with MySQL for inventory reservations–and it scaled](https://shopify.engineering/scaling-inventory-reservations) ⭐️ 8.0/10

Shopify’s engineering team migrated its inventory reservation system from Redis to MySQL, adopting a row-per-unit model that assigns a separate row to each sellable unit. To avoid the performance cost of scanning millions of rows for high-volume items, they maintain a bounded pool of available rows capped at 1,000 per item/location combination. Reservations consume rows from this pool, and a background replenishment process refills it when the pool runs low. This design sidesteps the locking and scaling challenges that plagued the Redis implementation, allowing the system to handle high concurrency without contention.

hackernews · adletbalzhanov · Aug 8, 22:32 · [Discussion](https://news.ycombinator.com/item?id=49226536)

**「Background」** High-volume e-commerce platforms must atomically reserve inventory to prevent overselling. Shopify previously used Redis, an in-memory data store, for its fast read/write performance in reservation handling, but faced challenges with consistency and scaling as concurrency grew. The engineering team migrated the reservation system to MySQL, a relational database, to leverage ACID guarantees and a novel bounded-pool, row-per-unit design that avoids locking contention.

**「Impact」** Organizations building high-concurrency inventory systems can evaluate this MySQL-based bounded-pool row-per-unit approach as a practical alternative to Redis, avoiding complex locking and scaling bottlenecks.

**「Community Discussion」** Some commenters speculated that the blog post was LLM-generated and questioned Shopify’s engineering credibility, while others proposed alternative reservation designs such as deduct-then-return flows. The bounded pool technique was acknowledged as a clever but possibly overengineered solution.

<details><summary>References</summary>
<ul>
<li><a href="https://shopify.engineering/scaling-inventory-reservations">We replaced Redis with MySQL for inventory reservations—and it scaled (2026) - Shopify</a></li>
<li><a href="https://www.hellointerview.com/learn/system-design/in-the-wild/shopify-inventory-reservations">How Shopify Moved Inventory Reservations from Redis to MySQL | Hello Interview System Design in a Hurry</a></li>

</ul>
</details>

**Tags**: `#inventory-systems`, `#mysql`, `#redis`, `#scalability`, `#concurrency`

---

<a id="item-tech-news-3"></a>
### [Generative AI Designs First Viable Novel Bacteriophages](https://www.reddit.com/r/MachineLearning/comments/1vjj4pr/r_generative_design_of_novel_bacteriophages_with/) ⭐️ 8.0/10

Researchers have demonstrated the first generative design of viable bacteriophage genomes using genome language models, successfully creating 16 novel phages with substantial evolutionary novelty. The study employed the frontier models Evo 1 and Evo 2 to generate whole-genome sequences based on the lytic phage ΦX174 template, retaining realistic genetic architectures and a desired host tropism. Experimental validation confirmed the functionality of the AI-generated genomes, marking a landmark achievement in AI-driven synthetic biology by proving that genome-scale language models can produce functional whole-genome designs.

reddit · r/MachineLearning · /u/moschles · Aug 9, 07:11

**「Genome Language Models and Bacteriophage Design」** Genome language models are large language models trained on DNA sequences to predict and generate genetic data. Evo 1 and Evo 2 are frontier models that have been applied to design biological systems, but generating functional whole genomes had remained untested. Bacteriophages are viruses that infect bacteria, and the phage ΦX174 is a well-characterized model organism with a small genome, making it a suitable template for whole-genome generation experiments.

**「Impact」** This work directly demonstrates for synthetic biologists and AI researchers that genome language models can generate functional, full-length phage genomes with experimental validation, opening a path to accelerated phage design for therapeutic and biotechnological applications.

<details><summary>References</summary>
<ul>
<li><a href="https://www.biorxiv.org/content/10.1101/2025.09.12.675911v1">Generative design of novel bacteriophages with genome language models | bioRxiv</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#generative models`, `#synthetic biology`, `#genome language models`, `#bioinformatics`

---

<a id="item-tech-news-4"></a>
### [Tencent&\#x27;s WorkBuddy AI Agent Becomes Strategic Priority, Tops Rivals](https://mp.weixin.qq.com/s/TRUjakoaprGFSYYQB301xw) ⭐️ 7.0/10

Tencent has elevated WorkBuddy, its office AI agent, to one of its highest strategic priorities, with internal sources calling it the third strategic product after QQ and WeChat. According to an Analysys report, WorkBuddy ranked first among domestic office AI platforms with 20.97 million PC monthly visits in Q2 2026, reaching 20 million monthly active users and millions of daily active users. The product integrates with Tencent Docs, WeCom, and Tencent Meeting and supports multiple models including Hunyuan, DeepSeek, and GLM. In July 2025, Tencent moved its QClaw business into the same department, consolidating AI explorations. WorkBuddy remains in an investment phase with no commercialization KPIs, and the focus for the year is on expanding enterprise customer coverage.

telegram · zaihuapd · Aug 8, 13:50

**「Background」** WorkBuddy is a desktop AI office agent launched by Tencent in 2026. It integrates with Tencent&\#x27;s ecosystem of productivity apps, including WeCom, Tencent Docs, and Tencent Meeting, and supports multiple large language models such as Hunyuan, DeepSeek, and GLM. The agent can autonomously execute complex tasks through multi-agent parallelism and skill extensions.

**「Impact」** Enterprise users of Tencent&\#x27;s ecosystem will gain a deeply integrated, multi-model AI assistant with no immediate pressure for monetization, potentially accelerating adoption and feature development within the widely used productivity suite.

<details><summary>References</summary>
<ul>
<li><a href="https://www.codebuddy.cn/work/">WorkBuddy - AI Agent 办 公 新范式</a></li>
<li><a href="https://www.pai.com.cn/p/01kk8t0p3tf9tem36es6dy989p">腾 讯 旗下全场景AI 智 能 体 WorkBuddy 正式上线 - 电商派</a></li>
<li><a href="https://www.leavescn.com/Articles/Content/3875">WorkBuddy 是什么？ 腾 讯 版OpenClaw AI 办 公 助手全面解析</a></li>

</ul>
</details>

**Tags**: `#AI products`, `#Tencent`, `#office agents`, `#Chinese tech`, `#enterprise AI`

---

<a id="item-tech-news-5"></a>
### [Elon Musk Unveils SpaceX Lunar Factory Plan for AI Satellites](https://finance.yahoo.com/technology/articles/pure-insanity-elon-musk-details-173635969.html) ⭐️ 7.0/10

SpaceX CEO Elon Musk announced a plan to build a fully automated factory on the Moon, using Starship rockets to deliver robotic equipment that would extract aluminum, titanium, and silicon from lunar soil. The factory would mass-produce AI computing satellites and launch them directly into orbit via an electromagnetic mass driver. The proposal faces extreme lunar conditions including abrasive dust, temperature swings, and two-week cycles of daylight and darkness. Former SpaceX VP Jim Cantrell called the plan “pure insanity” but expressed confidence in Musk’s ability to execute, while industry observers acknowledge its technical feasibility yet note Musk’s typically optimistic timelines. The announcement came during SpaceX’s first public earnings call, where the company reported $7.8 billion in quarterly revenue and a $205 million loss in its space division due to Starship development.

telegram · zaihuapd · Aug 9, 05:37

**「Background」** SpaceX recently became a public company, and Elon Musk unveiled the lunar factory plan during its first earnings call. The plan relies on Starship to deliver equipment to the Moon, and it builds on long-standing concepts of in-situ resource utilization and electromagnetic launch systems to send payloads from the lunar surface into orbit.

**「Impact」** If successful, the lunar factory could shift satellite manufacturing off Earth, potentially reducing launch costs and enabling faster deployment of AI satellites, but the plan remains highly speculative and faces immense technical and environmental challenges.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eweek.com/news/spacex-robots-moon-factories/">SpaceX Envisions Robots Building AI Satellite Factories on... | eWeek</a></li>
<li><a href="https://www.futura-sciences.com/en/elon-musk-plans-a-moon-factory-with-an-electromagnetic-catapult-to-launch-ai-satellites_25836/">Elon Musk plans a Moon factory with an... - Futura-Sciences</a></li>

</ul>
</details>

**Tags**: `#spacex`, `#lunar-factory`, `#ai-satellites`, `#robotics`, `#space-manufacturing`

---

<a id="item-tech-news-6"></a>
### [MiniMax H3 Team Reveals Plans to Open-Source 2K Model and Sparse Attention](https://www.reddit.com/r/StableDiffusion/s/fjM3d7AEV8) ⭐️ 7.0/10

During a Reddit AMA in r/StableDiffusion, the MiniMax H3 team announced plans to open-source H3-Regenerate-2K, a dedicated latent-space DiT regeneration model for high-resolution generation \(not a standard upscaler\), though no release date was provided. A sparse attention reference implementation is expected soon, with a goal of no perceptible quality loss. The team is also considering a 4/8-step low-step-count version and plans to derive a standalone image generation model from the H3 model lineage. Issues with Ref2VA quality degradation and texture blurriness reported by the community are being actively addressed.

telegram · zaihuapd · Aug 9, 08:28

**「Background」** MiniMax H3 is an open-source video generation model released by MiniMax, whose initial public weights output 768p video. The sparse-attention mechanism was not included in that release, and for 2K resolution, the team plans to offer a dedicated latent-space DiT regeneration model rather than a conventional super-resolution module.

**「Impact」** Developers and researchers in the video generation community will eventually gain access to a high-resolution regeneration model and a reference sparse attention implementation, but the lack of specific release dates means no immediate integration is possible.

<details><summary>References</summary>
<ul>
<li><a href="https://www.minimax.io/news/minimax-h3-open-source">Open General Intelligence: MiniMax H3 Is Now Open Source - MiniMax News | MiniMax</a></li>

</ul>
</details>

**Tags**: `#video generation`, `#open source`, `#sparse attention`, `#MiniMax`, `#AMA`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Berkshire Hathaway Q2 earnings up 16%, new CEO Abel starts deploying cash](https://www.cnbc.com/2026/08/08/berkshire-hathaway-earnings-q2-2026.html) ⭐️ 7.0/10

Berkshire Hathaway&\#x27;s operating earnings rose 16% to $12.98 billion in Q2 2026, and CEO Greg Abel accelerated share buybacks to $4.5 billion and made nearly $20 billion in net equity purchases, reversing a 14-quarter streak of selling stocks.

rss · CNBC Finance · Aug 8, 13:28

**「Background」** Abel took over from Warren Buffett at the start of 2026 after Buffett had built a record cash hoard of $397.4 billion and sold stocks for 14 consecutive quarters.

**Tags**: `#Berkshire Hathaway`, `#earnings`, `#share buybacks`, `#Greg Abel`, `#equity purchases`

---

<a id="item-finance-news-2"></a>
### [US Court Temporarily Blocks Pentagon Blacklist of WuXi AppTec](https://np-info.eastmoney.com/wap/notice/?referrer=appShare&amp;amp;infocode=AN202608091827791183) ⭐️ 7.0/10

A US federal court granted a preliminary injunction on August 7, 2026, temporarily blocking enforcement of a Pentagon blacklist that had designated WuXi AppTec as a Chinese military company, shielding the biotech firm from immediate contract bans.

telegram · zaihuapd · Aug 9, 10:13

**「Background」** The Department of Defense added WuXi AppTec to its 1260H list of Chinese military companies in June 2026, a move that would have prohibited the Pentagon from contracting with the firm and, starting in 2027, from buying its products through third parties.

**Tags**: `#biotech`, `#US-China`, `#legal`, `#trade-restrictions`, `#corporate`

---