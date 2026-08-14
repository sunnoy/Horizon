---
layout: default
title: "Horizon Summary: 2026-08-14 (EN)"
date: 2026-08-14
lang: en
---

> From 51 items, 22 important content pieces were selected

---

**Technology News**
1. [Spaghettifying DRAM Enables Unfettered Memory Access on AMD Jaguar](#item-tech-news-1) ⭐️ 9.0/10
2. [GLM-5.3: Frontier Coding with Emergent Cyber Capabilities](#item-tech-news-2) ⭐️ 8.0/10
3. [How Compaction Works in Pi](#item-tech-news-3) ⭐️ 8.0/10
4. [Single log line causes 49–110KB+ disk writes in systemd-journald](#item-tech-news-4) ⭐️ 8.0/10
5. [NP-overrated: When NP-hardness Doesn&\#x27;t Matter in Practice](#item-tech-news-5) ⭐️ 8.0/10
6. [Xiaohongshu Open-Sources dots3-note: 280B MoE with 16B Active Parameters](#item-tech-news-6) ⭐️ 8.0/10
7. [US Judge Orders Google to Remove Third-Party App Store Installation Barriers](#item-tech-news-7) ⭐️ 8.0/10
8. [Google Introduces Gemini 3.7 Flash with Introductory Pricing Set to Double in 2026](#item-tech-news-8) ⭐️ 7.0/10
9. [Why Claude Opus 5 Feels Worse to Work With](#item-tech-news-9) ⭐️ 7.0/10
10. [DeepSeek Harness: Early Developer Preview of Traceable Agent Framework](#item-tech-news-10) ⭐️ 7.0/10
11. [Bluesky Protocol Services Simplify Firehose Consumption with New Jetstream](#item-tech-news-11) ⭐️ 7.0/10
12. [Understanding is the new bottleneck](#item-tech-news-12) ⭐️ 7.0/10
13. [Link Rot Study Follows 657,607 Links to Map the Old Web&\#x27;s Decay](#item-tech-news-13) ⭐️ 7.0/10
14. [X Open-Sources Ranking Algorithm, Lets Users Check Shadowban Status](#item-tech-news-14) ⭐️ 7.0/10
15. [Vivodyne&\#x27;s AI-Powered Lab Tests 3 Million Human Tissues Yearly, Targeting Animal Testing Replacement](#item-tech-news-15) ⭐️ 7.0/10

**Financial News**
1. [Uber and Pony.ai plan to deploy 2,000 robotaxis across Europe](#item-finance-news-1) ⭐️ 8.0/10
2. [S&amp;P 500 profit margins reach record 16.9% in Q2, supporting stock rally](#item-finance-news-2) ⭐️ 8.0/10
3. [Bill Ackman&\#x27;s Pershing Square buys Netflix stake again, cites streaming dominance](#item-finance-news-3) ⭐️ 8.0/10
4. [US to Impose Up to 100% Tariff on Imported Drones from September 2026](#item-finance-news-4) ⭐️ 8.0/10
5. [Trustar Capital Nears Over $1.5 Billion Deal for Alibaba’s Gaming Unit](#item-finance-news-5) ⭐️ 8.0/10
6. [Reddit Surges 12% on S&amp;P 500 Inclusion; Applied Materials Drops 5%](#item-finance-news-6) ⭐️ 7.0/10
7. [Apple Proposes Up to 15% Commission on External App Purchases in the US](#item-finance-news-7) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Spaghettifying DRAM Enables Unfettered Memory Access on AMD Jaguar](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 9.0/10

Security researcher Christopher Domas has disclosed a novel hardware attack technique called &\#x27;spaghettifying DRAM&\#x27; that achieves unfettered memory access on AMD Jaguar \(AMD16h\) platforms. The method deeply manipulates DRAM controller behavior to bypass standard memory protections, granting ring-0 code access to memory regions normally hidden in negative ring territories. The GitHub repository provides a proof-of-concept for this 2013-era architecture, with notes about a different base address for memory controller registers on newer Zen 3 processors, but no confirmation of wider applicability. The technique exposes a significant attack surface inherent in the complexity of modern DRAM subsystems, and the upcoming Black Hat talk is expected to explain the underlying mechanisms in detail.

hackernews · matt\_d · Aug 13, 14:17 · [Discussion](https://news.ycombinator.com/item?id=49286341)

**「Background on DRAM Scrambling」** Modern CPUs scramble the mapping between physical addresses and DRAM cells to obscure the layout of sensitive regions like the Platform Security Processor \(PSP\), System Management Mode \(SMM\) memory, and microcode. The skitter-creek-bath-salts project by Christopher Domas shows that flipping specific configuration bits in the memory controller can rewrite this address translation, effectively &\#x27;spaghettifying&\#x27; memory to bypass these hardware-enforced isolation boundaries.

**「Impact」** On affected AMD Jaguar systems, an attacker with ring-0 access can completely bypass memory isolation and read or modify otherwise inaccessible memory regions, which poses a direct threat to the security model of game consoles like Xbox and PlayStation that rely on this CPU family.

**「Community Discussion」** Commenters expressed excitement for the technique and the forthcoming Black Hat presentation, while raising concerns about the limited scope of the demonstration; several noted that the disclosure only confirms the attack on the older AMD Jaguar architecture and questioned whether it works on newer processors, calling for more information on other CPU families.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/xoreaxeaxeax/skitter-creek-bath-salts">GitHub - xoreaxeaxeax/ skitter - creek - bath - salts : Unlocking...</a></li>
<li><a href="https://cybersecuritynews.com/dram-scrambling-attack/">New DRAM Scrambling Attack Exposes CPU&#x27;s Most Protected...</a></li>

</ul>
</details>

**Tags**: `#hardware`, `#security`, `#DRAM`, `#reverse-engineering`, `#vulnerabilities`

---

<a id="item-tech-news-2"></a>
### [GLM-5.3: Frontier Coding with Emergent Cyber Capabilities](https://z.ai/blog/glm-5.3) ⭐️ 8.0/10

Z.AI&\#x27;s GLM-5.3 model demonstrates emergent autonomous vulnerability discovery and red-teaming capabilities, including finding zero-day vulnerabilities in WordPress plugins, achieving remote code execution, and adapting a 6.8 kernel exploit. The model is deployed in a coordinated vulnerability disclosure \(CVD\) program that scans open-source software at scale, leading to multiple CVE assignments. While it still trails slightly behind top models like Sol and Fable on some benchmarks, its practical exploit generation and responsible disclosure infrastructure represent a significant advance in AI-driven cybersecurity. The model is based on GLM-5.2 with post-training enhancements, and weights are expected to be released in two weeks.

hackernews · pella · Aug 14, 05:19 · [Discussion](https://news.ycombinator.com/item?id=49294997)

**「Background」** GLM-5.3, released by Z.ai on August 14, 2026, is an update to the GLM-5.2 model that uses the same base architecture but achieves all performance gains through scaled-up post-training. This approach yields emergent cybersecurity capabilities, including autonomous vulnerability discovery and red-teaming, while the model weights are scheduled to be open-sourced.

**「Impact」** Software maintainers may see an influx of automated vulnerability reports from GLM-5.3&\#x27;s CVD program, potentially accelerating the disclosure and patching of critical flaws in widely used open-source projects.

**「Community Discussion」** Community members report successful red-team engagements with the model, note the large-scale CVD scanning generating many CVEs, and debate benchmark omissions; some praise the announcement&\#x27;s researcher-oriented tone.

<details><summary>References</summary>
<ul>
<li><a href="https://www.unite.ai/z-ai-launches-glm-5-3-with-frontier-coding-and-a-cyber-capability-that-outgrew-its-training/">Z.ai Launches GLM-5.3 With Frontier Coding and a Cyber Capability That Outgrew Its Training – Unite.AI</a></li>
<li><a href="https://blog.sandbase.ai/glm-5-3-release-watch-2026/">GLM-5.3 Launches: Frontier Coding and Emergent Cybersecurity | SandBase Blog</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cybersecurity`, `#vulnerability-research`, `#coding`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [How Compaction Works in Pi](https://earendil.com/posts/compaction-in-pi/) ⭐️ 8.0/10

The article explains Pi&\#x27;s compaction mechanism, which condenses long conversation histories into compact summaries to keep the LLM&\#x27;s context window manageable. It details how the algorithm identifies and preserves key information, such as user intents and important actions, while discarding low-value exchanges like side tangents or tool call outputs. This approach aims to maintain conversation coherence without the loss of nuance that can occur with simple summarization. The technique is of interest to developers building LLM agents that need to handle extended interactions.

hackernews · tosh · Aug 13, 17:57 · [Discussion](https://news.ycombinator.com/item?id=49289654)

**「Context Compaction in LLM Agents」** Pi is an AI coding agent that uses compaction to summarize older conversation history when the context exceeds the model&\#x27;s token limit. The compaction process generates a summary that is stored as plain text in the session, replacing the original messages to keep the context manageable while preserving key information. This technique contrasts with pruning, which removes low-value messages, and aims to maintain conversation continuity without losing intent.

**「Community Discussion」** Commenters debate compaction versus pruning, with some reporting that summarization can lose intent and that removing low-value messages outright \(pruning\) better preserves conversation history. Others share alternative techniques like nested-thread architectures that summarize entire sub-threads, and dual KV caches to summarize tokens during generation.

<details><summary>References</summary>
<ul>
<li><a href="https://earendil.com/posts/compaction-in-pi/">How Compaction Works in Pi | EARENDIL</a></li>
<li><a href="https://github.com/earendil-works/pi/blob/main/packages/coding-agent/docs/compaction.md">pi/packages/coding-agent/docs/compaction.md at main ... - GitHub</a></li>

</ul>
</details>

**Tags**: `#ai`, `#context-management`, `#compaction`, `#llm-agents`, `#pi`

---

<a id="item-tech-news-4"></a>
### [Single log line causes 49–110KB+ disk writes in systemd-journald](https://github.com/systemd/systemd/issues/40262) ⭐️ 8.0/10

An issue in systemd-journald reveals that a single log line can trigger 49KB+ of disk writes on ext4 and 110KB+ on btrfs due to the use of memory-mapped \(mmap\) file writes for logging. The write amplification stems from the mmap design, which is intended for random-access patterns but leads to excessive page dirtying and metadata updates when appending small log entries. The finding has sparked debate about the appropriateness of mmap for append-only logging, with critics arguing that pwrite or sequential file writes would be far more efficient. The issue \(systemd/systemd\#40262\) raises concerns about SSD wear and system performance for workloads that generate many log lines.

hackernews · ValdikSS · Aug 13, 18:41 · [Discussion](https://news.ycombinator.com/item?id=49290215)

**「systemd-journald&\#x27;s mmap-based logging」** systemd-journald, the default logging component of systemd, stores log entries in a binary format that uses memory-mapped file \(mmap\) access for writing, a design intended to ensure atomicity and crash resilience. This approach can cause significant write amplification because even a single short log line may trigger larger page-aligned metadata updates, especially on filesystems like ext4 and btrfs. The reported issue demonstrates that such writes can reach 49 KB or more on ext4 and 110 KB+ on btrfs, raising concerns about excessive disk I/O and storage wear, particularly on flash-based devices.

**「Impact」** A single log line written by systemd-journald can cause 49KB+ of disk writes on ext4 and 110KB+ on btrfs, unnecessarily increasing I/O overhead and wearing out SSDs on affected systems.

**「Community Discussion」** Community discussion highlights broad agreement that the mmap-based logging design is fundamentally wrong for append-only log files, with commenters advocating for pwrite or sequential writes. Users also report that journald&\#x27;s lack of fine-grained filtering amplifies the problem when buggy drivers or applications generate excessive log entries, further stressing disk I/O.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/systemd/systemd/issues/40262">Excessive IO caused by systemd - journald · Issue # 40262 ...</a></li>
<li><a href="https://unix.stackexchange.com/questions/704683/reducing-flash-wear-from-systemd-journald-embedded-device">Reducing flash wear from Systemd Journald (embedded device)</a></li>
<li><a href="https://eucloudservers.com/data-platforms-storage/single-log-line-is-49kb-ext4-110kb-btrfs-of-systemd-journald-disk-writes/">Single Log Line Is 49KB+ (Ext4) / 110KB+ (Btrfs) Of Systemd - journald ...</a></li>
<li><a href="https://zeli.app/en/story/49290215">systemd - journald writes 49KB+ per log line on ext4, 110KB+ on btrfs...</a></li>

</ul>
</details>

**Tags**: `#systemd`, `#journald`, `#mmap`, `#disk-io`, `#linux`, `#logging`

---

<a id="item-tech-news-5"></a>
### [NP-overrated: When NP-hardness Doesn&\#x27;t Matter in Practice](https://gruhn.me/blog/2026-08-13/) ⭐️ 8.0/10

A blog post on gruhn.me argues that NP-hardness is often overrated in practical software engineering, emphasizing that heuristics, problem restrictions, and approximate solutions frequently suffice for real-world instances. The post contends that the intimidating combinatorial explosion associated with NP-hard problems rarely materializes in typical use cases, and that practitioners can often achieve acceptable results without solving the general worst-case scenario. It highlights how many software engineering tasks, such as dependency resolution or type checking, are handled by avoiding the hardest subproblems or by using fast algorithms that work well in practice. The argument resonates with a community that shares examples of building practical systems around NP-hard problems, though some note that the classification remains essential for understanding theoretical limits.

hackernews · theanonymousone · Aug 13, 20:14 · [Discussion](https://news.ycombinator.com/item?id=49291268)

**「NP-hardness and practical solvability」** NP-hardness is a classification from computational complexity theory indicating that a problem is at least as hard as the hardest problems in NP, meaning exact solutions may require exponential time in the worst case. Despite this theoretical intractability, many NP-hard problems arising in real-world software engineering—such as dependency resolution, type checking, and scheduling—can be solved efficiently in practice using heuristics, approximations, or by restricting problem instances to those that avoid worst-case behavior.

**「Impact」** The post encourages software engineers to confidently tackle NP-hard problems using heuristic and approximation methods, recognizing that practical instances often avoid the worst-case exponential blow-ups that define the theoretical class.

**「Community Discussion」** Commenters largely agree that many real-world instances of NP-hard problems are tractable with heuristics, with one noting that dependency managers and type systems often restrict the problem space to avoid hardness entirely. Another commenter argues that the theoretical classification is not overrated, as it reveals the fundamental limits of computation and indicates where heuristics become necessary.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49291268">NP - Overrated | Hacker News</a></li>
<li><a href="https://zeli.app/en/story/49291268">NP-hard problems are not as hard as you think — NP - Overrated | Zeli</a></li>

</ul>
</details>

**Tags**: `#computer-science`, `#algorithms`, `#complexity-theory`, `#software-engineering`, `#heuristics`

---

<a id="item-tech-news-6"></a>
### [Xiaohongshu Open-Sources dots3-note: 280B MoE with 16B Active Parameters](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 8.0/10

Xiaohongshu&\#x27;s dots lab has open-sourced dots3-note preview, a 280-billion-parameter Mixture of Experts \(MoE\) model with 16 billion active parameters per token. The model supports a 512K context window and can process text, images, video, and audio. It introduces TEMPO, a novel reinforcement learning method that trains long-horizon agents using self-critique and test-time value estimation. Accompanying the release are the VibeSearchBench and VibeLifeBench real-world agent benchmarks. The open-weight release on Hugging Face makes this large-scale, cost-efficient multimodal model available for research and experimentation.

telegram · zaihuapd · Aug 14, 08:27

**「Background」** Mixture of Experts \(MoE\) models use a large number of total parameters but only activate a subset per input, greatly reducing inference cost. Xiaohongshu, a major Chinese social platform, has been building its own AI capabilities through its dots lab. The open-weight release of such a large model is notable as most Chinese labs keep their largest models proprietary.

**「Impact」** The open-weight release of a 280B-parameter MoE model with 16B active parameters makes cost-efficient large-scale multimodal experimentation accessible, and the TEMPO method with real-world benchmarks may accelerate agentic AI research.

**Tags**: `#AI model`, `#open-source`, `#MoE`, `#multimodal`, `#reinforcement learning`

---

<a id="item-tech-news-7"></a>
### [US Judge Orders Google to Remove Third-Party App Store Installation Barriers](https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/) ⭐️ 8.0/10

A US district judge has ordered Google to eliminate extra steps and warning dialogs in the Play Store that currently impede the installation of third-party Android app stores. The ruling, part of the Epic v. Google antitrust case, deems these multi-step &\#x27;view then install&\#x27; flows as deliberate anti-competitive friction designed to deter average users. Google must comply within one week, making the installation of competing stores as straightforward as sideloading any ordinary Android app. The decision follows a jury verdict that Google illegally monopolized Android app distribution.

telegram · zaihuapd · Aug 14, 09:55

**「Background」** The order arises from the Epic Games v. Google antitrust case, in which a jury found that Google maintained an illegal monopoly in Android app distribution through the Play Store. The court has been directing Google to remove anticompetitive friction, and this latest ruling specifically targets the extra warnings and multi-step process that users face when installing third-party app stores.

**「Impact on users and competition」** Starting within a week, Android users will be able to install third-party app stores without the extra warnings and multi-step dialogs that previously deterred non-technical users, as Google must make the process as straightforward as installing a regular app.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Epic_Games_v._Google">Epic Games v. Google - Wikipedia</a></li>
<li><a href="https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/">Google ordered to remove Android app store warning screens</a></li>
<li><a href="https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/">Google ordered to remove scary warnings when installing third-party app stores</a></li>
<li><a href="https://www.theverge.com/policy/979852/that-is-not-acceptable-judge-orders-google-to-make-rival-app-store-installs-easier">‘That is not acceptable’: Judge orders Google to make rival app store installs easier | The Verge</a></li>

</ul>
</details>

**Tags**: `#antitrust`, `#Google`, `#Android`, `#app stores`, `#Epic Games`

---

<a id="item-tech-news-8"></a>
### [Google Introduces Gemini 3.7 Flash with Introductory Pricing Set to Double in 2026](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 7.0/10

Google has released Gemini 3.7 Flash, a new multimodal AI model, with introductory pricing scheduled to double on December 31, 2026. The model shows strong vision capabilities, performing well on image-to-HTML tasks, though some community tests indicate it still trails behind Opus for that use case. The release comes just three weeks after Gemini 3.6 Flash, raising questions about iteration speed and long-term relevance. Comparison benchmarks against competing models like GPT-5.6 Luna are not yet available, and initial reactions note that Luna \(Max\) already outperforms Gemini 3.7 Flash on the DeepSWE 1.1 benchmark while being cheaper.

hackernews · thisisauserid · Aug 13, 17:23 · [Discussion](https://news.ycombinator.com/item?id=49289112)

**「Background」** Google&\#x27;s Gemini Flash series offers smaller, faster models than its full-scale counterparts. Gemini 3.7 Flash arrives just three weeks after the previous 3.6 Flash, and is described as the most intelligent Flash model for coding and agents. It is being introduced with temporary discounted pricing that will double at the end of 2026.

**「Impact」** Developers relying on Gemini Flash for cost-sensitive tasks will face a doubling of the model&\#x27;s price at the start of 2027, while the rapid release cadence may discourage long-term integration.

**「Community Discussion」** Comments highlight that Opus remains best-in-class for vision tasks, but Gemini 3.7 Flash is impressive relative to its price. The introductory pricing strategy is seen as unusual, and the lack of direct benchmarks against Luna/Terra is a notable gap. Several users consider the Flash series primarily for low-cost, high-volume text applications, and the quick succession of releases makes the model feel ephemeral.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/">Gemini 3 . 7 Flash : our most intelligent workhorse model</a></li>

</ul>
</details>

**Tags**: `#ai`, `#machine-learning`, `#llm`, `#google`, `#model-release`

---

<a id="item-tech-news-9"></a>
### [Why Claude Opus 5 Feels Worse to Work With](https://mun-logadan.github.io/why-does-opus-5-feel-worse/) ⭐️ 7.0/10

Users and developers report that Anthropic&\#x27;s Claude Opus 5 model produces writing that is overly elliptical, abstract, and prone to unnecessary confessions, making extended interactions exhausting. The model also frequently veers off-topic without strict prompting and has strict usage quotas that hinder agentic development. Some users suspect the model is smaller or more cost-optimized, leading to a perceived decline in quality compared to Opus 4.8 and competitors like OpenAI&\#x27;s models.

hackernews · numeri · Aug 14, 10:12 · [Discussion](https://news.ycombinator.com/item?id=49296740)

**「Background」** Claude Opus 5 is Anthropic&\#x27;s flagship large language model, built for demanding reasoning, coding, and long-horizon agentic tasks. It offers a 1-million-token context window, a maximum output of 128,000 tokens, and is priced at $5 per million input tokens and $25 per million output tokens via the API.

**「Impact」** Developers working on coding, agentic tasks, or creative projects are switching back to Opus 4.8 or moving to OpenAI&\#x27;s models due to Opus 5&\#x27;s tiring communication style and restrictive usage limits.

**「Community Discussion」** Commenters on Hacker News broadly agree that Opus 5&\#x27;s elliptical prose and unnecessary confessions degrade the user experience, with some attributing the decline to Anthropic&\#x27;s cost-cutting and dismissing benchmark improvements as marketing.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/anthropic/claude-opus-5">Claude Opus 5 - API Pricing &amp; Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#Claude`, `#user experience`, `#model evaluation`

---

<a id="item-tech-news-10"></a>
### [DeepSeek Harness: Early Developer Preview of Traceable Agent Framework](https://deepseek.com/harness/en/) ⭐️ 7.0/10

DeepSeek has released an open-source developer preview of Harness, a plugin-based AI agent framework licensed under MIT. The framework features hot-reloading and dynamic enabling/disabling of plugins, as well as full run traceability via an append-only session log that records system prompts, reasoning, tool calls, subagent scheduling, and context injections. A Trajectory view allows inspecting, resuming, forking, and replaying runs from the same event stream. The release is based on Cordis v4, a system for hot-loading and unloading plugins with state reversion, and the authors caution that it is an early preview with many rough edges and compatibility-breaking changes.

hackernews · bjin · Aug 13, 12:58 · [Discussion](https://news.ycombinator.com/item?id=49285244)

**「Background」** AI agent frameworks orchestrate language models to use tools, reason, and perform multi-step tasks. Plugin architectures allow developers to compose functionality modularly, but typically require restarting the process to add or remove plugins. DeepSeek Harness extends this idea with runtime dynamic plugin management and built-in traceability, building on the Cordis v4 library that has been used in the Koishi chatbot project for four years.

**「Impact」** Developers building AI agents gain an open-source, MIT-licensed alternative with full traceability, potentially enabling auditing and iterative improvement of agent behavior in ways that closed-source models do not permit, though the tool is not yet production-ready.

**「Community Discussion」** Commenters praised the append-only traceability as a standout feature, especially compared to US models that encrypt or obfuscate traces. The authors acknowledged the early, rough state and invited feedback. Some expressed skepticism about plugin-heavy architectures, while others emphasized the powerful state-reverting plugin management provided by Cordis v4.

**Tags**: `#DeepSeek Harness`, `#AI agents`, `#developer tools`, `#plugin system`, `#open source`

---

<a id="item-tech-news-11"></a>
### [Bluesky Protocol Services Simplify Firehose Consumption with New Jetstream](https://atproto.com/blog/introducing-bluesky-protocol-services) ⭐️ 7.0/10

Bluesky announced Protocol Services, a new suite aimed at simplifying interaction with the AT Protocol firehose and strengthening decentralized infrastructure. Central to the release is a new Jetstream service that allows developers to consume the firehose directly in the browser without needing a server. The original Jetstream already provided a lightweight way to access the stream of public events, and the new version refines that capability. This move is part of Bluesky’s broader effort to expand the protocol beyond its app, enabling more third-party innovation. The services are designed to make the AT Protocol ecosystem more accessible to builders.

hackernews · danabramov · Aug 14, 00:14 · [Discussion](https://news.ycombinator.com/item?id=49293324)

**「Background」** The AT Protocol \(Authenticated Transfer Protocol\) is an open standard for decentralized social networking, powering the Bluesky platform. Bluesky&\#x27;s firehose provides a real-time stream of all public events on the network, and the original Jetstream tool made it easy to consume this firehose even directly from a browser. The newly introduced Bluesky Protocol Services include Jetstream v2, which adds network replay and a TypeScript SDK, aiming to further simplify development on the AT Protocol.

**「Impact」** Developers can now integrate with the Bluesky firehose entirely client-side, eliminating server-side dependencies and lowering the barrier to entry for building decentralized applications.

**「Community Discussion」** Commenters praised the original Jetstream for its ease of use and quickly updated browser demos to the new service. Some raised broader ideas like using Bluesky for DNS, while others noted the expansion beyond the app coincides with a shrinking active user base.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AT_Protocol">AT Protocol - Wikipedia</a></li>
<li><a href="https://atproto.com/blog/introducing-bluesky-protocol-services">Introducing Bluesky Protocol Services - AT Protocol</a></li>

</ul>
</details>

**Tags**: `#decentralization`, `#protocols`, `#open-source`, `#social-media`, `#infrastructure`

---

<a id="item-tech-news-12"></a>
### [Understanding is the new bottleneck](https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck) ⭐️ 7.0/10

Geoffrey Litt argues that as AI tools increasingly generate code, the primary bottleneck in software engineering shifts from writing code to understanding it. The article contends that this changes the priorities for developers, who must now focus more on comprehension, review, and integration of machine-generated code. The piece suggests that this shift may reshape how engineers approach development, emphasizing the need for human judgment and analysis over raw coding speed.

hackernews · sebg · Aug 13, 18:47 · [Discussion](https://news.ycombinator.com/item?id=49290299)

**「Background」** With the rise of large language models capable of generating functional code, software engineers are facing a shift in bottlenecks: from writing code to understanding the code that AI produces. Geoffrey Litt, an engineer at Notion, explored this challenge in a July 2026 talk at the AI Engineer conference, warning that without deep comprehension, developers accumulate “cognitive debt” that can undermine system reliability.

**「Community Discussion」** Commenters largely agree that AI code generation amplifies the existing challenge of understanding code, but some argue that this bottleneck is not new and has long been a concern for engineering leadership. Others note that LLM-generated explanations lack the motivation and insight needed for true comprehension, and that human analysis remains essential to detect subtle breaks in underlying models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck.html">Understanding is the new bottleneck - geoffreylitt.com</a></li>
<li><a href="https://www.youtube.com/watch?v=WkBPX-oDMnA">Understanding is the new bottleneck — Geoffrey Litt, Notion Understanding is the new bottleneck — Geoffrey Litt, Notion Understanding: The New Bottleneck in AI Code Generation Understanding is the new bottleneck — Geoffrey Litt, Notion Understanding is the new bottleneck: does a human still need ...</a></li>

</ul>
</details>

**Tags**: `#software-engineering`, `#artificial-intelligence`, `#code-generation`, `#llm`, `#developer-productivity`

---

<a id="item-tech-news-13"></a>
### [Link Rot Study Follows 657,607 Links to Map the Old Web&\#x27;s Decay](https://0.mk/blog/link-rot) ⭐️ 7.0/10

An analysis of 657,607 links, published on the 0.mk blog, sought to quantify link rot—the phenomenon where once-valid URLs become dead or inaccessible. The study found that a substantial portion of the links from the past two decades are now broken, illustrating the rapid decay of the early web. The results prompted a lively discussion on the definition of the &\#x27;old web,&\#x27; with commenters placing its end anywhere from the pre-Google search era to the rise of Facebook. The findings highlight the fragility of digital history and the difficulty of preserving the web’s early content.

hackernews · tdx · Aug 13, 17:49 · [Discussion](https://news.ycombinator.com/item?id=49289532)

**「Background」** The study draws on a corpus of 657,607 links collected from the 0.mk URL shortener, which operated between 2009 and 2014. Link rot refers to the phenomenon where URLs become inaccessible over time, often due to websites shutting down or content being removed.

**「Community Discussion」** Commenters disagreed on when the &\#x27;old web&\#x27; ended, with suggestions ranging from before Google Search became public \(circa 1997\) to the decline of the blogosphere during Facebook&\#x27;s ascent \(2009–2014\). Some argued that the nostalgia for the old web is a cultural experience tied to personal discovery of online communities, while one contrarian viewpoint speculated that the decentralized, indie web might return as mainstream platforms lose appeal.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49289532">Where did the old web go? We followed 657,607 links to find ...</a></li>
<li><a href="https://www.egearge.com/haber/u-0d0ca0eaaa5a/where-did-the-old-web-go-we-followed-657-607-links-to-find-out">Where did the old web go? We followed 657,607 links to find out</a></li>

</ul>
</details>

**Tags**: `#link-rot`, `#web-preservation`, `#data-analysis`, `#internet`, `#history`

---

<a id="item-tech-news-14"></a>
### [X Open-Sources Ranking Algorithm, Lets Users Check Shadowban Status](https://techcrunch.com/2026/08/13/x-open-sources-its-ranking-algorithm-letting-users-see-if-theyve-been-shadowbanned/) ⭐️ 7.0/10

X has open-sourced its &\#x27;For You&\#x27; timeline ranking engine on GitHub under the Apache 2.0 license, with the released code being 10 to 15 times larger than previous contributions. The company also introduced a transparency tool that lets users with at least 10 posts in the past month download a JSON file indicating whether their account or posts were flagged by the ranking system; the tool will first roll out to test users whose accounts are at least one year old. Parts of the Grok system used to detect rule-breaking content remain closed. This move provides external researchers and developers with concrete code to analyze how X ranks content, while giving users direct insight into potential shadowbanning.

telegram · zaihuapd · Aug 14, 01:03

**「Background」** Ranking algorithms determine the order and visibility of posts on social media feeds, and &\#x27;shadowbanning&\#x27; refers to covertly limiting a user&\#x27;s reach without notification. X had previously released some recommendation-related code, but the full &\#x27;For You&\#x27; engine was not public. The Apache 2.0 license permits broad use and modification, which can facilitate independent audits of algorithmic bias.

**「Impact」** Developers and researchers can now audit X&\#x27;s recommendation system for fairness and technical behavior, while users gain a direct, data-driven check on whether they are being silently downranked—potentially increasing platform accountability. However, the full impact depends on the tool&\#x27;s adoption and the completeness of the disclosed code, as some violation-detection components remain closed.

**Tags**: `#open-source`, `#ranking-algorithm`, `#machine-learning`, `#social-media`, `#transparency`

---

<a id="item-tech-news-15"></a>
### [Vivodyne&\#x27;s AI-Powered Lab Tests 3 Million Human Tissues Yearly, Targeting Animal Testing Replacement](https://www.fastcompany.com/91589344/the-worlds-largest-biological-datacenter-could-help-make-animal-testing-obsolete) ⭐️ 7.0/10

Vivodyne has deployed 12 “hive” robotic labs in South San Francisco that grow human tissues and use AI to design experiments, aiming to better predict drug efficacy and safety. The system can test over 3 million human tissue samples per year—double the capacity of all US clinical trials combined. This scale is intended to address the fact that about 90% of clinical trials fail after passing animal tests. The AI-driven platform hopes to make animal testing obsolete by providing more reliable preclinical data.

telegram · zaihuapd · Aug 14, 01:48

**「Background」** Animal testing is a standard but imperfect predictor of human drug responses, with about 90% of drugs that pass animal trials failing in human clinical trials. Lab-grown human tissues aim to provide more accurate models, but scaling them for high-throughput testing has been a challenge.

**「Impact」** By providing more predictive human-relevant data, the platform could dramatically reduce the 90% clinical trial failure rate, potentially saving billions in drug development costs and diminishing the need for animal testing.

**Tags**: `#AI`, `#biotech`, `#drug-discovery`, `#robotics`, `#technology-industry`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Uber and Pony.ai plan to deploy 2,000 robotaxis across Europe](https://www.cnbc.com/2026/08/14/uber-partners-with-chinas-ponyai-for-2000-robotaxis-in-europe.html) ⭐️ 8.0/10

Uber and Pony.ai announced a partnership to deploy 2,000 self-driving taxis across Europe. The plan will expand their robotaxi service to four new cities, though no timeline or specific locations were disclosed.

rss · CNBC Finance · Aug 14, 01:02

**「Background」** The companies launched a commercial robotaxi service in Zagreb, Croatia in March, which they claim is the first in Europe.

**Tags**: `#autonomous vehicles`, `#robotaxi`, `#Uber`, `#Pony.ai`, `#Europe`

---

<a id="item-finance-news-2"></a>
### [S&amp;P 500 profit margins reach record 16.9% in Q2, supporting stock rally](https://www.cnbc.com/2026/08/13/these-charts-show-why-stocks-keep-rallying-profit-margins-are-highest-on-record.html) ⭐️ 8.0/10

In the second quarter, S&amp;P 500 companies’ net profit margins hit a record 16.9%, according to FactSet, up from 14.8% in the previous quarter and well above the five-year average of 12.4%.

rss · CNBC Finance · Aug 13, 20:21

**「Background」** The net profit margin measures the percentage of revenue a company retains after all expenses, and this record reading, driven by tech giants Alphabet and Amazon as well as broad-based improvements, has been tracked since 2009.

**「Impact」** The elevated profit margins provide a fundamental tailwind for the stock market by underpinning earnings growth and investor confidence.

**Tags**: `#corporate earnings`, `#stock market`, `#profit margins`, `#S&amp;P 500`, `#technology sector`

---

<a id="item-finance-news-3"></a>
### [Bill Ackman&\#x27;s Pershing Square buys Netflix stake again, cites streaming dominance](https://www.cnbc.com/2026/08/13/ackman-buys-netflix-again-four-years-later-says-it-won-streaming-wars.html) ⭐️ 8.0/10

Bill Ackman’s Pershing Square Capital Management disclosed a new Netflix stake, saying the streaming giant has won the streaming wars with over 325 million subscribers and its stock is now attractively valued after a 50% decline from its June 2025 high.

rss · CNBC Finance · Aug 13, 18:04

**「Background」** Ackman briefly owned Netflix in 2022 but sold the entire stake after the company reported its first subscriber decline in more than a decade.

**Tags**: `#hedge fund`, `#streaming`, `#stocks`, `#investing`, `#valuation`

---

<a id="item-finance-news-4"></a>
### [US to Impose Up to 100% Tariff on Imported Drones from September 2026](https://www.whitehouse.gov/presidential-actions/2026/08/adjusting-imports-of-unmanned-aircraft-systems-and-unmanned-aircraft-systems-components-into-the-united-states/) ⭐️ 8.0/10

The US President signed a proclamation on August 13 introducing new tariffs on imported drones and components. Effective September 3, 2026, drones over 25 kg, thermal imaging drones, drone base stations, and some key components will face a 100% tariff, while drones weighing 25 kg or less will be subject to a 25% tariff.

telegram · zaihuapd · Aug 14, 01:24

**「Background」** The tariffs are imposed under the authority of the Trade Expansion Act of 1962, as amended, which allows the President to adjust imports that threaten national security.

**「Impact」** The tariffs will raise costs for U.S. importers and businesses that depend on imported drones, such as those used in agriculture, surveillance, and delivery services.

<details><summary>References</summary>
<ul>
<li><a href="https://www.whitehouse.gov/presidential-actions/2026/08/adjusting-imports-of-unmanned-aircraft-systems-and-unmanned-aircraft-systems-components-into-the-united-states/">Adjusting Imports of Unmanned Aircraft Systems and Unmanned ...</a></li>

</ul>
</details>

**Tags**: `#drones`, `#tariffs`, `#trade policy`, `#imports`, `#US policy`

---

<a id="item-finance-news-5"></a>
### [Trustar Capital Nears Over $1.5 Billion Deal for Alibaba’s Gaming Unit](https://www.bloomberg.com/news/articles/2026-08-14/trustar-is-said-to-near-1-5-billion-deal-for-alibaba-gaming-arm) ⭐️ 8.0/10

Trustar Capital, a private equity arm of CITIC Group, is close to acquiring Alibaba’s video game unit Lingxi for a valuation that could exceed $1.5 billion, Bloomberg reported.

telegram · zaihuapd · Aug 14, 10:24

**「Background」** Alibaba is shedding non-core businesses to concentrate on artificial intelligence and cloud services under CEO Wu Yongming.

**Tags**: `#Mergers &amp; Acquisitions`, `#Gaming Industry`, `#Alibaba Group`, `#CITIC`, `#Divestiture`

---

<a id="item-finance-news-6"></a>
### [Reddit Surges 12% on S&amp;P 500 Inclusion; Applied Materials Drops 5%](https://www.cnbc.com/2026/08/14/stocks-making-the-biggest-moves-premarket-rddt-amat-sndk-w.html) ⭐️ 7.0/10

In premarket trading, Reddit shares surged 12% after S&amp;P Dow Jones Indices announced the company would join the S&amp;P 500 index, while Applied Materials fell over 5% following mixed quarterly results.

rss · CNBC Finance · Aug 14, 10:46

**「Background」** Index funds that track the S&amp;P 500 will need to buy Reddit shares, and Applied Materials&\#x27; revenue in its core semiconductor systems division only slightly exceeded the FactSet consensus estimate.

**Tags**: `#premarket movers`, `#S&amp;P 500 inclusion`, `#earnings reports`, `#analyst upgrades`, `#mergers and acquisitions`

---

<a id="item-finance-news-7"></a>
### [Apple Proposes Up to 15% Commission on External App Purchases in the US](https://9to5mac.com/2026/08/13/apple-proposes-commissions-of-up-to-15-for-off-app-store-purchases-in-the-us/) ⭐️ 7.0/10

Apple proposed a commission structure to a US court for purchases made outside its App Store, with rates of up to 15% for standard apps, 10% for video and news partnerships and subscription renewals, and 5% for small businesses.

telegram · zaihuapd · Aug 14, 02:33

**「Background」** The US Supreme Court earlier denied Apple’s request to pause the lower court’s review of commission rates, and the company expects to submit its written arguments to the Supreme Court by September 14.

**Tags**: `#Apple`, `#App Store`, `#commissions`, `#regulation`, `#Epic Games`

---