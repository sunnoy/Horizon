---
layout: default
title: "Horizon Summary: 2026-08-18 (EN)"
date: 2026-08-18
lang: en
---

> From 43 items, 14 important content pieces were selected

---

**Technology News**
1. [DuckDB 2.0 Preview Introduces Quack Engine](#item-tech-news-1) ⭐️ 9.0/10
2. [Linux 7.3 improves performance when running out of VRAM](#item-tech-news-2) ⭐️ 8.0/10
3. [Google buys Spirit Airlines&\#x27; data from bankruptcy auction for AI training](#item-tech-news-3) ⭐️ 8.0/10
4. [GitHub Copilot Autofix Injects Vulnerability into Snowflake&\#x27;s Jira CI/CD](#item-tech-news-4) ⭐️ 8.0/10
5. [Rust GPU Offload Paper Proposes Portable, Safe GPU Programming](#item-tech-news-5) ⭐️ 8.0/10
6. [Qwen 3.8 27B Scores 52, Matching GPT-5.6 Luna](#item-tech-news-6) ⭐️ 8.0/10
7. [Fairphone 6 Main Camera Now Works on PostmarketOS](#item-tech-news-7) ⭐️ 7.0/10
8. [AirTag Tracked Rare Books to Amazon’s AI Training Facility](#item-tech-news-8) ⭐️ 7.0/10
9. [macOS 26.7 Code Reveals Apple Intelligence Censorship for China](#item-tech-news-9) ⭐️ 7.0/10
10. [Enterprise WeChat 5.0.10 Opens CLI and MCP for AI Agent Integration](#item-tech-news-10) ⭐️ 7.0/10
11. [China Orders Early Removal of Tailored Windows 10 from State Agencies](#item-tech-news-11) ⭐️ 7.0/10

**Financial News**
1. [Buy-Now-Pay-Later Loans Expand to Rent and Utilities, U.S. Borrowing Hits $160 Billion in 2025](#item-finance-news-1) ⭐️ 8.0/10
2. [Prediction market traders see 1-in-4 odds Paramount’s Warner Bros. bid fails](#item-finance-news-2) ⭐️ 7.0/10
3. [Apple&\#x27;s US App Store Commission Revenue Falls 18% as Consumer Spending Declines 6%](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [DuckDB 2.0 Preview Introduces Quack Engine](https://duckdb.org/2026/08/17/duckdb-20-highlights) ⭐️ 9.0/10

The DuckDB team has shared a preview of the upcoming v2.0 release of the embedded analytical database. The update introduces a new query engine called Quack, alongside over 10,000 commits made in the last six months, signaling rapid development. DuckDB continues to excel at out-of-core, larger-than-memory data processing on consumer hardware, and the new version expands support for spatial data, graph processing, and real-time analytics. The preview has generated widespread enthusiasm among data engineers and developers.

hackernews · ibotty · Aug 17, 13:46 · [Discussion](https://news.ycombinator.com/item?id=49330781)

**「Background」** DuckDB is an embedded analytical database management system known for its high performance and ease of use. The upcoming version 2.0, currently in early development, previewed in August 2026, introduces server mode, triggers, a VARIANT type, asynchronous I/O, a new SQL parser, and a new storage format. This release builds on DuckDB&\#x27;s widespread adoption for data processing and analytics.

**「Impact」** The release is expected to bring meaningful performance gains and new capabilities, further lowering the barrier for complex data processing on modest hardware.

**「Community Discussion」** Commenters praised DuckDB&\#x27;s portability and versatility, with many sharing production use cases in streaming, pipelines, and analytics, and expressed strong anticipation for v2.0.

<details><summary>References</summary>
<ul>
<li><a href="https://duckdb.org/2026/08/17/duckdb-20-highlights">A Preview of DuckDB v2.0 – DuckDB</a></li>
<li><a href="https://duckdb.org/install/preview">DuckDB Preview (Nightly) Installation – DuckDB</a></li>

</ul>
</details>

**Tags**: `#duckdb`, `#databases`, `#analytics`, `#open-source`, `#release-preview`

---

<a id="item-tech-news-2"></a>
### [Linux 7.3 improves performance when running out of VRAM](https://pixelcluster.dev/VRAM-Overcommit/) ⭐️ 8.0/10

The upcoming Linux kernel 7.3 introduces a new VRAM overcommit mechanism that improves performance and reduces crashes when GPU memory is exhausted. The kernel now applies a more intelligent eviction policy for GPU memory allocations, similar to system RAM overcommit, allowing applications to continue running instead of failing with out-of-memory errors. This change is especially beneficial for AI, gaming, and GPU-accelerated desktop workloads where memory pressure is frequent. The implementation prioritizes critical allocations and gracefully degrades performance, mitigating the severe stuttering and system instability that previously occurred when VRAM was full.

hackernews · flaburgan · Aug 18, 07:51 · [Discussion](https://news.ycombinator.com/item?id=49342719)

**「Background」** Prior to Linux 7.3, the kernel’s handling of VRAM exhaustion could lead to severe performance drops or application crashes when the GPU ran out of dedicated video memory. The author of the article developed a set of kernel patches to redesign the VRAM overcommit logic, initially focused on improving AMDGPU’s memory management for low-end GPUs. These patches have now been merged upstream and are queued for the Linux 7.3 release.

**「Impact」** Users with low VRAM GPUs or memory-intensive workloads will experience fewer crashes and more graceful performance degradation when GPU memory is exhausted, avoiding the frequent reboots and compositor instability that plagued systems like those with a 2 GB NVIDIA 750 Ti.

**「Community Discussion」** Community members expressed strong enthusiasm for the kernel 7.3 update, with many recalling past VRAM exhaustion crashes on low-memory GPUs \(e.g., NVIDIA 750 Ti\) and noting that this improvement addresses a long-standing pain point; some also hoped for analogous overcommit handling for system RAM to prevent entire system freezes.

<details><summary>References</summary>
<ul>
<li><a href="https://pixelcluster.dev/VRAM-Overcommit/">VRAM Management Part 2: Beyond the Limits of Physical VRAM | pixelcluster&#x27;s GPU blog</a></li>
<li><a href="http://pixelcluster.dev/VRAM-Mgmt-fixed/">Fixing AMDGPU&#x27;s VRAM management for low-end GPUs | pixelcluster&#x27;s GPU blog</a></li>

</ul>
</details>

**Tags**: `#linux-kernel`, `#vram-overcommit`, `#gpu-memory`, `#performance`, `#memory-management`

---

<a id="item-tech-news-3"></a>
### [Google buys Spirit Airlines&\#x27; data from bankruptcy auction for AI training](https://www.theregister.com/ai-and-ml/2026/08/18/google-buys-crashed-airline-spirits-data-at-auction-because-ai/5288962) ⭐️ 8.0/10

Google acquired over 100 million emails, 500 million Microsoft Teams messages, 17 million OneDrive files, 20.5 million SharePoint items, 30 million customer service call recordings, 15 million customer service chat records, 600,000 ServiceNow tickets, 13.7 million active email addresses from Oracle Responsys, and 11 million in-flight Wi-Fi sales records from Spirit Airlines&\#x27; bankruptcy auction. The data is intended to train AI models, with a court-ordered third-party de-identification agent tasked with stripping personally identifiable information before Google receives the material. The purchase spotlights the growing market for corporate data as AI training fuel and raises significant privacy and ethical concerns despite the de-identification safeguards.

hackernews · pseudolus · Aug 18, 10:13 · [Discussion](https://news.ycombinator.com/item?id=49343559)

**「Background」** Spirit Airlines was a US carrier that struggled financially after the COVID-19 pandemic began in 2020 and ultimately ceased operations in May 2026. As part of its bankruptcy liquidation, the airline’s assets, including a vast collection of corporate data, were sold at auction. Google secured the dataset with a $5 million bid, outbidding other firms such as Mercor.

**「Impact」** Spirit Airlines customers and employees face the risk that their private emails, chat messages, and recorded calls could be used to train Google&\#x27;s AI models, with de-identification offering uncertain protection against re-identification.

**「Community Discussion」** Commenters expressed unease about the sale of sensitive corporate data for AI training, questioning the effectiveness of de-identification and the normalization of such transactions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theregister.com/ai-and-ml/2026/08/18/google-buys-crashed-airline-spirits-data-at-auction-because-ai/5288962">Google buys crashed airline Spirit ’ s data at auction , because AI</a></li>
<li><a href="https://www.businessinsider.com/google-buys-spirit-airlines-data-ai-model-development-2026-8">Google Buys Spirit Airlines Data for AI Model... - Business Insider</a></li>

</ul>
</details>

**Tags**: `#AI`, `#data-privacy`, `#training-data`, `#Google`, `#corporate-data`

---

<a id="item-tech-news-4"></a>
### [GitHub Copilot Autofix Injects Vulnerability into Snowflake&\#x27;s Jira CI/CD](https://www.wiz.io/blog/red-agent-snowflake-copilot-cicd-bug) ⭐️ 8.0/10

GitHub Copilot&\#x27;s autofix feature generated code that introduced a template injection vulnerability in Snowflake&\#x27;s Jira CI/CD pipeline. The flaw appeared in a GitHub Actions workflow \(jira\_issue.yml\) where user-controlled variables were expanded unsafely using \`$\{\{...\}\}\`, enabling code injection. The vulnerability was discovered by Wiz researchers while the workflow was being simplified from deprecated Atlassian actions to direct curl calls. This incident demonstrates how AI-generated code can introduce serious security flaws, especially in CI/CD pipelines where static analysis tools would have caught the template injection.

hackernews · galnagli · Aug 17, 14:18 · [Discussion](https://news.ycombinator.com/item?id=49331423)

**「Background」** GitHub Actions workflows can be triggered by repository events like new issues or comments, and the \`$\{\{ github.event.\* \}\}\` syntax injects that data into the workflow. When such unsanitized event data is placed directly inside a \`run:\` block, it creates a template injection vulnerability that allows arbitrary command execution. GitHub Copilot’s Autofix feature, which automatically suggests code changes to resolve flagged issues, was used in a pull request that modified a Snowflake workflow, leading to this exploitable condition.

**「Impact」** The template injection vulnerability could have allowed an attacker to execute arbitrary commands within Snowflake&\#x27;s CI/CD environment, potentially compromising internal Jira data and connected systems.

**「Community discussion」** Community members acknowledged that such mistakes are easy to make in GitHub Actions workflows and stressed the need for static analysis tools like zizmor. Some questioned whether the vulnerability was directly caused by Copilot&\#x27;s autofix, but the general consensus was that AI-generated code warrants rigorous review, and the incident reflects a broader culture of &quot;LGTM&quot; reviews that allows such flaws to slip through.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wiz.io/blog/red-agent-snowflake-copilot-cicd-bug">Red Agent Exploits Snowflake Vuln Missed by Github Copilot | Wiz Blog</a></li>
<li><a href="https://www.cyberkendra.com/2026/08/copilot-autofix-snowflake-jira-github-actions.html">Copilot Autofix Bug Exposed Snowflake&#x27;s Internal Jira - Cyber Kendra</a></li>

</ul>
</details>

**Tags**: `#security`, `#AI`, `#GitHub Actions`, `#Copilot`, `#supply-chain`

---

<a id="item-tech-news-5"></a>
### [Rust GPU Offload Paper Proposes Portable, Safe GPU Programming](https://arxiv.org/abs/2608.13759) ⭐️ 8.0/10

A new research paper proposes a Rust GPU offload system that enables safe, portable, and fast GPU programming without manual bindings. The system aims to provide automatic data movement and efficient default execution, with future plans for advanced unsafe interfaces. Rust developers in AI and systems programming have expressed strong interest, as it would eliminate the binding maintenance headache for custom LLM inference engines. The approach leverages Rust&\#x27;s ownership model to map well to GPU memory lifetimes, offering a potential edge over C++.

hackernews · linggen · Aug 17, 17:54 · [Discussion](https://news.ycombinator.com/item?id=49334991)

**「Background」** Rust&\#x27;s ownership model guarantees memory safety on host CPUs, but high-performance GPU programming has traditionally required unsafe languages or manual bindings that bypass these guarantees. The paper introduces a system based on LLVM Offload that allows Rust code to run directly on GPUs, aiming to provide a safe, portable, and fast GPU interface that did not previously exist.

**「Impact」** For Rust developers working on AI and systems projects, this system could simplify GPU programming by removing the need to write and maintain external bindings.

**「Community Discussion」** Comments are enthusiastic but raise questions about the compiler backend choice \(LLVM vs. direct PTX/HIP\) and the absence of published code, while noting Rust&\#x27;s ownership semantics suit GPU memory management.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.13759">[ 2608 . 13759 ] GPU Offload in Rust : Portable , Safe , and Fast</a></li>
<li><a href="https://xenospectrum.com/en/rust-gpu-offload-llvm-safe-kernels-performance/">A GPU kernel written in safe Rust matched... | XenoSpectrum</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#GPU`, `#compiler`, `#systems-programming`, `#open-source`

---

<a id="item-tech-news-6"></a>
### [Qwen 3.8 27B Scores 52, Matching GPT-5.6 Luna](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 8.0/10

The Qwen 3.8 27B model achieved a score of 52 on the Artificial Analysis Intelligence Index, matching the maximum score of GPT-5.6 Luna—a model of unknown but presumably much larger size—and trailing GLM-5.2 \(753B parameters\) and DeepSeek V4 Pro 0813 \(1.7T parameters\) by just one point. This result demonstrates that a 27-billion-parameter model can rival systems with hundreds of billions or even trillions of parameters, challenging the assumption that scale is the primary driver of AI capabilities. The benchmark highlights the efficiency and performance of smaller models, potentially reshaping deployment strategies for AI applications.

rss · Simon Willison · Aug 17, 23:58

**「Background」** The Artificial Analysis Intelligence Index is a composite benchmark used to assess the capabilities of AI models. Qwen 3.8 27B is a 27-billion-parameter language model that has previously been noted for its surprising performance.

**「Impact」** This result suggests that developers can achieve near state-of-the-art performance with models that require significantly less compute and memory, lowering the barrier to deploying advanced AI in resource-constrained environments.

**Tags**: `#ai`, `#machine-learning`, `#llms`, `#benchmarks`, `#qwen`

---

<a id="item-tech-news-7"></a>
### [Fairphone 6 Main Camera Now Works on PostmarketOS](https://catcrafts.net/posts/fairphone-6-postmarketos-working-main-camera) ⭐️ 7.0/10

A developer has enabled the main camera on the Fairphone 6 running PostmarketOS, advancing the state of Linux on smartphones. The work involved overcoming driver compatibility issues and included testing emergency calling capabilities. While the camera is functional, other essential hardware—such as internal speakers and microphones—remain unsupported, limiting daily usability. This achievement demonstrates progress toward a fully open mobile Linux experience but still requires significant development.

hackernews · pizzaiolo · Aug 17, 22:01 · [Discussion](https://news.ycombinator.com/item?id=49338285)

**「Background」** PostmarketOS is a Linux distribution for mobile devices based on Alpine Linux, aiming for long-term support. The Fairphone 6 \(2024\) uses a Qualcomm SM7635 \(milos\) SoC with camera hardware blocks TFE665, CSID665, and CSIPHY v2.2.1. Building on earlier work that enabled the wide-angle camera, a new driver now provides support for the main camera sensor including autofocus and initial color correction.

**「Impact」** For developers and open-source enthusiasts, this camera enablement removes a key barrier, but the device still lacks internal audio, so it cannot yet replace a standard smartphone.

**「Community Discussion」** Commenters expressed excitement about the potential for fully open Linux phones, but noted that essential features like internal speakers and microphones are still missing, making daily use impractical. Some shared experiences porting other devices, highlighting the challenges and the hope that projects like Fairphone advance faster.

<details><summary>References</summary>
<ul>
<li><a href="https://catcrafts.net/posts/fairphone-6-postmarketos-working-main-camera">Fairphone 6 + PostmarketOS working main camera! — Catcrafts</a></li>
<li><a href="https://nondescriptpointer.com/articles/fairphone-6-wide-camera-linux/">Experimental Linux support for the Fairphone 6 wide camera · nondescriptpointer</a></li>

</ul>
</details>

**Tags**: `#postmarketos`, `#fairphone`, `#linux-mobile`, `#camera-enablement`, `#open-source`

---

<a id="item-tech-news-8"></a>
### [AirTag Tracked Rare Books to Amazon’s AI Training Facility](https://simonwillison.net/2026/Aug/17/we-tracked-a-shipment-of-rare-books-it-ended-at-an-amazon-ai-tra/) ⭐️ 7.0/10

404 Media tracked a shipment of rare books to an Amazon AI training facility by placing an Apple AirTag inside a book from a bulk order of around 1,000 volumes. The package was delivered to the VGT3 area of the LAS8 Amazon facility in Las Vegas, where a logo of a dinosaur with a book hinted at destructive scanning. Online forum discussions among Amazon workers confirmed that VGT3 scans large volumes of books for AI training data. This investigation provides concrete evidence that companies are sourcing physical books, including rare ones, for AI training, fueling ongoing debates about data sourcing and AI ethics.

rss · Simon Willison · Aug 17, 15:21

**「Background」** Prior to this investigation, book dealers reported receiving large, price-insensitive orders for seemingly unrelated books, leading to suspicions that AI companies were acquiring them for training data. Documents from a lawsuit against Anthropic revealed that the company bought and destroyed millions of books to scan for AI training in 2024. Reports also indicated that Amazon was engaging in similar practices of buying and destroying printed books to feed its AI models.

**「Impact on Booksellers」** Booksellers now face an ethical dilemma because bulk orders from anonymous buyers could lead to their rare collections being destroyed for AI training data.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theatlantic.com/technology/2026/08/ai-companies-buying-used-books-for-data/688167/">Someone Is Mysteriously Snapping Up Used Books Around the World - The Atlantic</a></li>
<li><a href="https://www.eweek.com/news/amazon-books-ai-training-data/">Amazon Is Reportedly Buying and Destroying Books to Feed Its AI | eWeek</a></li>
<li><a href="https://www.ndtvprofit.com/technology/hidden-tracker-reveals-amazon-mass-scans-shred-books-just-to-feed-ai-report-11923001">Hidden Tracker &#x27;Reveals&#x27; Amazon Mass-Scans, Shred Books Just To Feed AI: Report</a></li>
<li><a href="https://arstechnica.com/tech-policy/2026/08/hidden-airtag-reveals-amazon-is-trashing-rare-books-to-train-ai/">Hidden Airtag reveals Amazon is trashing rare books to train AI - Ars Technica</a></li>

</ul>
</details>

**Tags**: `#AI training data`, `#Amazon`, `#investigative reporting`, `#data sourcing`, `#AI ethics`

---

<a id="item-tech-news-9"></a>
### [macOS 26.7 Code Reveals Apple Intelligence Censorship for China](https://www.macrumors.com/2026/08/17/macos-26-7-unreleased-apple-devices/) ⭐️ 7.0/10

Code in macOS 26.7 reveals that Apple Intelligence&\#x27;s writing tools for mainland China will include content safety filters, temporary restrictions after repeated alerts, and cloud-controlled censorship rules. The uncovered strings indicate that the system will prompt users to update content safety rules, display an inability to edit certain text, and temporarily disable the writing tools after multiple safety alerts. These mechanisms suggest a separate content moderation layer for the Chinese market, with remote rule updates. The development highlights how Apple is adapting its AI features to comply with local regulations.

telegram · zaihuapd · Aug 18, 02:16

**「Background」** Apple Intelligence is a set of AI-powered features, including writing tools, that Apple plans to roll out to devices. To operate in China, which has strict internet content regulations, companies often implement local censorship and compliance mechanisms. This code analysis shows specific technical measures Apple is building into macOS for the Chinese market.

**「Impact」** Users in mainland China may experience restricted AI writing capabilities, with content filters, temporary bans, and remote updates that could limit functionality based on safety alerts.

**Tags**: `#Apple Intelligence`, `#censorship`, `#China`, `#macOS`, `#content moderation`

---

<a id="item-tech-news-10"></a>
### [Enterprise WeChat 5.0.10 Opens CLI and MCP for AI Agent Integration](https://mp.weixin.qq.com/s/uJf57P15-FQL_u6jLHiGYA) ⭐️ 7.0/10

WeChat Work \(企业微信\) version 5.0.10 has opened Command Line Interface \(CLI\) and Model Context Protocol \(MCP\) capabilities to all enterprises, enabling AI agents such as WorkBuddy, DeepSeek Harness, and self-built agents to directly invoke ten core office modules. The integration includes security controls like permission isolation between human users and AI, manual approval for critical operations, time-limited authorization, and full audit logging. AI can now read documents and spreadsheets, analyze data, and generate proposal presentations or business dashboards within the platform.

telegram · zaihuapd · Aug 18, 06:22

**「Background」** WeChat Work \(企业微信\) is a widely used enterprise communication and collaboration platform in China. The Model Context Protocol \(MCP\) is an open standard that enables AI models to securely connect with external tools and data sources. CLI \(Command Line Interface\) provides a programmatic way for software to invoke platform functions.

**「Impact」** Enterprises using WeChat Work can now deploy AI assistants to automate document analysis, data reporting, and content generation across core office functions, while maintaining fine-grained security and compliance controls.

<details><summary>References</summary>
<ul>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol ( MCP )? - Model Context Protocol</a></li>

</ul>
</details>

**Tags**: `#enterprise-software`, `#ai-agents`, `#mcp`, `#wechat-work`, `#api-integration`

---

<a id="item-tech-news-11"></a>
### [China Orders Early Removal of Tailored Windows 10 from State Agencies](https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan) ⭐️ 7.0/10

China&\#x27;s Ministry of National Security has directed some government-affiliated organizations to uninstall a customized version of Windows 10 months ahead of the original February 2027 deadline, citing data security concerns. The accelerated removal was not accompanied by a disclosure of a specific vulnerability, and Microsoft has stated that it is unaware of any security incident affecting the product, which continues to receive regular security updates. The move reflects heightened scrutiny of foreign software supply chains within Chinese state entities.

telegram · zaihuapd · Aug 18, 06:22

**「Background」** China has been working to reduce its dependence on foreign technology, including operating systems, by promoting domestic alternatives. The customized Windows 10 version mentioned in the report was a government-only edition of the older Microsoft operating system, originally scheduled to be phased out by February 2027. The accelerated removal order comes amid broader data security concerns and efforts to replace foreign software.

**「Impact」** The directive forces affected Chinese government agencies to replace the customized Windows 10 with domestic alternatives months ahead of the planned February 2027 retirement, triggering a surge in shares of domestic OS vendors like Hunan Kylinsec and Archermind.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/software/operating-systems/china-reportedly-orders-state-agencies-to-uninstall-its-government-only-edition-of-windows-10">China reportedly orders state agencies to uninstall... | Tom&#x27;s Hardware</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan">China Removes Microsoft Windows at State Users Ahead of Plan</a></li>
<li><a href="https://www.tomshardware.com/software/operating-systems/china-reportedly-orders-state-agencies-to-uninstall-its-government-only-edition-of-windows-10">China reportedly orders state agencies to uninstall its government-only edition of Windows 10 — Beijing accelerates planned retirement over data security concerns | Tom&#x27;s Hardware</a></li>

</ul>
</details>

**Tags**: `#Windows`, `#China`, `#cybersecurity`, `#government IT`, `#software policy`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Buy-Now-Pay-Later Loans Expand to Rent and Utilities, U.S. Borrowing Hits $160 Billion in 2025](https://www.nytimes.com/2026/08/17/business/buy-now-pay-later.html) ⭐️ 8.0/10

Buy-now-pay-later loans in the U.S. expanded to cover rent, utilities, and other essentials in 2025, driving annual borrowing to $160 billion—nearly double the 2023 total, according to The New York Times.

telegram · zaihuapd · Aug 18, 01:41

**「Background」** These loans, previously used mainly for online shopping, now allow consumers to finance recurring household expenses through installment payments.

**「Impact」** A LendingTree survey found that half of users could not make ends meet without these loans, and a quarter had at least three simultaneously, raising concerns about overdraft fees and debt traps.

**Tags**: `#BNPL`, `#consumer debt`, `#fintech lending`, `#household finance`, `#US economy`

---

<a id="item-finance-news-2"></a>
### [Prediction market traders see 1-in-4 odds Paramount’s Warner Bros. bid fails](https://www.cnbc.com/2026/08/17/pskys-wbd-bid-has-1-in-4-odds-of-falling-through-kalshi-traders-say.html) ⭐️ 7.0/10

Prediction market traders on Kalshi give a 22% chance that Paramount’s acquisition of Warner Bros. Discovery will fail by July 2027, implying a 74% likelihood of success.

rss · CNBC Finance · Aug 17, 17:43

**「Background」** A lawsuit by 12 state attorneys general filed on July 13 to block the merger drove the success odds down from over 80% to as low as 66% before stabilizing around the current level.

**「Impact」** If the deal does not close by September 30, Paramount will owe Warner Bros. shareholders 25 cents per share each quarter, adding financial pressure while the trial is set for March 2027.

**Tags**: `#M&amp;A`, `#Media`, `#Prediction Markets`, `#Antitrust`, `#Warner Bros. Discovery`

---

<a id="item-finance-news-3"></a>
### [Apple&\#x27;s US App Store Commission Revenue Falls 18% as Consumer Spending Declines 6%](https://www.macrumors.com/2026/08/18/apple-app-store-revenue-falling/) ⭐️ 7.0/10

Apple&\#x27;s US App Store commission revenue fell 18% in the second quarter of 2026, according to Appfigures, while Sensor Tower reported a 6% year-over-year drop in consumer spending, reversing a 9% increase a year earlier. Apple said regulatory changes are weighing on its services business growth.

telegram · zaihuapd · Aug 18, 12:17

**「Background」** Apple has stated that regulatory changes are beginning to affect its Services growth, as new rules in the US and other markets have altered App Store commission structures.

<details><summary>References</summary>
<ul>
<li><a href="https://9to5mac.com/2016/11/14/apple-macbook-pro-touch-bar-demo-units-in-stock-apple-store/">Apple ’s new MacBook Pro with Touch Bar will be in stock... - 9to5Mac</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#App Store`, `#regulation`, `#services revenue`, `#consumer spending`

---