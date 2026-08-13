---
layout: default
title: "Horizon Summary: 2026-08-13 (EN)"
date: 2026-08-13
lang: en
---

> From 41 items, 16 important content pieces were selected

---

**Technology News**
1. [Qwen3.8-2.4T: 2.4T Parameter MoE Model Released](#item-tech-news-1) ⭐️ 9.0/10
2. [DeepMind Unveils SL2T Sign Language to Text Model, Debuts on Pixel 11](#item-tech-news-2) ⭐️ 9.0/10
3. [DeepSeek V4-Pro Open Weights and Harness Tool Released](#item-tech-news-3) ⭐️ 9.0/10
4. [Tailscale finds and fixes 16-year-old SQLite WAL race condition bug](#item-tech-news-4) ⭐️ 8.0/10
5. [Grok 4.6: Performance and API Controversy](#item-tech-news-5) ⭐️ 8.0/10
6. [Adam&\#x27;s Per-Coordinate Adaptivity Breaks Low-Rank Bias in Factored Models](#item-tech-news-6) ⭐️ 8.0/10
7. [Zed introduces Delta real-time collaborative multiplayer editing with AI](#item-tech-news-7) ⭐️ 7.0/10
8. [HTML over WebSockets for Real-Time SPAs with Minimal JS](#item-tech-news-8) ⭐️ 7.0/10
9. [Chrome JPEG optimization alters tiny image appearance](#item-tech-news-9) ⭐️ 7.0/10
10. [AI Coding Over-Reliance Risks Unmaintainable Codebases, Warns Engineer](#item-tech-news-10) ⭐️ 7.0/10
11. [City2Graph: Python library for heterogeneous graph neural networks in urban systems](#item-tech-news-11) ⭐️ 7.0/10
12. [Trump signs memo allowing private companies to conduct overseas surveillance and cyber attacks](#item-tech-news-12) ⭐️ 7.0/10

**Financial News**
1. [Chinese chipmaker YMTC jumps to third in global NAND memory shipments](#item-finance-news-1) ⭐️ 8.0/10
2. [EVs account for 65.1% of China&\#x27;s July car sales as overall market shrinks](#item-finance-news-2) ⭐️ 8.0/10
3. [CME Group to Launch AI Computing Power Futures Contracts](#item-finance-news-3) ⭐️ 8.0/10
4. [China&\#x27;s Economic Slowdown Pushes Gig Workers to 53 Million, Oversupply Squeezes Incomes](#item-finance-news-4) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Qwen3.8-2.4T: 2.4T Parameter MoE Model Released](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

Qwen released Qwen3.8-2.4T, a massive Mixture-of-Experts model with 2.4 trillion total parameters and 95 billion active parameters per token. The model card claims performance rivaling top models such as Opus 4.8 and Fable 5, making it a significant competitor to models like Kimi k3 and DeepSeek V4-Pro-0813. Initial releases are in bf16 \(4.9 TB\) and FP8 formats, with no official QAT int4 quantization, though third-party 1-bit quantized versions reduce the size to ~397 GB. The license permits free internal use or revenue under $50 million per year, with restrictions for larger-scale serving. The open-weight variant lacks vision input, 1M context length, and built-in tools that are available in the Qwen3.8-Max version.

hackernews · Philpax · Aug 12, 15:01 · [Discussion](https://news.ycombinator.com/item?id=49273478)

**「Background」** Qwen3.8-2.4T-A95B is a Mixture-of-Experts \(MoE\) large language model with 2.4 trillion total parameters but only 95 billion active per token, a design that reduces inference cost while maintaining large capacity. It is the first open-weight release of a Qwen-Max-class model, previously only available through Alibaba&\#x27;s API, and builds on the Qwen3.5 architecture with significant improvements in coding, reasoning, and agentic tasks.

**「Impact」** The open-weight Qwen3.8-2.4T&\#x27;s 4.9 TB BF16 footprint and restrictive commercial license \(free only for internal use or revenue under $50M\) mean that only well-funded teams can deploy it at full precision, while the absence of vision and 1M context support \(present in the Max version\) limits its utility for multimodal tasks without further model development.

**「Community Discussion」** Commenters express excitement about the model&\#x27;s performance potential and the practicality of quantized versions fitting into consumer hardware, but note concerns about the lack of official quantization and the missing features \(vision, extended context\) in the open-weight release. Comparisons to Kimi k3 and DeepSeek V4-Pro-0813 are common, and some speculate that affordable hardware for running the full model at speed may not arrive until around 2040.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B">Qwen/Qwen3.8-2.4T-A95B · Hugging Face</a></li>
<li><a href="https://developer.nvidia.com/blog/serve-qwen3-8-2-4t-a95b-a-2-4t-parameter-model-with-configurable-reasoning-on-nvidia-gb300-nvl72/">Serve Qwen3.8-2.4T-A95B, a 2.4T-Parameter Model, with Configurable Reasoning on NVIDIA GB300 NVL72 | NVIDIA Technical Blog</a></li>
<li><a href="https://www.eesel.ai/blog/qwen38-max-review">Qwen 3 . 8 Max review: Alibaba&#x27;s 2 . 4 T flagship, tested (2026) | eesel AI</a></li>

</ul>
</details>

**Tags**: `#qwen`, `#large language model`, `#MoE`, `#AI`, `#machine learning`

---

<a id="item-tech-news-2"></a>
### [DeepMind Unveils SL2T Sign Language to Text Model, Debuts on Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 9.0/10

DeepMind has introduced SL2T, a large-scale multilingual sign language to text model, trained on over 100,000 hours of data across 50+ sign languages. The model achieves a 70 BLEURT zero-shot score on the FLEURS-ASL benchmark, significantly surpassing prior records. For privacy, it processes only body keypoints rather than raw video. SL2T is first deployed in consumer products on the Pixel 11, appearing in Gboard and Live Transcribe for American Sign Language to English translation. This marks the first integration of such technology into a mainstream device, with plans to expand to more languages and devices.

telegram · zaihuapd · Aug 13, 08:55

**「Background」** Sign language translation has been limited by data scarcity and privacy concerns, as most models require raw video. DeepMind&\#x27;s approach uses only body keypoints to preserve privacy, and the model is trained on a diverse dataset of over 50 sign languages. The deployment on Pixel 11 represents a shift from research to a practical accessibility tool.

**「Impact」** For ASL users, Pixel 11 now offers real-time sign language to text translation in keyboard and live captioning, providing a practical, privacy-preserving communication tool; this integration could set a precedent for broader adoption of sign language AI across Android devices.

**Tags**: `#sign language`, `#AI`, `#accessibility`, `#DeepMind`, `#machine learning`

---

<a id="item-tech-news-3"></a>
### [DeepSeek V4-Pro Open Weights and Harness Tool Released](https://www.npmjs.com/package/@deepseek-ai/dsh) ⭐️ 9.0/10

DeepSeek has released open weights for its V4-Pro-0813 model and introduced a new plugin-based harness tool called DSH \(DeepSeek Harness\), which is available on npm and GitHub and driven by the Cordis framework. The V4-Pro formal version is also now live on the API, mobile app, and web, with support for three thinking modes \(low, high, max\) and native Responses API format for Codex compatibility. API pricing will shift to peak/off-peak rates, with off-peak costing half the peak rate, effective from August 17, 2026. The open weights allow local deployment and further customization, while the harness tool simplifies experimentation and deployment through its plugin architecture.

telegram · zaihuapd · Aug 13, 12:39

**「Background」** DeepSeek V4 Pro is a large-scale mixture-of-experts \(MoE\) model that was previewed in April 2026 with open-weight releases under the MIT license. The “0813” suffix on the current build marks the general-availability \(GA\) version that concludes the preview period, making it the stable flagship model for the V4 series. The accompanying DeepSeek Harness \(DSH\) tool adopts a plugin-based architecture driven by Cordis, designed to simplify deployment and experimentation with the weights.

**「Impact」** Machine learning engineers can now run DeepSeek-V4-Pro locally with open weights and leverage the DSH plugin system for flexible deployment, while API users will benefit from reduced off-peak pricing starting in August 2026.

**「Community Discussion」** Reactions are mixed: some users are disappointed compared to the V4 Flash 0731 model, which they found more capable for their interactive tasks, while others report positive results in complex simulations and note that the new model found significant gains without introducing new issues.

<details><summary>References</summary>
<ul>
<li><a href="https://www.unite.ai/deepseek-ships-v4-pro-as-its-flagship-model-leaves-preview/">DeepSeek Ships V4 Pro as Its Flagship Model Leaves Preview – Unite.AI</a></li>
<li><a href="https://lovableapp.org/blog/deepseek-v4-pro-0813">DeepSeek V4 Pro 0813 (2026): Complete Guide to Pricing, Benchmarks &amp; How It Stacks Up Against Fable 5 | Lovable APP Blog</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#AI`, `#open-source`, `#model weights`, `#ML`

---

<a id="item-tech-news-4"></a>
### [Tailscale finds and fixes 16-year-old SQLite WAL race condition bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 8.0/10

Tailscale discovered and fixed a 16-year-old race condition bug in SQLite&\#x27;s Write-Ahead Log \(WAL\) mode. The bug could cause database corruption when multiple connections were used with the same database, even though a single-writer design was intended. Tailscale funded the development of an open-source SQLite VFS shim to help isolate the race condition, which will aid in tracking down similar bugs in the future. The fix highlights the importance of deterministic concurrency testing and commercial support for open-source reliability.

hackernews · ropbear · Aug 12, 14:22 · [Discussion](https://news.ycombinator.com/item?id=49272832)

**「Background」** SQLite&\#x27;s Write-Ahead Log \(WAL\) mode improves concurrency by writing changes to a separate log file and periodically checkpointing those changes into the main database file. The 16-year-old WAL-reset bug was a race condition in the checkpointing logic that could cause committed transactions to vanish, leading to database corruption. Understanding this bug required knowledge of how SQLite&\#x27;s WAL mode manages concurrent reads and writes, and how checkpointing interacts with the WAL reset process.

**「Impact」** The 16-year-old WAL-reset bug caused at least 19 corruption incidents in Tailscale&\#x27;s control plane between 2025 and 2026, and the fix now prevents similar data-race corruption for all SQLite users who upgrade to a patched version.

**「Community Discussion」** Community members praised Tailscale for funding open-source debugging tools and noted that SQLite&\#x27;s existing testing methodology was outclassed by deterministic concurrency testing. Some commenters questioned how the race occurred under the intended single-writer design, while others highlighted the value of commercial support for correctness.

<details><summary>References</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL - Reset bug</a></li>
<li><a href="https://zeli.app/en/story/49272832">Tailscale Traces Database Corruption to 16 y/o SQLite WAL - Reset Bug</a></li>
<li><a href="https://www.theregister.com/databases/2026/08/12/tailscale-says-deeply-buried-16-year-old-sqlite-bug-caused-last-years-outages/5287004">Tailscale says deeply buried 16 - year - old SQLite bug caused last...</a></li>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL - Reset bug</a></li>
<li><a href="https://elsolitario.org/en/2026/08/13/tailscale-16-year-old-sqlite-wal-bug/">SQLite Bug : The 16-Year-Old Flaw Tailscale Found</a></li>

</ul>
</details>

**Tags**: `#SQLite`, `#debugging`, `#concurrent programming`, `#database reliability`, `#software engineering`

---

<a id="item-tech-news-5"></a>
### [Grok 4.6: Performance and API Controversy](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

xAI has released Grok 4.6, the latest version of its large language model, accompanied by detailed benchmarks and analysis. The model reportedly achieves performance comparable to leading competitors such as Fable, and beats GPT-5.6-Sol on most benchmarks according to early analysis. However, developers have noted that the Grok API now adds a default system prompt that overrides custom instructions, leading to unexpected refusals on certain topics. Grok 4.6 is also praised for its speed and conciseness in user experience, contrasting with the verbosity of some other models.

hackernews · iLuddite · Aug 12, 15:32 · [Discussion](https://news.ycombinator.com/item?id=49274027)

**「Background」** Grok is a large language model developed by xAI, the AI company founded by Elon Musk. Grok 4.6 is the latest version, succeeding Grok 4.5, and has been benchmarked against major competitors such as GPT-5.6 Sol and Fable 5. According to published benchmarks, Grok 4.6 matches the performance of these models on most tasks.

**「Impact」** Developers using the Grok API may encounter unexpected behavior where a default system prompt overrides their custom instructions, potentially causing the model to refuse to discuss system prompts or other topics.

**「Community Discussion」** Community comments are mixed: some users praise Grok 4.6&\#x27;s performance and user experience, while others express concerns about the API&\#x27;s default system prompt overriding custom instructions. There is also skepticism about the rapid pace of improvement across multiple labs, with suggestions of benchmark hacking.

<details><summary>References</summary>
<ul>
<li><a href="https://officechai.com/ai/grok-4-6-benchmarks/">SpaceXAI Releases Grok 4.6, Benchmarks Show Performance ...</a></li>

</ul>
</details>

**Tags**: `#Grok`, `#xAI`, `#AI models`, `#benchmarks`, `#LLM`

---

<a id="item-tech-news-6"></a>
### [Adam&\#x27;s Per-Coordinate Adaptivity Breaks Low-Rank Bias in Factored Models](https://www.reddit.com/r/MachineLearning/comments/1vmjb3p/the_loss_does_not_see_the_basis_but_adam_does_r/) ⭐️ 8.0/10

A new research result shows that Adam&\#x27;s per-coordinate second-moment estimate breaks the rotation invariance of the loss in factored models W = UV^T, causing it to lose the implicit low-rank bias that gradient descent \(GD\) preserves. Experiments on nine optimizers under matched training loss reveal two distinct clusters: GD, shared-scalar Adam, Muon, and Shampoo retain the bias, while Adam, RMSProp, Lion, signum, and Adafactor lose it. A one-parameter transition from per-coordinate to shared-scalar denominator shows recovery improves monotonically, confirming that anisotropy—not adaptivity in general—drives the degradation. Muon behaves unexpectedly: it is exact on truly low-rank targets but degrades quickly as a spectral tail is introduced, with GD overtaking it near 4% tail energy. The paper provides both theoretical guarantees for memoryless rules and a practical diagnostic criterion for optimizer selection, with code and logs available at https://github.com/idevender/loss-basis-adam.

reddit · r/MachineLearning · /u/EtherealGlyph · Aug 12, 16:39

**「Background」** In low-rank factorization, the loss function is invariant under rotations of the factor matrices, meaning the model&\#x27;s output depends only on the product UV^T, not on the specific basis. Gradient descent respects this symmetry, preserving an implicit bias toward low-rank solutions, but adaptive optimizers like Adam apply per-coordinate scaling that depends on the basis, potentially breaking the invariance and degrading this bias.

**「Impact」** Practitioners using Adam or similar adaptive optimizers in low-rank matrix factorization, matrix sensing, or deep-linear networks may unintentionally lose the implicit regularization that GD provides, leading to worse generalization without any change in training loss. The study offers a clear criterion—checking whether the optimizer respects rotation invariance—to guide optimizer choice, and demonstrates that a simple global norm clip can recover performance when per-coordinate scaling is the culprit.

**Tags**: `#machine learning`, `#optimization`, `#Adam`, `#implicit bias`, `#low-rank factorization`

---

<a id="item-tech-news-7"></a>
### [Zed introduces Delta real-time collaborative multiplayer editing with AI](https://zed.dev/blog/introducing-delta) ⭐️ 7.0/10

Zed has announced Delta, a real-time collaborative multiplayer editing feature that integrates AI agents to enable shared code conversations and document-style commenting. Delta allows multiple developers to edit code simultaneously with AI agents participating in the conversation, aiming to improve team collaboration and code review processes. The feature represents a novel approach to collaborative coding, turning the development workflow into a conversation-as-document paradigm.

hackernews · khy · Aug 12, 18:19 · [Discussion](https://news.ycombinator.com/item?id=49276574)

**「Background」** Zed is a high-performance code editor that has recently introduced Delta, a multiplayer environment for collaborative coding with AI agents. Delta is currently in private beta and is designed to facilitate real-time collaboration between human developers and AI agents, capturing every edit and conversation between commits. The environment aims to make agentic development collaborative while maintaining compatibility with standard git workflows, so teammates who do not use Delta still see a normal repository.

**「Community Discussion」** Community reactions are divided; some commenters see no need for multiplayer editing in a code editor, while others find potential value in mentoring junior developers. Concerns were also raised about verbose AI summaries and the page&\#x27;s readability.

<details><summary>References</summary>
<ul>
<li><a href="https://aitoolly.com/ai-news/article/2026-08-13-zed-introduces-delta-a-new-multiplayer-environment-for-collaborative-coding-with-ai-agents-and-real">Zed Delta : Multiplayer Coding Environment for AI Agents | AIToolly</a></li>
<li><a href="https://zeli.app/en/story/49276574">Zed launches Delta , a multiplayer coding environment with... | Zeli</a></li>
<li><a href="https://zed.dev/blog/introducing-delta">Introducing Delta — Zed &#x27;s Blog</a></li>

</ul>
</details>

**Tags**: `#code editor`, `#collaborative editing`, `#AI agents`, `#real-time collaboration`, `#Zed`

---

<a id="item-tech-news-8"></a>
### [HTML over WebSockets for Real-Time SPAs with Minimal JS](https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/) ⭐️ 7.0/10

The article explores using WebSockets to deliver HTML for real-time single-page applications \(SPAs\) with minimal JavaScript, building on patterns like Phoenix LiveView and Blazor. It discusses trade-offs between WebSockets and Server-Sent Events \(SSE\), with community debate on simplicity versus the need for bidirectional, low-latency communication. Historical context notes Chris McCord&\#x27;s earlier work on Rails Sync before moving to Phoenix, and new HTML streaming APIs in Chrome could further simplify this approach by allowing native insertion of HTML from WebSockets without custom JavaScript.

hackernews · redbell · Aug 12, 16:51 · [Discussion](https://news.ycombinator.com/item?id=49275335)

**「Background」** HTML over WebSockets is a technique where a server sends pre-rendered HTML fragments over a persistent WebSocket connection, allowing DOM updates with minimal client-side JavaScript. This approach, popularized by frameworks like Phoenix LiveView and Blazor Server, builds on earlier work such as Chris McCord&\#x27;s Sync for Rails. It contrasts with traditional SPAs that fetch JSON and render on the client, and with simpler alternatives like Server-Sent Events \(SSE\) or HTMX over HTTP.

**「Impact」** For developers building real-time web applications, the article reinforces that the choice between WebSockets and SSE depends on specific use cases: SSE is simpler for server-to-client push, while WebSockets remain necessary for bidirectional communication; internal tools or low-latency apps may benefit from server-side rendering over WebSockets.

**「Community Discussion」** Comments highlight a split between advocates of simpler SSE for most cases and defenders of WebSocket-based approaches for contextual needs, with references to historical precedents \(Rails Sync\) and newer HTML streaming APIs that may reduce JavaScript dependencies. A rebuttal link was also shared, indicating ongoing debate.

<details><summary>References</summary>
<ul>
<li><a href="https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/">HTML over WebSockets: real-time SPAs with barely any JavaScript | Andros Fenollosa</a></li>

</ul>
</details>

**Tags**: `#web-development`, `#real-time`, `#websockets`, `#JavaScript`, `#SPAs`

---

<a id="item-tech-news-9"></a>
### [Chrome JPEG optimization alters tiny image appearance](https://guillaumetech.github.io/posts/jpg-scaling-chrome/) ⭐️ 7.0/10

Chrome&\#x27;s JPEG decoding optimization decompresses images at a lower resolution when displayed at small sizes, causing visible differences compared to full decoding and scaling. This change affects how tiny JPEGs, such as icons, appear in browsers and Electron apps, breaking visual consistency. Firefox is exploring a similar approach but with a different implementation, as noted in a bug tracker. The artifact advises against using JPEGs for icons due to compression artifacts and recommends using images at appropriate resolutions for their display size. The investigation underscores a browser-specific rendering behavior that can disrupt web development workflows.

hackernews · gutechh · Aug 12, 14:00 · [Discussion](https://news.ycombinator.com/item?id=49272549)

**「Background」** JPEG images are compressed by dividing the image into 8×8 blocks and applying a discrete cosine transform \(DCT\) to separate high-frequency detail from low-frequency structure. When an image needs to be displayed much smaller than its original size, the high-frequency information is often imperceptible. Chrome&\#x27;s decoder, libjpeg-turbo, takes advantage of this by performing partial IDCT scaling—decoding only the low-frequency coefficients—which reduces memory and CPU usage but discards details that other browsers might preserve, leading to visible differences in very small JPEGs.

**「Impact」** Developers using small JPEGs or icons in Electron applications \(which embed Chrome\) may encounter broken visual appearance, forcing them to delay upgrades or switch to PNGs to maintain consistent rendering.

**「Community Discussion」** Commenters noted that the same issue occurs with PNGs, and that Chrome&\#x27;s scaling algorithm \(blurrier\) differs from Firefox&\#x27;s \(sharper with ringing\), contributing to the visible difference. Firefox is working on a similar optimization \(Bugzilla 2033250\), and the community consensus advises against using JPEGs for icons and using images at proper resolution rather than scaling large ones.

<details><summary>References</summary>
<ul>
<li><a href="https://guillaumetech.github.io/posts/jpg-scaling-chrome/">Why tiny JPEGs look different in Chrome</a></li>
<li><a href="https://zeli.app/en/story/49272549">Chrome&#x27;s Clever JPEG Decoding Trick Makes Tiny Images Look Different — Why Tiny JPEGs Look Different in Chrome | Zeli</a></li>

</ul>
</details>

**Tags**: `#browser rendering`, `#image processing`, `#web development`, `#JPEG`, `#Chrome behavior`

---

<a id="item-tech-news-10"></a>
### [AI Coding Over-Reliance Risks Unmaintainable Codebases, Warns Engineer](https://simonwillison.net/2026/Aug/12/florian-herrengt/) ⭐️ 7.0/10

Florian Herrengt, in a blog post cited by Simon Willison, warns that heavy reliance on AI for coding can produce convoluted, layered systems that no one on the team understands. He illustrates the problem with a scenario where developers cannot explain where data comes from and must ask an AI tool like Claude to interpret their own code. The result is a codebase so complex that even repeated AI-assisted attempts fail to fix recurring bugs. Herrengt argues this loss of comprehension erodes the team&\#x27;s ability to maintain or debug the software, making the system effectively unmanageable.

rss · Simon Willison · Aug 12, 15:08

**「Background」** Florian Herrengt&\#x27;s blog post argues that AI tools, by dramatically increasing the speed of code production, allow teams with weak engineering cultures to build complex systems that no one fully understands. The metaphor of &quot;removing the middle class&quot; refers to the displacement of developers who traditionally bridged high-level design and low-level implementation, as AI now generates code directly from prompts. This dynamic creates a &quot;cognitive debt&quot; where the codebase becomes opaque and unmaintainable, as no team member can trace the logic or fix bugs without relying on the AI again.

**「Impact」** Teams that habitually offload understanding to AI risk creating a codebase that no one can fully comprehend or reliably fix, leading to escalating technical debt and potential project failure.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.florianherrengt.com/ai-removing-middle-class-software-engineering.html">AI is removing the middle class of software engineering</a></li>
<li><a href="https://northeasttimes.com/2026/08/13/ai-is-hollowing-out-the-middle-class-of-software-engineering/">AI is hollowing out the middle class of software engineering</a></li>

</ul>
</details>

**Tags**: `#software engineering`, `#AI`, `#code quality`, `#technical debt`, `#team dynamics`

---

<a id="item-tech-news-11"></a>
### [City2Graph: Python library for heterogeneous graph neural networks in urban systems](https://www.reddit.com/r/MachineLearning/comments/1vn8oya/city2graph_a_python_library_for_heterogeneous/) ⭐️ 7.0/10

City2Graph is a new Python library that converts geospatial data from sources like OpenStreetMap and Overture Maps into heterogeneous graphs suitable for Graph Neural Networks and spatial analysis. The library supports morphological, transport, mobility, and proximity graph constructions, covering buildings, streets, GTFS transit feeds, and OD matrices, and provides seamless conversion between GeoDataFrames, NetworkX, rustworkx, and PyTorch Geometric. A paper describing the library has been published in Computers, Environment and Urban Systems \(volume 130, 2026, article 102492\). The library is designed to treat urban data as heterogeneous graphs rather than flat feature tables, preserving geometry and graph structure across conversions, and is open-source with contributions welcome.

reddit · r/MachineLearning · /u/Tough\_Ad\_6598 · Aug 13, 11:59

**「Background」** Heterogeneous graphs contain multiple types of nodes and edges, allowing representation of different urban entities \(buildings, streets, transit stops\) and their relationships. City2Graph builds on the concept that urban data is more naturally modeled as such graphs, enabling advanced GeoAI techniques like graph neural networks for tasks such as urban morphology analysis and mobility prediction.

**「Impact」** Researchers and practitioners in urban computing and spatial analysis can now efficiently convert geospatial data into heterogeneous graph structures ready for PyTorch Geometric, reducing the barrier to applying graph neural networks to urban systems.

**Tags**: `#geospatial`, `#graph neural networks`, `#Python`, `#urban computing`, `#open source`

---

<a id="item-tech-news-12"></a>
### [Trump signs memo allowing private companies to conduct overseas surveillance and cyber attacks](https://www.bloomberg.com/news/articles/2026-08-13/trump-enlists-private-sector-to-boost-cyber-offensive-arsenal) ⭐️ 7.0/10

President Trump signed a memorandum authorizing private companies under direct federal control and supervision to conduct overseas surveillance and cyber attacks. The program targets foreign networked organized crime groups that target Americans. The Department of Homeland Security will administer the program in coordination with the Department of Justice. Participating companies must maintain a minimum $1 million bond or escrow account, which will be forfeited for non-compliance.

telegram · zaihuapd · Aug 13, 05:10

**「Background」** Traditionally, offensive cyber operations against foreign adversaries have been conducted exclusively by U.S. government agencies such as the National Security Agency or U.S. Cyber Command. The new memorandum creates a framework that encourages private-sector companies to enter into agreements with federal and local agencies to conduct surveillance and offensive operations, expanding the scope of national security activities beyond the government domain.

**「Impact」** This policy shift enables private-sector execution of offensive cyber operations, potentially expanding the scope of cyber conflict and introducing new legal and ethical considerations for companies involved in national security activities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-13/trump-enlists-private-sector-to-boost-cyber-offensive-arsenal">Trump Signs Memo Allowing Private Firms to Conduct Cyber Attacks Abroad - Bloomberg</a></li>
<li><a href="https://www.the-independent.com/tech/security/trump-cyber-attack-security-memo-b3032324.html">Trump signs memo allowing US firms to carry out cyber attacks | The Independent</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#policy`, `#surveillance`, `#private sector`, `#national security`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Chinese chipmaker YMTC jumps to third in global NAND memory shipments](https://www.cnbc.com/2026/08/13/chinese-firm-tops-micron-kioxia-shipments-nand-memory-chips.html) ⭐️ 8.0/10

Chinese memory chip maker YMTC rose to third place in global NAND shipments in the second quarter, capturing a 14% market share and overtaking U.S. rival Micron and Japan&\#x27;s Kioxia, according to Counterpoint Research.

rss · CNBC Finance · Aug 13, 02:59

**「Background」** NAND memory chips are a type of flash storage that retains data when power is off, commonly used in smartphones, SSDs, and data centers. YMTC had narrowly beaten Kioxia a year earlier but fell back before regaining the third spot this quarter.

**「Impact」** The shift underscores China&\#x27;s growing competitiveness in the semiconductor sector, though YMTC still trails in revenue and focuses more on consumer products than the higher-value data center market.

**Tags**: `#NAND memory`, `#YMTC`, `#semiconductor market share`, `#China technology`, `#memory chips`

---

<a id="item-finance-news-2"></a>
### [EVs account for 65.1% of China&\#x27;s July car sales as overall market shrinks](https://www.cnbc.com/2026/08/12/china-car-sales-data-byd-tesla-geely-vw.html) ⭐️ 8.0/10

New energy vehicles, including battery and hybrid cars, accounted for 65.1% of new passenger car sales in China in July, up from 54% a year earlier, while overall passenger car sales fell 20.3% in the first seven months of the year, according to the China Passenger Car Association and Autohome data.

rss · CNBC Finance · Aug 13, 01:31

**「Background」** The data reflects the accelerating shift to electric vehicles in the world&\#x27;s largest auto market, where Geely&\#x27;s Xingyuan electric hatchback was the best-selling model in the six months through July with nearly 197,500 units sold, followed by Tesla&\#x27;s Model Y.

**「Impact」** Traditional foreign automakers like Volkswagen, the only one in the top 10, face growing pressure, while BYD&\#x27;s passenger car sales dropped more than 10% in the first half of the year as domestic rivals such as Geely and Leapmotor gain market share.

**Tags**: `#China auto market`, `#electric vehicles`, `#Geely`, `#Tesla`, `#BYD`

---

<a id="item-finance-news-3"></a>
### [CME Group to Launch AI Computing Power Futures Contracts](https://www.cnbc.com/2026/08/11/ai-computing-power-becomes-a-tradable-asset-class-as-cme-starts-futures.html) ⭐️ 8.0/10

CME Group plans to launch the first futures contracts for AI computing power on October 5, pending regulatory approval, tied to the rental cost of Nvidia’s H100 and Blackwell B200 GPUs, with each contract representing a month’s rent for the H100 chip based on indexes tracking hourly GPU rental prices.

rss · CNBC Finance · Aug 12, 14:14

**「Background」** Futures contracts are agreements to buy or sell an asset at a future date at a predetermined price, commonly used for commodities like oil. This new offering creates a public benchmark for AI computing capacity, which has lacked price transparency, according to Silicon Data CEO Carmen Li.

**「Impact」** The contracts could help channel investment into AI infrastructure by giving investors a way to gain exposure to computing capacity and allowing AI developers to hedge their costs, adding to broader efforts by Wall Street and Nvidia to finance the AI buildout.

**Tags**: `#AI computing`, `#futures contracts`, `#CME Group`, `#GPU rental`, `#financial innovation`

---

<a id="item-finance-news-4"></a>
### [China&\#x27;s Economic Slowdown Pushes Gig Workers to 53 Million, Oversupply Squeezes Incomes](https://www.ft.com/content/a3803e70-cb4d-444f-a31e-05be2f2c44f6?accessToken=zwAAAZ_5xcXzkdOjgD5wy01ET9OjHgW-LyxE9g.MEUCIQCWTIny3JTJV8e-PGyK0XL2tg5g_7Ay-rpKkwGZCpp1-AIgbMgJQPlqWgqAsX4s1k4gYaC4b8k0JveZOs35OJQvbZ4&amp;amp;sharetype=gift&amp;amp;token=7e8483bb-395d-429e-afca-2f4ab5ad150b) ⭐️ 8.0/10

China&\#x27;s economic slowdown has driven the number of gig workers—mainly delivery and ride-hailing drivers—to 53 million as of 2025, an increase of 10 million in two years, but oversupply is lowering incomes and extending working hours, according to the Financial Times.

telegram · zaihuapd · Aug 13, 06:40

**「Background」** The real estate downturn, weak consumption, contraction in manufacturing and construction, and automation have pushed excess labor into the gig economy, creating a surplus of workers.

**「Impact」** Gig workers, such as taxi drivers at airports like Shanghai Pudong and Beijing Daxing, now face wait times of up to 10 hours, and Shenzhen declared its ride-hailing market saturated in June, directly squeezing incomes and hours for millions of workers.

**Tags**: `#China economy`, `#gig economy`, `#employment`, `#labor market`, `#economic slowdown`

---