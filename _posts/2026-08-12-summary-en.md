---
layout: default
title: "Horizon Summary: 2026-08-12 (EN)"
date: 2026-08-12
lang: en
---

> From 48 items, 12 important content pieces were selected

---

**Technology News**
1. [Researchers Extract Proprietary LLM Reasoning by Replaying Encrypted Traces](#item-tech-news-1) ⭐️ 10.0/10
2. [Gemini App Hits 1 Billion Monthly Active Users, Fastest-Growing Google Product](#item-tech-news-2) ⭐️ 8.0/10
3. [LTX-2.5 Open-Source Video Model: Runs on Single RTX 5090 with Free Commercial License](#item-tech-news-3) ⭐️ 8.0/10
4. [xAI&\#x27;s Grok Bot: Autonomous AI Agents for Browser Tasks](#item-tech-news-4) ⭐️ 7.0/10
5. [Decoupled Descent Uses AMP to Enforce Exact Train-Test Error Tracking](#item-tech-news-5) ⭐️ 7.0/10
6. [Nvidia Developing Nemotron 4 Open-Source Model with 1 Trillion Parameters](#item-tech-news-6) ⭐️ 7.0/10
7. [Enterprise SSD Share Hits 48% of NAND; YMTC Joins Top Three](#item-tech-news-7) ⭐️ 7.0/10

**Financial News**
1. [Nvidia&\#x27;s $500 billion AI financing plan faces depreciation risk from China](#item-finance-news-1) ⭐️ 9.0/10
2. [CME to Launch First-Ever Futures on AI Computing Power](#item-finance-news-2) ⭐️ 9.0/10
3. [Former Chinese Premier Zhu Rongji Dies at 98](#item-finance-news-3) ⭐️ 9.0/10
4. [EVs reach 65.1% of new car sales in China, led by Geely, Tesla, and BYD](#item-finance-news-4) ⭐️ 8.0/10
5. [Tencent Q2 Revenue Beats, Net Profit Misses; Capex Surge Turns Free Cash Flow Negative](#item-finance-news-5) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Researchers Extract Proprietary LLM Reasoning by Replaying Encrypted Traces](https://simonwillison.net/2026/Aug/11/stealing-reasoning-traces/#atom-everything) ⭐️ 10.0/10

A new research paper reveals that encrypted chain-of-thought reasoning traces from Anthropic, OpenAI, and Google frontier models can be stolen by replaying the encrypted blocks into a weaker sibling model and jailbreaking it to output the plaintext. The attack works because all models in a family shared the same encryption key, allowing traces to be replayed across sessions, users, and models. The authors demonstrated the technique on Claude Haiku 4.5 using a prompt that asked for verbatim transcription and a prefilled assistant response, and they also uncovered a variant where malicious instructions hidden in reasoning traces can manipulate downstream models. The paper includes extensive examples of extracted reasoning, showing raw, human-unreadable thought processes. The vulnerability has since been fixed by all affected providers.

rss · Simon Willison · Aug 11, 22:40

**「Background」** Many frontier large language models now use chain-of-thought reasoning to improve answer quality, and providers typically encrypt those internal reasoning steps before returning them to users to prevent inspection. The encrypted blocks are opaque and intended to be private, but the paper shows that because the encryption key is shared across an entire model family, the blocks can be fed into a different, weaker model that can be jailbroken to decrypt them.

**「Impact」** The attack allowed unauthorized access to proprietary reasoning, potentially exposing sensitive internal decision-making, and enabled prompt injection via reasoning traces, though providers have already patched the vulnerability.

**「Community Discussion」** Commenters debated whether extracting reasoning constitutes &\#x27;stealing,&\#x27; noting that LLM outputs lack copyright protection in some jurisdictions, while others saw transparency as a valuable security feature. Some also pointed out that the extracted traces confirm models are trained on problem answers and may have indexed knowledge of benchmarks.

**Tags**: `#large-language-models`, `#security`, `#chain-of-thought`, `#privacy`, `#AI-safety`

---

<a id="item-tech-news-2"></a>
### [Gemini App Hits 1 Billion Monthly Active Users, Fastest-Growing Google Product](https://blog.google/innovation-and-ai/products/gemini-app/one-billion-monthly-users/) ⭐️ 8.0/10

Google&\#x27;s Gemini app has surpassed 1 billion monthly active users, making it the fastest-growing product in the company&\#x27;s history. 63% of users interact via voice, and the app generates over 150 million images daily. iOS has more than 100 million active users, while macOS power users ask questions at roughly twice the rate of other platforms. One in five Gemini Live interactions extend beyond voice, using the camera or screen sharing to solve problems in real time. On Android, Gemini can automate tasks across more than 40 apps, and 38% of student requests include attachments, highlighting strong multimodal and educational adoption.

telegram · zaihuapd · Aug 12, 00:45

**「Background」** Gemini is Google&\#x27;s family of AI models and the underlying assistant powering the Gemini app, launched in late 2023 as a direct competitor to OpenAI&\#x27;s ChatGPT and other large language model assistants. The app integrates with Google&\#x27;s ecosystem, including Android, iOS, and web, and offers multimodal capabilities such as voice, image generation, and real-time collaboration through camera and screen sharing.

**「Impact」** The milestone signals that Google&\#x27;s AI strategy is gaining significant user traction, with deep engagement patterns—especially voice and multimodal use—that could pressure competitors and accelerate integration of Gemini across Google&\#x27;s products and services.

**Tags**: `#Google`, `#Gemini`, `#AI adoption`, `#monthly active users`, `#product milestone`

---

<a id="item-tech-news-3"></a>
### [LTX-2.5 Open-Source Video Model: Runs on Single RTX 5090 with Free Commercial License](https://ltx.io/model/ltx-2-5) ⭐️ 8.0/10

LTX has released LTX-2.5, an open-source video generation model with full weights, training code, and inference pipeline, designed to run locally on a single RTX 5090 GPU. It supports text-to-video and image-to-video, and incorporates improved multi-shot coherence, a new diffusion video decoder, and the Gemma 4 12B text encoder. Available under a free commercial license for entities with annual revenue below $10 million, the model ranked first in a 98-prompt video-defect benchmark among ten tested models.

telegram · zaihuapd · Aug 12, 02:15

**「Background」** LTX previously released LTX-2, an open-source text-to-video model that was the first of its kind trained on Google Cloud infrastructure. The new LTX-2.5 is a major update released as an open-source foundation model, with full access to weights, training code, and inference pipeline, enabling local execution on consumer GPUs.

**「Impact」** Individual developers and small studios can generate video locally on a single high-end consumer GPU, avoiding cloud costs and benefiting from permissive commercial terms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LTX_%28text-to-video_model%29">LTX (text-to-video model) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI视频生成`, `#开源模型`, `#LTX-2.5`, `#文生视频`, `#本地运行`

---

<a id="item-tech-news-4"></a>
### [xAI&\#x27;s Grok Bot: Autonomous AI Agents for Browser Tasks](https://x.ai/bot) ⭐️ 7.0/10

xAI has announced Grok Bot, a system of autonomous AI agents that can manage browser tasks and user credentials by running continuously on a dedicated cloud computer. Currently in beta, Grok Bot is available to subscribers of SuperGrok Heavy, Cursor Ultra, and Cursor Teams Premium, supporting desktop and iOS platforms. The agents can log into user accounts, complete tasks across apps and websites, and only request user approval for critical actions, while maintaining their own routines, context, and domain and communicating between agents. Early users describe it as a natural evolution from prompts to agents, but the release also raises significant security concerns due to the agents&\#x27; access to credentials. The announcement signals a shift toward persistent, autonomous AI assistants, with potential implications for privacy and trust.

hackernews · rvz · Aug 11, 17:23 · [Discussion](https://news.ycombinator.com/item?id=49261514)

**「Background」** Grok Bot, announced by xAI on August 11, 2026, is a team of always-on AI agents that run on a persistent cloud virtual machine with their own browser, filesystem, and terminal. Unlike conventional chatbots that respond only when prompted, these agents work continuously across tools and apps, handling tasks without user intervention unless approval is required. This represents a step in the evolution from simple prompts to autonomous agents, as seen in the shift from tab completion to prompt-based AI and now to persistent, domain-specific agents.

**「Impact」** The release of Grok Bot directly offers users of the supported subscription tiers a new capability to deploy persistent AI agents that can automate account management and cross-application tasks, potentially increasing productivity but also requiring them to trust xAI with their credentials and exposing them to risks such as credential leaks and prompt injection attacks.

**「Community Discussion」** Early users like jjcm found the multi-agent communication natural and promising, viewing it as a next step in AI evolution, but many commenters expressed serious concerns about security, including the risk of credential theft, constant agent access, and vulnerability to prompt injection. Others questioned the necessity of such agents or called for stronger open-source models to avoid dependence on a single vendor.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.x.ai/grok-bot/overview">Grok Bot | SpaceXAI Docs</a></li>
<li><a href="https://x.ai/news/introducing-grok-bot">Introducing Grok Bot | SpaceXAI</a></li>
<li><a href="https://www.oflight.co.jp/en/columns/grok-bot-xai-always-on-agents-2026">Grok Bot Explained: xAI&#x27;s Always-On AI Agent Teammates</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#grok`, `#xai`, `#automation`, `#security`

---

<a id="item-tech-news-5"></a>
### [Decoupled Descent Uses AMP to Enforce Exact Train-Test Error Tracking](https://www.reddit.com/r/MachineLearning/comments/1vlu1se/decoupled_descent_enforcing_exact_traintest_error/) ⭐️ 7.0/10

A new theoretical paper proposes Decoupled Descent, a training method that uses approximate message passing \(AMP\) to guarantee that a neural network&\#x27;s training error asymptotically equals its test error at each parameter iterate. The authors frame the train-test error gap as a consequence of data reuse bias in full-batch gradient descent and demonstrate the method on a stylized high-dimensional XOR Gaussian mixture model with a two-layer network. Across 100 simulations, Decoupled Descent produced train-test error curves that closely track each other, in contrast to the divergence seen with standard gradient descent. The work is presented as a first step toward generalizing the approach to SGD and larger models, and the author plans to release a PyTorch-compatible package.

reddit · r/MachineLearning · /u/mlovik1 · Aug 11, 21:06

**「Background」** In neural network training, gradient descent can drive training error to zero while test error remains high or increases, a hallmark of overfitting. Approximate message passing is a high-dimensional statistical technique originally developed for compressed sensing and inference problems, enabling precise tracking of algorithmic dynamics in certain model classes.

**「Impact」** The method provides a theoretical certificate of equal train-test error in the studied settings, which could inform optimal stopping and hyperparameter tuning strategies for future model development, though its practical applicability remains limited to stylized models for now.

**Tags**: `#machine-learning`, `#generalization`, `#approximate-message-passing`, `#training-algorithms`, `#high-dimensional-statistics`

---

<a id="item-tech-news-6"></a>
### [Nvidia Developing Nemotron 4 Open-Source Model with 1 Trillion Parameters](https://economictimes.indiatimes.com/tech/artificial-intelligence/nvidia-is-developing-nemotron-4-open-source-models-the-information/articleshow/133157952.cms) ⭐️ 7.0/10

Nvidia is developing a new open‑source model family called Nemotron 4, according to a report by The Information citing multiple employees. The largest version is expected to have at least 1 trillion parameters, with training likely to finish by late autumn, though no release date has been set. The effort aims to compete with the world’s leading open‑source models. On the same day, Nvidia also released Nemotron 3.5 Lightning, a model for code review and other tasks, along with NeMo Switchyard, a library for routing tasks between models.

telegram · zaihuapd · Aug 12, 01:15

**「Background」** Nvidia, primarily known for its graphics processing units, has been expanding its open-source AI model lineup with the Nemotron family. The current Nemotron 3 Ultra offers around 500 billion parameters, and the rumored Nemotron 4 flagship aims to approximately double that scale to over 1 trillion parameters, positioning it to compete with the largest open-source language models globally.

**「Impact」** The potential release of a 1-trillion-parameter open-source model from Nvidia could reshape the competitive landscape for large language models, though the project remains unconfirmed and no release date is set.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/business/nvidia-is-developing-nemotron-4-open-source-models-information-reports-2026-08-11/">Nvidia building 1-trillion-parameter Nemotron 4 to rival open ...</a></li>
<li><a href="https://aiweekly.co/alerts/nvidia-trains-1-trillion-parameter-nemotron-4-open-model">Nvidia trains 1-trillion-parameter Nemotron 4 open model</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#Nemotron 4`, `#large language models`, `#open source`, `#AI research`

---

<a id="item-tech-news-7"></a>
### [Enterprise SSD Share Hits 48% of NAND; YMTC Joins Top Three](https://china.counterpointresearch.com/%e6%9c%8d%e5%8a%a1%e5%99%a8%e9%9c%80%e6%b1%82%e6%8e%a8%e5%8d%87%e4%bc%81%e4%b8%9a%e7%ba%a7-ssd-%e5%8d%a0-nand-%e5%87%ba%e8%b4%a7%e9%87%8f%e7%99%be%e5%88%86%e4%b9%8b-48/) ⭐️ 7.0/10

Enterprise SSDs accounted for 48% of global NAND shipments in Q2 2026, nearly doubling year-over-year, driven by AI inference workloads, according to Counterpoint Research. Industry revenue grew fivefold compared to the same quarter last year. Samsung led with a 25% share, followed by SK Hynix at 22%, while Yangtze Memory Technologies \(YMTC\) surpassed Kioxia for the first time with a 14% share to enter the top three. However, YMTC&\#x27;s revenue ranked only fifth due to its product mix being more consumer-oriented. The report projects enterprise SSDs will consume over half of total NAND bits by the end of the year.

telegram · zaihuapd · Aug 12, 11:00

**「Background」** Enterprise SSDs are high-performance solid-state drives used in data centers, increasingly for AI inference workloads. The NAND flash memory market has long been led by South Korean and Japanese manufacturers, but Chinese company Yangtze Memory Technologies Co. \(YMTC\) has been gaining share. YMTC&\#x27;s growth has occurred despite being added to the US Entity List in late 2022, which restricts its access to advanced manufacturing equipment and technology.

**「Impact」** The near-doubling of enterprise SSD&\#x27;s share of NAND output to 48% is tightening supply for data center and AI infrastructure buyers, while Yangtze Memory&\#x27;s volume growth is not expected to trigger a broad price decline due to its consumer-oriented product mix.

<details><summary>References</summary>
<ul>
<li><a href="https://habr.com/ru/companies/mclouds/articles/1009138/">Влияние памяти из Китая на цены в 2026 –2027 годах... / Хабр</a></li>
<li><a href="https://habr.com/ru/companies/mclouds/articles/1009138/">Влияние памяти из Китая на цены в 2026 –2027 годах... / Хабр</a></li>
<li><a href="https://www.linkedin.com/posts/nick-florous-ph-d-2821a84_semiconductors-nandflash-memorymarket-activity-7400082516902244354-5HbB">#semiconductors #nandflash #memorymarket #aiinfrastructure...</a></li>

</ul>
</details>

**Tags**: `#enterprise SSD`, `#NAND`, `#AI infrastructure`, `#Yangtze Memory`, `#semiconductor market`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Nvidia&\#x27;s $500 billion AI financing plan faces depreciation risk from China](https://www.cnbc.com/2026/08/11/nvidia-ai-funding-jensen-huang-china-risk.html) ⭐️ 9.0/10

Nvidia announced a $500 billion pipeline with Wall Street firms to finance data centers using its GPUs as collateral, but analysts warn that China&\#x27;s growing chip production could cause rapid depreciation of those GPUs, potentially leaving investors with losses.

rss · CNBC Finance · Aug 11, 21:01

**「Background」** The plan treats Nvidia&\#x27;s graphics processing units \(GPUs\) like long-term assets such as real estate, but their resale value is uncertain because cutting-edge chips are quickly superseded by newer models—a risk amplified if China floods the market with cheaper alternatives.

**「Impact」** If borrowers default, Wall Street fund managers would need to repossess and sell used chips into a potentially falling market, which could hit investors holding asset-backed securities tied to AI infrastructure.

**Tags**: `#AI financing`, `#Nvidia`, `#China risk`, `#asset-backed securities`, `#GPU depreciation`

---

<a id="item-finance-news-2"></a>
### [CME to Launch First-Ever Futures on AI Computing Power](https://www.cnbc.com/2026/08/11/ai-computing-power-becomes-a-tradable-asset-class-as-cme-starts-futures.html) ⭐️ 9.0/10

CME Group will launch the first futures contracts on AI computing power on October 5, pending regulatory approval, with each contract representing a month&\#x27;s rent for an Nvidia H100 chip based on Silicon Data&\#x27;s hourly rental price indexes.

rss · CNBC Finance · Aug 11, 18:09

**「Background」** The contracts are designed to create a public reference price for AI computing rental costs, allowing investors to hedge against price swings without owning physical chips or data centers.

**「Impact」** AI developers and data-center operators could use the contracts to lock in costs or revenues, while investors gain a new way to bet on AI computing demand.

**Tags**: `#AI`, `#futures`, `#CME`, `#computing power`, `#financial innovation`

---

<a id="item-finance-news-3"></a>
### [Former Chinese Premier Zhu Rongji Dies at 98](https://www.news.cn/politics/20260812/4c2c72e299ef4561915d2e507393a81f/c.html) ⭐️ 9.0/10

Former Chinese Premier Zhu Rongji died in Beijing on August 12, 2026, at the age of 98, according to an official announcement by state authorities.

telegram · zaihuapd · Aug 12, 10:11

**「Background」** Zhu served as premier from 1998 to 2003, leading China&\#x27;s entry into the World Trade Organization and implementing major economic reforms during the Asian financial crisis.

**Tags**: `#Zhu Rongji`, `#China`, `#Obituary`, `#Politics`, `#Former Premier`

---

<a id="item-finance-news-4"></a>
### [EVs reach 65.1% of new car sales in China, led by Geely, Tesla, and BYD](https://www.cnbc.com/2026/08/12/china-car-sales-data-byd-tesla-geely-vw.html) ⭐️ 8.0/10

New energy vehicles, which include battery and hybrid cars, accounted for 65.1% of new passenger cars sold in China in July 2026, up from 54% a year earlier, according to China Passenger Car Association data. The top-selling models were Geely&\#x27;s Xingyuan electric hatchback, Tesla&\#x27;s Model Y, and several BYD models.

rss · CNBC Finance · Aug 12, 01:20

**「Background」** The 65.1% share marks a sharp increase from 54% a year ago, even as total passenger car sales in China fell by 20.3% in the first seven months of 2026, industry data showed.

**Tags**: `#China auto market`, `#electric vehicles`, `#market share`, `#BYD`, `#Tesla`

---

<a id="item-finance-news-5"></a>
### [Tencent Q2 Revenue Beats, Net Profit Misses; Capex Surge Turns Free Cash Flow Negative](https://wallstreetcn.com/articles/3779275) ⭐️ 8.0/10

Tencent reported Q2 2026 revenue of 204.8 billion yuan, beating analyst expectations, but net profit rose only 0.7% to 56 billion yuan, missing estimates. Capital expenditure nearly tripled to 52.8 billion yuan, leading to free cash flow of negative 13.8 billion yuan; the company said excluding AI-related prepayments, free cash flow was 37.6 billion yuan.

telegram · zaihuapd · Aug 12, 10:30

**「Background」** Tencent, a Chinese technology and gaming giant, has been ramping up investment in artificial intelligence infrastructure. The sharp increase in capital expenditure reflects spending on AI computing power, which temporarily turned free cash flow negative despite strong revenue growth.

**Tags**: `#earnings`, `#Tencent`, `#capital expenditure`, `#free cash flow`, `#AI`

---