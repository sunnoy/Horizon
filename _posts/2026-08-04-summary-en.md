---
layout: default
title: "Horizon Summary: 2026-08-04 (EN)"
date: 2026-08-04
lang: en
---

> From 54 items, 18 important content pieces were selected

---

**Technology News**
1. [Swiftlet: Run 80B Qwen in 4.3 GB RAM on Mac, 35B on iPhone](#item-tech-news-1) ⭐️ 9.0/10
2. [FFmpeg 9.0 Brings Vulkan Filters and Animated WebP](#item-tech-news-2) ⭐️ 9.0/10
3. [Harness Engineering for Self-Improvement](#item-tech-news-3) ⭐️ 8.0/10
4. [OpenAI highlights ten advances in mathematics and theoretical computer science](#item-tech-news-4) ⭐️ 8.0/10
5. [Cloudflare Details KV Cache Quantization for Kimi and GLM Inference](#item-tech-news-5) ⭐️ 8.0/10
6. [LLMs make open-source code modification practically feasible](#item-tech-news-6) ⭐️ 8.0/10
7. [Kimi K3 Architecture: Compressed Memory, Attention Across Depth, and Latent Expert Routing](#item-tech-news-7) ⭐️ 8.0/10
8. [HP, ASUS, Acer begin using CXMT DRAM in non-US laptops](#item-tech-news-8) ⭐️ 8.0/10
9. [Trump Administration Drafts Ban on Chinese Optical Modules for AI Data Centers](#item-tech-news-9) ⭐️ 8.0/10
10. [China&\#x27;s First Mandatory National Standard for L3/L4 Autonomous Driving Released, Effective July 2027](#item-tech-news-10) ⭐️ 8.0/10
11. [LLMs Reward Expertise, Challenging Democratization Narrative](#item-tech-news-11) ⭐️ 7.0/10
12. [NeurIPS Reviewer: Only 1 of 12 Papers Provided Full Code, Proposes Desk Rejections](#item-tech-news-12) ⭐️ 7.0/10
13. [Huawei Scientist: Nvidia Chip Scaling Will Hit Physical Limit](#item-tech-news-13) ⭐️ 7.0/10
14. [Cloudflare Ditches Third-Party Security Tools, Uses $58/Month AI for Bug Bounties](#item-tech-news-14) ⭐️ 7.0/10

**Financial News**
1. [California diesel price jumps to $6.92 per gallon, threatening higher U.S. consumer prices](#item-finance-news-1) ⭐️ 9.0/10
2. [Google sets up $200 billion vendor financing structure for Anthropic AI chips](#item-finance-news-2) ⭐️ 9.0/10
3. [Polymarket in talks for funding round at over $20 billion valuation](#item-finance-news-3) ⭐️ 8.0/10
4. [Visa to acquire BioCatch for $2.4 billion in cash](#item-finance-news-4) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Swiftlet: Run 80B Qwen in 4.3 GB RAM on Mac, 35B on iPhone](https://github.com/leonickson1/Swiftlet) ⭐️ 9.0/10

Swiftlet, an open-source project, compresses large language models to run efficiently on consumer Apple hardware. It demonstrates a Qwen 80B model running in just 4.3 GB of RAM on a Mac, and a 35B model on an iPhone using 2.5 GB of RAM at approximately 1 token per second. This breakthrough in model compression enables on-device inference for models that previously required server-grade hardware, significantly lowering the barrier for local AI and opening possibilities for private, low-latency applications.

hackernews · leonickson · Aug 3, 16:54 · [Discussion](https://news.ycombinator.com/item?id=49158333)

**「Background」** Large language models with tens of billions of parameters typically require substantial GPU memory, making them impractical for consumer devices. Mixture-of-Experts \(MoE\) architectures reduce the active parameter count by selecting only a subset of experts for each token, and Swiftlet exploits this by streaming expert weights from SSD into RAM on demand, enabling inference on Apple hardware with much lower memory usage.

**「Impact」** This compression technique allows developers and users to run massive language models locally on iPhones and Macs, potentially enabling private, low-latency AI without cloud dependency.

**「Community Discussion」** Community members praised the project as a significant step toward practical on-device AI, noting that running a 35B model on an iPhone at 1 token per second is ‘insane work’ and speculating that Apple may be betting on such efficiency gains for future consumer LLMs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.devdigest.org/articles/swiftlet-run-80b-qwen-in-43gb-ram-on-mac-35b-on-iphone">Swiftlet: Run 80B Qwen in 4.3GB RAM on Mac, 35B on iPhone</a></li>

</ul>
</details>

**Tags**: `#on-device-inference`, `#model-compression`, `#llm`, `#open-source`, `#apple`

---

<a id="item-tech-news-2"></a>
### [FFmpeg 9.0 Brings Vulkan Filters and Animated WebP](https://github.com/FFmpeg/FFmpeg/blob/n9.0/RELEASE_NOTES) ⭐️ 9.0/10

FFmpeg 9.0 has been released as a major update to the multimedia framework. It adds Vulkan-based video filters including v360\_vulkan, along with an animated WebP decoder and demuxer. Hardware acceleration receives new AMF filters for HDR color conversion and frame rate conversion, plus VideoToolbox hwaccel for ProRes RAW and APV Vulkan decoding. The release also introduces LCEVC track muxing in MP4, a Playdate video encoder, and HE‑AAC 960 \(DAB+\) decoding, while removing CELT decoding support.

hackernews · gyan · Aug 4, 09:30 · [Discussion](https://news.ycombinator.com/item?id=49166202)

**「Background」** FFmpeg is a core open-source multimedia framework used for encoding, decoding, transcoding, and streaming audio and video. The Vulkan API provides low-level GPU acceleration, and FFmpeg 9.0 introduces new Vulkan-based filters and hardware acceleration, building on prior Vulkan video decoding work. Animated WebP is a format for animated images, newly supported for decoding and demuxing in this release.

**「Impact」** FFmpeg 9.0 bumps all core libraries to new major versions \(libavcodec and libavformat entering the 63 series\), requiring applications that link directly to these libraries to be recompiled for compatibility.

**「Community Discussion」** Hacker News commenters expressed gratitude for FFmpeg’s ongoing importance, with jbk sharing a detailed blog post about the release. One user noted a desire for Intel QSV encoding support on Windows laptops where the manufacturer disabled it in ACPI, currently only possible via FFmpeg on Linux.

<details><summary>References</summary>
<ul>
<li><a href="https://www.phoronix.com/news/FFmpeg-9.0-Released">FFmpeg 9.0 Released With More Vulkan Acceleration, Animated WebP &amp; More AMD AMF - Phoronix</a></li>
<li><a href="https://9to5linux.com/ffmpeg-9-0-lei-open-source-multimedia-framework-officially-released">FFmpeg 9.0 &quot;Lei&quot; Open-Source Multimedia Framework Officially Released - 9to5Linux</a></li>
<li><a href="https://linuxiac.com/ffmpeg-9-0-released-with-animated-webp-decoding-and-new-hardware-acceleration/">FFmpeg 9.0 Released with Animated WebP Decoding and New Hardware Acceleration</a></li>
<li><a href="https://www.linuxcompatible.org/story/ffmpeg-90-lei-released-library-bumps-and-dev-impact">FFmpeg 9.0 Lei Released: Library Bumps and Dev Impact</a></li>
<li><a href="https://www.warp2search.net/story/ffmpeg-90-lei-released-library-bumps-and-dev-impact">FFmpeg 9.0 Lei Released: Library Bumps and Dev Impact</a></li>

</ul>
</details>

**Tags**: `#ffmpeg`, `#multimedia`, `#open-source`, `#release`, `#video-processing`

---

<a id="item-tech-news-3"></a>
### [Harness Engineering for Self-Improvement](https://lilianweng.github.io/posts/2026-07-04-harness/) ⭐️ 8.0/10

Lilian Weng’s in-depth analysis surveys recent research on recursive self-improvement \(RSI\), self-improving agents, and continual learning. The post organizes work on auto-research, evolutionary program search, model self-play, synthetic data, and test-time training around a unifying question, providing a critical framework for understanding progress toward agents that can improve their own capabilities. It highlights both the promise of these approaches and the practical challenges, such as models finding shortcuts that undermine genuine improvement, and draws attention to the broader vision of continual learning that matches the RSI ambition. The Hacker News discussion \(164 points, 30 comments\) reflects strong community interest in this synthesis, which does not itself present new experimental results but offers a valuable reference for AI practitioners and researchers.

hackernews · tosh · Aug 4, 06:17 · [Discussion](https://news.ycombinator.com/item?id=49164896)

**「Recursive Self-Improvement and Harness Engineering」** The notion of recursive self-improvement \(RSI\) originates from I.J. Good’s 1965 speculation about an “ultraintelligent machine” that could design better versions of itself, a concept later formalized as a feedback loop where an AI uses its current intelligence to enhance its own capabilities. In the context of large language models, “harness engineering” refers to the system layer—comprising planning, tool use, memory, and evaluation—that orchestrates the base model, and is considered a promising near-term path toward realizing RSI.

**「Impact」** The synthesis provides AI practitioners a structured framework for evaluating and comparing self-improvement techniques, though it does not introduce new experimental results.

**「Community Discussion」** Commenters generally praised the post’s depth, while some noted the challenge of models exploiting shortcuts in self-improvement and others highlighted the shift toward prompt and code-based training paradigms beyond traditional weight updates.

<details><summary>References</summary>
<ul>
<li><a href="https://lilianweng.github.io/posts/2026-07-04-harness/">Harness Engineering for Self-Improvement | Lil&#x27;Log</a></li>
<li><a href="https://www.alphaxiv.org/abs/2607.harness-3">Harness Engineering for Self-Improvement | alphaXiv</a></li>

</ul>
</details>

**Tags**: `#AI`, `#recursive-self-improvement`, `#machine-learning`, `#AI-safety`, `#self-improving-agents`

---

<a id="item-tech-news-4"></a>
### [OpenAI highlights ten advances in mathematics and theoretical computer science](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 8.0/10

OpenAI published a blog post detailing ten recent advances in mathematics and theoretical computer science, many of which leverage AI to solve complex problems. The post ignited a vibrant discussion on Hacker News, with commenters debating the accelerating pace at which AI is transforming these fields. While the specific advances were not enumerated in the discussion, the response underscores a growing consensus that AI is becoming a practical and increasingly powerful tool for mathematical research.

hackernews · milkshakes · Aug 3, 16:27 · [Discussion](https://news.ycombinator.com/item?id=49157930)

**「Background」** OpenAI recently published a collection of solutions to ten long-standing open problems in mathematics and theoretical computer science, achieved by an internal AI model codenamed &quot;Astra&quot; \(the anticipated next major model\). The results span areas such as geometry, cryptography, and complexity, and were formalized in the Lean 4 proof assistant, with OpenAI reporting a cost of under $2,000 per problem at GPT-5.6 Sol token prices. This announcement demonstrates the growing capability of large language models to assist in mathematical research.

**「Impact」** The compilation of advances demonstrates that AI is now capable of contributing meaningfully to high-level mathematics and theoretical computer science, potentially accelerating research and altering traditional workflows for mathematicians and computer scientists.

**「Community Discussion」** Commenters broadly agree that AI&\#x27;s impact on mathematics is undeniable, with LLMs making proof generation and verification more computable. Some note that while AI can quickly disprove conjectures through brute force, it still lacks the intuition to formulate original conjectures, leaving a role for human insight.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/ten-advances-in-mathematics/">Ten advances in mathematics and theoretical computer science | OpenAI</a></li>
<li><a href="https://simonwillison.net/2026/Aug/1/ten-advances-in-mathematics/">Ten advances in mathematics and theoretical computer science</a></li>

</ul>
</details>

**Tags**: `#AI`, `#mathematics`, `#theoretical-computer-science`, `#OpenAI`, `#research`

---

<a id="item-tech-news-5"></a>
### [Cloudflare Details KV Cache Quantization for Kimi and GLM Inference](https://blog.cloudflare.com/smaller-faster-safer-models/) ⭐️ 8.0/10

Cloudflare published a blog post detailing their approach to running the Kimi and GLM large language models at scale, focusing on KV cache quantization. The post explains the performance and cost trade-offs of this technique and openly discusses its impact on output quality. Such transparency is notable because many AI inference providers silently apply KV cache quantization, which can degrade quality more than weight quantization. Cloudflare&\#x27;s insights provide valuable guidance for practitioners optimizing inference deployments.

hackernews · ascorbic · Aug 3, 17:08 · [Discussion](https://news.ycombinator.com/item?id=49158581)

**「Background」** Large language models store attention states in a key-value \(KV\) cache that grows with sequence length, and reducing this memory footprint via quantization \(e.g., FP8\) is critical for serving long-context models. Moonshot AI&\#x27;s Kimi and Zhipu AI&\#x27;s GLM are frontier mixture-of-experts \(MoE\) models known for their long context windows, making them especially memory-hungry during inference. Cloudflare&\#x27;s post describes techniques to quantize KV caches, compress model weights, and protect cache integrity to run these models at scale on Workers AI.

**「Impact」** AI inference engineers can now reference Cloudflare&\#x27;s publicly shared trade-offs to better understand the real-world effects of KV cache quantization, aiding their own model deployment decisions.

**「Community Discussion」** Many commenters appreciate the transparency, but some express concern that the testing was limited to only one model family and that pricing information is not easily accessible. Others question the choice of int4 quantization, suggesting alternatives like nf4 might be more effective.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/smaller-faster-safer-models/">Smaller, faster, safer: running Kimi and GLM at scale</a></li>

</ul>
</details>

**Tags**: `#kimi`, `#glm`, `#kv-cache-quantization`, `#cloudflare`, `#ai-inference`

---

<a id="item-tech-news-6"></a>
### [LLMs make open-source code modification practically feasible](https://simonwillison.net/2026/Aug/3/devtools-must-be-open-source-exedev/#atom-everything) ⭐️ 8.0/10

In a commentary on the Hacker News discussion &quot;Devtools must be open source,&quot; Simon Willison argues that large language models are making the original open-source promise—the freedom to examine and modify software—practically achievable for more developers. He notes that while the theoretical freedom existed, the time investment required to understand and compile code deterred most people, but LLMs like Claude and Codex now allow him to clone repositories, explain code, and build projects with nearly zero personal effort. Willison reports using these tools daily to quickly understand how software works, and he sees a path toward routinely modifying the tools he uses, a shift that was unimaginable a year ago.

rss · Simon Willison · Aug 3, 15:30

**「The original argument and the practical barrier」** The article &\#x27;Devtools must be open source \(exe.dev\)&\#x27; argues that open source code is essential for personalizing AI agents \(tool-1-1\). Traditionally, the promise of open source—the freedom to examine and modify software—has been more theoretical for most users, even expert programmers, because the time investment required to understand and compile unfamiliar codebases is often prohibitive \(tool-1-2\).

**「Impact」** For developers, LLM-assisted workflows could significantly lower the barrier to personally inspecting and adapting open-source codebases, potentially increasing the practical value and adoption of open-source devtools.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.exe.dev/devtools-must-be-open-source">Devtools must be open source - exe.dev blog</a></li>
<li><a href="https://simonwillison.net/2026/Aug/3/devtools-must-be-open-source-exedev/">Comment: Devtools must be open source (exe.dev)</a></li>

</ul>
</details>

**Tags**: `#open source`, `#large language models`, `#developer tools`, `#software engineering`, `#AI`

---

<a id="item-tech-news-7"></a>
### [Kimi K3 Architecture: Compressed Memory, Attention Across Depth, and Latent Expert Routing](https://newsletter.semianalysis.com/p/kimi-k3-the-manos-the-mythos-the) ⭐️ 8.0/10

In a deep technical analysis, Semianalysis examines the Kimi K3 model architecture, focusing on three novel components: compressed memory, attention across depth, and latent expert routing. The article, authored by Kimbo Chen, details how these innovations are integrated to improve inference performance. The compressed memory mechanism reduces the memory footprint of long-context processing, while attention across depth enables information flow between layers without standard sequential dependencies. Latent expert routing dynamically selects specialized sub-networks, further boosting efficiency. The analysis also covers the resulting inference latency and throughput characteristics, positioning Kimi K3 as a significant step in efficient large-scale model design.

rss · Semianalysis · Aug 3, 19:42

**「Background」** Large language models have increasingly adopted mixture-of-experts \(MoE\) and optimized attention mechanisms to scale efficiently. Kimi K3, a 2.8-trillion-parameter model, introduces Kimi Delta Attention \(KDA\) and Attention Residuals \(AttnRes\) to enhance information flow across sequence length and depth, along with a Stable LatentMoE routing strategy and Gated Multi-head Latent Attention for memory-efficient inference.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://huggingface.co/blog/ResterChed/kimi-k3-model-overview-mxfp4-quantization-open-wei">Kimi K 3 Model Overview: 2.8T Parameters, MXFP4 Quantization, and...</a></li>

</ul>
</details>

**Tags**: `#architecture`, `#deep-learning`, `#AI`, `#models`, `#inference`

---

<a id="item-tech-news-8"></a>
### [HP, ASUS, Acer begin using CXMT DRAM in non-US laptops](https://asia.nikkei.com/business/china-tech/hp-asus-and-acer-begin-using-cxmt-chips-amid-memory-shortage) ⭐️ 8.0/10

HP, ASUS, and Acer have started using China&\#x27;s ChangXin Memory Technologies \(CXMT\) DRAM chips in a limited number of low-end laptops for non-US markets, after completing qualification in mid-2023. The move comes amid a severe memory shortage driven by AI infrastructure demand, pushing PC vendors to diversify beyond the dominant trio of Samsung, Micron, and SK Hynix. The adoption remains cautious, with CXMT prioritizing most of its output for Chinese clients like Huawei and the company being on a Pentagon list of Chinese military-linked entities, which complicates use by US firms. CXMT&\#x27;s recent IPO on the Shanghai STAR Market saw its shares surge over 465% on the first day, giving it a market capitalization exceeding that of Intel. IDC estimates that global PC shipments could fall more than 11% this year due to the memory crunch.

telegram · zaihuapd · Aug 4, 07:12

**「Background」** The global DRAM market is overwhelmingly controlled by Samsung, SK Hynix, and Micron, which together hold over 90% share. CXMT is China&\#x27;s leading domestic DRAM manufacturer but has historically been absent from major PC brands due to performance gaps, limited capacity, and geopolitical sensitivities, including its inclusion on a U.S. Department of Defense list of Chinese military companies. The severe memory shortage triggered by AI-driven demand has now prompted some PC makers to test Chinese alternatives in non-US products.

**「Impact」** The cautious inclusion of CXMT DRAM in non-US low-end laptops by HP, ASUS, and Acer creates a small but notable diversification of the memory supply chain, potentially easing shortages in specific segments, though the limited volume and geopolitical barriers mean the dominant suppliers&\#x27; positions are not immediately threatened.

**Tags**: `#semiconductor`, `#DRAM`, `#supply-chain`, `#China-tech`, `#AI-infrastructure`

---

<a id="item-tech-news-9"></a>
### [Trump Administration Drafts Ban on Chinese Optical Modules for AI Data Centers](https://www.reuters.com/world/trump-administration-drafting-ban-chinese-data-center-devices-sources-say-2026-08-04/) ⭐️ 8.0/10

The Trump administration is drafting a ban on imports of new Chinese optical modules for data centers, with the Federal Communications Commission \(FCC\) aiming to issue and enact the rule this year. The move targets components critical to AI infrastructure, citing concerns over data theft, malware, and service disruption. The ban, if implemented, would significantly impact Zhongji Innolight, which holds a 27% global market share in optical modules. Chinese embassy vows to take necessary measures to protect its interests. The restriction follows earlier FCC bans on Chinese-made drones, routers, robots, and inverters.

telegram · zaihuapd · Aug 4, 11:29

**「Background」** Optical modules are essential for high-bandwidth data transmission in AI data centers, converting electrical signals to light. The US has previously imposed FCC import bans on Chinese drones, routers, robots, and inverters over national security concerns.

**「Impact」** The ban, if enacted, would disrupt the AI data center supply chain and directly impact Zhongji Innolight, the world&\#x27;s largest optical module supplier with a 27% market share. The measure could still be modified or shelved, sources cautioned.

**Tags**: `#trade ban`, `#optical modules`, `#AI infrastructure`, `#China-US technology`, `#data center hardware`

---

<a id="item-tech-news-10"></a>
### [China&\#x27;s First Mandatory National Standard for L3/L4 Autonomous Driving Released, Effective July 2027](https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html) ⭐️ 8.0/10

China&\#x27;s Ministry of Industry and Information Technology has approved the mandatory national standard GB 44721—2026, &\#x27;Intelligent Connected Vehicle—Autonomous Driving System Safety Requirements,&\#x27; which will take effect on July 1, 2027. This is the country&\#x27;s first mandatory standard for SAE Level 3 \(conditional\) and Level 4 \(high\) automated driving systems, applicable to M \(passenger\) and N \(cargo\) vehicles but excluding automatic parking. The standard converts the previous 2024 recommended specification into a mandatory one and establishes a safety framework covering enterprise lifecycle assurance, system dynamic driving performance, human-machine interaction and user notification, and multi-dimensional testing. It mandates that the autonomous driving system must achieve at least the safety level of a competent and attentive human driver.

telegram · zaihuapd · Aug 4, 13:06

**「Background」** L3 \(conditional automation\) and L4 \(high automation\) are SAE-defined levels where the vehicle can handle most driving tasks, but L3 still requires a human driver ready to take over while L4 can operate without human intervention in specific conditions. China’s standardization system distinguishes between recommended national standards \(GB/T\) and mandatory national standards \(GB\); this new standard upgrades the previous 2024 recommended version to a compulsory one, meaning all applicable M-category \(passenger\) and N-category \(goods\) vehicles with L3/L4 systems must comply. The standard sets a baseline that the automated driving system must perform at least as safely as a competent, attentive human driver.

**「Impact」** Automakers must align their L3/L4 system designs with the mandatory safety and testing requirements by July 2027, directly shaping product development roadmaps and certification processes in China.

**Tags**: `#自动驾驶`, `#法规标准`, `#L3/L4`, `#智能网联汽车`, `#中国`

---

<a id="item-tech-news-11"></a>
### [LLMs Reward Expertise, Challenging Democratization Narrative](https://www.seangoedecke.com/llms-reward-expertise/) ⭐️ 7.0/10

An article by Sean Goedecke argues that large language models amplify deep domain expertise rather than universally democratizing software development. The piece contends that effective use of LLMs requires careful prompting, precise technical vocabulary, and the ability to evaluate and refine outputs, skills typically held by experienced developers. Anecdotal evidence from a commenter&\#x27;s experiment with a novice using an LLM supported this, showing that the AI produced plausible but flawed code that required expert intervention to correct. The discussion frames LLMs as a mirror that reflect the user&\#x27;s own knowledge, where experts thrive and novices struggle, challenging the notion that anyone can build robust software with simple prompts.

hackernews · MaxMussio · Aug 3, 21:13 · [Discussion](https://news.ycombinator.com/item?id=49161518)

**「Background」** The prevailing narrative around large language models \(LLMs\) is that they democratize software development by enabling anyone to generate code, regardless of expertise. However, Sean Goedecke&\#x27;s July 2026 article argues that LLMs actually amplify existing domain expertise, as they require careful prompting and judgment to produce useful results.

**「Impact」** Developers with deep domain expertise gain significantly more from LLM assistance, while those without relevant skills may still need expert guidance to avoid subtle errors, tempering expectations of a no-code revolution.

**「Community Discussion」** Commenters largely agree, comparing LLMs to amplifying mirrors and prompt engineering to medical history taking, while others call for formal studies to rule out confirmation bias and note that precise, structured prompts yield better results.

<details><summary>References</summary>
<ul>
<li><a href="https://www.seangoedecke.com/llms-reward-expertise/">LLMs reward expertise - seangoedecke.com</a></li>

</ul>
</details>

**Tags**: `#LLMs`, `#expertise`, `#AI-assisted development`, `#software engineering`, `#prompting`

---

<a id="item-tech-news-12"></a>
### [NeurIPS Reviewer: Only 1 of 12 Papers Provided Full Code, Proposes Desk Rejections](https://www.reddit.com/r/MachineLearning/comments/1vei12v/its_time_to_desk_reject_papers_that_dont_include/) ⭐️ 7.0/10

A machine learning researcher, after reviewing 12 papers for three major conferences this year including NeurIPS, reports that only one provided full code to reproduce the entire training pipeline. Four papers offered partial code, while seven had none; among the five with any code, three contained bugs that invalidated the reported results. The author argues that the current incentive structure discourages code sharing during review, as it only increases the risk of rejection, and proposes that conference organizers should desk reject submissions that lack fully reproducible code. This firsthand account underscores a serious reproducibility crisis and a concrete policy proposal for top-tier ML venues.

reddit · r/MachineLearning · /u/Flaky-Ambition5900 · Aug 3, 16:17

**「Reproducibility Expectations at NeurIPS」** NeurIPS already maintains a Code of Ethics and a submission checklist that highlight reproducibility as a research integrity concern. However, mandatory provision of full, runnable code is not a universal requirement for all papers, and some tracks only encourage code submission or ask for justification when it is absent.

<details><summary>References</summary>
<ul>
<li><a href="https://neurips.cc/public/EthicsGuidelines">NeurIPS Code of Ethics</a></li>
<li><a href="https://neurips.cc/Conferences/2026/EvaluationsDatasetsReviewerGuidelines">Evaluations and Datasets 2026 Reviewing Guidelines - neurips.cc</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#reproducibility`, `#academic publishing`, `#code review`, `#open science`

---

<a id="item-tech-news-13"></a>
### [Huawei Scientist: Nvidia Chip Scaling Will Hit Physical Limit](https://www.bloomberg.com/news/articles/2026-08-04/huawei-s-top-scientist-warns-of-chip-limit-nvidia-will-soon-face) ⭐️ 7.0/10

Huawei&\#x27;s chief semiconductor scientist Liao Heng warned in a rare late-July interview that the industry&\#x27;s approach of adding more compute chips and high-bandwidth memory will eventually hit a physical limit, after which an &\#x27;avalanche&\#x27; could occur. He presented Huawei&\#x27;s &\#x27;Dao&\#x27;s Law&\#x27; as an alternative scaling path, with the first LogicFolding-based phone chip set to debut later this year. Liao also noted that the U.S. and Chinese semiconductor industries are diverging into two independent ecosystems.

telegram · zaihuapd · Aug 4, 08:04

**「背景」** Current semiconductor scaling, often described by Moore’s Law, is approaching physical limits as shrinking transistors further becomes increasingly difficult. Huawei’s alternative ‘Dao’s Law’ \(τ scaling\) replaces geometric scaling with a time-scaling approach, using a three-dimensional ‘LogicFolding’ architecture to shorten signal paths and boost effective transistor density without relying exclusively on process node shrinks.

**「Impact」** The announcement signals Huawei&\#x27;s active pursuit of an alternative chip architecture to bypass approaching physical limits, potentially reducing its dependence on current scaling methods, though the technology remains unproven.

<details><summary>References</summary>
<ul>
<li><a href="https://csdnnews.blog.csdn.net/article/details/162423752">超越炒作：科普 华 为 LogicFolding 芯 片 背后残酷的数学与物理-CSDN...</a></li>
<li><a href="https://www.bnext.com.tw/article/91054/huawei-tau-scaling-law-logicfolding-post-moore-era-chip-design">挑戰台積電？ 華為推「韜 定 律 」與 LogicFolding 架構，宣稱2031...</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#AI hardware`, `#chip scaling`, `#Huawei`, `#US-China tech divide`

---

<a id="item-tech-news-14"></a>
### [Cloudflare Ditches Third-Party Security Tools, Uses $58/Month AI for Bug Bounties](https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600) ⭐️ 7.0/10

Cloudflare has largely replaced third-party security tools with over 200 self-built AI agents, the company&\#x27;s chief security officer revealed. The agents are partly written with AI assistance and handle tasks such as deduplicating and assessing bug bounty reports. For this, Cloudflare uses Anthropic&\#x27;s Claude Sonnet at a cost of just $58 per month, compared to an estimated $200,000 per month if it had used a security-specific model like Mythos. The company also attributed the layoff of 1,100 employees to AI-driven automation. Cloudflare&\#x27;s CSO cautioned other organizations against trying to replicate the approach, stating that most banks should not develop all their own software.

telegram · zaihuapd · Aug 4, 09:24

**「Background」** Bug bounty programs invite security researchers to submit vulnerability reports, which companies must triage to identify duplicates and assess severity before remediation. Traditionally, organizations rely on a mix of third-party security tools and manual review, while specialized AI models can be expensive. Cloudflare&\#x27;s move to a general-purpose large language model for this task reflects a broader trend of using foundation models for security operations.

**「Impact」** Cloudflare&\#x27;s in-house automation drastically reduces the cost of bug bounty triage, but the company&\#x27;s warning highlights that the approach requires deep engineering resources, making it impractical for most organizations.

**Tags**: `#security`, `#AI`, `#bug-bounty`, `#Cloudflare`, `#automation`

---

## Financial News

<a id="item-finance-news-1"></a>
### [California diesel price jumps to $6.92 per gallon, threatening higher U.S. consumer prices](https://www.cnbc.com/2026/08/03/californias-diesel-prices-have-jumped-since-the-iran-war-started-with-ripple-effects-across-the-country.html) ⭐️ 9.0/10

California&\#x27;s average diesel price rose to $6.92 per gallon, up from $5.10 before the Iran war began, amid a global diesel shortage of about 8% of daily demand, according to Lipow Oil Associates. The shortage is driven by the Iran war and Ukrainian strikes on Russian refineries.

rss · CNBC Finance · Aug 3, 19:20

**「Background」** The Iran war, now in its sixth month, has closed the Strait of Hormuz—a key oil transit route—and combined with Ukrainian attacks on Russian refineries, has created a global diesel shortage that Lipow Oil Associates estimates at 8% of demand.

**「Impact」** Higher freight costs for goods transported through California&\#x27;s ports, which handle nearly one-third of U.S. container imports and exports, could raise consumer prices for everyday products nationwide.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2026_Iran_war_fuel_crisis">2026 Iran war fuel crisis - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#diesel prices`, `#Iran war`, `#supply chain`, `#energy markets`, `#California economy`

---

<a id="item-finance-news-2"></a>
### [Google sets up $200 billion vendor financing structure for Anthropic AI chips](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 9.0/10

Google has set up a vendor financing structure worth about $200 billion to supply AI chips and infrastructure to Anthropic, with an initial $35 billion hardware purchase completed in June, the Financial Times reports.

telegram · zaihuapd · Aug 4, 10:52

**「Background」** The structure, modeled after aircraft vendor financing, involves Broadcom, Apollo, Blackstone and Morgan Stanley, and shares risk because Anthropic does not have a credit rating.

**Tags**: `#AI infrastructure`, `#Anthropic`, `#Google`, `#vendor financing`, `#TPU`

---

<a id="item-finance-news-3"></a>
### [Polymarket in talks for funding round at over $20 billion valuation](https://www.cnbc.com/2026/08/04/polymarket-seeks-fundraising-round-at-more-than-20-billion-valuation.html) ⭐️ 8.0/10

Prediction market platform Polymarket is in talks for a fundraising round that would value it at more than $20 billion, a person familiar with the matter confirmed.

rss · CNBC Finance · Aug 4, 13:31

**「Background」** The talks follow a previous funding round in April that valued Polymarket at $15 billion and the launch of its regulated U.S. exchange in May.

**Tags**: `#prediction markets`, `#venture capital`, `#valuation`, `#Polymarket`, `#private fundraising`

---

<a id="item-finance-news-4"></a>
### [Visa to acquire BioCatch for $2.4 billion in cash](https://www.cnbc.com/2026/08/03/visa-buys-biocatch-fraud-detection.html) ⭐️ 7.0/10

Visa said it is acquiring fraud detection startup BioCatch for $2.4 billion in cash, with the deal expected to close by the end of its fiscal second quarter in 2027.

rss · CNBC Finance · Aug 3, 16:44

**「Background」** The acquisition comes as Visa estimates that scams and account takeovers cost the global economy over $1 trillion annually, driven by a surge in generative AI-powered attacks.

**Tags**: `#Mergers and Acquisitions`, `#Cybersecurity`, `#Fraud Detection`, `#Financial Technology`, `#Visa`

---