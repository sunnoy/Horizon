---
layout: default
title: "Horizon Summary: 2026-08-07 (EN)"
date: 2026-08-07
lang: en
---

> From 43 items, 13 important content pieces were selected

---

**Technology News**
1. [AMD acquires Taalas to boost inference performance by etching models in silicon](#item-tech-news-1) ⭐️ 8.0/10
2. [Datasette 1.0a38 fixes SQL injection in mixed-permission databases](#item-tech-news-2) ⭐️ 8.0/10
3. [OpenAI Introduces Agent Plugins Open Standard on GPT-5’s First Anniversary](#item-tech-news-3) ⭐️ 8.0/10
4. [US Reviews China&\#x27;s Offshore Nvidia Chip Access](#item-tech-news-4) ⭐️ 8.0/10
5. [Taste Is All That&\#x27;s Left](#item-tech-news-5) ⭐️ 7.0/10
6. [GitHub Actions and Pages Outage Amid AI-Generated Commit Surge](#item-tech-news-6) ⭐️ 7.0/10
7. [Alibaba to Charge Large Users for Qwen Open-Source AI Model](#item-tech-news-7) ⭐️ 7.0/10
8. [SK Hynix Confirms 375-Layer V10 NAND with Wafer Bonding](#item-tech-news-8) ⭐️ 7.0/10

**Financial News**
1. [Copper futures reach record $6.90 a pound after Congo bans exports](#item-finance-news-1) ⭐️ 8.0/10
2. [Nasdaq’s 23-Hour Trading Day Approved by SEC, Starts December 6, 2026](#item-finance-news-2) ⭐️ 8.0/10
3. [Chevrolet Ends Chinese Retail Sales After 21 Years, Shifts to Export Manufacturing](#item-finance-news-3) ⭐️ 8.0/10
4. [After-hours earnings moves: Trade Desk drops 22%, Twilio jumps 16%](#item-finance-news-4) ⭐️ 7.0/10
5. [United Wholesale Mortgage Sinks 35% After Dividend Suspension and Capital Raise](#item-finance-news-5) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [AMD acquires Taalas to boost inference performance by etching models in silicon](https://www.theregister.com/systems/2026/08/06/amd-acquires-ai-chip-startup-taalas-to-boost-inference-performance-by-etching-models-into-silicon/5284344) ⭐️ 8.0/10

AMD has acquired Taalas, a startup that develops technology to embed AI models directly into silicon, aiming to dramatically improve inference performance and energy efficiency. The move could commoditize high-speed, low-power AI inference, enabling large language models to run on edge devices such as cars, appliances, and robotics with battery-level power consumption. By etching models into silicon, the approach promises to replicate the historical integration of video decoding hardware, making real-time AI a standard feature and potentially challenging NVIDIA&\#x27;s GPU-centric dominance in the AI hardware market.

hackernews · itvision · Aug 6, 20:23 · [Discussion](https://news.ycombinator.com/item?id=49201970)

**「Background」** Taalas is a startup that bakes AI model weights directly into silicon, a process that can boost inference performance by an order of magnitude or more. AMD plans to integrate this technology into its product roadmap, including with its Instinct GPUs, to differentiate its AI hardware offerings.

**「Impact」** If successfully commercialized, AMD&\#x27;s acquisition of Taalas could enable silicon-embedded AI inference that delivers high performance at low power, directly undercutting NVIDIA&\#x27;s GPU-based solutions and accelerating the deployment of AI in edge devices from robotics to consumer electronics.

**「Community Discussion」** Commenters view the acquisition as a step toward commoditizing AI inference, comparing it to the integration of video decoding into silicon, and expect it to enable real-time AI in robotics, cars, and appliances, with some noting that it could undercut NVIDIA&\#x27;s market position. Several expressed surprise that firms like OpenAI or Anthropic did not make a similar move first, and enthusiasm for the prospect of dense models running at tens of thousands of tokens per second on edge devices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theregister.com/systems/2026/08/06/amd-acquires-ai-chip-startup-taalas-to-boost-inference-performance-by-etching-models-into-silicon/5284344">AMD acquires AI chip startup Taalas to boost inference performance...</a></li>
<li><a href="https://ir.amd.com/news-events/press-releases/detail/1296/amd-acquires-taalas-to-advance-compute-solutions-for-rapidly-growing-ai-inference-market">AMD Acquires Taalas to Advance Compute Solutions for Rapidly...</a></li>

</ul>
</details>

**Tags**: `#hardware`, `#ai`, `#inference`, `#acquisition`, `#silicon`

---

<a id="item-tech-news-2"></a>
### [Datasette 1.0a38 fixes SQL injection in mixed-permission databases](https://simonwillison.net/2026/Aug/6/datasette/#atom-everything) ⭐️ 8.0/10

Datasette 1.0a38 patches a SQL injection vulnerability that allowed read-only access to private tables in databases configured with a mix of public and private tables using the Datasette permissions system. The bug let users with access to any public table bypass the disabled execute-sql permission, executing SQL injection attacks to view data in private tables of the same database. The fix is also backported to Datasette 0.65.3. The affected configuration—serving public and private tables from the same database within one instance—is likely rare, according to the project maintainer.

rss · Simon Willison · Aug 6, 18:24

**「Background」** Datasette is an open-source tool for exploring and publishing SQLite databases, with a permissions system that can restrict access to specific tables and the ability to run raw SQL queries via the execute-sql permission. SQL injection is a common attack where malicious SQL statements are inserted into input fields to manipulate database queries. In this case, a flaw in Datasette’s handling of SQL queries allowed injection even when the execute-sql permission was explicitly disabled.

**「Impact」** Site administrators running Datasette instances that serve both public and private tables in the same database must upgrade to 1.0a38 or 0.65.3 and keep the execute-sql permission disabled to prevent attackers from reading private data via SQL injection.

**Tags**: `#security`, `#datasette`, `#sql injection`, `#open source`, `#release`

---

<a id="item-tech-news-3"></a>
### [OpenAI Introduces Agent Plugins Open Standard on GPT-5’s First Anniversary](https://9to5mac.com/2026/08/06/gpt-5-turning-one-as-openai-shares-new-agent-plugins-standard/) ⭐️ 8.0/10

On the eve of GPT-5’s first anniversary, OpenAI announced Agent Plugins, an open, vendor-neutral standard for packaging agent skills and MCP servers into portable plugins. The specification is developed openly under a steering committee that includes Amazon, Cursor, Microsoft, OpenAI, and Vercel, enabling compatible clients to uniformly discover and load agent capabilities. This move aims to improve AI agent interoperability across platforms and tools. GPT-5 has seen rapid iteration over the past year, with versions up to 5.6, while GPT-6 remains unannounced.

telegram · zaihuapd · Aug 7, 00:46

**「Background」** GPT-5, OpenAI&\#x27;s language model that replaced GPT-4o as ChatGPT&\#x27;s default, launched on August 7, 2025, and has since been integrated into Apple Intelligence. The new Agent Plugins standard aims to package AI agent skills and MCP \(Model Context Protocol\) servers into a portable format that can be discovered and loaded by compatible clients, with a steering committee that includes Amazon, Cursor, Microsoft, and Vercel.

**「Impact」** Software engineers and AI practitioners can expect more consistent agent tooling and easier integration across different platforms, as the open standard backed by major tech companies reduces fragmentation.

<details><summary>References</summary>
<ul>
<li><a href="https://9to5mac.com/2026/08/06/gpt-5-turning-one-as-openai-shares-new-agent-plugins-standard/">GPT-5 turning one as OpenAI shares new Agent Plugins standard</a></li>
<li><a href="https://thenextweb.com/news/openai-agent-plugins-open-standard-skills-mcp">OpenAI and four rivals just agreed on one standard for AI agents</a></li>

</ul>
</details>

**Tags**: `#GPT-5`, `#OpenAI`, `#Agent Plugins`, `#open standard`, `#AI ecosystem`

---

<a id="item-tech-news-4"></a>
### [US Reviews China&\#x27;s Offshore Nvidia Chip Access](https://www.bloomberg.com/news/articles/2026-08-07/us-reviews-china-s-offshore-access-to-nvidia-chips-after-ai-breakthroughs) ⭐️ 8.0/10

The US Commerce Department&\#x27;s Bureau of Industry and Security \(BIS\) is systematically reviewing how Chinese AI companies obtain and use Nvidia chips overseas, including through remote computing rentals and shell companies. The review includes compiling a list of black-market countries for smuggled chips and a list of countries where Chinese firms remotely rent compute. The investigation was triggered after AI startup Moonshot AI released its Kimi K3 model, which a White House official claimed illegally accessed Nvidia chips via Thailand, and separate revelations that Alibaba used a Cayman Islands entity and a Singapore shell company to access Nvidia chips in Malaysia through a firm under US investigation. While remote access itself is not illegal, the BIS is exploring whether it can restrict such cloud computing arrangements, and a bipartisan House bill aims to grant that authority despite expected opposition from Nvidia and other tech companies.

telegram · zaihuapd · Aug 7, 11:18

**「Background」** US export controls have long restricted the sale of advanced AI chips to China, but Chinese firms have found workarounds by smuggling hardware or renting cloud computing capacity in third countries. The BIS is the agency responsible for enforcing these controls, and its authority over remote computing services remains legally ambiguous. The recent release of Moonshot AI&\#x27;s Kimi K3, which approached the performance of leading US models, intensified concerns that Chinese AI development is advancing despite the restrictions.

**「Impact」** The investigation could lead to new restrictions on remote cloud access to Nvidia chips, potentially disrupting Chinese AI companies&\#x27; ability to scale advanced models like Kimi K3.

**Tags**: `#AI`, `#hardware`, `#export controls`, `#Nvidia`, `#US-China`

---

<a id="item-tech-news-5"></a>
### [Taste Is All That&\#x27;s Left](https://notashelf.dev/posts/taste-is-all-thats-left) ⭐️ 7.0/10

A reflective essay argues that taste is the last human differentiator in the age of AI-generated content, sparking a Hacker News discussion. The conversation explores taste as a guiding principle for building coherent AI systems, with some commenters asserting that taste forms the necessary guardrails for reliable outputs, while others question whether AI writing can ever carry meaningful signal. The essay&\#x27;s own style and contradictions become a point of contention, as one commenter points out the tension between the author&\#x27;s distinctive short sentences and the stated intention to write plainer in the future. Overall, the piece and responses highlight the ongoing debate about authenticity and human judgment in AI-assisted creation.

hackernews · tsak · Aug 6, 17:01 · [Discussion](https://news.ycombinator.com/item?id=49199346)

**「Background」** The essay by notashelf argues that in an era where generative AI can produce code and text with ease, the primary challenge shifts from creation to curation, making taste—the ability to discern quality—the essential human skill. It draws on philosophical ideas, such as Harry Frankfurt’s concept of &\#x27;bullshit&\#x27; and Sturgeon’s Law, to underscore that taste involves judgment and intentionality, not just technical ability.

**「Community Discussion」** Commenters are divided: some emphasize taste as a set of rules that accumulate over time to narrow AI paths and produce user-trustworthy systems, while others express skepticism that large language models can produce writing with real signal, noting contradictions in the essay&\#x27;s own stance on authorial voice and plain writing.

<details><summary>References</summary>
<ul>
<li><a href="https://notashelf.dev/posts/taste-is-all-thats-left">Taste Is All That&#x27;s Left | Blog - notashelf.dev</a></li>
<li><a href="https://dev.to/trismegistus/when-ai-writes-all-the-code-whats-left-for-developers-the-case-for-taste-980">When AI Writes All the Code, What&#x27;s Left for Developers? The ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#writing`, `#taste`, `#generative-AI`, `#philosophy`

---

<a id="item-tech-news-6"></a>
### [GitHub Actions and Pages Outage Amid AI-Generated Commit Surge](https://www.githubstatus.com/incidents/qcvjkzcs7j74) ⭐️ 7.0/10

GitHub Actions and Pages are experiencing a significant outage that has lasted over five hours, leaving workflows unable to run even for self-hosted runners because the scheduling API is unavailable. The incident highlights mounting scaling challenges as the platform faces a massive surge in AI-generated code, with commits now reaching 275 million per week—on pace for 14 billion this year—and Actions minutes growing from 500 million per week in 2023 to 2.1 billion this week. Users report that GitHub&\#x27;s reliability has declined sharply over the past year, with frequent outages eroding trust in the service.

hackernews · Footkerchief · Aug 6, 15:49 · [Discussion](https://news.ycombinator.com/item?id=49198302)

**「Background」** GitHub Actions is a continuous integration and delivery service that executes automated workflows, while GitHub Pages hosts static websites directly from repositories. The platform has experienced an unprecedented increase in activity, driven by the widespread adoption of AI coding assistants that generate large volumes of commits, pushing weekly commit counts to 275 million and weekly Actions minutes to 2.1 billion. This rapid growth is straining GitHub&\#x27;s infrastructure, contributing to more frequent and severe outages.

**「Impact」** The outage prevents developers and organizations from running CI/CD pipelines and deploying static sites, directly blocking software releases, testing, and updates for those who depend on GitHub&\#x27;s hosted services.

**「Community Discussion」** The community reaction is overwhelmingly critical, with users emphasizing that even self-hosted runners are non-functional due to the API outage and attributing the recent spate of failures to GitHub&\#x27;s inability to scale amid the surge in AI-generated commits, with some calling the platform&\#x27;s reliability into question and suggesting the company has lost respect for its customers.

**Tags**: `#GitHub`, `#outage`, `#CI/CD`, `#scaling`, `#AI-generated code`

---

<a id="item-tech-news-7"></a>
### [Alibaba to Charge Large Users for Qwen Open-Source AI Model](https://www.reuters.com/business/retail-consumer/alibaba-plans-charge-big-users-its-next-open-source-ai-model-sources-say-2026-08-07/) ⭐️ 7.0/10

Alibaba plans to introduce a revenue-sharing fee for large commercial users of its upcoming Qwen open-source AI model, according to sources cited by Reuters. Previously, the company only charged for model usage on its cloud platform and allowed free deployment on customers&\#x27; own data centers. The new licensing model mirrors the terms set by Chinese AI startup Moonshot for its Kimi K3 model, which requires service providers with annual revenue exceeding $20 million to enter a commercial agreement, reportedly with a revenue share of up to 30%. The precise revenue share for Qwen is still under discussion as Chinese AI companies accelerate the formation of business models to capture market share from U.S. competitors.

telegram · zaihuapd · Aug 7, 01:29

**「Background」** Open-source AI models are typically released under permissive licenses that allow free use, modification, and deployment, including in commercial settings. Alibaba previously followed this norm with its Qwen models, offering them for free self-deployment while monetizing only through its cloud hosting services. The shift to revenue sharing for large commercial users represents a departure from that practice, similar to dual-licensing or open-core models seen in the software industry.

**「Impact」** Large enterprises that deploy Alibaba&\#x27;s new Qwen model on their own infrastructure will face a new revenue-sharing obligation, potentially increasing the total cost of ownership and influencing build-vs-buy decisions for AI services. The exact financial impact remains uncertain as the share percentage is still being negotiated.

**Tags**: `#Alibaba`, `#Qwen`, `#open-source`, `#licensing`, `#AI business model`

---

<a id="item-tech-news-8"></a>
### [SK Hynix Confirms 375-Layer V10 NAND with Wafer Bonding](https://www.gelonghui.com/live/2599953) ⭐️ 7.0/10

SK Hynix, in its FMS 2026 press release, confirmed that its next-generation V10 NAND flash uses 375-layer stacking, marking the first adoption of wafer bonding technology in the company’s NAND products. This follows the 321-layer V9 “4D NAND,” and SK Hynix claims the V10 delivers 2.5× the per-watt performance of its predecessor. The design is optimized for AI infrastructure environments that demand both high energy efficiency and robust performance. The announcement highlights a continued push toward higher-density, more power-efficient storage for data-intensive workloads.

telegram · zaihuapd · Aug 7, 12:19

**「Background」** 3D NAND flash memory stacks memory cells vertically to increase density, and manufacturers are competing to add more layers. SK hynix’s current V9 generation uses 321 layers; the upcoming V10 will have 375 layers and is expected to enter mass production in early 2027. It is SK hynix’s first NAND product to adopt wafer bonding, a technique that bonds two separately fabricated wafers to surpass the layer limits of traditional monolithic stacking.

**「Impact」** AI infrastructure builders may benefit from significantly improved energy efficiency per storage operation, though the 2.5× per-watt claim awaits independent verification.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ajupress.com/view/20260805101311102">Samsung, SK hynix wage next battle for AI memory... | Aju Press</a></li>
<li><a href="https://www.trendforce.com/news/2026/08/05/news-samsung-unveils-industry-first-400-layer-v10-bv-nand-memory-density-up-58-vs-v9/">[News] Samsung Unveils Industry-First 400+ Layer V 10 BV- NAND ...</a></li>

</ul>
</details>

**Tags**: `#NAND`, `#flash memory`, `#semiconductor`, `#AI infrastructure`, `#hardware`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Copper futures reach record $6.90 a pound after Congo bans exports](https://www.cnbc.com/2026/08/06/copper-jumps-to-its-highest-level-ever-what-the-metal-is-telling-us-.html) ⭐️ 8.0/10

U.S. copper futures hit a record high of about $6.90 a pound on Thursday after the Democratic Republic of Congo officially banned exports of copper and cobalt concentrates.

rss · CNBC Finance · Aug 6, 20:07

**「Background」** Copper is a metal used in construction, electronics, and power grids, and its price has traditionally been seen as a signal of global economic growth. However, analysts say the current rally is driven more by supply constraints—such as mine disruptions in Chile and the Congo export ban—and demand from AI data centers and electrification rather than a broad economic boom.

**Tags**: `#copper prices`, `#supply disruptions`, `#electrification demand`, `#economic indicators`, `#commodities`

---

<a id="item-finance-news-2"></a>
### [Nasdaq’s 23-Hour Trading Day Approved by SEC, Starts December 6, 2026](https://finance.sina.com.cn/stock/bxjj/2026-08-07/doc-inimnkup0012339.shtml) ⭐️ 8.0/10

The U.S. Securities and Exchange Commission approved Nasdaq’s plan for a 23-hour trading day, launching December 6, 2026, with the market closing only from 8 p.m. to 9 p.m. Eastern Time for system maintenance.

telegram · zaihuapd · Aug 7, 10:03

**「Background」** The approval follows similar extended-hours plans from NYSE Arca and Cboe, and comes as retail investors already trade overnight through alternative trading systems, though these sessions have lower liquidity and wider spreads.

**Tags**: `#SEC`, `#Nasdaq`, `#trading hours`, `#market regulation`, `#extended trading`

---

<a id="item-finance-news-3"></a>
### [Chevrolet Ends Chinese Retail Sales After 21 Years, Shifts to Export Manufacturing](https://m.mydrivers.com/newsview/1142126.html) ⭐️ 8.0/10

SAIC-GM announced that Chevrolet will stop selling new cars to Chinese consumers, ending a 21-year retail presence, after annual sales collapsed to 52,000 units in 2025 from a peak of 600,000. Its Chinese factories will now produce vehicles for export.

telegram · zaihuapd · Aug 7, 11:12

**「Background」** Chevrolet’s sales had been declining as Chinese buyers increasingly chose domestic electric vehicle brands over joint-venture gasoline models.

**「Impact」** Current owners can still access after-sales service through Buick authorized dealerships, and the SAIC-GM joint venture remains in place until 2047.

**Tags**: `#automotive industry`, `#China market`, `#brand exit`, `#General Motors`, `#electric vehicles`

---

<a id="item-finance-news-4"></a>
### [After-hours earnings moves: Trade Desk drops 22%, Twilio jumps 16%](https://www.cnbc.com/2026/08/06/stocks-making-the-biggest-moves-after-hours-sg-abnb-dkng-ttd.html) ⭐️ 7.0/10

Trade Desk shares fell 22% after the digital advertising company reported second-quarter adjusted earnings of 34 cents per share and revenue of $715 million, missing LSEG consensus estimates of 40 cents and $751 million. Twilio shares surged 16% after the company issued third-quarter guidance for adjusted earnings of $1.42 to $1.47 per share on revenue of $1.51 billion to $1.52 billion, above the LSEG consensus of $1.39 per share and $1.46 billion.

rss · CNBC Finance · Aug 6, 21:53

**「Background」** The moves occurred in after-hours trading after several companies released second-quarter earnings results that diverged from analyst expectations compiled by LSEG.

**Tags**: `#earnings`, `#after-hours trading`, `#stocks`, `#market movers`, `#technology`

---

<a id="item-finance-news-5"></a>
### [United Wholesale Mortgage Sinks 35% After Dividend Suspension and Capital Raise](https://www.cnbc.com/2026/08/06/united-wholesale-mortgage-plunges-40percent-suspends-dividend-raises-capital-.html) ⭐️ 7.0/10

United Wholesale Mortgage shares plunged 35% after the lender suspended its dividend, raised $2.05 billion in equity capital, and reported a $451.9 million quarterly loss.

rss · CNBC Finance · Aug 6, 20:37

**「Background」** Mortgage lenders are operating in a challenging environment as elevated mortgage rates, tied to higher Treasury yields, keep homebuyers on the sidelines and limit refinancing activity.

**Tags**: `#mortgage industry`, `#capital raise`, `#dividend suspension`, `#earnings loss`, `#housing market`

---