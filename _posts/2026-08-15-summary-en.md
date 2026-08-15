---
layout: default
title: "Horizon Summary: 2026-08-15 (EN)"
date: 2026-08-15
lang: en
---

> From 37 items, 12 important content pieces were selected

---

**Technology News**
1. [Qwen 3.8 27B-FP8 Delivers Strong Reasoning and SWE Performance on Local Hardware](#item-tech-news-1) ⭐️ 8.0/10
2. [Firefox is now the last major browser that still supports uBlock Origin](#item-tech-news-2) ⭐️ 8.0/10
3. [Doom&\#x27;s Renderer Compiled into a 21B-Parameter Transformer](#item-tech-news-3) ⭐️ 8.0/10
4. [PostgreSQL Patches to\_char Heap Overflow \(CVE-2026-14669\)](#item-tech-news-4) ⭐️ 8.0/10
5. [Law enforcement hacking grows as encryption &\#x27;goes dark&\#x27;](#item-tech-news-5) ⭐️ 7.0/10
6. [RustDesk Adds True Unattended Remote Access on Wayland](#item-tech-news-6) ⭐️ 7.0/10
7. [Tagging content with LLMs by generating then matching embeddings](#item-tech-news-7) ⭐️ 7.0/10
8. [BDH-CQ: 150M Model Achieves 29.5% pass@2 on ARC-AGI-1 at Low Cost](#item-tech-news-8) ⭐️ 7.0/10
9. [Apple trains custom AI model for China with Alibaba support, set to be first foreign approval](#item-tech-news-9) ⭐️ 7.0/10

**Financial News**
1. [Berkshire Hathaway makes Alphabet a top three holding, ends 14-quarter net selling streak](#item-finance-news-1) ⭐️ 8.0/10
2. [Goldman Sachs benefits from Nvidia’s $500 billion AI financing plan and stock offerings](#item-finance-news-2) ⭐️ 8.0/10
3. [China to lift Manus founder&\#x27;s travel ban; former investors eye $2bn buyback from Meta](#item-finance-news-3) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Qwen 3.8 27B-FP8 Delivers Strong Reasoning and SWE Performance on Local Hardware](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 8.0/10

Qwen 3.8 27B-FP8 has been released as a new local language model demonstrating strong reasoning and software engineering capabilities that rival Gemma 4 on private benchmarks. Community reports indicate it correctly solved a challenging private reasoning benchmark, though it required 5x more tokens and 12 minutes 30 seconds with MTP enabled compared to Gemma 4’s implicit reasoning. In software engineering evals, it successfully set up a local git repo, wrote a functional JavaScript todo list app skeleton, and handled the same task in Rust with Tauri, suggesting practical utility for developers. The model also exhibits a distinctive thinking trace style that omits function words like “to” and “we,” producing almost caveman-like note-form reasoning. However, VRAM usage appears less efficient than Gemma 4 or Glimmer, with only 32K context observed.

hackernews · erdaltoprak · Aug 14, 15:00 · [Discussion](https://news.ycombinator.com/item?id=49299605)

**「Background」** Qwen is a family of open-weight large language models developed by Qwen. The Qwen3.8 series includes the heavyweight Qwen3.8-Max and the smaller Qwen3.8-27B, a 27‑billion‑parameter model with a 262k token context window, released on August 14, 2026. When quantized to 4‑bit precision, it can run locally on consumer hardware with about 17 GB of RAM or VRAM.

**「Impact」** Local LLM users can now tackle complex reasoning and software engineering tasks offline with Qwen 3.8 27B, though they should expect 5x higher token usage and longer inference times compared to Gemma 4, along with less efficient VRAM utilization.

**「Community Discussion」** Community testers report that Qwen 3.8 27B is the second local model to pass a private reasoning benchmark, but it requires significantly more tokens and time, and exhibits less efficient VRAM usage than alternatives. The model also impressed with accurate software engineering tasks, including a todo-list app and a well-drawn pelican SVG, though some minor details were missing, and its thinking trace style drew attention for its terse, note-form language.

<details><summary>References</summary>
<ul>
<li><a href="https://www.yottalabs.ai/post/qwen-3-8-27b-specs-hardware-requirements-how-to-run-2026">Qwen 3.8 27B: Specs, Hardware Requirements, and How to Run It (2026) | Yotta Labs</a></li>
<li><a href="https://aireleasetracker.com/model/qwen/qwen3.8-27b">Qwen3.8-27B — Benchmarks, Specs &amp; Release Date</a></li>

</ul>
</details>

**Tags**: `#Qwen`, `#local LLM`, `#model release`, `#reasoning`, `#software engineering`

---

<a id="item-tech-news-2"></a>
### [Firefox is now the last major browser that still supports uBlock Origin](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 8.0/10

Firefox remains the only major browser to fully support the uBlock Origin extension after Google Chrome&\#x27;s transition to Manifest V3, which limits ad-blocking capabilities. Mozilla&\#x27;s browser also uniquely performs manual reviews of uBlock Origin&\#x27;s code on every update to ensure it remains free of spyware or malware. This distinction highlights the growing tension between user freedom and platform control in the browser ecosystem, leaving users of Chromium-based browsers like Chrome and Edge with less effective ad-blocking tools.

hackernews · DemiGuru · Aug 14, 19:03 · [Discussion](https://news.ycombinator.com/item?id=49303202)

**「Background」** uBlock Origin is a widely used content-blocking browser extension that relies on powerful network request APIs to filter ads and trackers. Google’s transition to Manifest V3 for Chrome extensions removes the older webRequest API that extensions like uBlock Origin depend on, replacing it with a more limited declarativeNetRequest API that cannot fully support the extension’s capabilities. Consequently, Chromium-based browsers such as Chrome, Edge, and Brave no longer support the full uBlock Origin, while Firefox continues to maintain its own extension framework that preserves the necessary APIs.

**「Impact」** Chrome&\#x27;s Manifest V3 update deprecates the APIs that uBlock Origin relies on, leaving Firefox as the only major browser that still fully supports the extension, forcing users who want to retain its full ad-blocking capabilities to switch to Firefox.

**「Community Discussion」** Community comments reflect a consensus that Google&\#x27;s Manifest V3 represents a restriction of user freedom, with many appreciating Firefox&\#x27;s continued support for uBlock Origin and its manual review process. Some express concern that the broader web may be threatened by locked-down platforms, while others highlight the stark difference between an ad-laden web and the clean browsing experience provided by Firefox and uBlock Origin.

<details><summary>References</summary>
<ul>
<li><a href="https://www.dexerto.com/tech/ad-blockers-manifest-v3-2859978/">Google Chrome Adblock changes explained: uBlock Lite &amp; Manifest V 3</a></li>
<li><a href="https://www.gamermarkt.com/blog/chrome-ad-blockers-manifest-v3-alternatives/">Chrome Ad Blockers Are Done: Manifest V 3 Explained</a></li>
<li><a href="https://techstory.in/the-end-of-ad-free-browsing-chrome-moves-toward-fully-phasing-out-ad-blockers-with-manifest-v3/">The End of Ad - Free Browsing: Chrome Moves Toward... - TechStory</a></li>

</ul>
</details>

**Tags**: `#browsers`, `#privacy`, `#ad-blocking`, `#open-source`, `#Manifest V3`

---

<a id="item-tech-news-3"></a>
### [Doom&\#x27;s Renderer Compiled into a 21B-Parameter Transformer](https://www.reddit.com/r/MachineLearning/comments/1voazhm/i_compiled_dooms_renderer_into_a_21bparameter/) ⭐️ 8.0/10

A developer compiled the Doom rendering algorithm into a 21-billion-parameter transformer model using a custom compiler that converts computation graphs into standard transformer weights, without any training. The model takes a scene prompt and autoregressively generates a token sequence of pixel drawing commands, which when mechanically interpreted produce the famous E1M1 frame. A single render requires a 3,614-token prompt and 53,747 generated tokens, taking just over 40 minutes on an NVIDIA B200 GPU—equivalent to 35 frames per day. The checkpoint is a standard Hugging Face format, and the entire inference host program is 43 lines of Python. The project demonstrates a novel approach to executing deterministic algorithms inside transformer architectures, which could inform interpretability research and unconventional model usage.

reddit · r/MachineLearning · /u/notforrob · Aug 14, 15:50

**「Background」** The original Doom engine uses a rasterization algorithm to render 3D scenes into 2D pixels. Transformers are deep learning architectures that normally learn from data, but their forward pass can be viewed as a sequence of programmable operations. The project repurposes that capability by compiling an explicit computation graph of Doom&\#x27;s rendering steps into the weight matrices of a large transformer, allowing the model to execute the algorithm directly during generation.

**Tags**: `#transformers`, `#compiler`, `#doom`, `#computation-graphs`, `#novel-approach`

---

<a id="item-tech-news-4"></a>
### [PostgreSQL Patches to\_char Heap Overflow \(CVE-2026-14669\)](https://www.postgresql.org/support/security/CVE-2026-14669/) ⭐️ 8.0/10

PostgreSQL disclosed CVE-2026-14669, a heap buffer overflow in the to\_char\(timestamptz\) function when processing overly long POSIX timezone abbreviations. An authenticated database user with the ability to set the session timezone can exploit it to execute arbitrary code with the operating system privileges of the PostgreSQL service process. The vulnerability has a CVSS score of 8.8 and affects versions before 18.5 \(which was not released due to a regression\), 17.11, 16.15, 15.19, and 14.24. Users of the 18 series should upgrade to 18.6, while other branches should move to 17.11, 16.15, 15.19, or 14.24 respectively; the update requires only replacing program files and restarting the service.

telegram · zaihuapd · Aug 14, 14:35

**「Background」** The to\_char function formats timestamp values, and for timestamptz it converts the timezone offset into a human-readable abbreviation using the system&\#x27;s timezone data. A crafted POSIX timezone name can trigger an overflow in the abbreviation formatting logic, corrupting heap memory.

**「Impact」** A low-privileged database user who can set the timezone can gain arbitrary code execution with the operating system rights of the database server process, making immediate patching essential for all exposed instances.

**Tags**: `#PostgreSQL`, `#security`, `#vulnerability`, `#CVE`, `#database`

---

<a id="item-tech-news-5"></a>
### [Law enforcement hacking grows as encryption &\#x27;goes dark&\#x27;](https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/) ⭐️ 7.0/10

As strong encryption becomes the default in communications and data storage, law enforcement agencies are increasingly turning to hacking techniques—such as exploiting software vulnerabilities or deploying malware—to gain access to suspects&\#x27; information. This shift, described as the era of law enforcement hacking, raises fundamental tensions between investigative needs and the security of digital infrastructure for all users. The blog post argues that while governments may attempt to mandate backdoors or restrict encryption, the practical reality is that they will rely on discovering and weaponizing technical flaws, which simultaneously undermines the security of the systems everyone depends on. The trend is accelerating as more data and communications are end-to-end encrypted, potentially pushing law enforcement toward a future where hacking is a primary investigative tool.

hackernews · vslira · Aug 14, 20:52 · [Discussion](https://news.ycombinator.com/item?id=49304447)

**「Background」** The &\#x27;Going Dark&\#x27; problem refers to the difficulty law enforcement faces in accessing digital communications as strong encryption becomes ubiquitous. Historically, wiretapping required physical line taps, but modern encrypted channels make interception ineffective, leading agencies to increasingly rely on endpoint hacking to bypass encryption. The blog post from Matthew Green&\#x27;s cryptographic engineering blog discusses these developments in the context of a recent Usenix Security conference.

**「Impact」** The proliferation of law enforcement hacking incentivizes the hoarding of zero-day vulnerabilities, making the broader software ecosystem less secure and potentially exposing innocent users to the same flaws that are exploited for investigations.

**「Community Discussion」** Commenters note that the increasing use of AI-generated code may increase the number of exploitable bugs, challenging the idea that the supply of useful vulnerabilities will soon hit a ceiling. Others point out that biometrics could be used to compel suspects to unlock devices, temporarily delaying the &\#x27;going dark&\#x27; problem, while some highlight the stark contrast between sophisticated state hacking and the frequent security failures in commercial software.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/">Everything is about to “go dark”</a></li>

</ul>
</details>

**Tags**: `#security`, `#cryptography`, `#law-enforcement`, `#privacy`, `#vulnerabilities`

---

<a id="item-tech-news-6"></a>
### [RustDesk Adds True Unattended Remote Access on Wayland](https://rustdesk.com/blog/unattended-remote-access-wayland/) ⭐️ 7.0/10

RustDesk now supports true unattended remote access on Wayland, solving a critical gap for Linux remote desktop users. The feature allows connections to a machine without any user interaction, overcoming Wayland&\#x27;s security restrictions that previously obstructed such functionality. This update marks a significant usability improvement for the open-source RustDesk, which is often used as an alternative to proprietary tools like TeamViewer or AnyDesk.

hackernews · rustdesk · Aug 14, 16:12 · [Discussion](https://news.ycombinator.com/item?id=49300759)

**「Background」** Wayland is the default display server protocol on many modern Linux distributions, replacing the older X11. Unlike X11, Wayland restricts applications from capturing the screen without user consent for security, which historically prevented unattended remote desktop access. RustDesk&\#x27;s new implementation specifically addresses this limitation to enable true unattended remote control.

**「Impact」** Linux users can now rely on RustDesk for fully unattended remote access on Wayland-based systems, eliminating the need for X11 fallback or interactive user consent.

**「Community Discussion」** Users welcomed the fix, with one commenting that it resolved a recent hiccup. However, a long-standing limitation remains: self-hosted connections lack encryption \(issue \#3714\), and some question RustDesk&\#x27;s advantages over alternatives like VNC, Remmina, or Sunshine/Moonlight.

**Tags**: `#remote-desktop`, `#open-source`, `#wayland`, `#linux`, `#rustdesk`

---

<a id="item-tech-news-7"></a>
### [Tagging content with LLMs by generating then matching embeddings](https://simonwillison.net/2026/Aug/14/dont-classify-hallucinate/) ⭐️ 7.0/10

Simon Willison describes a workaround for tagging content with a large existing vocabulary: instead of passing the full tag set to an LLM, prompt the model to generate novel, fitting tags. The generated tags are vectorized and matched against the embeddings of the real tags to find the closest matches. This technique, demonstrated with a product classification example, sidesteps token limits and makes LLM-based tagging feasible for large tag corpora.

rss · Simon Willison · Aug 14, 21:54

**「Background」** Large language models have finite context windows, making it difficult to supply a tag vocabulary of hundreds or thousands of items. Vector embeddings are numerical representations of text that allow measuring semantic similarity between strings.

**「Impact」** Developers can use this method to tag content with very large vocabularies without worrying about token limits, using only prompt engineering and a precomputed embedding index.

**Tags**: `#LLM`, `#tagging`, `#embeddings`, `#classification`, `#prompt-engineering`

---

<a id="item-tech-news-8"></a>
### [BDH-CQ: 150M Model Achieves 29.5% pass@2 on ARC-AGI-1 at Low Cost](https://www.reddit.com/r/MachineLearning/comments/1vov5r5/bdhcq_incontext_learning_with_recurrent_latent/) ⭐️ 7.0/10

BDH-CQ introduces a reasoning system that combines in-context learning with recurrent latent reasoning. The model updates its recurrent memory using demonstrations of a previously unseen task, then solves the query through iterative computation in a high-dimensional latent space, without decoding intermediate reasoning steps into language. Neither task identifiers nor evaluation-task demonstration pairs are used during training, and no parameters are updated at inference time. A 150M-parameter configuration achieves 29.5% pass@2 on the ARC-AGI-1 benchmark at a cost of $0.00070 per task, breaking through the previously reported cost–accuracy Pareto frontier. This approach demonstrates that efficient adaptation and inference can be achieved without verbalized intermediate reasoning.

reddit · r/MachineLearning · /u/moschles · Aug 15, 06:18

**「Background」** ARC-AGI-1 is a benchmark designed to measure passive fluid intelligence, requiring models to infer patterns from few examples without task-specific training. The cost-accuracy Pareto frontier illustrates the trade-off between solving tasks accurately and doing so cheaply, with previous models lying on a curve where higher accuracy came at higher cost. The BDH-CQ model from Pathway uses recurrent latent reasoning, where it updates its internal memory from example demonstrations and then performs iterative computation in a latent space, without language decoding, to produce answers.

**「Impact」** Researchers can now achieve competitive ARC-AGI-1 performance at a fraction of the cost of prior methods, potentially enabling broader experimentation with recurrent latent reasoning systems.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/ai/articles/pathways-150m-parameter-model-breaks-113000925.html?fr=sycsrp_catchall">Pathway&#x27;s 150M-Parameter Model Breaks the ARC-AGI-1 Cost ...</a></li>
<li><a href="https://www.morningstar.com/news/business-wire/20260811268264/pathways-150m-parameter-model-breaks-the-arc-agi-1-cost-efficiency-frontier">Pathway&#x27;s 150M-Parameter Model Breaks the ARC-AGI-1 Cost ...</a></li>
<li><a href="https://arcprize.org/leaderboard">ARC Prize - Leaderboard</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#in-context learning`, `#reasoning`, `#ARC-AGI`, `#recurrent latent reasoning`

---

<a id="item-tech-news-9"></a>
### [Apple trains custom AI model for China with Alibaba support, set to be first foreign approval](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 7.0/10

Apple is training its own large language model \(LLM\) specifically for the Chinese market, breaking from its earlier strategy of relying on third-party models, and has secured support from Alibaba. The model, part of Apple Intelligence, is expected to roll out in China via an iOS update in the coming months. China&\#x27;s Cyberspace Administration has already filed the generative AI service, and if approved, Apple would become the first foreign company authorized by Beijing to offer its own AI model in the country. This move gives Apple greater control over the AI experience for Chinese users and marks a significant strategic shift in navigating restricted markets.

telegram · zaihuapd · Aug 14, 14:47

**「Background」** Apple’s on-device AI system, Apple Intelligence, requires local regulatory approval in China, where generative AI services must be filed with the Cyberspace Administration. Initially, Apple had planned to incorporate Alibaba’s Qwen model, but it has now shifted to training its own proprietary large language model with Alibaba’s support. This would make Apple the first foreign company permitted by Beijing to offer a self-developed AI model in the country.

**「Impact」** Apple’s custom model could give it a competitive edge in China’s tightly regulated AI landscape while setting a regulatory precedent for other foreign companies seeking to deploy their own AI systems locally.

<details><summary>References</summary>
<ul>
<li><a href="https://macdailynews.com/2026/08/14/apple-trains-proprietary-ai-model-for-china-alongside-alibaba/">Apple trains proprietary AI model for China alongside Alibaba - MacDailyNews</a></li>
<li><a href="https://www.macrumors.com/2026/08/14/apple-trained-own-ai-model-for-china/">Apple Trained Own AI Model for China Market With Help From Alibaba - MacRumors</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#AI`, `#China`, `#LLM`, `#Alibaba`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Berkshire Hathaway makes Alphabet a top three holding, ends 14-quarter net selling streak](https://www.cnbc.com/2026/08/14/berkshire-hathaway-boosts-alphabet-to-a-top-three-holding-ups-delta-and-housing-bets.html) ⭐️ 8.0/10

Berkshire Hathaway increased its Alphabet stake by 83% in the second quarter, making the Google parent its third-largest U.S. listed equity holding at $37.9 billion. The conglomerate also shifted to nearly $20 billion in net equity purchases after 14 straight quarters of net sales.

rss · CNBC Finance · Aug 14, 21:06

**「Background」** The Alphabet position jump largely reflects a $10 billion private stock purchase in June, and the net buying shift ended a 14-quarter streak of net sales that had pushed cash to a record $397.4 billion.

**Tags**: `#Berkshire Hathaway`, `#Alphabet`, `#Delta Air Lines`, `#homebuilders`, `#portfolio changes`

---

<a id="item-finance-news-2"></a>
### [Goldman Sachs benefits from Nvidia’s $500 billion AI financing plan and stock offerings](https://www.cnbc.com/2026/08/14/goldmans-latest-cash-cow-is-all-about-funding-the-ai-infrastructure-boom.html) ⭐️ 8.0/10

Goldman Sachs was a key facilitator for Nvidia’s plan to raise $500 billion for AI infrastructure. The bank also served as a joint book-running manager for Intel’s $20 billion and Alphabet’s $85 billion stock offerings.

rss · CNBC Finance · Aug 14, 20:05

**「Background」** As a joint book-running manager, Goldman Sachs earns fees from the spread between the discounted price it pays the issuer and the public offering price, with the revenue flowing to its Global Banking &amp; Markets division.

**Tags**: `#Goldman Sachs`, `#AI infrastructure`, `#equity underwriting`, `#technology financing`, `#investment banking`

---

<a id="item-finance-news-3"></a>
### [China to lift Manus founder&\#x27;s travel ban; former investors eye $2bn buyback from Meta](https://www.ft.com/content/fa479d50-7c79-4b6d-99c3-3830e37c1503?syn-25a6b1a6=1) ⭐️ 8.0/10

China plans to lift the travel restrictions on Manus&\#x27; founder, CEO Xiao Hong, who has informed staff of plans to return to Singapore. Former investors and management, including Tencent, are planning to buy back the AI startup from Meta at a valuation of about $2 billion, pending regulatory approval; Tencent would become the largest minority shareholder and Manus would remain independent in Singapore.

telegram · zaihuapd · Aug 15, 08:05

**「Background」** Chinese regulators previously ordered Meta to unwind its acquisition of AI startup Manus and barred its founders from leaving the country, citing data security concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/world/asia-pacific/china-blocks-foreign-acquisition-ai-startup-manus-2026-04-27/">China orders Meta to unwind $2 billion purchase of AI startup Manus | Reuters</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/manus-returns-independence-china-blocks-170145849.html">Manus returns to independence after China blocks Meta acquisition</a></li>

</ul>
</details>

**Tags**: `#cross-border M&amp;A`, `#AI buyback`, `#Tencent`, `#Meta`, `#China travel restrictions`

---