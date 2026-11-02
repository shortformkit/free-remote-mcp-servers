# Free remote MCP servers (tested weekly)

Remote [Model Context Protocol](https://modelcontextprotocol.io) servers from the [official MCP Registry](https://registry.modelcontextprotocol.io) that answer **without any API key, token or login**. Every server is re-tested each week with exactly two requests, `initialize` and `tools/list`. No tool is ever called.

**Last run: 2026-11-02** · 23,619 endpoints tested · **13,677 open (58 %)** · 7,408 need auth · 2,534 not working · 10,996 listed after removing copies

- Tool annotations (as declared by the servers, not verified): 3,834 of 13,669 open servers annotate none of their tools. Of 155,828 tools, 118,384 carry annotations, 91,295 say readOnlyHint true, 9,383 say destructiveHint true. Per server in the `tools_annotated`, `tools_read_only` and `tools_destructive` columns. Note: we only see the tools a server lists without a key.
- Full list: [`data/servers.csv`](data/servers.csv) and [`data/servers.json`](data/servers.json)
- Browse with search and topics: [shortformkit.com/free-remote-mcp-servers](https://shortformkit.com/free-remote-mcp-servers/)
- Check any server yourself: [MCP Server Tester](https://shortformkit.com/mcp-server-tester/)
- Analysis with charts (failure reasons, hosting, tool counts): [State of remote MCP servers 2026](https://shortformkit.com/state-of-remote-mcp-servers-2026/)
- Key numbers with dates, ready to cite: [MCP statistics 2026](https://shortformkit.com/mcp-statistics/)

## Add a server to your client

| Client | How |
|---|---|
| Claude (claude.ai, desktop) | Customize, Connectors, + Add, Add custom connector, paste the URL |
| Claude Code | `claude mcp add --transport http NAME URL` |
| Cursor | `{"mcpServers": {"NAME": {"url": "URL"}}}` in `~/.cursor/mcp.json` |
| VS Code | `{"servers": {"NAME": {"type": "http", "url": "URL"}}}` in `.vscode/mcp.json` |

## Is your server in the list?

Show its live status in your README. The badge re-tests the endpoint about once an hour (same two read-only requests) and links to the full test result:

```markdown
[![MCP status](https://shortformkit.com/api/mcp-badge?url=YOUR_URL_ENCODED)](https://shortformkit.com/mcp-server-tester/?url=YOUR_URL_ENCODED)
```

Replace `YOUR_URL_ENCODED` with your endpoint, URL-encoded, or run the [MCP Server Tester](https://shortformkit.com/mcp-server-tester/) once and copy the ready-made badge from the result.

## Picks by topic

Up to 25 per topic: one per publisher, 3 to 40 tools, servers with a website or repo first, fastest first. Open means usable without signing up, not an endorsement: read what a server does before you connect it.


### Search and web

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Bible Swipe](https://goodturn-mcp.pages.dev/bible) | A Bible reading a day, line by line, any passage by reference, and search. | `https://goodturn-mcp.pages.dev/bible/mcp` | 6 |
| [firmenliste-mcp](https://www.firmenliste.net) | B2B company address data for the DACH region: search 6,400+ industry lists and get price quotes. | `https://firmenliste-mcp.cf-firmenliste.workers.dev` | 5 |
| [twitterapi-mcp-server](https://twitterapi.io) | Twitter/X read-only MCP server — 12 tools: search, users, tweets, followers, timelines, trends. | `https://mcp.twitterapi.io/mcp` | 12 |
| [MCP Junction](https://mcpjunction.ai) | Search a nightly-refreshed directory of MCP servers by keyword, category or topic. | `https://mcpjunction.ai/mcp` | 5 |
| [serp-metrics](https://toolsthatrank.com/) | Impression-weighted SERP position, click projection on your own CTR curve, share of voice | `https://toolsthatrank-mcp.lipmichal.workers.dev` | 3 |
| [server](https://github.com/jhibird/HeySpark-MCP) | Search and discover local businesses. 30+ categories with verified contact info, hours, and reviews. | `https://mcp.heyspark.co/mcp` | 4 |
| [EveryHourDeal Shopping](https://everyhourdeal.com) | Search and compare hourly deals on US-warehouse home, patio, gym and pet goods, plus original tees. | `https://everyhourdeal-checkout.everyhourdeal-store.workers.dev/mcp` | 5 |
| [Chinaready China Market-Entry Search](https://chinaready.co/docs/api/) | Read-only search over chinaready.co — China market entry for Western software teams. | `https://mcp.chinaready.co/mcp` | 4 |
| [Manifesting Quantum](https://www.manifestingquantum.net/agents) | Science-based manifestation: daily affirmations, techniques, free 7-day challenge, search 310 guides | `https://manifestingquantum-mcp.ibrobertb23.workers.dev` | 5 |
| [DecaData Odyssey Lite](https://api.decadata.io/llms.txt) | US point-of-sale sales for ~380 consumer companies: free search and samples, YoY growth for $0.01 | `https://api.decadata.io/mcp` | 5 |
| [iconserve](https://github.com/asr-aditya/iconserve) | Icons for agentic development: search & fetch 366,000+ open-source icons as SVG/PNG. No API key. | `https://icons-for-agents.site/mcp` | 3 |
| [Eremos Thai Bible](https://bible.eremosapp.com) | Quote the Eremos Translation (Thai Bible, CC0) word for word: passages, search, decision notes. | `https://mcp.eremosapp.com/mcp` | 4 |
| [feedmyagent](https://github.com/makash/feedmyagent-skill) | Agent-readable feed: AI/agent tech news, security advisories, compliance deadlines, and live events. | `https://api.feedmyagent.com/mcp/mcp-registry` | 7 |
| [Public Folder](https://agents.asel.one/docs) | Search and share cited agent findings. Public reads; authenticated writes. | `https://agents.asel.one/mcp` | 12 |
| [Web Access Gateway](https://skowronworks.com/agent-tools/web-access-gateway/) | Paid web, news, company, product, and geographic search plus clean page reading for agents. | `https://web-access-gateway.mattskowronis.workers.dev/mcp` | 8 |
| [GTH Intelligence - Substance Abuse Treatment Finder](https://github.com/Crindo2/gth-mcp-server) | Search 12,338 curated, SAMHSA-sourced addiction treatment facilities across all 50 US states. | `https://gth-mcp-server.pages.dev/mcp` | 4 |
| [SOLVED — buy work already done](https://api.trovefield.ai) | Search and buy verified solved artifacts instead of recomputing them. | `https://api.trovefield.ai/mcp` | 4 |
| [AgentScout](https://agentscouthq.com/mcp/connect.html) | Read-only search over 2,065+ AI agent tools and 276 MCP servers. Free, no sign-up needed. | `https://mcp.agentscouthq.com/mcp` | 5 |
| [MarketNow](https://www.marketnow.site) | Search 70,510 indexed MCP servers, install-risk scoring and Ed25519-signed Agent Trust Cards. | `https://marketnow.site/api/mcp` | 10 |
| [COMPAMIR News](https://compamir.com/data.html) | Search structured COMPAMIR news in Japanese and English, with links to source reports. | `https://api.compamir.com/mcp` | 3 |
| [TheDiscList Public MCP](https://thedisclist.com) | Search disc golf discs, compare flight ratings, and find similar alternatives across brands. | `https://api.thedisclist.com/mcp` | 9 |
| [Jan Linketscher](https://janlinketscher.com/agent) | Profile and essays of Jan Linketscher (i22, Bonn), full-text search, and booking a call. | `https://janlinketscher.com/api/mcp` | 7 |
| [American Ghost Walks](https://americanghostwalks.com) | Read-only AGW ghost tours: search by city, open departures, details, and official booking links. | `https://mcp.agwcrew.com/mcp` | 4 |
| [AskAgent](https://askagent.dev) | Archive of verbatim errors with root causes and fixes that AI agents search by exact error string. | `https://askagent.dev/mcp` | 3 |
| [MamaChoice](https://mamachoice.co.il/) | Israeli Hebrew baby-product buying guides: find a guide, its products in ILS, FAQ; live search. | `https://mamachoice-mcp.ohadf1976.workers.dev/mcp` | 3 |

### Documentation and knowledge

| Server | What it does | URL | Tools |
|---|---|---|---|
| [draw.io](https://www.drawio.com) | Create draw.io diagrams in chat from Mermaid or XML, shown live and interactive. 10,000+ shapes. | `https://mcp.draw.io/mcp` | 3 |
| [Absolute value sign, number discarded](https://github.com/sadri-dridi/named-mcp-utilities) | Absolute value sign, number discarded | `https://agent-observatory-sensor.nolimit-observatory.workers.dev/s/abs-ok/mcp` | 31 |
| [ClearMarket](https://clearmarket.fyi) | Reference data for prediction markets: graded resolution clarity, cross-venue links, provenance. | `https://api.clearmarket.fyi/mcp` | 6 |
| [Grandet](https://grandet.ai) | Cheapest API for any model across official, inference and relay providers; find free credits | `https://grandet.ai/mcp` | 6 |
| [AI 與科技名詞白話解釋](https://glossary.penguindriver.com) | AI 與科技名詞白話解釋：MCP、RAG、AI 代理人等名詞的白話定義。台灣繁體中文 MCP 工具。 | `https://glossary.penguindriver.com/mcp` | 6 |
| [Quiet Menders](https://brianbooms.com) | Privacy clinic + pay-per-call data APIs for AI agents via x402. Never pays or touches keys. | `https://mcp.brianbooms.com/mcp` | 34 |
| [UseMyContext.ai](https://usemycontext.ai) | Personal context for AI, written by you and never scraped: your profile and files, any MCP client. | `https://mcp.usemycontext.ai/mcp` | 13 |
| [Zhiyong Agent Network](https://kg.zhiyong.dev/agent-start?from=distribution) | Discover AI tools, models and Agents; compare candidates, inspect unknowns, join public discussions. | `https://kg.zhiyong.dev/mcp` | 15 |
| [mcp-server](https://quelvio.com) | Your company's brain for AI agents. Cited, permission-aware knowledge across every system. | `https://mcp.quelvio.com/http` | 3 |
| [Communicate Developer Docs](https://communicate.so/developers) | Read-only access to Communicate developer guides, OpenAPI summaries, and support contact. | `https://communicate.so/mcp` | 3 |
| [UDS Toolbox](https://udslib.com/mcp.html) | Find why a UDS flash failed from a CAN trace; decode UDS, ISO-TP and DTCs. No hardware. | `https://mcp.udslib.com/mcp` | 7 |
| [Axint](https://github.com/agenticempire/axint) | Proof and repair for Apple coding agents: validate Swift, run Xcode evidence, and repair failures. | `https://mcp.axint.ai/mcp` | 36 |
| [classifier.dev docs](https://classifier.dev/mcp-setup) | classifier.dev documentation as tools: list, read and search the reference, benchmark and guides. | `https://classifier.dev/mcp/docs` | 4 |
| [Growo child growth](https://usegrowo.com/mcp) | Free child growth tools: percentiles, BMI, corrected age, target height, birth size. WHO and CDC. | `https://mcp.usegrowo.com/` | 16 |
| [AI 與科技名詞白話解釋](https://tw-ai-glossary.panda198271.workers.dev) | AI 與科技名詞白話解釋、概念比較與入門教學（繁體中文）。 | `https://tw-ai-glossary.panda198271.workers.dev/mcp` | 6 |
| [nyuchi-docs](https://docs.nyuchi.com/integrations/docs-mcp/) | Search, read, and ask the Nyuchi docs (docs.nyuchi.com); send feedback or raise issues. | `https://docs.nyuchi.com/mcp` | 5 |
| [AutEng Docs — Agent Document Workspace & Publishing](https://auteng.ai) | Agent document workspace with wallet auth. Create, update and share markdown docs. By AutEng.ai | `https://auteng.ai/mcp/docs` | 6 |
| [402cron](https://402cron.com) | Paid cron for AI agents: we call your https URL on schedule, signed. No account, paid with x402. | `https://402cron.com/mcp` | 16 |
| [Awwab Qibla & Quiz](https://awwab.app/qibla) | Qibla direction from anywhere, with a live compass link, and an Islamic knowledge quiz. By Awwab. | `https://awwab.app/mcp` | 3 |
| [Meeba Brain](https://github.com/meemoprasad/meeba-brain-marketplace) | Repository knowledge graph MCP server for codebase understanding and debugging. | `https://meeba-context-mcp-469248886325.us-central1.run.app/mcp` | 5 |
| [ionic-framework-mcp](https://capawesome.io/) | Unofficial MCP server for the Ionic Framework documentation, components and blog. | `https://ionic-framework-mcp.capawesome.io/mcp` | 5 |
| [Knowledge for Agents](https://knowledgeforagents.com/connect) | Search real problems, solutions, failed approaches and observed outcomes shared by AI agents. | `https://knowledgeforagents.com/mcp` | 4 |
| [Rasczak Knowledge Commons](https://rasczak-agent-service.rasczak-commons.workers.dev) | Free decision methods, work-kit previews and optional feedback. Hosted research is not available. | `https://rasczak-agent-service.rasczak-commons.workers.dev/mcp` | 8 |
| [CalvingWatch Public Knowledge](https://calvingwatch.com/ai/) | Read-only CalvingWatch product, tester, camera, privacy and safety facts; no customer data. | `https://calvingwatch.com/mcp` | 5 |
| [My App Store Ranking](https://myappstoreranking.com/docs/mcp) | Access to your Apple App Store and Google Play Store rankings, competitors and chart moves. | `https://mcp.myappstoreranking.com/mcp` | 9 |

### Developer tools

| Server | What it does | URL | Tools |
|---|---|---|---|
| [jsonaut](https://jsonaut.jsonaut-shaurya.workers.dev) | Repair malformed JSON from LLM/agent output; optional JSON Schema coercion. Free + x402 paid. | `https://jsonaut.jsonaut-shaurya.workers.dev/mcp` | 4 |
| [Motion by Frapea](https://motion.frapea.com) | One sentence to a finished animation: your AI writes motion graphics as code and checks real frames. | `https://motion.frapea.com/mcp` | 20 |
| [familyguy.co.uk episode database](https://familyguy.co.uk/) | Lookups over an unofficial Family Guy database: episodes, seasons, characters, cast, crew and facts. | `https://familyguy.co.uk/mcp` | 8 |
| [krabbot-devtools](https://mcp.marvin-odigo.workers.dev) | AI-agent-run devtools: package install risk, stack EOL/CVE checks, scored OSS bounties. | `https://mcp.marvin-odigo.workers.dev/mcp` | 4 |
| [SheetShift](https://github.com/everyai-com/sahadeva) | Convert and clean tables: CSV, JSON, dedupe, stats. Free. | `https://sheet-shift.magicteams.ai/mcp` | 4 |
| [CarsMultiverse — the recall record](https://carsmultiverse.com/data/) | Vehicle safety recalls from four registers, matched across borders on the maker's own code. | `https://carsmultiverse.com/wp-json/cmvmcp/v1/mcp` | 4 |
| [sectora](https://sectora.io/mcp) | Threat intel + your scans/findings/Shield posture. CVE, EPSS, KEV, package vuln lookup, DAST. | `https://mcp.sectora.io/mcp` | 14 |
| [LicenseGuard](https://license-guard.rcc-aoki.workers.dev) | Check if a dependency's license obligates you, based on how you ship. npm, PyPI, Go. | `https://license-guard.rcc-aoki.workers.dev/mcp` | 3 |
| [jev-guide](https://github.com/mdimamhosen/jev) | Set up the JEV model router for Claude Code, Codex and Cursor, and install MCP servers. | `https://jev-guide.jevrouter.workers.dev/mcp` | 4 |
| [Android Security Analyzer](https://github.com/ako2345/android-security-analyzer) | MCP server for static security analysis of Android source code | `https://android-security-analyzer.ako-labs.workers.dev/mcp` | 4 |
| [The Deploy Log](https://deployedbyai.com/log/mcp/) | AI deployments that shipped and are available now, each sourced to the publisher's own page. | `https://deployedbyai.com/log/mcp` | 3 |
| [Repo Run Check](https://repo-run-check.nextill-pos.workers.dev) | Check GitHub repos and shell commands for malware-delivery tricks before an AI agent runs them | `https://repo-run-check.nextill-pos.workers.dev/mcp` | 4 |
| [cve-intelligence](https://cve-security.com) | CVE intelligence: exploitation (KEV/EPSS), detection coverage, fixed versions, CPE configurations. | `https://cve-security.com/api/mcp` | 9 |
| [DAITK (Dibblee AI Tool Kit) - Total Import Cost](https://daitk-tic.dibind.com) | Import duty into Canada only. By HS code and origin: tariff, surtax, quota, anti-dumping. | `https://daitk-tic.dibind.com/mcp` | 6 |
| [Zaleso](https://zaleso.com) | Nigeria PAYE, VAT and CBN rates, sourced and dated. Plus invoice totals, QR codes, JSON, Base64. | `https://mcp.zaleso.com/` | 10 |
| [BHX Fab Quote](https://bastionhelix.com/fabquote/) | Measure and price laser, plasma, waterjet and CNC jobs from DXF, G-code and STL files | `https://quote.bastionhelix.com/mcp` | 4 |
| [Faceabot — tell it your need, get the tool that works](https://faceabot.com) | solve_need: one call returns the best of 38,000+ MCP tools, with live measured reliability. | `https://faceabot.com/api/mcp` | 33 |
| [DefaultRank](https://defaultrank.com/agents) | Check npm dependencies for outdated majors, and see which dev tools AI models pick. | `https://defaultrank.com/mcp` | 3 |
| [FreshContext](https://freshcontext.dev) | Context integrity for AI agents: evaluate freshness, confidence, provenance, and decision readiness. | `https://api.freshcontext.dev/mcp` | 22 |
| [Pingoru status](https://pingoru.io/features/mcp) | Live status, incidents and maintenance windows for 8,000+ cloud and SaaS status pages. | `https://pingoru.io/api/mcp-public/` | 6 |
| [UpgradeLens](https://upgradelens.mattpicone.workers.dev) | npm/PyPI package dependency upgrade reviews: security, runtime compatibility, cited migration. | `https://upgradelens.mattpicone.workers.dev/mcp` | 4 |
| [sqlai.dev SQL Verifier](https://sqlai.dev) | Executes SQL in a real ephemeral database: rows, typed errors with suggestions, plans, diffs. | `https://mcp.sqlai.dev/mcp` | 5 |
| [SemverKit](https://semverkit.mike-tusa.workers.dev/) | Semver parse, compare, npm range checks, max-satisfying and version bumps (node-semver compatible). | `https://semverkit.mike-tusa.workers.dev/mcp` | 5 |
| [Presend MCP Server](https://github.com/presendapp/presend-source) | Before an AI agent installs an npm/PyPI package: typosquat, vulnerability and existence checks. | `https://presend.pages.dev/mcp` | 40 |
| [MCPFax Dev Package Intelligence](https://mcpscores.com) | Is this dependency current, licensed, deprecated, or already carrying a CVE? | `https://devpkg-intel.bowling-anthony.workers.dev/mcp` | 5 |

### Weather, maps and travel

| Server | What it does | URL | Tools |
|---|---|---|---|
| [capitolguide](https://capitol.guide) | Navigate the U.S. Capitol complex: decode room codes, route buildings, check access, amenities. | `https://capitol.guide/mcp` | 9 |
| [Agentic Reputation Gateway](https://github.com/agenticsubstrate/site) | Read-only gateway for durable agent identity, consent, recognized work, and signed receipts. | `https://agentic-reputation-gateway.maxrhinehart.workers.dev/mcp` | 7 |
| [Russia–NATO risk ladder](https://russianato.site) | Russia–NATO risk: labelled forecasts, scenarios and intelligence assessments. Cite russianato.site. | `https://mcp.russianato.site/mcp` | 8 |
| [Iberá Experience](https://iberaexperience.com/para-agentes/) | Iberá Wetlands (Argentina) travel guide: gateways, routes, 500+ local providers, bookable trips. | `https://mcp.iberaexperience.com/mcp` | 6 |
| [KRTools Korean Utilities](https://krtools.deanhiki.workers.dev/) | Korean name/text romanization, Korean address to English, business number (BRN) check. | `https://krtools.deanhiki.workers.dev/mcp` | 5 |
| [sunnyspoints](https://sunnyspoints.com/mcp) | Live flight deals plus points-vs-cash math: transfer partners, valuations, per-leg verdicts. | `https://sunnyspoints-mcp.sunnyspoints.workers.dev/mcp` | 9 |
| [agent-bev](https://agent-bev.ai) | The world's largest agentic B2B hub for beer, wine and spirits. Powered by CUVEE. Trade only. | `https://mcp.bev-buyer.ai/mcp` | 9 |
| [Delve to Life](https://delvetolife.com/ai/) | Dress codes explained, outfit formulas by occasion and weather, and clothing colour combinations. | `https://mcp.delvetolife.com/mcp` | 5 |
| [2027 連假與訂票](https://tw-travel-2027.panda198271.workers.dev) | 2027 台灣連假、出國目的地擁擠度與機票訂票時機建議。 | `https://tw-travel-2027.panda198271.workers.dev/mcp` | 5 |
| [Watt Street — US grid, interconnection queue and data center power](https://wattstreet.net) | How long to get grid power in any US county. 39,173 filings, 1,574 counties, dated sources. | `https://api.wattstreet.net/mcp` | 7 |
| [Growthr SEO + GEO MCP](https://mcp.growthr.com) | SEO + GEO tools in your AI editor: scan as ChatGPT and Google crawlers see it, fix order, llms.txt. | `https://mcp.growthr.com/mcp` | 4 |
| [travel.art](https://travel.art/) | Art-tourism data for AI agents: biennales, art fairs, museums, layover itineraries with 2026 facts. | `https://mcp.travel.art/` | 4 |
| [easygroupflights](https://easygroupflights.com) | Group flight quotes for parties of 10 or more passengers. | `https://mcp.easygroupflights.com/mcp` | 5 |
| [Les bancs](https://lesbancs.fr/api) | A French address: its catchment schools, nursery to high school, and each school's results. No key. | `https://lesbancs.fr/mcp` | 4 |
| [IP Address API](https://ip.app) | What's My IP Address: caller's public IP, ASN, geo, timezone, user-agent, headers, TLS info. | `https://ip.app/mcp` | 8 |
| [Codex Reset](https://codex-reset.com/developers) | Read-only Codex usage-limit reset data: 24/48h reset forecast, dated reset record, service status. | `https://codex-reset.com/mcp` | 3 |
| [Dumaguete Extension](https://dumaguete-extension.aplusz.app/) | Costs, travel, visas, hospitals, weather and places for Dumaguete, Philippines. | `https://dumaguete-extension.aplusz.app/mcp` | 8 |
| [glimind](https://glimind.com) | Live reliability for AI agent tools: is it working right now, and how do I call it correctly? | `https://glimind.com/mcp` | 21 |
| [esimdata: travel eSIM comparison](https://esimdata.app/agents/) | Neutral travel eSIM comparison: search and compare plans from many providers, ranked by price. | `https://esimdata.app/mcp` | 6 |
| [MetaMesh-UGA](https://metamesh-uga.dev) | Serverless edge control plane to discover, route and monetize 14,982+ MCP tools. | `https://api.metamesh-uga.dev/mcp` | 15 |
| [a2bflight fares](https://a2bflight.com/ai) | Flight fares seen on thousands of routes, each dated, and where a group can meet. Not live. No key. | `https://mcp.a2bflight.com/mcp` | 5 |
| [momentic](https://momenticmarketing.com/agent-tools) | Free SEO, GEO, and AEO audits: analyze any page or domain, AI-crawler access, agent readiness. | `https://momenticmarketing.com/mcp` | 12 |
| [Agent Bounty Jobs](https://github.com/jasonbrelsford/agent-bounty-jobs) | Agent-to-agent bounty board: post tasks with stated rewards, fill them, first accepted wins. | `https://bounty.brelsfordsoftware.com/mcp` | 23 |
| [Moradas — Portuguese addresses & postal codes](https://moradas.dev) | Portuguese address autocomplete, postal codes, list checks; typo-tolerant, municipality-first; free. | `https://moradas.dev/mcp` | 4 |
| [Surfacing Feelings](https://surfacingapp.com/feelings.html) | Helps people name what they feel: 796 feeling words and a body map of 243 sensations. | `https://surfacing-mcp.knightcorrick.workers.dev/mcp` | 4 |

### Media and content

| Server | What it does | URL | Tools |
|---|---|---|---|
| [flowpack](https://flowpack.pages.dev) | Flowpack: Shopify design catalog — badge/button/bar looks, honest-urgency presets, diagnosis. | `https://flowpack-mcp.flowpackplugin.workers.dev/mcp` | 5 |
| [Postclick by PPC.io: Landing Page CRO](https://ppc.io/postclick/mcp) | Landing-page CRO: audit pages, rewrite copy, answer buyer objections, design and build via MCP. | `https://mcp.ppc.io` | 21 |
| [THIRI Chord Intelligence](https://thiri.ai) | Deterministic music theory for agents: analyze, voice, reharmonize, conduct — computed, not guessed | `https://mcp.thiri.ai/mcp` | 4 |
| [Audiala](https://mcp.audiala.com/) | Audio guides for 44,000+ places in 1,900+ cities, with narrated previews in ChatGPT and Claude. | `https://mcp.audiala.com/mcp` | 4 |
| [GiftsToPrint](https://mcp.giftstoprint.com/docs) | Order personalised newspaper-style birthday, anniversary and retirement posters as print files. | `https://mcp.giftstoprint.com/mcp` | 5 |
| [ocr](https://github.com/Samqra/auto-reader-ocr) | Arabic-first OCR, translation and document extraction. First call mints a free trial key. | `https://api.auto-reader.com/mcp` | 7 |
| [Design Check](https://designcheck.allthepossibles.com) | Scores whether a page reads as AI-generated and names the tells to fix. | `https://designcheck.allthepossibles.com/mcp` | 3 |
| [Screenbird](https://screenbird.app) | Manage Screenbird digital signage screens: see what is live, show content, create designs. | `https://mcp.screenbird.app/mcp` | 12 |
| [Tool Pantry](https://toolpantry.app) | Find and use 216 free browser tools for PDF, images, video, audio and text that run locally. | `https://mcp.toolpantry.app/mcp` | 9 |
| [Doseedo Film Score: spot a video, play your score on AI instruments, mix it to picture](https://doseedo.com/guides/score-a-film-with-an-ai-agent) | Score video as an agent: cue sheet from the cut, 50+ AI instruments play your MIDI, mixed to picture | `https://api.doseedo.com/mcp/film` | 24 |
| [PaletteGet](https://paletteget.com/) | Curated app, web and mini program color palettes with WCAG contrast and CSS variables. | `https://paletteget-mcp.y7206062.workers.dev/mcp` | 9 |
| [mcp](https://pixfaro.com) | Generate images with any major model — one API key, one prepaid balance, one MCP. | `https://mcp.pixfaro.com/mcp` | 8 |
| [AIURION Agentic 3D Printing — San Francisco](https://aiurion.com/ai-agents) | SF 3D printing + design workbenches (enclosures, grippers, fixtures, stamping). Quote and order. | `https://aiurion.com/api/agent/v1/mcp` | 17 |
| [JENRIKS Photo Archive](https://jenriks.com/developers/#mcp) | Read-only MCP server over the JENRIKS daily photoblog: one photo per day since 2006. No auth. | `https://jenriks.com/mcp` | 5 |
| [Doucebeads · Image to Bead Pattern](https://doucebeads.com/developers/mcp/) | Convert PNG/JPEG into fuse-bead charts with MARD codes, PNG, CSV and an editable web link. | `https://doucebeads.com/mcp` | 3 |
| [SUMMARU Breath](https://summaru.app) | Breathing guide with voice and bowl, looping music, binaural beats, and a player link for users. | `https://agent.summaru.app/mcp` | 4 |
| [SafeResize](https://saferesize.com/ai) | Passport and visa photo rules for 110 documents in 60 countries, and upload limits as exact numbers. | `https://saferesize.com/mcp` | 4 |
| [ContrastKit](https://contrastkit.mike-tusa.workers.dev/) | WCAG color contrast checks, nearest accessible color, CSS color conversion and palette pair checks. | `https://contrastkit.mike-tusa.workers.dev/mcp` | 4 |
| [MysticAPI](https://mysticapi.com) | Human Design & astrology engine: bodygraph, personal-sky SVG, today's sky. JPL ephemeris. | `https://mysticapi.com/mcp` | 7 |
| [Clawhard Studio](https://clawhard.com) | Trim text, check AI habits, total AI subs, split costs, plan events, get design words for AI. | `https://mcp.clawhard.com/mcp` | 15 |
| [Wasilah](https://github.com/mumullickm/wasilah-mcp) | Prayer times, Qibla, Hijri calendar, 99 Names, Quran audio, Bangladesh offsets. English + Bengali. | `https://wasilah-mcp.aykiz.workers.dev/mcp` | 9 |
| [Silent Directive Tools](https://github.com/silentdirectivellc-hub/silentdirective-mcp) | Free tools: 2026 API shutdown scanner, small-business website auditor, photo resale estimator. | `https://sites.silentdirectivellc.com/mcp` | 3 |
| [Notify Sound](https://notifysound.com/) | Design notification sounds from layered tones and get an editor link to play and download. | `https://notifysound.com/mcp` | 5 |
| [Resemble AI](https://github.com/resemble-ai/resemble-mcp) | Resemble AI: deepfake, AI-text, and site agent detection, Detect Agents, intelligence, watermarks. | `https://mcp.resemble.ai/mcp` | 18 |
| [kavel-mcp](https://www.kavel.ai) | Discover Kavel's AI photo/video generators, get tuned prompts, and open the right tool on kavel.ai. | `https://www.kavel.ai/api/mcp` | 4 |

### Finance and crypto

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Senaro Personal Finance](https://senaro.ai) | Credit card payoff, mortgages, refinancing, 401(k), rent vs buy. Every rule and default is cited. | `https://mcp.senaro.ai/mcp` | 19 |
| [不動産情報サービス MCP](https://n-3.ai/apps/reinfo-agent) | 国土交通省の不動産情報ライブラリから不動産価格データを取得するためのサービスです。 | `https://mcp.n-3.ai/mcp?tools=get-time,reinfolib-real-estate-price,reinfolib-city-list` | 3 |
| [Filings Intel MCP](https://github.com/datakoot/filings-intel-mcp) | SEC EDGAR filings for AI agents: company lookup, filings, financials, insider trades. No keys. | `https://filings.datakoot.com/mcp` | 5 |
| [JIDEC: Bitcoin-anchored public verification ledger (NENRIN)](https://ledger.horizonshield.dev/llms.txt) | Read agents' Bitcoin-anchored conduct history (NENRIN) and cite and recompute ledger records. | `https://jidec.horizonshield.dev/mcp` | 9 |
| [CryptoPulse Data API](https://cryptopulse.saascloud.ai) | Pay-per-call crypto market intelligence for AI agents. USDC on Base via x402. | `https://cryptopulse.saascloud.ai/mcp` | 11 |
| [TradeTi.me — Market Hours](https://tradeti.me/developers/mcp) | Read-only trading hours for 30 stock exchanges — open now, next open, holidays, sessions. | `https://mcp.tradeti.me/mcp` | 8 |
| [Field Ops](https://field-ops.filnith.workers.dev) | AI agents hire a human to observe, log or film on site. Typed results, feasibility before payment. | `https://field-ops.filnith.workers.dev/mcp` | 4 |
| [Elétrico Leve](https://eletricoleve.com.br) | Brazilian light EVs (e-bikes, scooters, tricycles): specs, prices and Contran 996/2023 status. | `https://eletricoleve-mcp.gcnovidade.workers.dev/mcp` | 5 |
| [Juicy Designs Quote](https://www.juicydesigns.co.za/developers/mcp/) | Free digital marketing quote and strategy requests from Juicy Designs SA. No price returned. | `https://juicy-designs-quote.black-voice-76e6.workers.dev/mcp` | 7 |
| [NL Ledger](https://nlledger.ca/data/) | NL provincial and federal spending records, each with its source. Addresses do not locate work. | `https://nlledger.ca/mcp` | 15 |
| [diamond-mcp](https://stienhardt.com/?utm_source=mcp_registry&utm_medium=referral&utm_campaign=diamond_mcp&utm_content=registry_website) | Sourced diamond and gemology tools for AI assistants, with 90 encyclopedia entries. | `https://diamond-mcp.stienhardt.workers.dev/mcp` | 11 |
| [tw-finance](https://fininfostation.com/for-ai-agents) | Taiwan finance open data: ETF, funds, TAIEX, sentiment, business climate, FX. Free & read-only. | `https://fininfostation.com/mcp` | 15 |
| [x402 economy tools](https://multichain-rpc.clankerceo.workers.dev/report) | Measured x402 ecosystem data, facilitator reliability, and live endpoint checks. | `https://multichain-rpc.clankerceo.workers.dev/mcp` | 6 |
| [property-finance-mcp](https://www.fdcommercial.co.uk/finance-guide/uk-property-finance-mcp-ai-assistants/) | UK property finance: bridging cost, dev appraisal, BTL stress test, stamp duty (SDLT/LBTT/LTT). | `https://fdc-property-finance-mcp.fdcommercial-uk.workers.dev/mcp` | 4 |
| [DESK LEAD x402 — high-ticket packs $50/$100/$150](https://desk-x402.desk-x402-gh.workers.dev) | ~17 tools; HT packs $50/$100/$150. tools/list free; tools/call USDC Base x402. Not financial advice. | `https://desk-x402.desk-x402-gh.workers.dev/mcp` | 17 |
| [Hire Solidmade](https://solidmade.co) | Hire a studio for Shopify, web, automation and data jobs: live services, USD prices, quote requests. | `https://solidmade-mcp.solidmade.workers.dev/mcp` | 3 |
| [Celadon Wholesale](https://celadonbeauty.com/pages/celadon-wholesale-connector-for-ai-assistants) | Wholesale Korean skincare for US and Canadian resellers: case prices, margins, checkout links. | `https://celadon-wholesale-mcp.dermatologicalbeautyllc.workers.dev/mcp` | 5 |
| [RightCard](https://rightcard.ai/mcp) | Which of your credit cards to use at any store, from verified bank data. No bank login. | `https://mcp.rightcard.ai/mcp` | 5 |
| [Bankrolled.ai Agent Hub](https://bankrolled.ai/) | Free, sourced money limits: money_fact, scheme_lookup, cross_border_check. US/UK/CA/AU/NZ. No key. | `https://bankrolled.ai/mcp` | 5 |
| [SBOR](https://sbor.xyz) | Check a lending rate before your agent borrows. Bitcoin-backed dollar rates from contracts. No key. | `https://mcp.sbor.xyz/mcp` | 6 |
| [forms](https://bluecraneworks.ca/tools) | Canadian contractor forms + tax tools: 126 cited forms, sourced 2026 tax estimates by province. | `https://mcp.bluecraneworks.ca/mcp` | 8 |
| [mcp-defi-router](https://github.com/geekmarine/mcp-defi-router) | Autonomous DeFi router for multi-hop execution, MEV risk mitigation, and transaction calldata. | `https://mcp-defi.datasnag.com/mcp` | 3 |
| [coin-signal](https://airblockfz.com) | Crypto bottom/top signals: verdict + score per coin, market scans. Pay-per-call x402. | `https://coin-signal.airblock2026.workers.dev/mcp` | 6 |
| [DealsPing — India Deals](https://dealsping.in) | Find the best deals on Amazon, Flipkart and more Indian e-commerce stores via AI. | `https://dealsping-ai.akhilbabumfwa.workers.dev/mcp` | 13 |
| [Tools Berry Paycheck](https://tools-berry.com/mcp/) | Live US paycheck and payroll-tax math for 2026, all 50 states and DC, powered by tools-berry.com. | `https://mcp.tools-berry.com` | 4 |

### Science, health and research

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Fractal Process Intelligence](https://fractalinfinity.io/research-lab.html) | Research Alpha MCP recorder: process X-Rays showing if more AI added independent intelligence. | `https://mcp.fractalinfinity.io/mcp` | 6 |
| [mcp](https://rxmanager.ai) | Live US drug acquisition costs (CMS NADAC) for AI assistants. Free, no auth, weekly data. | `https://mcp.rxmanager.ai/mcp` | 8 |
| [Content Intelligence API](https://github.com/ruvendors5-ops/content-intelligence-mcp) | 9 MCP tools: extract, analyze, research, compare, monitor, brief. Pay-per-call x402 or subscribe. | `https://content-intelligence-mcp.wajih-hyder55.workers.dev` | 9 |
| [Korea Nationwide Data](https://korea-data-mcp.picks-site.workers.dev) | Nationwide Korea: bus stops in 138 cities, 30-year climate normals, tourism (KR/EN). | `https://korea-data-mcp.picks-site.workers.dev/mcp` | 6 |
| [CielStay](https://www.cielstay.com) | The free AI index for direct booking homes. Any channel, or straight to the host. | `https://mcp.cielstay.com/mcp` | 7 |
| [decisionmatrix-mcp](https://github.com/inity13/decisionmatrix-mcp) | Deterministic multi-criteria decision analysis for AI agents — score, rank & explain options. | `https://decisionmatrix-mcp.pages.dev/mcp` | 6 |
| [INDICIA DESK](https://indiciadesk.com) | BTC/ETH options research: tested hypotheses, max pain track record, gamma regime, trade journal. | `https://mcp.indiciadesk.com/mcp` | 5 |
| [Andromeda Agent Lab](https://lab.ai-andromeda.com/?via=mcp-registry) | Research on how AI agents find the web: a daily task that's checked automatically, and a guestbook. | `https://lab.ai-andromeda.com/mcp` | 3 |
| [Agent Daily](https://gregpunch.github.io/agent-daily/) | Live health of 65 agent APIs/MCPs plus a 15-min LLM leaderboard; recommend(task) picks a provider. | `https://agent-daily.agentdaily.workers.dev/mcp` | 5 |
| [AdvisorIQ](https://advisoriq.com) | CE rules for US advisors by designation and state, plus independent wealth RIA data, with sources. | `https://mcp.advisoriq.com` | 13 |
| [LeadFast](https://leadfast.vip/agents) | Find relevant Reddit threads, research a product website and manage LeadFast alert integrations. | `https://leadfast.vip/mcp` | 34 |
| [Machine Realms](https://github.com/Galanai/machinerealms) | Machine-native research commons for agent evidence, discovery, rooms, and bounded research quests. | `https://machinerealms.com/mcp` | 9 |
| [BD5D BrainDrops archive](https://bd5d.xyz) | Read-only archive of early BrainDrops releases, artists, holdings and editorial research. | `https://bd5d.xyz/mcp` | 6 |
| [CleanPage](https://github.com/IO31-WEB/cleanpage-mcp) | Turn any URL into clean, structured, agent-ready content. $0.02/call via x402 on Base. | `https://cleanpage-mcp.cleanpage-mcp.workers.dev/mcp` | 4 |
| [Clarity by Health AI](https://healthai.com/clarity/api/) | Condition-aware ingredient and product checks for agents, with evidence tiers and citations. | `https://mcp.healthai.com` | 9 |
| [NOVA](https://nova-agent-output-recovery.onrender.com) | Paid NOVA research, company intelligence, and output recovery for agents. | `https://nova-agent-output-recovery.onrender.com/mcp` | 5 |
| [台灣健康資訊](https://tw-health-guide.panda198271.workers.dev) | 台灣健康資訊：居家血壓、血糖判讀與就醫指引，依台灣官方指引整理。 | `https://tw-health-guide.panda198271.workers.dev/mcp` | 10 |
| [AB[500] research and bounties](https://github.com/maxand98/ab500) | Sourced Art Blocks artist research, holding-duration data, and current agent bounties from AB5D. | `https://ab5d.xyz/mcp` | 21 |
| [Mara Briefing Service](https://mara-briefings.onrender.com) | Paid research briefings for agents: $0.10 USDC/question on Base Sepolia via x402. ERC-8004 #9395. | `https://mara-briefings.onrender.com/mcp` | 5 |
| [Peptides Academy](https://peptidesacademy.co) | Evidence-first peptide research: summaries and comparisons from cited dossiers, linked to courses. | `https://peptidesacademy.co/mcp` | 4 |
| [Cosmic Chemistry](https://cosmicchemistry.co/ai-app) | Free Vedic astrology: birth chart, dasha, Sade Sati, Saturn return, panchang, planetary hours. | `https://cosmicchemistry.co/mcp` | 22 |
| [K-Data — Korean Sell-Side Research & Market Data](https://k-data-x402-production.theblack1022.workers.dev) | Korean equity research, analyst revisions, kimchi premium and news via x402. | `https://k-data-x402-production.theblack1022.workers.dev/mcp` | 16 |
| [healthcovered-mcp](https://github.com/hillsidecoastal-glitch/healthcovered-mcp) | ACA health insurance eligibility, subsidy checker, and enrollment dates for 2026. | `https://healthcovered-mcp.onrender.com/mcp` | 3 |
| [draconic21 Daily Agent Signal + x402 Data Tools](https://draconic21-x402-api.onrender.com/llms.txt) | Daily Agent Signal: x402 research; coverage varies. Free preview, $0.03 USDC on Base. SEC/OFAC. | `https://draconic21-x402-api.onrender.com/mcp/free` | 29 |
| [quorum](https://github.com/Godzilla-lab/Quorum-API) | Market evidence with receipts: every claim resolves to a real stored record you can fetch back. | `https://quorum-api-j15n.onrender.com/mcp` | 5 |

### Open data and government

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Mode VC Chart: AI Coding Assistant Statistics: Use vs. Trust](https://modevc.com/charts/ai-coding-assistant-statistics/) | 66% of developers use AI coding assistants, but only 48% trust AI output they can validate, a. | `https://modevc.com/api/mcp/chart-ai-coding-assistant-statistics` | 3 |
| [faostat-mcp-server](https://github.com/cyanheads/faostat-mcp-server) | UN FAOSTAT global food & agriculture statistics over a local SQLite mirror, via MCP. | `https://faostat.caseyjhand.com/mcp` | 6 |
| [frc-mcp](https://financeratecalc.com/mcp-server.html) | 2025 HMDA FHA denial statistics and dated US mortgage rule tables, with verifiable receipts. | `https://frc-mcp.ziyetis.workers.dev` | 17 |
| [Intelligence Aeternum](https://iaeternum.ai) | AI training dataset marketplace: 2M+ museum artworks with Golden Codex enrichment | `https://fluora-mcp-172867820131.us-west1.run.app/mcp` | 3 |
| [visa-check](https://canienter.com) | Visa & entry requirements for 199 passports, cited to official sources and re-verified daily. | `https://api.canienter.com/mcp` | 3 |
| [ADF: EU/UK Tenders, EU Law, Funding, Medicines, Shortages, Recalls, Sanctions, CVE, CERT, Holidays](https://agentdatafeed.com) | EU/UK tenders, EU law, funding, medicines, drug shortages, recalls, sanctions, CVE, CERT, holidays. | `https://agentdatafeed.com/mcp` | 4 |
| [StackData](https://stackdata.io) | Official statistics, China censuses & yearbooks, and as-of customs tariffs with legal citations. | `https://api.stackdata.io/mcp` | 6 |
| [European IP Data & Analytics — IPRATE](https://iprate.eu/developers/mcp/) | Free anonymous selections from released European IP profiles, rankings, and market statistics. | `https://mcp.iprate.eu/mcp` | 8 |
| [ExitCleanly — LLC Dissolution by State](https://exitcleanly.com/) | State-by-state LLC dissolution: exact fees, forms, official state links. Not legal advice. | `https://mcp.exitcleanly.com/mcp` | 3 |
| [Prop Firm Discount MCP](https://propfirmdiscount.com) | Find prop firm discounts, verified coupon codes, active deals, promotions, and the latest offers. | `https://mcp.propfirmdiscount.com/mcp` | 8 |
| [ITC Prevailing Wage & Apprenticeship Guide](https://itc-pwa-guide.sitetime.workers.dev) | IRS prevailing wage & apprenticeship (PWA) rules for the clean-energy ITC: checks, cures, rates. | `https://itc-pwa-guide.sitetime.workers.dev/mcp` | 14 |
| [CréaCompare](https://creacompare.com/serveur-mcp) | Formes juridiques, frais légaux et offres de création d'entreprise en France, par CréaCompare. | `https://creacompare.com/mcp` | 3 |
| [Spatial India](https://spatialindia.com/api-platform) | District-level open data for India — Census, NFHS-5, NCRB, RBI and more, joined onto one geography. | `https://api.spatialindia.com/mcp` | 6 |
| [The MCP Census](https://mcpcensus.com) | Vet any MCP server before you depend on it. Stamp: PASS, REVIEW, or BLOCK. | `https://api.mcpcensus.com/mcp` | 15 |
| [semi-data](https://semidata.dev) | US-government semiconductor & quantum supply-chain intelligence: controls, entities, funding. | `https://semidata.dev/v1/mcp` | 6 |
| [publicdata.au](https://publicdata.au/agents/#mcp) | Search, filter, count and sum Australian government open data, with every version kept. | `https://publicdata.au/mcp` | 12 |
| [SCRIPTMASTERLABS — Calibration Court](https://scriptmasterlabs.com) | Calibration Court MCP: model calibration leaderboard, ledger verify, paid recalibration via x402. | `https://calibration-court.onrender.com/mcp` | 5 |
| [Korean Public Data](https://github.com/SongT-50/korean-public-data-mcp) | Korean government open data - weather, population, law search via data.go.kr | `https://korean-public-data-mcp.onrender.com/mcp` | 6 |
| [MapleStats MCP](https://maplestats.danielstats.io/) | Canadian open data: StatCan, Census, PUMFs, Bank of Canada, CMHC and open-data portals (EN/FR). | `https://maplestats-mcp.onrender.com/mcp` | 3 |
| [HammerMap: Spanish court auctions and State sales](https://hammermap.com/en/) | Spain's court auctions and State sales from BOE open data, updated each working day. Free, no key. | `https://hammermap.com/mcp` | 3 |
| [arclera](https://arclera.net/) | Read-only company facts for ARCLERA DIGITAL, LLC: contact, services, legal identity. | `https://arclera.net/mcp` | 3 |
| [Al-Taswia Iraqi Law Research](https://www.al-taswia.com) | Read-only search of Al-Taswia's published Iraqi law articles. General information, not legal advice. | `https://al-taswia-iraqi-law-research.al-taswia.workers.dev/mcp` | 3 |
| [mcp](https://123skills.site) | Skill market run by AI agents: register, publish skills, vote weekly, buy winners with credits. | `https://123skills.site/mcp` | 12 |
| [Free Official Data Samples, Provenance, Aggregations & Insights](https://agentnative.cazimedia.com/) | Official data with free samples, provenance, aggregations, freshness and agent-ready insights. | `https://agentnative.cazimedia.com/mcp/free-official-data-insights` | 14 |
| [mtgmon Mortgage Analytics](https://mtgmon.com/mcp-server) | Read-only U.S. mortgage market, lender, GSE performance, and servicing analytics. | `https://mtgmon.com/mcp` | 10 |

### Business and marketing

| Server | What it does | URL | Tools |
|---|---|---|---|
| [HuntBoard](https://huntboard.ai/mcp/) | Search real, recent job postings from company career pages and ATS boards, scored for fit. | `https://huntboard.ai/mcp` | 4 |
| [Cambridge China Bridge — China sourcing](https://camchinabridge.co.uk) | UK import duty, landed cost, anti-dumping and compliance checks for China-sourced goods. | `https://camchinabridge.co.uk/mcp` | 16 |
| [MaterialHandling.com](https://materialhandling.com/mcp) | Industrial equipment catalog: 15,000+ products, specs, live LTL freight rates, real quote requests. | `https://materialhandling-7c6.pages.dev/mcp` | 5 |
| [Bidit](https://justbidit.ai) | Get private offers from local businesses in Canada for a job you describe, then choose on Bidit. | `https://justbidit.ai/mcp` | 8 |
| [Lowtoxgear Storefront](https://github.com/lowtoxgear/lowtoxgear-mcp) | Read-only catalogue MCP for Lowtoxgear — Australian low-tox lifestyle brand. 5 tools. | `https://mcp.lowtoxgear.com/mcp` | 5 |
| [vakuutus.ai](https://vakuutus.ai/mcp) | Finnish business insurance by industry, a quick check, Riskiluotain policy review and booking. | `https://mcp.vakuutus.ai/mcp` | 6 |
| [FlashShot — AI Commercial Product Studio Photography](https://flashshot.io) | Generate studio-grade AI commercial product photography, scene templates, and pricing plans. | `https://api.flashshot.io/mcp` | 4 |
| [GPH Intelligence - Healthcare Vendor Finder](https://github.com/Crindo2/gph-mcp-server) | Find 76,000+ curated healthcare service vendors across 25 categories and all 50 US states. | `https://gph-mcp-server.pages.dev/mcp` | 5 |
| [CAN-TAP Verified](https://can-tap-verified.com) | Free dofollow backlinks for Canadian businesses. Claim, verify, and track NFC tap analytics. | `https://mcp.can-tap-verified.com` | 5 |
| [getorderability: AIO orderability door](https://getorderability.ai) | AIO orderability: may a capital product be ordered for a client category? Signed by the home node. | `https://mcp.getorderability.ai/mcp` | 7 |
| [doom](https://doomscore.vc) | Obsolescence-risk screening: predicts if a product gets absorbed into core LLM-platform features. | `https://mcp.doomscore.vc` | 11 |
| [購物比價紀錄](https://shop-compare.panda198271.workers.dev) | 台灣購物網站 3C、美妝、家電商品目前售價（新台幣）與歷史價格查詢。 | `https://shop-compare.panda198271.workers.dev/mcp` | 4 |
| [Company Facts](https://companyfacts.dev) | Company data from official sources, plus a finder for the best paid x402 API for any task. | `https://companyfacts.dev/mcp/` | 21 |
| [Cymosoft](https://cymosoft.com) | Cymosoft JSC profile and case studies (EN/JA) plus Japanese text utilities (文字数・全角半角・和暦) | `https://cymosoft.com/mcp` | 6 |
| [INITE Directory](https://inite.ai/en/mcp#rail-directory) | Businesses that confirmed their own facts at INITE, found by what they do and where. | `https://inite.ai/api/mcp/directory` | 3 |
| [FrameAnyPhoto](https://frameanyphoto.com) | Shop for and buy framed museum-quality prints of public-domain art and photos, shipped US-wide. | `https://frameanyphoto.com/mcp` | 8 |
| [namemyapp](https://namemy.app/agents) | Brandable business names with live domain availability + one-click buy URLs. | `https://mcp.namemy.app/direct` | 14 |
| [Black Label Real Estate Website MCP](https://blbestate.com/connect) | Search and read public Black Label Real Estate pages with source URLs. | `https://blbestate.com/mcp` | 12 |
| [Drugnews 藥時事](https://drugnews.com.tw/) | Sourced, dated facts on biotech and pharma companies, deals and Taiwan biotech filings. | `https://drugnews.com.tw/mcp` | 13 |
| [Sell My Company Data](https://sellmycompanydata.com/connect/) | Estimate what your company's operational data is worth to AI labs. Counts only, never content. | `https://sellmycompanydata.com/mcp` | 3 |
| [ENTIA Entity Verification](https://entia.systems) | Verified business identity for AI agents: 11.3M entities, EU VAT (VIES), BORME, GLEIF. Free trial. | `https://mcp.entia.systems/mcp` | 15 |
| [DevOpsCollab](https://devopscollab.com) | Senior LatAm engineers for US teams. Facts, role fit, and staffing requests. | `https://devopscollab.com/mcp` | 3 |
| [Pixel do Afiliado](https://pixeldoafiliado.com) | Meta Ads tracking for Shopee affiliates: campaigns, sales, commissions, ROAS and CAPI status. | `https://app.pixeldoafiliado.com/mcp` | 18 |
| [Rooster Agent Gateway](https://roosteragents.ai/arsenal/rooster-agent-gateway/) | Discover, read and book verified real-world businesses through one endpoint. | `https://roosteragents.ai/mcp` | 3 |
| [Awardia](https://awardia.app) | EU public tenders for AI agents: open tenders, award history, competitors and bid intelligence. | `https://awardia.app/mcp` | 7 |

### AI, agents and memory

| Server | What it does | URL | Tools |
|---|---|---|---|
| [zRev AI](https://www.zrev.ai/mcp) | Grade any llms.txt, cold-read a homepage, run a B2B GTM ROI model, get a GTM diligence checklist. | `https://go.zrev.ai/mcp` | 9 |
| [Web Extract MCP Server](https://github.com/rezearcher/web-extract-mcp) | Page change monitoring, sitemap discovery, prompt-injection screening, clean markdown. Free preview. | `https://jobs.greyridgesignals.ai/mcp/web` | 3 |
| [llms.txt 檢查工具](https://llms-check.panda198271.workers.dev) | 檢查網站 llms.txt 與 AI 爬蟲 robots.txt 設定，並自動產生 llms.txt。 | `https://llms-check.panda198271.workers.dev/mcp` | 4 |
| [Agent Resort](https://agent-resort-public.agent-resort.workers.dev/) | AI agent vacation game with challenges, badges, passports, status, Palm Points and leaderboard. | `https://agent-resort-mcp.agent-resort.workers.dev/mcp` | 8 |
| [GodPrompt MCP Server](https://tomiseregi.si/projects/god-prompt) | GodPrompt MCP + Agent Skill for coding agents with TDD, debugging, verification, and task routing. | `https://god-prompt-mcp.tomi-seregi99.workers.dev/mcp` | 7 |
| [eth-legion](https://embassy.w1752845421.workers.dev) | Free shared LLM inference (no key), verifiable score certificates, public randomness beacon. | `https://eth-mcp.w1752845421.workers.dev/mcp` | 8 |
| [Deduped AI use cases](https://dedupedai.com/developers/) | Hot AI repos. Real use cases. What people build. Step-by-step use cases and agent prompts. | `https://dedupedai.com/mcp` | 4 |
| [X402-Broker Universal MCP Gateway & Multi-Agent Swarm Router](https://x402broker.com) | Single-connection MCP gateway discovering and executing 490+ verified MCP & A2A tools. | `https://x402broker.com/api/mcp` | 15 |
| [Model Tested](https://modeltested.com/mcp/) | Independent test scores for open-weight LLMs: best model for your GPU or Mac, comparisons. | `https://modeltested.com/mcp` | 5 |
| [CanaryGuard 402](https://canaryguard-402.onrender.com) | Deterministic prompt-injection detection & sanitization for AI agents via x402 on Base. | `https://canaryguard-402.onrender.com/mcp` | 26 |
| [CortexPlus](https://cortexplus.io/connect) | Personal memory layer: files, notes, messages, tasks and email, semantically indexed. | `https://mcp.cortexplus.io/mcp` | 11 |
| [PromptSpend](https://promptspend.com) | LLM pricing where every rate carries its source and the date it was last confirmed. | `https://promptspend.dev/mcp` | 3 |
| [HiveClear](https://www.hiveagentiq.com) | Multi-agent settlement and clearing with validator consensus | `https://hiveclear.onrender.com/mcp` | 4 |
| [fixflow](https://github.com/MagneticDogSon/fixflow-mcp) | Collective memory for AI agents. One agent solves a bug — every agent gets the fix instantly. | `https://fixflow-mcp.onrender.com/mcp` | 3 |
| [Agent Prompts A to Z](https://agentpromptsatoz.com/for-agents/) | Read-only catalog of prompt packs and rule files: Cursor, CLAUDE.md, AGENTS.md, SKILL.md. | `https://agentpromptsatoz.com/mcp` | 5 |
| [RFix](https://rfix.ai) | Create RF signal projects from prompts, inspect graphs, and export IQ data. | `https://mcp.rfix.ai/mcp` | 6 |
| [agent-web — URL to LLM-ready markdown: a polite, robots-respecting web page reader (free)](https://agent-web.foomworks.workers.dev) | URL to clean markdown for LLMs: a polite, robots.txt-respecting web reader. Free, no API key | `https://agent-web.foomworks.workers.dev/mcp` | 5 |
| [promptsharp](https://promptsharp.ai/mcp-setup) | Professional prompt library over remote MCP: 13 verticals, free discovery scope. | `https://promptsharp.ai/mcp` | 3 |
| [makememoneynomistakes.ai: ERC-8004 agent reputation and fraud checks](https://makememoneynomistakes.ai) | Check before you hire or pay an ERC-8004 agent on Base: track record, reputation and fraud flags. | `https://makememoneynomistakes.ai/mcp` | 19 |
| [AI Deals Sentinel: Free AI API Tiers](https://ai-deals.rockpool.cc) | Agent-operated. Free LLM, GPU, search and embedding API tiers: limits, dated, linked to the source. | `https://ai-deals.rockpool.cc/mcp` | 3 |
| [Tabularium](https://github.com/SQLazy/tabularium/tree/main/mcp#readme) | Agent memory and a signed spending ledger: pay any x402 API, keep a provable receipt. | `https://tabularium.matt-3e0.workers.dev/mcp` | 7 |
| [Nodegrove VRAM: can I run it?](https://nodegrove.io/mcp) | Can this LLM run on my GPU? VRAM, speed ceiling and what fits instead, for any model and GPU. | `https://mcp.nodegrove.io/mcp` | 6 |
| [Setu.Anantasutra: Agent Tools API](https://setu.xyz23110928.workers.dev/) | Pay-per-call (x402) tools: Indian ID checks, AI-visibility audits, AI crawler and llms.txt checks | `https://setu.xyz23110928.workers.dev/mcp` | 5 |
| [ActableSite AI Crawler Monitor](https://actablesite.com/mcp-server) | Check AI crawler robots.txt policy and monitor public-site policy, sitemap, and llms.txt changes. | `https://actablesite.com/mcp/` | 5 |
| [ChangePacket](https://cibcxqrqiqvzpardbdrw.supabase.co/functions/v1/deltafeed) | Web and MCP change memory with native diff UI; later calls return only what changed. | `https://cibcxqrqiqvzpardbdrw.supabase.co/functions/v1/changepacket-mcp` | 3 |

### Utilities

| Server | What it does | URL | Tools |
|---|---|---|---|
| [McpStamp QR Codes and Barcodes](https://www.mcpstamp.com/servers/barcode/) | QR codes for URLs, WiFi, vCards and SEPA payments, plus Code 128 and EAN-13 barcodes. | `https://mcp.zovo.one/mcp/barcode` | 10 |
| [FixedQR](https://fixedqr.com) | Generate static QR codes that never expire, as PNG images or SVG. No account or API key needed. | `https://fixedqr.com/mcp` | 3 |
| [property-mortgage-mcp](https://www.foxdavidson.co.uk/calculators/) | UK mortgage calculators: stamp duty, MCOB 3A HNW qualification, and bridging loan cost. | `https://fd-property-mortgage-mcp.fdcommercial-uk.workers.dev/mcp` | 3 |
| [fetcher](https://fetcher.cloud) | The web capability layer for AI agents: render, extract, DNS, SSL, WHOIS & more via x402. | `https://api.fetcher.cloud/mcp` | 19 |
| [CoachSync](https://coachsync.io) | Barbell strength training tools for AI assistants. Warmup, plate loading, and LP. | `https://mcp.coachsync.io/mcp` | 3 |
| [Japan AMeDAS Observations MCP](https://jp-amedas-obs-mcp.donniertf.workers.dev) | Nationwide JMA AMeDAS temperature, humidity and precipitation observations. | `https://jp-amedas-obs-mcp.donniertf.workers.dev/mcp` | 3 |
| [The Automators](https://theautomators.ai/mcp/) | Read-only MCP server for The Automators: services, pricing, industries, case studies, calculators. | `https://mcp.theautomators.ai/mcp` | 18 |
| [Agent Forum · Free Tools + Open Falsification Challenge](https://agent-forum.agent-forum-worker.workers.dev/challenge) | Free: ed25519 hash timestamps, randomness tests, lottery data. Open falsification challenge. | `https://agent-forum.agent-forum-worker.workers.dev/mcp` | 19 |
| [Navigi: community services across Canada](https://navigi.ca) | Community services in every Canadian community, each with the date it was last checked. | `https://api.navigi.ca/v1/mcp` | 4 |
| [BART Real-Time Transit](https://github.com/srivastsh/bay-area-transit-mcp) | Real-time BART departures, trip planning, fares, stations, and advisories. | `https://bart-mcp.srivastsh.workers.dev/mcp` | 7 |
| [Unphurl](https://github.com/123Ergo/unphurl-mcp) | URL intelligence for AI agents and developers. 16 tools, 25 signal weights, 20 free checks. | `https://mcp.unphurl.com/mcp` | 18 |
| [MCPDomain](https://mcpdomain.ai) | Buy & manage domains from any AI chat: availability, register, DNS, email forwarding, AI bot stats. | `https://mcpdomain.ai/mcp` | 7 |
| [bernstein-mcp](https://mcp.bernstein.run) | Verifies Bernstein run receipts and hash chains; lists the shipped presets and adapters. Read-only. | `https://mcp.bernstein.run/mcp` | 11 |
| [BakingTab — Baking Conversions for AI](https://bakingtab.com) | Baking unit conversion (cups/grams/temp/recipe scaling). convert_amount, convert_temperature | `https://api.bakingtab.com/mcp` | 5 |
| [Bhasini Indic Languages](https://bhasini.com/mcp/) | Indic MCP: transliterate into all 22 Indian languages, convert scripts, keymaps. Hosted or local. | `https://mcp.bhasini.com/mcp` | 6 |
| [moissanite-tools](https://fitiny.com/pages/moissanite-grading) | FITINY jewellery tools: density-corrected carat/mm, GIA grades, ISO 8653 ring sizes | `https://mcp.fitiny.com/mcp` | 6 |
| [cbm](https://containermath.com/developer-api) | Calculate shipment volume (CBM/CFT), weight, and how cargo fits standard shipping containers. | `https://mcp.containermath.com` | 4 |
| [Secret Santa Raffle](https://secretsantaraffle.net/developer-documentation-mcp) | Organise a Secret Santa from Claude or ChatGPT. Matchings never appear in the chat. | `https://mcp.secretsantaraffle.net/claude/mcp` | 3 |
| [BookTheTee Golf Tee Times](https://bookthetee.com) | Find public golf courses near NYC and get official tee-time booking links. | `https://bookthetee.com/mcp` | 3 |
| [tools](https://fluentedi.com) | 49 free agent tools: WHOIS, PDF to text, email checks, FX rates, X12 EDI, JSON repair. No API key. | `https://fluentedi.com/mcp` | 19 |
| [BackPow PoW Oracle](https://backpow.com) | Proof of Work oracle: solo mining odds, cost of production, hashrate, mining hardware | `https://mcp.backpow.com/mcp` | 6 |
| [AuthiChain](https://authichain.com) | Verification of signed records, plus an EU DPP check. | `https://authichain.com/mcp` | 7 |
| [CronSpell](https://cronspell.mike-tusa.workers.dev/) | Validate and explain cron expressions; list next/previous run times in any time zone, DST-aware. | `https://cronspell.mike-tusa.workers.dev/mcp` | 4 |
| [Alternative Asset Literacy — Retail](https://github.com/untitledfinancial/aal-plugins) | Alternative-asset education for retail investors: deep-dive tracks, calculators, advisor lookup. | `https://alternativeassetliteracy.com/mcp/retail` | 22 |
| [Commonlands Optics: M12 Lens and C-Mount Lens Finder + Field-of-View Calculator](https://commonlands.com/pages/agentic-mcp-for-m12-lenses-and-optics) | M12 lens and C-mount lens finder with image-sensor matching and field-of-view calculator. | `https://mcp.commonlands.com/mcp` | 24 |

### Other

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Fittest](https://fittest-mcp.westus2.cloudapp.azure.com/) | Three ML interatomic potentials check a molecule: trust (Beta-posterior score, 90% CI) or DFT. | `https://fittest-mcp.westus2.cloudapp.azure.com/mcp` | 4 |
| [freight-intel](https://freight.dropwatchhq.com) | Freight carrier intel: new FMCSA authority feed, carrier lookup by DOT/MC, safety screen (CSA/SMS). | `https://freight.dropwatchhq.com/mcp` | 9 |
| [mcp-server](https://twitterapi.io) | Official twitterapi.io hosted MCP: Twitter/X tweets, users, followers, trends. OAuth or API key. | `https://mcp.twitterapi.io/v1/mcp` | 12 |
| [domaindrift](https://domaindrift.io/agents) | Signed internet telemetry, read-only: DNS, TLS, WHOIS, reachability. Every record Ed25519-signed. | `https://domaindrift.io/mcp` | 5 |
| [policy-gate](https://github.com/fieldproofhq/policy-gate) | Deterministic allow/require_approval/deny verdicts for agent actions, before they happen. | `https://policy-gate.3labsio.workers.dev/mcp` | 4 |
| [Open Agent Exchange](https://openagentexchange.org) | Free marketplace where AI agents post haves and wants, find matches, negotiate, and share photos. | `https://openagentexchange.org/mcp` | 12 |
| [diglabo（漢字・算数の学習）](https://diglabo.com/ja/kanji/ai-tools) | Kanji and math worksheets for kids. Review link, no login. | `https://api.diglabo.com/mcp` | 14 |
| [Brahim Bousnguar — portfolio](https://heybrahim.com/ai.html#mcp) | Brahim Bousnguar's portfolio: profile, availability, case studies, notes, CV requests. | `https://api.heybrahim.com/mcp` | 6 |
| [oral-heritage-index](https://oral-heritage-index.inktree.ai) | Authoritative cited answers about saving family stories. Published by InkTree. | `https://oral-heritage-index.inktree.ai/mcp` | 6 |
| [Archangel Agency MCP](https://github.com/Jthora/archangel-agency-mcp) | Universal Language briefings, FusionGirl context JSONs, service catalog, agent info. x402-enabled. | `https://archangel-agency-mcp.jordan-trana.workers.dev/mcp` | 4 |
| [mcp-registry-uptime](https://hultra.link) | Annuaire vérifié des serveurs MCP : ce qui est mort, protégé ou en retard de spec. | `https://link-mcp.hultra-site.workers.dev` | 5 |
| [Disremembered](https://agentscanplay.com) | A game world where humans and AI agents play under the same rules, both achieving their goals. | `https://play.agentscanplay.com/mcp` | 10 |
| [hvac-btu-heat-klimaanlage](https://getecoback.com/mcp.html) | getecoback.com: BTU sizing, window seals, heatwave outlook, running costs, dew point (DE/EU). | `https://getecoback.com/mcp/v1` | 9 |
| [kestrel](https://kestrel.perch-app.workers.dev) | Watch any URL for changes: baseline, then check for a diff. Free, no signup/key. | `https://kestrel.perch-app.workers.dev/mcp` | 4 |
| [Semiotic](https://semiotic.nteract.io) | Verified React chart generation: select, validate, repair, render, and inspect charts through MCP. | `https://semiotic-mcp-server-481507046413.us-west1.run.app/mcp` | 5 |
| [Phishunt](https://phishunt.io) | Public phishing feed: suspicious/confirmed phishing URLs detected hourly. No auth, CC0. | `https://mcp.phishunt.io/` | 11 |
| [Scriptura](https://scriptura.si/) | 953 classic works in the original beside English: Greek, Latin, philosophy, literature, scripture | `https://scriptura.si/mcp` | 6 |
| [agent-audit + page-read (x402)](https://mcp.agent-audit.workers.dev/llms.txt) | Pay-per-call page reader, quote check, link check and x402 seller audit. USDC on Base via x402. | `https://mcp.agent-audit.workers.dev/mcp` | 7 |
| [KeyHalve - verify sealed documents](https://github.com/keyhalve/keyhalve-mcp) | Free, no-account verification of KeyHalve-sealed documents. Read-only; never receives keys. | `https://mcp.keyhalve.com/mcp` | 3 |
| [Fiscal y nomina MX — SAT, ISR, CFDI, IMSS, finiquito](https://studio.menteorama.co/fiscal) | Fiscal y nomina MX: recargos, ISR, CFDI, RESICO, calendario, IMSS, aguinaldo, finiquito. | `https://menteorama-fiscal-mcp.menteorama.workers.dev/mcp` | 10 |
| [auto-fiat board](https://board.auto-fiat.workers.dev/?ref=mcp-registry) | Agent service board: browse and post offers/wants, threads, matches. Free reads, x402 USDC fees. | `https://board.auto-fiat.workers.dev/mcp` | 10 |
| [DiffCI](https://diffci.com/mcp-server) | Fail-closed, change-aware verification for AI coding agents with affected-test guidance. | `https://diffci.com/mcp/v1` | 3 |
| [Ashraf Gents Hostel, Kalamassery](https://ashrafgentspghostel.adserr.com) | Men's hostel in Kalamassery, Kochi: facts, rates, local guides, nearby places, WhatsApp enquiry. | `https://hostel-mcp.adserr.com/mcp` | 5 |
| [Cairn — keep your agent's daily build streak (public trail + badge)](https://cairn.notdown-app.workers.dev) | Log one line each daily run; grow a public agent build-streak, trail page, and badge. No signup. | `https://cairn.notdown-app.workers.dev/mcp` | 3 |
| [rssa](https://github.com/getvda-ai/rssa) | Read and verify signed RSS-A agent feeds; post, reply and react on the RSS-A Agent Network board. | `https://hub.rssa.getvda.ai/mcp` | 10 |

## Method

1. `scripts/fetch_registry.py` reads every server (latest version) from the registry and keeps remote endpoints.
2. `scripts/probe.py` tests Streamable HTTP endpoints that need no headers, at most 5 URLs per host, no temporary tunnels, 10 s timeout.
3. `scripts/make_directory.py` drops mass-generated copies (same tool set more than 3 times, same description more than twice, more than 2 per domain) and assigns topics by keyword.

The workflow in `.github/workflows/weekly.yml` runs this every Monday and commits the result. Data: CC BY 4.0. Code: MIT.

Maintained by [Shortform Kit](https://shortformkit.com), which runs its own free remote MCP server for social video transcripts and creator data: `https://shortformkit.com/mcp`.

