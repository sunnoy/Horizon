---
layout: default
title: "Horizon Summary: 2026-08-05 (EN)"
date: 2026-08-05
lang: en
---

> From 46 items, 18 important content pieces were selected

---

**Technology News**
1. [A Custom Color Space for Generating Diverse Skin Tones](#item-tech-news-1) ⭐️ 8.0/10
2. [Eight Myths on Software Engineering and GenAI](#item-tech-news-2) ⭐️ 8.0/10
3. [LLM 0.32 Adds Reasoning Traces, Server-Side Tools, and OpenAI Responses Support](#item-tech-news-3) ⭐️ 8.0/10
4. [llm-anthropic 0.26 Adds Claude 5 Models and Server-Side Tools](#item-tech-news-4) ⭐️ 8.0/10
5. [White House Reverses on Open-Source AI Regulation, Silicon Valley Split Deepens](#item-tech-news-5) ⭐️ 8.0/10
6. [ChainDrop Supply Chain Worm Infects Over 1,300 npm Packages](#item-tech-news-6) ⭐️ 8.0/10
7. [ByteDance Releases SeedRealtime: Native Audio-Video Full-Duplex Model for Doubao](#item-tech-news-7) ⭐️ 8.0/10
8. [FFmpeg 9.0 Released with Animated WebP Support and AI-Assisted Development](#item-tech-news-8) ⭐️ 8.0/10
9. [MLX Port Enables MiniMax-H3 Omni-Modal Video Generation on Apple Silicon](#item-tech-news-9) ⭐️ 7.0/10
10. [SpaceX to Exclusively Use NVIDIA Vera Rubin AI Architecture](#item-tech-news-10) ⭐️ 7.0/10
11. [Samsung, SK Hynix Test AMEC Etching Tools to Hedge Against US Export Controls](#item-tech-news-11) ⭐️ 7.0/10

**Financial News**
1. [Polymarket in talks for fundraising at over $20 billion valuation](#item-finance-news-1) ⭐️ 8.0/10
2. [Goldman Sachs Equities Revenue Hits Record $7.42 Billion in Q2](#item-finance-news-2) ⭐️ 8.0/10
3. [DeepSeek Restarts Second Funding Round with Pre-Money Valuation of 500 Billion Yuan](#item-finance-news-3) ⭐️ 8.0/10
4. [宇树科技科创板 IPO 启动询价](#item-finance-news-4) ⭐️ 8.0/10
5. [Citadel posts best month in years after acquiring discounted assets from collapsed AI hedge fund](#item-finance-news-5) ⭐️ 7.0/10
6. [Philadelphia Fed President Paulson says current rates sufficient, but open to recalibration](#item-finance-news-6) ⭐️ 7.0/10
7. [Jeff Bezos Files to Sell $4.1 Billion in Amazon Shares](#item-finance-news-7) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [A Custom Color Space for Generating Diverse Skin Tones](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 8.0/10

A developer has introduced a custom color space and algorithm for generating diverse skin tones, presented as a Show HN post with interactive demos. The approach uses principal component analysis on real skin color data to reduce the three-dimensional color space to two dimensions, then fits curves to define a crescent-shaped region of plausible skin colors. The creation includes a color picker and a procedural generation function, designed to help digital artists and game developers easily select or generate realistic, varied skin tones. The methodology is openly documented, with the author noting potential improvements, and the resulting color distribution aligns with the characteristic crescent shape observed in skin tone data when plotted in perceptual color spaces like Oklab.

hackernews · automatoney · Aug 4, 15:16 · [Discussion](https://news.ycombinator.com/item?id=49170165)

**「Background」** Standard color models like RGB and HSL are not designed to capture the narrow, crescent-shaped range of human skin tones, which primarily span brown and orange hues. The Pantone SkinTone Guide provides a physical reference of 110 skin tone colors for consistent matching, while perceptual color spaces such as Oklab aim to improve uniformity for tasks like blending and interpolation. This project addresses the gap by introducing a custom color space and algorithm that simplifies the generation of diverse, realistic skin tones for digital art and game development.

**「Impact」** The tool provides digital artists and game developers with a practical way to procedurally generate diverse, realistic skin tones, reducing manual selection effort and potential bias.

**「Community Discussion」** Commenters praised the technical approach, particularly the function fitting after PCA, and noted that the generated colors match the well-known crescent distribution of skin tones in color spaces like Oklab. Some raised that skin color modeling is inherently complex, involving perception and lighting, and suggested comparisons with existing standards like Pantone Skin Tones.

<details><summary>References</summary>
<ul>
<li><a href="https://www.pantone.com/skintone">PANTONE® USA | Pantone SkinTone Guide | Accurate Skin Tone Color Matching</a></li>
<li><a href="https://en.wikipedia.org/wiki/Oklab_color_space">Oklab color space - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#color-spaces`, `#skin-tones`, `#procedural-generation`, `#graphics`, `#game-dev`

---

<a id="item-tech-news-2"></a>
### [Eight Myths on Software Engineering and GenAI](https://queue.acm.org/detail.cfm?id=3807963) ⭐️ 8.0/10

The article critically examines eight common misconceptions about generative AI&\#x27;s role in software engineering, challenging exaggerated claims of automation and productivity gains. It cites evidence that developers spend only a small fraction of their time coding, and that LLMs can introduce biases, reduce code ownership, and impose a &\#x27;competence penalty&\#x27; on users perceived as less capable. The piece argues that agentic AI is not an imminent replacement for human engineers and that current tools augment rather than substitute for expert judgment. The myths are deconstructed using recent research to provide a realistic, evidence-based perspective for practitioners and researchers.

hackernews · tchalla · Aug 4, 23:50 · [Discussion](https://news.ycombinator.com/item?id=49176830)

**「Background」** The article examines eight common myths about generative AI in software engineering, drawing on research from Microsoft and other studies. It challenges exaggerated claims—such as the arrival of AI-driven 10x developers or that AI will drastically cut coding time—by presenting evidence-based counterpoints.

**「Impact」** Developers and engineering leaders should temper expectations, integrating generative AI tools as aids rather than replacements, because over-reliance can erode developer engagement, codebase understanding, and introduce subtle biases, while the technology remains far from autonomous software creation.

**「Community Discussion」** Commenters pointed out that some cited studies, like the early-2025 METR study, are already outdated. Others reported personal experiences of losing motivation and feeling disconnected from codebases when using LLMs extensively, and questioned the methodology of the &\#x27;competence penalty&\#x27; study, noting its limited geographic scope.

<details><summary>References</summary>
<ul>
<li><a href="https://queue.acm.org/detail.cfm?id=3807963">Eight Myths on Software Engineering and GenAI - ACM Queue</a></li>
<li><a href="https://explainx.ai/blog/eight-myths-software-engineering-genai-acm-queue-august-2026">8 GenAI Coding Myths Debunked ( ACM Queue 2026) | explainx.ai</a></li>

</ul>
</details>

**Tags**: `#software engineering`, `#generative AI`, `#myths`, `#LLM`, `#developer productivity`

---

<a id="item-tech-news-3"></a>
### [LLM 0.32 Adds Reasoning Traces, Server-Side Tools, and OpenAI Responses Support](https://simonwillison.net/2026/Aug/4/new-release-of-llm/#atom-everything) ⭐️ 8.0/10

LLM 0.32, the latest major release of the open-source CLI tool for interacting with language models, adds support for reasoning traces \(displayed to stderr\), server-side provider tools such as OpenAI&\#x27;s CodeInterpreter and WebSearch, and the GPT-5.6 Luna model as the new default. The update also introduces a redesigned content-addressable SQLite log, a new \`llm openai endpoint\` command for one-off prompts against any OpenAI-compatible API, and a Python API that now allows direct message passing and structured event streaming to handle reasoning, tool calls, and mixed outputs. The accompanying llm-anthropic plugin provides its own server-side tools including WebSearch, WebFetch, CodeExecution, and an MCP connector for single-request interactions.

rss · Simon Willison · Aug 4, 23:58

**「Background」** LLM is a widely used open-source CLI tool and Python library that provides a consistent interface for interacting with multiple large language model providers. Reasoning traces are the internal chain-of-thought steps that some models generate before producing a final answer; server-side tools allow models to call external APIs, run code, or fetch web content during a response. The OpenAI Responses API is a newer endpoint that supports more complex interactions, including tool calls and streaming of structured events.

**「Impact」** Developers using LLM can now inspect model reasoning, leverage provider-hosted tools, and integrate with the OpenAI Responses API, making it easier to build and debug applications that rely on these capabilities without additional custom infrastructure.

**Tags**: `#LLM`, `#CLI`, `#open-source`, `#AI-tools`, `#OpenAI-API`

---

<a id="item-tech-news-4"></a>
### [llm-anthropic 0.26 Adds Claude 5 Models and Server-Side Tools](https://simonwillison.net/2026/Aug/4/llm-anthropic/#atom-everything) ⭐️ 8.0/10

The llm-anthropic plugin version 0.26, released alongside LLM 0.32, introduces support for Anthropic&\#x27;s Claude 5 family of models: claude-fable-5, claude-sonnet-5, and claude-opus-5. It adds server-side tools—WebSearch, WebFetch, CodeExecution, and AnthropicMCP—accessible through the CLI&\#x27;s -T flag, replacing the previous -o web\_search\* options. Reasoning, tool calls, tool results, and server-side tool results now stream as typed events, and reasoning output is displayed on standard error unless --hide-reasoning/-R is used. The extended thinking configuration has been simplified to thinking and thinking\_effort \(low, medium, high, xhigh, or max\), with Claude 5 models thinking by default; the old thinking\_budget, thinking\_display, and thinking\_adaptive options are removed. This update gives developers immediate access to Anthropic&\#x27;s latest models and integrated tool capabilities from the command line.

rss · Simon Willison · Aug 4, 22:00

**「Background」** LLM is a command-line tool by Simon Willison that provides a unified interface for interacting with various large language models. The llm-anthropic plugin extends LLM to support Anthropic&\#x27;s models, including the newly released Claude 5 series, which features built-in reasoning and extended thinking capabilities. The plugin now requires LLM 0.32, which introduced a typed event streaming system for reasoning and tool interactions.

**「Impact」** Developers using the LLM CLI tool can now directly access Claude 5 models and integrate server-side web search, fetching, code execution, and MCP tools into their workflows, with a streamlined configuration that replaces deprecated options.

**Tags**: `#llm`, `#anthropic`, `#claude-5`, `#cli-tools`, `#ai`

---

<a id="item-tech-news-5"></a>
### [White House Reverses on Open-Source AI Regulation, Silicon Valley Split Deepens](https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html) ⭐️ 8.0/10

The Trump administration has abruptly shifted its approach to open-source AI regulation, moving from considering sanctions, trade blacklists, and a ban on US–China collaboration to focusing on boosting US competitiveness. The reversal was triggered by the Chinese open-source model Kimi matching top OpenAI performance, and by intense pushback from companies like Nvidia and Meta, who advocate for open ecosystems. On August 4, 2026, the White House invited tech firms to discuss a new cybersecurity review framework for pre-release model scrutiny. OpenAI and Anthropic pushed for restrictions on Chinese competitors, citing national security, while the opposing camp, including Nvidia CEO Jensen Huang, formed a 230-member safety alliance to defend open-source AI.

telegram · zaihuapd · Aug 4, 15:22

**「Background」** Open-source AI models allow anyone to inspect, modify, and distribute the underlying code, which can accelerate innovation but also raise concerns about misuse and strategic advantage. The US has previously debated export controls and investment restrictions on Chinese AI firms, but open-source models complicate enforcement because they can be freely shared globally, including across borders.

**「Impact」** The proposed cybersecurity review framework could introduce mandatory pre-release vetting for AI models, directly affecting how US companies release open-source systems and potentially altering the competitive landscape between closed and open AI development.

**Tags**: `#artificial intelligence`, `#open source`, `#regulation`, `#geopolitics`, `#technology industry`

---

<a id="item-tech-news-6"></a>
### [ChainDrop Supply Chain Worm Infects Over 1,300 npm Packages](https://www.bleepingcomputer.com/news/security/massive-chaindrop-npm-supply-chain-attack-infects-hundreds-of-packages/) ⭐️ 8.0/10

The ChainDrop worm has infiltrated over 1,300 npm packages, collectively amassing 2 billion monthly downloads. The attack began with the compromise of the Keyv maintainer&\#x27;s GitHub account and spread to packages from organizations like Deliveroo, Qlik, and ServiceTitan. Malicious versions were published through legitimate GitHub Actions workflows, carrying a valid provenance, and included a dropper script \(setup.mjs\) and a stealer \(Math\_Symbol.js\) that execute on npm install. The malware harvests credentials for GitHub, npm, AWS, and Kubernetes, and actively propagates by infecting other maintainers&\#x27; packages. Security researchers advise that any system that installed an affected version should be considered fully compromised, requiring environment rebuilds, token rotation, and log inspection, with the domain npm-cache\[.\]com serving as an indicator of compromise.

telegram · zaihuapd · Aug 5, 03:04

**「Background」** npm is the dominant package registry for JavaScript, and supply chain attacks exploit trusted packages to deliver malicious code to a wide user base. A worm is malware that self-replicates across systems, in this case spreading to other packages in the registry.

**「Impact」** Developers who installed any of the compromised packages should immediately treat their environment as compromised, revoke and rotate all exposed secrets, and rebuild from a clean state. Because the worm is still spreading, the number of affected packages is expected to rise.

**Tags**: `#supply-chain-attack`, `#npm`, `#malware`, `#security`, `#credentials-theft`

---

<a id="item-tech-news-7"></a>
### [ByteDance Releases SeedRealtime: Native Audio-Video Full-Duplex Model for Doubao](https://seed.bytedance.com/zh/blog/seedrealtime-%E9%9F%B3%E8%A7%86%E9%A2%91%E5%85%A8%E5%8F%8C%E5%B7%A5%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%8F%91%E5%B8%83-%E8%B5%B0%E5%90%91%E5%85%A8%E6%A8%A1%E6%80%81%E8%87%AA%E7%84%B6%E4%BA%A4%E4%BA%92) ⭐️ 8.0/10

ByteDance released SeedRealtime, a native audio-video full-duplex large model, on August 5 and deployed it across the Doubao app. The model replaces traditional cascaded systems that chain ASR, VLM, and TTS modules with a unified end-to-end architecture that processes audio, video, and text continuously in real time, enabling simultaneous perception, understanding, and expression without external voice activity detection. End-to-end human evaluations show that conversational rhythm issues, including premature cut-offs, are reduced by half compared to cascade models. The model supports three core capabilities: joint audio-video understanding, proactive environmental awareness, and smooth conversational pacing.

telegram · zaihuapd · Aug 5, 04:42

**「Background」** Most real-time conversational AI systems rely on a cascade of separate modules for automatic speech recognition, visual understanding, and speech synthesis, which introduces latency and information loss. In contrast, a full-duplex model like SeedRealtime uses a unified end-to-end architecture that natively integrates audio, video, and text processing. This allows simultaneous perception, reasoning, and response without requiring external turn-taking signals.

**「Impact」** Doubao app users now experience more natural real-time conversations with significantly fewer interruptions and halved rhythm-related problems.

<details><summary>References</summary>
<ul>
<li><a href="https://www.stcn.com/article/detail/4059425.html">字 节 跳 动 推出 原 生 音 视 频 全 双 工 大 模 型 SeedRealtime</a></li>

</ul>
</details>

**Tags**: `#multimodal AI`, `#real-time interaction`, `#conversational AI`, `#full-duplex models`, `#audio-visual processing`

---

<a id="item-tech-news-8"></a>
### [FFmpeg 9.0 Released with Animated WebP Support and AI-Assisted Development](https://news.ycombinator.com/item?id=49166202) ⭐️ 8.0/10

FFmpeg 9.0 has been released, adding an animated WebP decoder and demuxer, a v360\_vulkan filter, a Playdate video encoder and muxer, HE-AAC 960 decoding for DAB+, a transpose\_cuda filter, an AMF frame rate converter, and an ONNX Runtime DNN backend. The development team used Anthropic&\#x27;s Claude AI via the Claude for Open Source Program to help identify missing backports, though some community members have expressed concerns about the security review of AI-assisted contributions. This release brings new Vulkan and CUDA-based filters and a neural network backend, extending FFmpeg&\#x27;s multimedia processing capabilities for a wide range of platforms and formats.

telegram · zaihuapd · Aug 5, 10:32

**「Background」** FFmpeg is a widely used open-source multimedia framework for handling video, audio, and other media files. Version 9.0 introduces animated WebP decoding, new Vulkan and CUDA filters, and a Playdate video encoder, among other additions. The release also highlights the use of Anthropic’s Claude AI for backport identification, though the team notes it was not used for core development.

**「Impact」** FFmpeg 9.0 adds animated WebP decoding, Vulkan-accelerated ProRes RAW and v360 video filters, HE-AAC 960 decoding, and an ONNX Runtime DNN backend, enabling AI-powered video workflows and improved HDR metadata handling.

<details><summary>References</summary>
<ul>
<li><a href="https://www.phoronix.com/news/FFmpeg-9.0-Released">FFmpeg 9 . 0 Released With More Vulkan Acceleration, Animated ...</a></li>
<li><a href="https://www.heise.de/en/news/FFmpeg-9-0-WebP-in-GIF-out-11398216.html">FFmpeg 9 . 0 : WebP in, GIF out | heise online</a></li>
<li><a href="https://www.phoronix.com/news/FFmpeg-9.0-Released">FFmpeg 9.0 Released With More Vulkan Acceleration, Animated WebP &amp; More AMD AMF - Phoronix</a></li>
<li><a href="https://linuxiac.com/ffmpeg-9-0-released-with-animated-webp-decoding-and-new-hardware-acceleration/">FFmpeg 9.0 Released with Animated WebP Decoding and New Hardware Acceleration</a></li>
<li><a href="https://www.heise.de/en/news/FFmpeg-9-0-WebP-in-GIF-out-11398216.html">FFmpeg 9.0: WebP in, GIF out | heise online</a></li>

</ul>
</details>

**Tags**: `#ffmpeg`, `#multimedia`, `#release`, `#open-source`, `#ai-assisted-development`

---

<a id="item-tech-news-9"></a>
### [MLX Port Enables MiniMax-H3 Omni-Modal Video Generation on Apple Silicon](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 7.0/10

PipeNetwork released minimax-h3-mlx, a Python package that ports the recently released MiniMax-H3 omni-modal generative model to MLX for local execution on Apple Silicon. MiniMax-H3 accepts text, images, audio, and video inputs and can generate up to 15-second video clips with audio. Simon Willison successfully ran the model on an M5 Max MacBook Pro, generating a video from a text prompt after downloading approximately 115 GB of model files; the generation took just under 45 minutes. The output video was visually impressive, but the audio was incoherent speech due to a lack of prompt guidance for audio, highlighting the need for the separate prompting guide. The port makes a cutting-edge multimodal model available for local experimentation, albeit with significant hardware requirements.

rss · Simon Willison · Aug 4, 19:10

**「Background」** MLX is Apple&\#x27;s open-source machine learning framework optimized for Apple Silicon, enabling efficient local execution of large models. MiniMax-H3 is a new general-purpose, omni-modal generative system that can process and generate across text, image, audio, and video modalities. The minimax-h3-mlx package converts the original MiniMax-H3 model to run on MLX, making it accessible to developers with Macs equipped with Apple Silicon.

**「Impact」** Developers can now run MiniMax-H3&\#x27;s video generation locally on Apple Silicon, but the ~115 GB model footprint and 45-minute generation time for a 15-second clip on a high-end M5 Max may limit practical use without further optimization.

**Tags**: `#MLX`, `#multimodal`, `#video-generation`, `#MiniMax-H3`, `#Apple-Silicon`

---

<a id="item-tech-news-10"></a>
### [SpaceX to Exclusively Use NVIDIA Vera Rubin AI Architecture](https://wccftech.com/elon-musk-commits-spacex-exclusively-to-nvidia-gpus-citing-theyre-the-best/) ⭐️ 7.0/10

During SpaceX&\#x27;s first earnings call on August 4, Elon Musk announced that the company will run its AI services exclusively on NVIDIA systems, calling the Vera Rubin architecture the &quot;best AI compute architecture.&quot; SpaceX plans to deploy NVIDIA Vera Rubin NVL72 rack systems across global ground data centers and in space, targeting over 2 GW of AI compute capacity by the end of this year and nearly 10 GW by the end of 2027. The company also intends to use these systems for the &quot;Starmind&quot; satellite project, with launches expected next year to build orbital AI data centers, leveraging NVIDIA&\#x27;s space-grade Space-1 Vera Rubin modules for high-performance AI inference in orbit.

telegram · zaihuapd · Aug 5, 02:04

**「Background」** The Vera Rubin architecture is Nvidia’s next-generation AI computing platform, combining Rubin GPUs and Vera CPUs. SpaceX is collaborating with Nvidia to design the Starmind AI1 satellite payload, which will carry these components for datacenter-level compute in orbit. Starmind satellites are scheduled to begin launching next year, forming an orbital AI data center network.

**「Impact」** SpaceX&\#x27;s exclusive commitment and massive scale—eventually reaching 10 GW of AI compute—will likely accelerate NVIDIA&\#x27;s dominance in space-based AI infrastructure and drive the first large-scale orbital AI data centers through the Starmind project.

<details><summary>References</summary>
<ul>
<li><a href="https://www.blocktempo.com/spacex-exclusive-nvidia-ai-architecture-vera-rubin-space-data-center-starmind-2026/">SpaceX 獨家鎖定輝達 AI 架構，太空資料中心 Starmind 計劃明年啟動 | 動區動趨-最具影響力的區塊鏈新聞媒體</a></li>
<li><a href="https://x.com/SpaceX/status/2084723854534951218">SpaceX is partnering with @Nvidia to design the Starmind AI1 ...</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#NVIDIA`, `#AI infrastructure`, `#Vera Rubin`, `#satellite computing`

---

<a id="item-tech-news-11"></a>
### [Samsung, SK Hynix Test AMEC Etching Tools to Hedge Against US Export Controls](https://www.reuters.com/world/china/samsung-sk-hynix-test-chinese-chip-tools-hedge-against-us-risks-2026-08-05/) ⭐️ 7.0/10

Samsung and SK Hynix are reportedly testing Chinese semiconductor etching tools from AMEC for their plants in China, according to Reuters sources. The evaluations, which began about two years ago, aim to mitigate risks from tightening U.S. export controls on chip equipment. No decision has been made on large-scale deployment. Samsung denied the testing, while SK Hynix declined to comment. Chinese equipment is typically 20% to 30% cheaper, and adoption by major global chipmakers could significantly boost the credibility of Chinese suppliers in the $28 billion Chinese wafer fabrication equipment market.

telegram · zaihuapd · Aug 5, 04:32

**「Background」** The U.S. has steadily tightened export controls on advanced semiconductor manufacturing equipment to China, revoking Samsung and SK Hynix’s “validated end-user” status for their Chinese fabs in 2025 and replacing it with annual licenses. Both Korean firms operate large memory chip production facilities in China and fear that future restrictions might extend to the maintenance of existing Western equipment. Exploring Chinese alternatives like AMEC’s etching tools is a strategic hedge against such supply chain disruptions.

**「Impact」** If AMEC’s etching tools prove viable and are adopted by Samsung and SK Hynix, it would give a historic endorsement to Chinese semiconductor equipment makers, potentially accelerating their market share in China’s $28 billion wafer fabrication equipment market. However, the tests remain inconclusive, and no deployments have been committed.

**Tags**: `#semiconductors`, `#export controls`, `#supply chain`, `#chip manufacturing`, `#geopolitics`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Polymarket in talks for fundraising at over $20 billion valuation](https://www.cnbc.com/2026/08/04/polymarket-seeks-fundraising-round-at-more-than-20-billion-valuation.html) ⭐️ 8.0/10

Prediction market platform Polymarket is in talks for a fundraising round that would value the company at more than $20 billion, a person familiar with the matter confirmed to CNBC.

rss · CNBC Finance · Aug 4, 13:31

**「Background」** The talks follow a $15 billion valuation in an April funding round and the May launch of its regulated U.S. exchange.

**Tags**: `#Prediction markets`, `#Fundraising`, `#Valuation`, `#Polymarket`, `#Fintech`

---

<a id="item-finance-news-2"></a>
### [Goldman Sachs Equities Revenue Hits Record $7.42 Billion in Q2](https://www.cnbc.com/2026/08/01/goldman-traders-are-on-pace-for-a-record-year-a-close-up-look-at-how-theyre-doing-it.html) ⭐️ 8.0/10

Goldman Sachs&\#x27; equities division posted a record $7.42 billion in revenue last quarter, a 72% surge that handily beat analyst estimates.

rss · CNBC Finance · Aug 4, 19:38

**「Background」** The bank attributed the growth to a strategy of linking equities services with its investment banking and wealth management clients, as well as market volatility and the AI-driven capital expenditure cycle.

**「Impact」** The strong quarter puts Goldman on track for a record full-year trading revenue, according to executives.

**Tags**: `#Goldman Sachs`, `#equities trading`, `#earnings`, `#investment banking`, `#financial sector`

---

<a id="item-finance-news-3"></a>
### [DeepSeek Restarts Second Funding Round with Pre-Money Valuation of 500 Billion Yuan](https://finance.sina.com.cn/wm/2026-08-05/doc-inimfmyv1554159.shtml) ⭐️ 8.0/10

Multiple deal sources say DeepSeek has restarted its second funding round, aiming to raise 50 billion yuan at a pre-money valuation of about 500 billion yuan, a 43% increase from its first-round valuation.

telegram · zaihuapd · Aug 5, 02:46

**「Background」** DeepSeek is a Chinese AI startup, spun off from quantitative hedge fund High-Flyer, that gained attention for an AI model competitive with ChatGPT using less computing power.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nbcnews.com/tech/tech-news/deepseek-ai-model-china-chat-gpt-tech-stocks-what-know-rcna189604">What is DeepSeek, the Chinese AI startup shaking up tech stocks and spooking investors?</a></li>
<li><a href="https://techcrunch.com/2025/09/29/deepseek-everything-you-need-to-know-about-the-ai-chatbot-app/">DeepSeek: Everything you need to know about the AI chatbot app | TechCrunch</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#AI funding`, `#valuation`, `#China tech`, `#private equity`

---

<a id="item-finance-news-4"></a>
### [宇树科技科创板 IPO 启动询价](https://m.jrj.com.cn/madapter/stock/2026/08/05141758022724.shtml) ⭐️ 8.0/10

宇树科技科创板IPO启动询价，拟募资42亿元，对应市值超400亿元，2025年营收16.99亿元，净利润2.78亿元。

telegram · zaihuapd · Aug 5, 07:40

**Tags**: `#IPO`, `#科创板`, `#机器人`, `#企业融资`, `#财务数据`

---

<a id="item-finance-news-5"></a>
### [Citadel posts best month in years after acquiring discounted assets from collapsed AI hedge fund](https://www.cnbc.com/2026/08/05/ken-griffins-citadel-posts-best-month-in-years-after-scooping-up-situational-awareness-stocks.html) ⭐️ 7.0/10

Citadel&\#x27;s hedge funds posted strong gains in July, with the equities fund returning 14.2%—its best month ever—after purchasing discounted stocks from the collapsed AI-focused hedge fund Situational Awareness.

rss · CNBC Finance · Aug 5, 11:13

**「Background」** Situational Awareness, founded by Leopold Aschenbrenner, was forced to unwind positions after margin calls triggered by a sharp reversal in AI trades, allowing Citadel to buy its public-stock portfolio at a significant discount.

**「Impact」** The forced liquidation and Citadel&\#x27;s purchase helped stabilize AI stocks that had sharply declined, with names like Nebius and Micron rebounding in the final days of July as traders viewed the event as a clearing event that prompted short sellers to take profits.

**Tags**: `#hedge funds`, `#AI stocks`, `#forced liquidation`, `#Citadel`, `#market dislocation`

---

<a id="item-finance-news-6"></a>
### [Philadelphia Fed President Paulson says current rates sufficient, but open to recalibration](https://www.cnbc.com/2026/08/04/philadelphia-fed-president-paulson-content-with-current-rates-but-keeping-an-open-mind.html) ⭐️ 7.0/10

Philadelphia Fed President Anna Paulson said she is content with the current interest rate target of 3.5% to 3.75% and believes it is mildly restrictive enough to bring inflation down to 2% over time. She added that she would be open to recalibrating policy if inflation progress stalls.

rss · CNBC Finance · Aug 4, 17:49

**「Background」** The Federal Open Market Committee voted 9-3 last week to keep rates steady, with three dissenting members questioning whether the current level is sufficiently restrictive.

**Tags**: `#monetary policy`, `#federal reserve`, `#interest rates`, `#inflation`, `#FOMC`

---

<a id="item-finance-news-7"></a>
### [Jeff Bezos Files to Sell $4.1 Billion in Amazon Shares](https://www.cnbc.com/2026/08/04/jeff-bezos-just-filed-to-sell-4-billion-in-amazon-the-shares-are-falling.html) ⭐️ 7.0/10

Jeff Bezos filed a plan to sell about 15 million Amazon shares worth roughly $4.1 billion, according to a regulatory filing.

rss · CNBC Finance · Aug 4, 16:14

**「Background」** The filing came after Amazon’s stock hit a record high following strong quarterly earnings, and the sale was made under a prearranged trading plan established in November 2025.

**Tags**: `#insider-transactions`, `#Amazon`, `#Jeff-Bezos`, `#stock-market`, `#SEC-filing`

---