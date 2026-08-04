---
layout: default
title: "Horizon Summary: 2026-08-04 (EN)"
date: 2026-08-04
lang: en
---

> From 49 items, 19 important content pieces were selected

---

**Technology News**
1. [Waymo Robotaxi Service Opens to Public in Dallas](#item-tech-news-1) ⭐️ 8.0/10
2. [Running DeepSeek V4 Flash on a Single AMD MI300X](#item-tech-news-2) ⭐️ 8.0/10
3. [Keyv and friends compromised in active Shai-Hulud supply chain attack](#item-tech-news-3) ⭐️ 8.0/10
4. [MiniMax-H3 MLX port brings video generation with audio to Apple Silicon](#item-tech-news-4) ⭐️ 8.0/10
5. [Cloudflare Replaces Third-Party Security Tools with AI, Bug Bounty Processing Costs $58/Month](#item-tech-news-5) ⭐️ 8.0/10
6. [China&\#x27;s First Mandatory L3/L4 Autonomous Driving Standard Takes Effect July 2027](#item-tech-news-6) ⭐️ 8.0/10
7. [White House Reverses on Chinese Open-Source AI Regulation](#item-tech-news-7) ⭐️ 8.0/10
8. [Mistral releases Shieldstral: 3B open-weights multimodal moderation model](#item-tech-news-8) ⭐️ 7.0/10
9. [Novel Algorithm and Color Space for Generating Diverse Skin Tones](#item-tech-news-9) ⭐️ 7.0/10
10. [Thanks FedEx, This Is Why We Keep Getting Phished \(2024\)](#item-tech-news-10) ⭐️ 7.0/10
11. [Apple Alleges More Ex-Employees Took Data to OpenAI](#item-tech-news-11) ⭐️ 7.0/10
12. [Harness Engineering for Self-Improving AI](#item-tech-news-12) ⭐️ 7.0/10
13. [White House Finalizes Voluntary AI Model Assessment Framework, Details Secret](#item-tech-news-13) ⭐️ 7.0/10
14. [iPhone-Windows Clipboard Sharing Coming to iOS 28 in EU](#item-tech-news-14) ⭐️ 7.0/10
15. [Huawei&\#x27;s Chief Scientist Warns of NVIDIA Chip Scaling Limit](#item-tech-news-15) ⭐️ 7.0/10
16. [Trump Administration Drafting Ban on Chinese Optical Module Imports](#item-tech-news-16) ⭐️ 7.0/10

**Financial News**
1. [Google orchestrates $200bn financing for Anthropic&\#x27;s AI chips](#item-finance-news-1) ⭐️ 9.0/10
2. [Polymarket seeks funding at over $20 billion valuation](#item-finance-news-2) ⭐️ 8.0/10
3. [China&\#x27;s State Post Bureau Investigates Shentong Express Over Safety Failures](#item-finance-news-3) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Waymo Robotaxi Service Opens to Public in Dallas](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 8.0/10

Waymo has opened its fully autonomous ride-hailing service to the general public in Dallas, Texas, expanding into one of the largest low-density, car-dependent metroplexes in the US. The service operates within a defined service area and uses the same Waymo Driver technology already deployed in other cities. This launch marks a significant step in scaling robotaxi operations to sprawling urban areas with limited public transit, demonstrating the potential for autonomous vehicles to serve as a primary mobility option in such environments.

hackernews · xnx · Aug 4, 18:29 · [Discussion](https://news.ycombinator.com/item?id=49172836)

**「About Waymo」** Waymo is an autonomous driving technology company, a subsidiary of Alphabet Inc., originally the Google self-driving car project. It operates a robotaxi service that has been gradually expanding to multiple U.S. cities, including Phoenix, San Francisco, and Los Angeles.

**「Impact」** The introduction of publicly available robotaxis in Dallas could reduce traffic accidents and provide a model for decoupling housing development from parking requirements, potentially lowering construction costs and supporting affordable housing in a region where driving is dominant.

**「Community Discussion」** Hacker News commenters generally view the expansion positively, citing the vehicles&\#x27; predictable driving behavior, lower incident rates compared to human drivers, and the potential to reduce parking mandates that drive up housing costs. Some noted occasional minor hiccups where Waymos get stuck, but overall consider them a welcome addition to car-dependent Dallas.

<details><summary>References</summary>
<ul>
<li><a href="https://en.m.wikipedia.org/wiki/Waymo">Waymo - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#autonomous-vehicles`, `#robotaxi`, `#urban-mobility`, `#Waymo`, `#Dallas`

---

<a id="item-tech-news-2"></a>
### [Running DeepSeek V4 Flash on a Single AMD MI300X](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 8.0/10

A practical guide demonstrates running DeepSeek V4 Flash at full inference weights on a single AMD MI300X GPU, preserving model quality and achieving over 150 tokens per second. The setup uses the hardware&\#x27;s high HBM capacity to fit the large Mixture-of-Experts model, trading the native 1M context window for a 256k window to remain within memory limits. This highlights the viability of high-HBM accelerators for self-hosting large language models, offering a cost-effective alternative to cloud-based inference for organizations with access to such hardware.

hackernews · zhoutong · Aug 4, 10:00 · [Discussion](https://news.ycombinator.com/item?id=49166386)

**「Background」** DeepSeek is a Chinese AI research company that released large language models such as DeepSeek-R1 in early 2025. The DeepSeek V4 Flash is a later Mixture-of-Experts \(MoE\) model with full inference weights that benefit from high GPU memory. The AMD Instinct MI300X is a data center GPU with 192 GB of HBM3, often used in multi-GPU nodes but here explored for single-accelerator inference of memory-intensive MoE models.

**「Impact」** For AI infrastructure engineers, the guide confirms that a single high-HBM GPU can serve DeepSeek V4 Flash at full performance, but the practical barrier is that the MI300X is typically sold as an 8-GPU system costing ~250K EUR, limiting single-unit availability.

**「Community Discussion」** Commenters noted that the MI300X is only available as an 8-GPU module, making single-unit testing expensive, and suggested the upcoming MI350P PCIe card with 144GB as a more accessible alternative due to the model&\#x27;s native MXFP4 quantization. Others mentioned that DwarfStar was omitted from the prior art and praised the 256k context window tradeoff as practical.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AMD MI300X`, `#DeepSeek V4`, `#LLM inference`, `#MoE`, `#GPU`

---

<a id="item-tech-news-3"></a>
### [Keyv and friends compromised in active Shai-Hulud supply chain attack](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 8.0/10

The npm package Keyv and several of its dependencies were compromised in an active supply chain attack named Shai-Hulud. Attackers injected malicious code into pre-install hooks that execute automatically when the package is installed, allowing arbitrary code execution on developers&\#x27; machines. The attack affects the broader JavaScript ecosystem because Keyv is a popular key-value store library. Security researchers advise developers to audit their dependency trees immediately and consider restricting the use of pre-install scripts.

hackernews · cimi\_ · Aug 4, 11:01 · [Discussion](https://news.ycombinator.com/item?id=49166874)

**「Background」** Keyv is a widely used npm key-value storage library with approximately 127 million weekly downloads. The attack leveraged a compromised GitHub account belonging to the maintainer to inject malicious pre-install hooks that steal credentials and spread like a worm across the dependency tree, a classic supply chain attack exploiting npm&\#x27;s install lifecycle.

**「Impact」** Developers who have recently installed or updated Keyv or its compromised dependencies may have run unauthorized code, potentially leading to credential theft or further compromise of build environments.

**「Community Discussion」** Many commenters argue that pre-install hooks should be deprecated or require explicit approval, citing the ease of abuse. Some suggest practical defenses like setting a minimum npm registry age for packages to avoid freshly released malicious versions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack">Keyv and friends compromised in npm supply chain attack</a></li>
<li><a href="https://www.wiz.io/blog/keyv-and-cacheable-npm-supply-chain-attack">keyv and cacheable npm Package Hijacked in Supply Chain Attack | Wiz Blog</a></li>

</ul>
</details>

**Tags**: `#supply-chain-attack`, `#npm`, `#security`, `#open-source`, `#malware`

---

<a id="item-tech-news-4"></a>
### [MiniMax-H3 MLX port brings video generation with audio to Apple Silicon](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 8.0/10

MiniMax released MiniMax-H3, an omni-modal generative model that accepts text, images, audio, and video to produce up to 15-second video clips with synchronized audio. PipeNetwork has ported this model to MLX, allowing it to run locally on Apple Silicon Macs. Simon Willison successfully ran the model on an M5 Max MacBook Pro, downloading ~115 GB of model files and generating a video in 45 minutes. The video was visually impressive, but the audio was garbled because no audio prompt was provided; a detailed prompting guide is available to improve results.

rss · Simon Willison · Aug 4, 19:10

**「Background」** MiniMax-H3 is a general-purpose omni-modal generative system that can understand multimodal inputs and generate video with native stereo audio at up to 2K resolution and 15 seconds in length. The open-source port by PipeNetwork uses MLX, Apple&\#x27;s machine learning framework, to enable local execution on Apple Silicon Macs.

**「Impact」** The MLX port allows local experimentation with MiniMax-H3’s omni-modal video generation on Apple Silicon Macs, demanding 115 GB of storage and 45 minutes of generation time on an M5 Max.

<details><summary>References</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H 3 : An Open Model Breaking the Boundaries Between Tasks...</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#multimodal-models`, `#video-generation`, `#apple-silicon`, `#mlx`

---

<a id="item-tech-news-5"></a>
### [Cloudflare Replaces Third-Party Security Tools with AI, Bug Bounty Processing Costs $58/Month](https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600) ⭐️ 8.0/10

Cloudflare has largely replaced its third-party security tools with over 200 autonomous AI agents, and now uses Anthropic&\#x27;s Claude Sonnet model to automatically process bug bounty reports. The AI-driven triage system handles deduplication and report valuation, costing just $58 per month compared to an estimated $200,000 per month if a specialized security model like Mythos were used. Chief Security Officer Grant Bourzikas disclosed these changes at an event in Sydney, noting that the company&\#x27;s self-developed security applications, partially written with AI assistance, have nearly eliminated reliance on third-party tools. However, Bourzikas cautioned other organizations against attempting the same approach, citing Cloudflare&\#x27;s unique capability to build its own security software. Chief Strategy Officer Stephanie Cohen also attributed a previous layoff of 1,100 employees to AI-driven automation and revealed plans for Cloudflare to mediate micropayments between AI companies and publishers.

telegram · zaihuapd · Aug 4, 09:24

**「Background」** Cloudflare operates a large-scale security infrastructure and runs a bug bounty program to receive vulnerability reports from external researchers. Traditionally, organizations use third-party security tools to triage and validate these reports.

**「Impact」** Cloudflare&\#x27;s example demonstrates dramatic cost reduction for bug bounty triage, but its approach is not recommended for organizations without similar in-house development capabilities. The move also signals a broader shift toward AI-native security operations that may reshape the security vendor landscape.

**Tags**: `#AI 安全`, `#漏洞赏金自动化`, `#Cloudflare`, `#安全工程`, `#成本优化`

---

<a id="item-tech-news-6"></a>
### [China&\#x27;s First Mandatory L3/L4 Autonomous Driving Standard Takes Effect July 2027](https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html) ⭐️ 8.0/10

China’s Ministry of Industry and Information Technology has published the mandatory national standard GB 44721—2026, Safety Requirements for Autonomous Driving Systems of Intelligent Connected Vehicles, which will come into force on July 1, 2027. It is the country’s first compulsory standard covering Level 3 \(conditional automation\) and Level 4 \(high automation\) systems, applicable to M‑category passenger vehicles and N‑category cargo vehicles but not to automatic parking. The standard upgrades the previous 2024 recommended guideline to a mandatory framework, building safety requirements across four dimensions: enterprise lifecycle safety assurance, system dynamic driving capability, human‑machine interaction and user notification, and multi‑dimensional inspection and testing. At a minimum, the autonomous driving system must perform at the level of a qualified and attentive human driver.

telegram · zaihuapd · Aug 4, 13:06

**「Background」** SAE defines L3 as conditional automation where the driver must be ready to retake control, and L4 as high automation that can operate without driver intervention in specific operational domains. China’s 2024 recommended standard provided voluntary guidance; the new GB 44721—2026 makes those safety requirements legally binding for L3 and L4 systems deployed in passenger and cargo vehicles.

**「Impact」** Automakers and suppliers of L3 and L4 systems for passenger and cargo vehicles in China must ensure their systems meet the minimum safety performance of a competent human driver by July 2027, or face compliance barriers in a market that is central to autonomous driving development.

**Tags**: `#autonomous driving`, `#China`, `#regulations`, `#safety standards`, `#L3/L4`

---

<a id="item-tech-news-7"></a>
### [White House Reverses on Chinese Open-Source AI Regulation](https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html) ⭐️ 8.0/10

The White House abruptly abandoned plans to restrict Chinese open-source AI models after strong pushback from Silicon Valley. Chief of Staff Susie Wiles and Treasury Secretary Scott Bessent had considered sanctions, trade blacklists, and banning U.S. firms from working with Chinese companies, but the administration pivoted to focus on boosting U.S. AI competitiveness. On August 4, the White House invited tech companies to discuss a new framework that would require cybersecurity reviews before AI models are released. The policy reversal came after a Chinese open-source model, Kimi, matched the performance of OpenAI’s top systems, intensifying a divide between companies like OpenAI and Anthropic, which pushed for restrictions on national security grounds, and Nvidia and Meta, which defended the open ecosystem. Nvidia CEO Jensen Huang posted on X for the first time to defend open-source AI and formed a security alliance with over 230 members.

telegram · zaihuapd · Aug 4, 15:22

**「Background」** The Trump administration had previously weighed sanctions or trade restrictions on Chinese AI models, citing national security concerns. Silicon Valley companies split over the issue, with OpenAI and Anthropic pushing for curbs while Meta, Nvidia, and others defended open-source ecosystems. The debate intensified after a Chinese open-source model, Kimi, demonstrated performance rivalling OpenAI&\#x27;s top models.

**「Impact」** The shift away from sanctions and toward a pre-release cybersecurity review means that U.S. companies can continue collaborating with Chinese open-source projects, but they may soon face new federal scrutiny before model launches.

**Tags**: `#AI regulation`, `#open-source AI`, `#Silicon Valley`, `#Chinese AI models`, `#technology policy`

---

<a id="item-tech-news-8"></a>
### [Mistral releases Shieldstral: 3B open-weights multimodal moderation model](https://mistral.ai/news/shieldstral/) ⭐️ 7.0/10

Mistral has released Shieldstral, a 3-billion-parameter open-weights model for multimodal content moderation. The model accepts text and image inputs and can be queried with a single yes/no question, such as &\#x27;Does this content promote physical violence?&\#x27;, to evaluate safety. Shieldstral is designed to serve as an efficient first line of defense for AI applications, enabling developers to integrate safety checks without relying on large proprietary systems. It is available on Hugging Face as part of Mistral&\#x27;s broader strategy of offering smaller, specialized models for specific use cases.

hackernews · riadsila · Aug 4, 16:36 · [Discussion](https://news.ycombinator.com/item?id=49171268)

**「Background」** Mistral AI, a company known for releasing open-weights models, has introduced Shieldstral as a 3-billion-parameter multimodal safety classifier. The model treats moderation as answering a policy-adaptive yes/no question, enabling it to evaluate text and images against customizable safety rules. It runs efficiently on a single consumer GPU, outperforming much larger models in this role.

**「Impact」** Developers gain an open-weights, multimodal moderation tool that can be deployed as a fast, initial safety filter in AI pipelines, with the understanding that its non-deterministic outputs may require human review for high-stakes decisions.

**「Community Discussion」** Commenters are interested in whether Shieldstral can be tuned to arbitrary moderation rulesets beyond a fixed set of categories, or if it is limited to predefined policies. Some appreciate Mistral&\#x27;s focus on small, fine-tuned models, while others note that such a model can act as a practical first defense before human review, though its non-determinism limits full reliance on sensitive content.

<details><summary>References</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral. | Mistral AI</a></li>
<li><a href="https://x.com/MistralAI/status/2084684735725379637">🛡️Introducing Shieldstral, Mistral&#x27;s 3B open-weights ...</a></li>

</ul>
</details>

**Tags**: `#moderation`, `#multimodal`, `#open-weights`, `#AI safety`, `#Mistral`

---

<a id="item-tech-news-9"></a>
### [Novel Algorithm and Color Space for Generating Diverse Skin Tones](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 7.0/10

A developer created an interactive color space and algorithm to procedurally generate diverse skin tones, motivated by difficulty picking plausible shades for digital art and games. The approach uses principal component analysis \(PCA\) on skin tone data and hand-fitted functions to define a 2D space, resulting in a color picker and JavaScript demos. While the methodology is acknowledged as somewhat shaky, the tool provides a practical way to sample a wide range of realistic skin colors. The project includes detailed explanations of the construction and properties of the space, and is openly shared for community feedback and improvement.

hackernews · automatoney · Aug 4, 15:16 · [Discussion](https://news.ycombinator.com/item?id=49170165)

**「Background」** Skin tones exhibit a distinctive crescent shape when plotted in standard color spaces, making uniform selection difficult. Principal component analysis \(PCA\) reorients the data to simplify this shape, and function fitting can then map it to a 2D parameter space for intuitive color picking.

**「Impact」** Digital artists and game developers gain a freely available, interactive tool for generating diverse and plausible skin tones without manual trial and error.

**「Community Discussion」** Commenters praised the function fitting idea and the presentation, while noting the complexity of skin color modeling and referencing related work like Pantone Skin Tones and Oklab crescent shapes; some questioned the presence of green, blue, and purple hues in the generated space.

<details><summary>References</summary>
<ul>
<li><a href="https://toneyalexander.github.io/inclusive-color-space/">What Colors Are We? Constructing A Color Space For Skin Tones</a></li>

</ul>
</details>

**Tags**: `#color-science`, `#algorithm`, `#computer-graphics`, `#generative-art`, `#skin-tone`

---

<a id="item-tech-news-10"></a>
### [Thanks FedEx, This Is Why We Keep Getting Phished \(2024\)](https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/) ⭐️ 7.0/10

Troy Hunt exposes how FedEx and other companies send legitimate emails that mimic phishing tactics, such as using generic greetings, suspicious links, and attachments from unknown senders. These practices condition users to ignore red flags, making them more susceptible to actual phishing attacks. Even security-conscious individuals struggle to verify the authenticity of such messages, and inconsistent corporate communication standards worsen the problem. Hunt argues that companies must adopt clearer, more secure email practices to avoid undermining user security training.

hackernews · stymaar · Aug 4, 21:09 · [Discussion](https://news.ycombinator.com/item?id=49175192)

**「The Security Risk of Normalizing Phishing-Like Emails」** Phishing is a social engineering attack where fraudulent emails imitate trusted organizations to steal sensitive information or deliver malware. Security awareness training encourages users to spot red flags like misspellings, unusual sender addresses, and urgent language to avoid falling victim. When legitimate companies send messages that exhibit these same patterns, they inadvertently condition recipients to ignore warning signs, weakening the effectiveness of anti-phishing education.

**「Impact」** Users are increasingly unable to distinguish legitimate corporate emails from phishing attempts, heightening the risk of falling for scams, even among those who follow security best practices. This erosion of trust is reinforced by real-world confusion over emails from FedEx and Google, as noted in community comments.

**「Community Discussion」** Commenters share firsthand experiences: a FedEx customs notice from a random employee with a PDF seemed fraudulent but was confirmed legitimate, and a Google storage warning used a confusing domain \(c.gle\) that even tech-savvy users couldn&\#x27;t verify. The proliferation of obscure TLDs and scam-like voice systems in legitimate services further normalizes suspicious communication, making it harder for non-technical people to stay safe.

**Tags**: `#phishing`, `#cybersecurity`, `#social engineering`, `#email security`, `#corporate practices`

---

<a id="item-tech-news-11"></a>
### [Apple Alleges More Ex-Employees Took Data to OpenAI](https://techcrunch.com/2026/08/04/apple-says-more-ex-employees-may-have-taken-confidential-data-to-openai/) ⭐️ 7.0/10

Apple has told a court that additional former employees may have taken confidential hardware data to OpenAI, escalating a legal battle over alleged trade secret theft. The company claims that at least one ex-staffer exploited an authentication bug to download 37 sensitive documents, and that screenshots were taken of internal information. The dispute centers on Apple&\#x27;s hardware secrets and OpenAI&\#x27;s hardware ambitions under Sam Altman, highlighting tensions between talent mobility and intellectual property protection.

hackernews · thewebguyd · Aug 4, 15:37 · [Discussion](https://news.ycombinator.com/item?id=49170479)

**「Background」** Apple previously filed a lawsuit against OpenAI, alleging that former Apple employees who joined OpenAI took confidential hardware design documents. The legal dispute focuses on claims that these ex-employees improperly accessed and retained proprietary information about Apple&\#x27;s hardware projects. Apple now says its trade secrets investigation has widened, with additional former staff possibly involved.

**「Impact」** The lawsuit threatens to derail OpenAI&\#x27;s hardware project, which critics have labeled a costly vanity endeavor.

**「Community Discussion」** Commenters debate whether Apple&\#x27;s lawsuit is a typical scare tactic or a legitimate response to serious allegations of document theft, while some dismiss OpenAI&\#x27;s hardware project as a costly misadventure. Others highlighted the claim that an ex-employee exploited an authentication bug to download 37 documents, underscoring the technical nature of the alleged breach.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/08/04/apple-says-more-ex-employees-may-have-taken-confidential-data-to-openai/">Apple says more ex - employees may have taken confidential data ...</a></li>

</ul>
</details>

**Tags**: `#apple`, `#openai`, `#legal`, `#data-theft`, `#hardware`

---

<a id="item-tech-news-12"></a>
### [Harness Engineering for Self-Improving AI](https://lilianweng.github.io/posts/2026-07-04-harness/) ⭐️ 7.0/10

Lilian Weng&\#x27;s blog post examines the engineering of harnesses—the surrounding tooling, prompts, and evaluation infrastructure—that enable AI systems to self-improve. It discusses how organizations can define quality via fitness functions, allow agents to analyze production traces, and generate their own tools to optimize performance and cost. The work emphasizes a shift from training model weights to systematically refining the harness layer, including evals, validation splits, and automated research loops.

hackernews · tosh · Aug 4, 06:17 · [Discussion](https://news.ycombinator.com/item?id=49164896)

**「Background」** In AI engineering, a “harness” refers to the surrounding infrastructure—prompts, tools, evaluation suites, and runtime environments—that enables an agent to operate and improve itself. Lilian Weng is a respected AI researcher known for work on large language model \(LLM\) agents and reinforcement learning. Her recent post explores systematic approaches to constructing such harnesses so that AI systems can self-optimize efficiently.

**「Impact」** AI engineers working on agentic systems may adopt harness-centric optimization, using auto-research and trace analysis to improve agent reliability and efficiency without modifying the underlying model.

**「Community Discussion」** Practitioners confirmed that auto-research on harnesses is powerful when agents can inspect production traces and write their own tools, though it requires careful validation splits. Some commenters speculated that harnesses might eventually generate their own RLHF training sets and fine-tune models, while others cautioned about the challenges of defining quality metrics for large codebases.

**Tags**: `#ai`, `#self-improvement`, `#harness-engineering`, `#software-engineering`, `#llm`

---

<a id="item-tech-news-13"></a>
### [White House Finalizes Voluntary AI Model Assessment Framework, Details Secret](https://www.axios.com/2026/08/03/white-house-finalizes-ai-framework-behind-closed-doors) ⭐️ 7.0/10

On August 3, the White House announced it had finalized a voluntary assessment framework for advanced AI models, as required by a June 2 executive order, but declined to disclose the framework&\#x27;s details, the list of reviewers, or when companies will begin using it. The framework mandates that companies grant government access to models up to 30 days before public release and includes provisions on confidentiality, cybersecurity, intellectual property protection, and non-disclosure agreements, along with a list of &\#x27;trusted partners&\#x27; authorized for early access. The executive order also classifies the specific network capability benchmarks and thresholds used for model evaluation. The administration is engaging with numerous industry partners—far more than just Anthropic, OpenAI, and Google—and will hold a staff-level meeting with those three labs to review the framework.

telegram · zaihuapd · Aug 4, 02:31

**「Background」** In June 2026, President Biden signed an executive order directing the White House to create a voluntary framework for advanced AI model assessments, focusing on national security risks such as cyber capabilities. The framework is intended to give the government early access to models before they are publicly released, while protecting companies&\#x27; intellectual property. The order required its completion by early August 2026.

**「Impact」** AI labs developing advanced models must now prepare for a pre-release government access window of up to 30 days, under terms that remain largely opaque. The classified benchmarks and undisclosed trusted partner list further complicate compliance planning.

**Tags**: `#AI regulation`, `#government policy`, `#model evaluation`, `#voluntary framework`, `#AI safety`

---

<a id="item-tech-news-14"></a>
### [iPhone-Windows Clipboard Sharing Coming to iOS 28 in EU](https://appleinsider.com/articles/26/08/04/iphone-to-windows-clipboard-sharing-coming-to-ios-28-in-the-eu) ⭐️ 7.0/10

Under the EU&\#x27;s Digital Markets Act \(DMA\), Apple has approved Microsoft&\#x27;s interoperability request to develop cross-device clipboard sharing between iPhone and Windows PCs. The feature is expected to ship with iOS 28 in fall 2027, enabling EU users to copy on one device and paste on the other without third-party apps or repeated authorization. It will utilize a one-time pairing through AccessorySetupKit, similar to the accessory notification framework introduced in iOS 26.5. Apple has not yet confirmed whether the capability will be included in the initial iOS 28 release or expanded beyond the EU.

telegram · zaihuapd · Aug 4, 03:15

**「Background」** The DMA&\#x27;s interoperability mandates require designated gatekeepers like Apple to allow third-party access to core platform features. Clipboard sharing between iOS and Windows has historically relied on third-party tools or manual methods, so this built-in integration marks a significant step toward seamless cross-platform use driven by regulation.

**「Impact」** EU iPhone users will gain a native clipboard sharing feature with Windows in iOS 28, removing the need for third-party apps and the existing per-copy-paste permission prompt. The feature is currently limited to the EU and may not ship with the initial iOS 28 release.

<details><summary>References</summary>
<ul>
<li><a href="https://appleinsider.com/articles/26/08/04/iphone-to-windows-clipboard-sharing-coming-to-ios-28-in-the-eu">iPhone to Windows clipboard sharing coming to iOS 28 in the EU</a></li>
<li><a href="https://www.hngn.com/articles/272564/20260804/apple-bring-iphone-windows-clipboard-sharing-eu-users-under-microsofts-dma-request.htm">Apple To Bring iPhone-Windows Clipboard Sharing To EU Users Under Microsoft&#x27;s DMA Request</a></li>

</ul>
</details>

**Tags**: `#cross-platform`, `#interoperability`, `#clipboard`, `#iOS`, `#DMA`

---

<a id="item-tech-news-15"></a>
### [Huawei&\#x27;s Chief Scientist Warns of NVIDIA Chip Scaling Limit](https://www.bloomberg.com/news/articles/2026-08-04/huawei-s-top-scientist-warns-of-chip-limit-nvidia-will-soon-face) ⭐️ 7.0/10

Huawei&\#x27;s chief semiconductor scientist Liao Heng warned in a rare four-hour interview that NVIDIA&\#x27;s approach of scaling up compute chips and high-bandwidth memory will eventually hit a physical limit, after which an &\#x27;avalanche&\#x27; effect could occur. He proposed Huawei&\#x27;s alternative path, Tao&\#x27;s Law, and announced that the first phone chip using the LogicFolding technology framework will debut later this year. Liao also noted that the US and Chinese semiconductor industries are splitting into two separate ecosystems, each requiring complete manufacturing and supply capabilities to survive.

telegram · zaihuapd · Aug 4, 08:04

**「Background」** The semiconductor industry has long pursued performance gains by steadily increasing transistor density and employing high-bandwidth memory \(HBM\) to accelerate data exchange between compute chips. This approach of scaling up compute chips and HBM, as practiced by companies like NVIDIA, is now approaching fundamental physical constraints such as power density limits and atomic-scale quantum effects.

**「Impact」** Liao&\#x27;s warning reinforces the perception that the US and Chinese semiconductor ecosystems are diverging into two separate, self-sufficient supply chains.

<details><summary>References</summary>
<ul>
<li><a href="https://theunum.io/en/news/read/huawei-scientist-liao-heng-announced-the-physical-scaling-limits-of-nvidia-chips">Huawei scientist Liao Heng announced the physical scaling limits of...</a></li>

</ul>
</details>

**Tags**: `#semiconductor physics`, `#AI hardware`, `#chip scaling`, `#NVIDIA`, `#Huawei`

---

<a id="item-tech-news-16"></a>
### [Trump Administration Drafting Ban on Chinese Optical Module Imports](https://www.reuters.com/world/trump-administration-drafting-ban-chinese-data-center-devices-sources-say-2026-08-04/) ⭐️ 7.0/10

The Trump administration is drafting a ban on imports of new Chinese data center components, focusing on optical modules. The FCC aims to publish and enforce the ban this year to protect AI-critical infrastructure from data theft, malware, and service disruption. The measure is still in draft and could be modified or shelved. If enacted, it would directly hit Innolight, which holds 27% of the global optical module market. China&\#x27;s embassy warned it would take all necessary measures to safeguard its interests.

telegram · zaihuapd · Aug 4, 11:29

**「Background」** Optical modules are transceivers that convert electrical signals to optical signals for fiber-optic communication, essential for high-speed interconnects inside AI data centers. The U.S. Federal Communications Commission \(FCC\) has previously imposed similar import restrictions on Chinese-made drones, routers, robots, and inverters on national security grounds.

**「Impact」** If enacted, the ban would directly disrupt the AI hardware supply chain by cutting off Innolight, the world&\#x27;s largest optical module supplier with a 27% market share.

**Tags**: `#technology policy`, `#optical modules`, `#data centers`, `#AI infrastructure`, `#supply chain`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Google orchestrates $200bn financing for Anthropic&\#x27;s AI chips](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 9.0/10

The Financial Times reports that Google has orchestrated a $200 billion financing scheme, with $150 billion allocated for AI chips, to support AI start-up Anthropic through a special purpose vehicle and vendor-financing model. An initial $35 billion in hardware, including 1 million TPUs, was purchased in June by the Compute SPV.

telegram · zaihuapd · Aug 4, 10:52

**「Background」** Anthropic, which lacks a credit rating, cannot fund the chip purchases alone, so the structure spreads risk: Google guarantees data centers, Broadcom buys and helps finance chips, and Apollo and Blackstone fund the hardware and lease it back to Anthropic.

**「Impact」** The off-balance-sheet approach shifts the heavy capital burden of AI hardware away from any single company, potentially enabling more large-scale AI infrastructure projects to be financed similarly.

**Tags**: `#AI`, `#Infrastructure Financing`, `#Semiconductors`, `#Anthropic`, `#Google`

---

<a id="item-finance-news-2"></a>
### [Polymarket seeks funding at over $20 billion valuation](https://www.cnbc.com/2026/08/04/polymarket-seeks-fundraising-round-at-more-than-20-billion-valuation.html) ⭐️ 8.0/10

Polymarket is in talks for a fundraising round that would value the prediction market platform at more than $20 billion, a person familiar with the matter told CNBC. The company said in late June that its annualized revenue was well above $1 billion.

rss · CNBC Finance · Aug 4, 13:31

**「Background」** The discussions follow a $15 billion valuation in April and the May launch of its regulated U.S. exchange, which now handles over $100 million in daily notional volume. Rival Kalshi was valued at $22 billion in a funding round announced in May.

**Tags**: `#prediction markets`, `#Polymarket`, `#fundraising`, `#valuation`, `#fintech`

---

<a id="item-finance-news-3"></a>
### [China&\#x27;s State Post Bureau Investigates Shentong Express Over Safety Failures](https://www.spb.gov.cn/gjyzj/c100015/c100016/202608/c4467c234e1c4db0a6e393cff2e64902.shtml) ⭐️ 8.0/10

China&\#x27;s State Post Bureau announced on August 4 that it has opened an investigation into Shentong Express for safety lapses and a lack of unified safety management.

telegram · zaihuapd · Aug 4, 12:07

**「Background」** The investigation follows multiple production safety accidents and repeatedly identified safety hazards since 2026 at courier businesses using the Shentong brand, with the company accused of failing to enforce unified safety management as required by regulations.

**Tags**: `#regulatory investigation`, `#logistics`, `#Shentong Express`, `#production safety`, `#listed company`

---