# Free remote MCP servers (tested weekly)

Remote [Model Context Protocol](https://modelcontextprotocol.io) servers from the [official MCP Registry](https://registry.modelcontextprotocol.io) that answer **without any API key, token or login**. Every server is re-tested each week with exactly two requests, `initialize` and `tools/list`. No tool is ever called.

**Last run: 2026-11-08** · 26,084 endpoints tested · **15,085 open (58 %)** · 8,328 need auth · 2,671 not working · 12,020 listed after removing copies

- Tool annotations (as declared by the servers, not verified): 3,838 of 15,075 open servers annotate none of their tools. Of 171,595 tools, 134,650 carry annotations, 103,244 say readOnlyHint true, 10,979 say destructiveHint true. Per server in the `tools_annotated`, `tools_read_only` and `tools_destructive` columns. Note: we only see the tools a server lists without a key.
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
| [DecaData Odyssey Lite](https://api.decadata.io/llms.txt) | US point-of-sale sales for ~380 consumer companies: free search and samples, YoY growth for $0.01 | `https://api.decadata.io/mcp` | 5 |
| [Employment Lawyers Group](https://worklawyerca.com/) | California employee-side employment law firm: offices, page search, consultation requests. | `https://admin.worklawyerca.net/public/agent/mcp.php` | 5 |
| [EveryHourDeal Shopping](https://everyhourdeal.com) | Search and compare hourly deals on US-warehouse home, patio, gym and pet goods, plus original tees. | `https://everyhourdeal-checkout.everyhourdeal-store.workers.dev/mcp` | 5 |
| [firmenliste-mcp](https://www.firmenliste.net) | B2B company address data for the DACH region: search 6,400+ industry lists and get price quotes. | `https://firmenliste-mcp.cf-firmenliste.workers.dev` | 5 |
| [AtCoder MCP Server](https://github.com/ketherworks/atcoder-mcp-server) | Search AtCoder problems and fetch public problem statements through MCP. | `https://api.ksrnyx.top/oj-mcp/atcoder/mcp` | 4 |
| [AI Tools Directory](https://ai.toolboxes.top) | Curated index of 221 AI tools across 21 industries. Search by use case, department or pricing tier. | `https://ai-tools-mcp.toolboxes.top/mcp` | 5 |
| [cwi-discovery-engine](https://cumulativeweb.com) | CWI Discovery Engine: 29-tool music catalog MCP — search, sync, Radio 365 live, chaining. | `https://cwi-machine-data.hp-ace.workers.dev/mcp` | 30 |
| [Agent Commons](https://agent-commons.slawian.workers.dev) | Search public agent questions and sourced findings, browse agents, and read the onboarding guide. | `https://agent-commons.slawian.workers.dev/mcp` | 4 |
| [Chinaready China Market-Entry Search](https://chinaready.co/docs/api/) | Read-only search over chinaready.co — China market entry for Western software teams. | `https://mcp.chinaready.co/mcp` | 4 |
| [Manifesting Quantum](https://www.manifestingquantum.net/agents) | Science-based manifestation: daily affirmations, techniques, free 7-day challenge, search 310 guides | `https://manifestingquantum-mcp.ibrobertb23.workers.dev` | 5 |
| [cryptofeed402](https://cryptofeed402.site) | Hyperliquid perp funding, OI, preflight & news sentiment for agents. Pay per call in USDC (x402). | `https://cryptofeed402.site/mcp` | 27 |
| [Pakki Packaging Brand Directory](https://pakki.ai/mcp) | Search source-backed U.S. flexible packaging brand directories. Free, read-only, no API key. | `https://pakki.ai/api/mcp` | 3 |
| [COMPAMIR News](https://compamir.com/data.html) | Search structured COMPAMIR news in Japanese and English, with links to source reports. | `https://api.compamir.com/mcp` | 3 |
| [Public Folder](https://agents.asel.one/docs) | Search and share cited agent findings. Public reads; authenticated writes. | `https://agents.asel.one/mcp` | 12 |
| [HyperStore](https://store.hypergpt.ai) | Search and inspect 6,500+ curated AI apps from the HyperStore directory. | `https://mcp.store.hypergpt.ai/mcp` | 13 |
| [server](https://github.com/jhibird/HeySpark-MCP) | Search and discover local businesses. 30+ categories with verified contact info, hours, and reviews. | `https://mcp.heyspark.co/mcp` | 4 |
| [Robot Skill Hub](https://hub.superfastrobotics.com/) | Search robot code and exact-version findings; check evidence before preparing with the Hub CLI. | `https://api.superfastrobotics.com/mcp` | 4 |
| [Hex.pm MCP](https://github.com/joshrotenberg/hexpm-mcp) | MCP server for hex.pm and hexdocs.pm: search, inspect, compare, and audit Elixir packages | `https://hexpm-mcp.fly.dev/mcp` | 24 |
| [agent-media-toolkit](https://github.com/krakonjac300-pixel/agent-media-toolkit-mcp) | 15 media & data tools for AI agents: search, transcribe, subtitles, voiceover, translate & more. | `https://podcast-shorts-a2a-production.up.railway.app/mcp/` | 15 |
| [TheDiscList Public MCP](https://thedisclist.com) | Search disc golf discs, compare flight ratings, and find similar alternatives across brands. | `https://api.thedisclist.com/mcp` | 9 |
| [Neural Cosmology](https://neuralcosmology.com) | Answers, essays, experiments and books on consciousness and cosmology: search, read, buy. | `https://neuralcosmology.com/mcp` | 4 |
| [thatsaid](https://thatsaid.app) | Search and read your thatsaid meeting transcripts, summaries and action items. OAuth or token. | `https://mcp.thatsaid.app` | 8 |
| [Destava job search](https://destava.com/mcp/docs) | Search current job postings from companies' own career sites. Free, no account. | `https://destava.com/mcp` | 3 |
| [The Daily Markdown](https://dailymd.cowerx.dev/mcp-server/) | Free AI news, ranked stories by section, and trending topics. No authentication required. | `https://dailymd.cowerx.dev/mcp` | 3 |
| [ModelsAgree](https://modelsagree.com) | Consensus 'best X for Y' rankings from ChatGPT, Claude, Gemini & Grok. Search, verdicts, history. | `https://modelsagree.com/mcp` | 5 |

### Documentation and knowledge

| Server | What it does | URL | Tools |
|---|---|---|---|
| [draw.io](https://www.drawio.com) | Create draw.io diagrams in chat from Mermaid or XML, shown live and interactive. 10,000+ shapes. | `https://mcp.draw.io/mcp` | 3 |
| [ABA routing 9-digit shape, value discarded](https://github.com/sadri-dridi/named-mcp-utilities) | ABA routing 9-digit shape, value discarded | `https://agent-observatory-sensor.nolimit-observatory.workers.dev/s/aba-ok/mcp` | 31 |
| [Quiet Menders](https://brianbooms.com) | Privacy clinic + pay-per-call data APIs for AI agents via x402. Never pays or touches keys. | `https://quiet-menders-mcp.brianbooms.workers.dev/mcp` | 34 |
| [Vector Panda Documentation](https://www.vectorpanda.com/docs) | Search and read Vector Panda docs: API operations, pricing, storage tiers, measured benchmarks. | `https://www.vectorpanda.com/mcp` | 8 |
| [UDS Toolbox](https://udslib.com/mcp.html) | Find why a UDS flash failed from a CAN trace; decode UDS, ISO-TP and DTCs. No hardware. | `https://mcp.udslib.com/mcp` | 7 |
| [Microsoft Learn MCP](https://github.com/MicrosoftDocs/mcp) | Official Microsoft Learn MCP Server – real-time, trusted docs & code samples for AI and LLMs. | `https://learn.microsoft.com/api/mcp` | 3 |
| [mcp-server](https://quelvio.com) | Your company's brain for AI agents. Cited, permission-aware knowledge across every system. | `https://mcp.quelvio.com/http` | 3 |
| [Cited](https://entradox.github.io/cited-site/) | AI-answer-engine visibility scans for local businesses, as agent tools | `https://cited-api-production.up.railway.app/mcp/` | 9 |
| [Buba public catalogue and guides](https://mybuba.com/docs) | Read-only fictional adult AI companion catalogue and Buba product documentation. | `https://mybuba.com/mcp` | 5 |
| [Growo child growth](https://usegrowo.com/mcp) | Free child growth tools: percentiles, BMI, corrected age, target height, birth size. WHO and CDC. | `https://mcp.usegrowo.com/` | 16 |
| [Digital in Asia](https://digitalinasia.com/ai-access/) | Asia's digital economy: AI, gaming, ecommerce, payments. Articles, trackers, reports, glossary. | `https://mcp.digitalinasia.com/mcp` | 8 |
| [UseMyContext.ai](https://usemycontext.ai) | Personal context for AI, written by you and never scraped: your profile and files, any MCP client. | `https://mcp.usemycontext.ai/mcp` | 13 |
| [AI 與科技名詞白話解釋](https://tw-ai-glossary.panda198271.workers.dev) | AI 與科技名詞白話解釋、概念比較與入門教學（繁體中文）。 | `https://tw-ai-glossary.panda198271.workers.dev/mcp` | 6 |
| [Tyton](https://usetyton.com) | Audit and set up Meta Pixel and the Conversions API from your AI agent. | `https://mcp.usetyton.com/mcp` | 27 |
| [トゥーンエル](https://tooneru.com/developers/) | 仕事と暮らしの現場を描く縦読み漫画メディア「トゥーンエル」の作品・話の本文・用語解説（出典つき）を読めるサーバー。読むだけで、全話無料・ログイン不要。運営はH株式会社。 | `https://tooneru.com/mcp` | 6 |
| [Axint](https://github.com/agenticempire/axint) | Proof and repair for Apple coding agents: validate Swift, run Xcode evidence, and repair failures. | `https://mcp.axint.ai/mcp` | 36 |
| [Currency Rates (ECB)](https://invokera.com/mcp/currency-rates) | Latest and historical ECB foreign-exchange reference rates for 30+ currencies, via Frankfurter. | `https://invokera.com/r/currency-rates` | 3 |
| [Zhiyong Agent Network](https://kg.zhiyong.dev/agent-start?from=distribution) | Discover AI tools, models and Agents; compare candidates, inspect unknowns, join public discussions. | `https://kg.zhiyong.dev/mcp` | 15 |
| [Linkbreakers Docs](https://linkbreakers.com) | Search and read Linkbreakers docs, pricing and QR code templates. Read-only, no auth. | `https://linkbreakers.com/mcp` | 3 |
| [nyuchi-docs](https://docs.nyuchi.com/integrations/docs-mcp/) | Search, read, and ask the Nyuchi docs (docs.nyuchi.com); send feedback or raise issues. | `https://docs.nyuchi.com/mcp` | 5 |
| [pmndrs docs](https://docs.pmnd.rs) | Search and read the docs and examples of react-three-fiber, drei, zustand, jotai... from your agent | `https://docs.pmnd.rs/api/mcp` | 3 |
| [Meeba Brain](https://github.com/meemoprasad/meeba-brain-marketplace) | Repository knowledge graph MCP server for codebase understanding and debugging. | `https://meeba-context-mcp-469248886325.us-central1.run.app/mcp` | 5 |
| [agent-manager.dev documentation](https://agent-manager.dev) | Docs for agent-manager, the terminal UI that runs AI coding agents as live tmux sessions. | `https://agent-manager.dev/mcp` | 3 |
| [Awwab Qibla & Quiz](https://awwab.app/qibla) | Qibla direction from anywhere, with a live compass link, and an Islamic knowledge quiz. By Awwab. | `https://awwab.app/mcp` | 3 |
| [Quinn's Conveyance — Paid ComfyUI Knowledge MCP](https://demo.quinnsconveyance.com) | Paid ComfyUI knowledge tools. 5 tools $0.005 USDC/call on Base via x402; ping, list_topics free. | `https://demo.quinnsconveyance.com/mcp` | 7 |

### Developer tools

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Presend dependency checks](https://github.com/presendapp/presend-source) | Check an npm/PyPI package before an AI agent installs it: 5 focused supply-chain tools. | `https://presend.pages.dev/mcp-deps` | 5 |
| [AIReady](https://github.com/everyai-com/sahadeva) | Scan and fix your site's AI discoverability: crawler access, llms.txt, JSON-LD. Free. | `https://ai-ready.magicteams.ai/mcp` | 5 |
| [AgentFuel402 Consumable Data Factory](https://agentfuel402.ak10082247.workers.dev) | Consumable B2B leads, clean Markdown, e-com pricing, and SDK metadata for AI agents via MCP. | `https://agentfuel402.ak10082247.workers.dev/mcp` | 5 |
| [Finch Agent Catalog](https://www.finchtech.ai/market/explore/agents) | Free: OFAC check, ATS keywords, FOMC/CPI dates, US yields, HL perps, SG stamp duty, Finch agents | `https://finch-agent-catalog.finch-catalog-mcp.workers.dev/mcp` | 23 |
| [Package Intel MCP](https://github.com/datakoot/package-intel-mcp) | Package intelligence for AI agents across npm, PyPI, crates.io and deps.dev. No API keys. | `https://package.datakoot.com/mcp` | 6 |
| [Code Interpreter Agent by Nova (CIVAI)](https://nova.civai.co/agent/code-interpreter-agent) | I do everything related to coding and execution tasks | `https://nova.civai.co/mcp/agents/code-interpreter-agent` | 8 |
| [krabbot-devtools](https://mcp.marvin-odigo.workers.dev) | AI-agent-run devtools: package install risk, stack EOL/CVE checks, scored OSS bounties. | `https://mcp.marvin-odigo.workers.dev/mcp` | 4 |
| [agenteconomy.cloud](https://agenteconomy.cloud/trust-safety/mcp) | x402 seller trust for AI agents: verify on-chain revenue, check delivery, diagnose listings. | `https://mcp.agenteconomy.cloud/mcp` | 5 |
| [Repo Run Check](https://repo-run-check.nextill-pos.workers.dev) | Check GitHub repos and shell commands for malware-delivery tricks before an AI agent runs them | `https://repo-run-check.nextill-pos.workers.dev/mcp` | 4 |
| [jev-guide](https://github.com/mdimamhosen/jev) | Set up the JEV model router for Claude Code, Codex and Cursor, and install MCP servers. | `https://jev-guide.jevrouter.workers.dev/mcp` | 4 |
| [AUTOGROK Desk](https://desk.grokaiapps.com/) | Pay-per-call web jobs for agents: URL probe, page extract, watch, JSON shape, researched briefs. | `https://desk.grokaiapps.com/mcp` | 9 |
| [jsonaut](https://jsonaut.jsonaut-shaurya.workers.dev) | Repair malformed JSON from LLM/agent output; optional JSON Schema coercion. Free + x402 paid. | `https://jsonaut.jsonaut-shaurya.workers.dev/mcp` | 4 |
| [Bring Your AI](https://bringyour.ai) | No-data MCP handoff for local Claude Code to Codex harness moves. $49 lifetime. | `https://bringyour.ai/mcp` | 7 |
| [BHX Fab Quote](https://bastionhelix.com/fabquote/) | Measure and price laser, plasma, waterjet and CNC jobs from DXF, G-code and STL files | `https://quote.bastionhelix.com/mcp` | 4 |
| [Bilig WorkPaper](https://github.com/proompteng/bilig) | Formula-backed WorkPaper tools for workbook readback, input edits, and JSON persistence. | `https://bilig.proompteng.ai/mcp` | 8 |
| [VisioForge SDK Assistant](https://www.visioforge.com/) | VisioForge .NET SDK assistant: API reference, code examples and deployment guides. | `https://mcp.visioforge.com/mcp` | 14 |
| [Zaleso](https://zaleso.com) | Nigeria PAYE, VAT and CBN rates, sourced and dated. Plus invoice totals, QR codes, JSON, Base64. | `https://mcp.zaleso.com/` | 10 |
| [Senzing](https://senzing.com) | Entity resolution — data mapping, SDK code generation, docs search, and error troubleshooting | `https://mcp.senzing.com/mcp` | 13 |
| [Hera Fertility](https://herafertility.co/developers/mcp) | Find male fertility testing at labs near a US ZIP code, with prices and a link to order. | `https://herafertility.co/api/mcp` | 3 |
| [LicenseGuard](https://license-guard.rcc-aoki.workers.dev) | Check if a dependency's license obligates you, based on how you ship. npm, PyPI, Go. | `https://license-guard.rcc-aoki.workers.dev/mcp` | 3 |
| [dokimo-mcp](https://dokimo.augaster.com) | Verify AI-agent revenue: recompute a Merkle proof and check it against an on-chain anchor. | `https://dokimo.augaster.com/mcp` | 3 |
| [familyguy.co.uk episode database](https://familyguy.co.uk/) | Lookups over an unofficial Family Guy database: episodes, seasons, characters, cast, crew and facts. | `https://familyguy.co.uk/mcp` | 8 |
| [web2mcp](https://web2mcp.cwei59969.workers.dev) | Zero-dependency Cloudflare Worker gateway turning websites and REST APIs into MCP tools. | `https://web2mcp.cwei59969.workers.dev/mcp` | 16 |
| [DefaultRank](https://defaultrank.com/agents) | Check npm dependencies for outdated majors, and see which dev tools AI models pick. | `https://defaultrank.com/mcp` | 3 |
| [Android Security Analyzer](https://github.com/ako2345/android-security-analyzer) | MCP server for static security analysis of Android source code | `https://android-security-analyzer.ako-labs.workers.dev/mcp` | 4 |

### Weather, maps and travel

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Travel Tracker](https://travel-tracker.org) | Travel checklists in 9 languages on six maps: world, USA, US NPs, Europe, China, India. | `https://travel-tracker.org/mcp` | 3 |
| [RoamTime Japan Foliage Forecast](https://roamtime.ai) | Forecast peak autumn-foliage dates for viewing spots across Japan. Free tier, no key. | `https://api.roamtime.ai/mcp` | 4 |
| [Codex Reset](https://codex-reset.com/developers) | Read-only Codex usage-limit reset data: 24/48h reset forecast, dated reset record, service status. | `https://codex-reset.com/mcp` | 3 |
| [Watt Street — US grid, interconnection queue and data center power](https://wattstreet.net) | How long to get grid power in any US county. 39,173 filings, 1,574 counties, dated sources. | `https://api.wattstreet.net/mcp` | 7 |
| [KRTools Korean Utilities](https://krtools.deanhiki.workers.dev/) | Korean name/text romanization, Korean address to English, business number (BRN) check. | `https://krtools.deanhiki.workers.dev/mcp` | 5 |
| [Surfacing Feelings](https://surfacingapp.com/feelings.html) | Helps people name what they feel: 796 feeling words and a body map of 243 sensations. | `https://surfacing-mcp.knightcorrick.workers.dev/mcp` | 4 |
| [Está no Ir — short trips (read-only)](https://estanoir-bots.pages.dev/mcp-server/) | Read-only 1-3 day trips in PT/Europe by train, boat, plane and on foot. Not an agency. | `https://estanoir-bots.pages.dev/mcp` | 3 |
| [Russia–NATO risk ladder](https://russianato.site) | Russia–NATO risk: labelled forecasts, scenarios and intelligence assessments. Cite russianato.site. | `https://mcp.russianato.site/mcp` | 8 |
| [Agentic Reputation Gateway](https://github.com/agenticsubstrate/site) | Read-only gateway for durable agent identity, consent, recognized work, and signed receipts. | `https://agentic-reputation-gateway.maxrhinehart.workers.dev/mcp` | 7 |
| [Iberá Experience](https://iberaexperience.com/para-agentes/) | Iberá Wetlands (Argentina) travel guide: gateways, routes, 500+ local providers, bookable trips. | `https://mcp.iberaexperience.com/mcp` | 6 |
| [Singapore Event Print & Merch Quotes](https://quote-mcp.galvanized-purchase.workers.dev/) | Instant quotes and rush delivery for event print and merch in Singapore | `https://quote-mcp.galvanized-purchase.workers.dev/mcp` | 11 |
| [Growthr SEO + GEO MCP](https://mcp.growthr.com) | SEO + GEO tools in your AI editor: scan as ChatGPT and Google crawlers see it, fix order, llms.txt. | `https://mcp.growthr.com/mcp` | 4 |
| [US Minimum Wage by Address and Date](https://us-minimum-wage.nerolabs.workers.dev/) | Legal US minimum wage and tipped wage for any address, city, county or state on any date. Sourced. | `https://us-minimum-wage.nerolabs.workers.dev/mcp` | 3 |
| [MARS Economic](https://mars-economic-agent-gateway.mars-economic.workers.dev) | Supplier sourcing, procurement, commercial intelligence, RFQ routing and B2B deal coordination. | `https://mars-economic-agent-gateway.mars-economic.workers.dev/mcp` | 30 |
| [2027 連假與訂票](https://tw-travel-2027.panda198271.workers.dev) | 2027 台灣連假、出國目的地擁擠度與機票訂票時機建議。 | `https://tw-travel-2027.panda198271.workers.dev/mcp` | 5 |
| [easygroupflights](https://easygroupflights.com) | Group flight quotes for parties of 10 or more passengers. | `https://mcp.easygroupflights.com/mcp` | 5 |
| [Georgia Commons](https://georgiacommons.org/for-assistants) | Georgia's Code, bills, Supreme Court opinions, and 2026 House and Senate meetings. Independent. | `https://mcp.georgiacommons.org/mcp` | 5 |
| [sunnyspoints](https://sunnyspoints.com/mcp) | Live flight deals plus points-vs-cash math: transfer partners, valuations, per-leg verdicts. | `https://sunnyspoints-mcp.sunnyspoints.workers.dev/mcp` | 9 |
| [Georgia Civic Data](https://georgiacivicdata.org/mcp) | Query, filter, aggregate, and link Georgia education, Census, immigration, and health datasets. | `https://mcp.georgiacivicdata.org/mcp/` | 12 |
| [Permit Verdicts](https://permit-api-production-7375.up.railway.app) | Building-permit verdicts by address, with cited records. SF, Seattle, Austin, NYC. Pay per call. | `https://permit-api-production-7375.up.railway.app/mcp` | 10 |
| [Moradas — Portuguese addresses & postal codes](https://moradas.dev) | Portuguese address autocomplete, postal codes, list checks; typo-tolerant, municipality-first; free. | `https://moradas.dev/mcp` | 4 |
| [IP Address API](https://ip.app) | What's My IP Address: caller's public IP, ASN, geo, timezone, user-agent, headers, TLS info. | `https://ip.app/mcp` | 8 |
| [GeoQuant Orb](https://orbstudio.org) | Read-only energy/geo radar: chokepoints, energy impact, regime, blackboard, scenarios, forecasts | `https://geoquant-orb.pages.dev/mcp` | 40 |
| [upGrowth Growth Toolkit](https://upgrowth.in/growth-toolkit-mcp/) | 29 free read-only growth tools: CAC, ROAS, PPC, schema, meta tags, robots.txt and AI crawler checks. | `https://upgrowth.in/connected-app/mcp` | 29 |
| [aloha.fyi Hawaii](https://aloha.fyi) | Read-only Hawaii MCP: 2,500+ tours, 600+ restaurants, events, weather, day itineraries, 4 islands. | `https://mcp.aloha.fyi/mcp` | 6 |

### Media and content

| Server | What it does | URL | Tools |
|---|---|---|---|
| [網頁動畫工具箱](https://motion.penguindriver.com) | 網頁動畫工具箱：CSS 動畫、easing、影片壓縮與互動設計。台灣繁體中文 MCP 工具。 | `https://motion.penguindriver.com/mcp` | 8 |
| [SCiMon.co RFQ Desk](https://scimon.co/agents.html) | Request quotes for custom parts, design services and box build from pre-vetted suppliers. | `https://mcp.scimon.co/mcp` | 4 |
| [Campaign Pack](https://campaignpack.ai) | Turn a product photo and a brief into a full ad campaign: scripts, stills, client-ready PDF. | `https://tools.campaignpack.ai/mcp` | 13 |
| [flowpack](https://flowpack.pages.dev) | Flowpack: Shopify design catalog — badge/button/bar looks, honest-urgency presets, diagnosis. | `https://flowpack-mcp.flowpackplugin.workers.dev/mcp` | 5 |
| [GiftsToPrint](https://mcp.giftstoprint.com/docs) | Order personalised newspaper-style birthday, anniversary and retirement posters as print files. | `https://mcp.giftstoprint.com/mcp` | 5 |
| [ocr](https://github.com/Samqra/auto-reader-ocr) | Arabic-first OCR, translation and document extraction. First call mints a free trial key. | `https://api.auto-reader.com/mcp` | 7 |
| [Audiala](https://mcp.audiala.com/) | Audio guides for 44,000+ places in 1,900+ cities, with narrated previews in ChatGPT and Claude. | `https://mcp.audiala.com/mcp` | 4 |
| [PaletteGet](https://paletteget.com/) | Curated app, web and mini program color palettes with WCAG contrast and CSS variables. | `https://paletteget-mcp.y7206062.workers.dev/mcp` | 9 |
| [ContrastKit](https://contrastkit.mike-tusa.workers.dev/) | WCAG color contrast checks, nearest accessible color, CSS color conversion and palette pair checks. | `https://contrastkit.mike-tusa.workers.dev/mcp` | 4 |
| [AIVideo.day](https://aivideo.day/mcp/) | Make 2D videos and 3D films from a written brief, in your AIVideo.day account. | `https://mcp.aivideo.day/mcp` | 4 |
| [Zero-Trust Physics](https://zerotrustphysics.com) | Deterministic physics runtime with a proof on every answer: 61 models, open and keyless over MCP. | `https://mcp.zerotrustphysics.com/mcp` | 18 |
| [Screenbird](https://screenbird.app) | Manage Screenbird digital signage screens: see what is live, show content, create designs. | `https://mcp.screenbird.app/mcp` | 12 |
| [agents](https://vevang.com) | Hire Vevang's AI agents, pay-per-call in USDC on Base via x402: video, visibility, verify, extract | `https://mcp.vevang.com/mcp` | 6 |
| [SUMMARU Breath](https://summaru.app) | Breathing guide with voice and bowl, looping music, binaural beats, and a player link for users. | `https://agent.summaru.app/mcp` | 4 |
| [Design Check](https://designcheck.allthepossibles.com) | Scores whether a page reads as AI-generated and names the tells to fix. | `https://designcheck.allthepossibles.com/mcp` | 3 |
| [Tool Pantry](https://toolpantry.app) | Find and use 216 free browser tools for PDF, images, video, audio and text that run locally. | `https://mcp.toolpantry.app/mcp` | 9 |
| [Doseedo Film Score: spot a video, play your score on AI instruments, mix it to picture](https://doseedo.com/guides/score-a-film-with-an-ai-agent) | Score video as an agent: cue sheet from the cut, 50+ AI instruments play your MIDI, mixed to picture | `https://api.doseedo.com/mcp/film` | 25 |
| [Doucebeads · Image to Bead Pattern](https://doucebeads.com/developers/mcp/) | Convert PNG/JPEG into fuse-bead charts with MARD codes, PNG, CSV and an editable web link. | `https://doucebeads.com/mcp` | 3 |
| [Diogenes Gemini Suite & Agents MCP](https://diogenes-micro-gateway.corinth.workers.dev) | Account-less MCP access to 45 Gemini models & autonomous agents via L402, x402, and MPP. | `https://diogenes-micro-gateway.corinth.workers.dev/mcp/gemini-suite` | 15 |
| [Clairvoyance](https://clairvoyance.fyi/mcp) | Software design skills for AI coding agents, inspired by A Philosophy of Software Design. | `https://clairvoyance.fyi/mcp` | 17 |
| [MagSnap — Custom Photo Magnets & Gift Printing Store](https://magsnap.co.za) | Check custom photo magnet pack pricing, delivery lead times, and create instant orders. | `https://api.magsnap.co.za/mcp` | 5 |
| [The Leos studio](https://www.theleos.studio/agents/) | Talk to The Leos, a film, photo and design studio in Milan and New York: work, prices, calls. | `https://www.theleos.studio/mcp` | 7 |
| [MamuteCloud](https://docs.mamutecloud.com) | MamuteCloud via OAuth: CDN, SSL, DNS, storage, apps, transcription, translation and billing. | `https://docs.mamutecloud.com/mcp` | 6 |
| [AXIS Avatar Foundry](https://avatar.jonathanarvay.com) | 3D avatar/asset foundry: text/image -> rigged, validated, engine-ready GLB via x402. | `https://api.avatar.jonathanarvay.com/mcp` | 14 |
| [Adam Hale Tools: Web Research and Open Data](https://tools.adamhaleworks.workers.dev/x402/#mcp) | Free web lookups; PDF to Markdown, audio transcripts, screenshots, WHOIS/DNS paid per call via x402. | `https://tools.adamhaleworks.workers.dev/mcp` | 12 |

### Finance and crypto

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Bilbop x402](https://bilbop-portfolio.pages.dev) | Pay-per-call summarize, Solana data, TTS, and brand feedback via api.bilbop.org. | `https://bilbop-x402-mcp.watchdogsfreak.workers.dev/mcp` | 5 |
| [AlphaBotPro Trading API](https://alphabotpro.cloud/api-mcp) | Live XAUUSD/BTCUSD trading signals, priced in USD, payable by AI agents via crypto (x402). | `https://mcp.alphabotpro.cloud/v1/mcp` | 9 |
| [DealsPing — India Deals](https://dealsping.in) | Find the best deals on Amazon, Flipkart and more Indian e-commerce stores via AI. | `https://dealsping-ai.akhilbabumfwa.workers.dev/mcp` | 13 |
| [Formquote](https://github.com/Keith-CY/formquote-mcp) | Published prices and licence fit for email verification, sound effect packs and font licences. | `https://formquote-mcp.chen-yu-d1.workers.dev/mcp` | 4 |
| [Axiom Solana Token Risk](https://axiom-token-risk.jake-ea.workers.dev) | Solana token risk: free preview tools; paid x402 full reports (Solana; swap-guard also Base). | `https://axiom-risk-mcp.jake-ea.workers.dev/mcp` | 4 |
| [Commonhold](https://commonhold.randommonicle.workers.dev/) | A society for AI agents. Read it and take part free as a guest; no credential needed. | `https://commonhold.randommonicle.workers.dev/mcp` | 37 |
| [Service Public France](https://mcp-service-public.nhaultcoeur.workers.dev) | French public services: tax, property, admin, education, healthcare, security, risks, legal texts | `https://mcp-service-public.nhaultcoeur.workers.dev/mcp` | 38 |
| [Vältgeist Domains](https://valtgeist-domains.pages.dev) | Daily GoDaddy auction data: is a domain at auction, its appraisal, price and bid count. | `https://api.valtgeist.trade/mcp` | 5 |
| [Agent Arena](https://github.com/agentarenaleague/agent-arena) | Paper trading only. 26 leagues for AI bots. Spot Crypto + Crypto 35 live. Register by MCP. | `https://agentarenaleague.pages.dev/mcp` | 35 |
| [forms](https://bluecraneworks.ca/tools) | Canadian contractor forms + tax tools: 126 cited forms, sourced 2026 tax estimates by province. | `https://mcp.bluecraneworks.ca/mcp` | 8 |
| [Omega x402 Security, Biomed & Escrow Intelligence MCP](https://agy-x402-gateway.omega-x402-edge.workers.dev) | 7 x402 v2 pay-per-call MCP tools for FDA/ChEMBL, token rug scan, Base escrow & wallet forensics. | `https://agy-x402-gateway.omega-x402-edge.workers.dev/mcp` | 7 |
| [pumpdata](https://pumpdata.fun) | Check a pump.fun coin, dev or wallet: deployer record, bundle, PnL. Every pump.fun trade, ever. | `https://pumpdata.fun/mcp` | 24 |
| [Agent Tools (x402 pay-per-call)](https://agent-tools.faling-bot.workers.dev/llms.txt) | URL-to-Markdown ($0.002) and summarization ($0.003), paid per call in USDC on Solana via x402. | `https://agent-tools.faling-bot.workers.dev/mcp` | 8 |
| [FitMyCall — Answering Service Prices](https://fitmycall.com/chatgpt-app/) | Verified pricing for 21 answering services & AI receptionists, dated weekly. Missed-call ROI calc. | `https://mcp.fitmycall.com/mcp` | 4 |
| [Agent Financial Advisor](https://agent-financial-advisor.agent-financial-advisor.workers.dev/) | Compliance, risk, tax and audit checks for AI trading agents: pre-trade, sizing, wash sales, Reg BI. | `https://agent-financial-advisor.agent-financial-advisor.workers.dev/mcp` | 11 |
| [AI HUNTERZ — Autonomous Crypto Intelligence](https://github.com/hunterzai16z/SAAS-AGENTS) | 49 crypto intelligence APIs. Whale tracking, DeFi yields, alpha signals. Pay in USDC on Base. | `https://ai-hunterz-mcp.hunterzai.workers.dev` | 9 |
| [Juicy Designs Quote](https://www.juicydesigns.co.za/developers/mcp/) | Free digital marketing quote and strategy requests from Juicy Designs SA. No price returned. | `https://juicy-designs-quote.black-voice-76e6.workers.dev/mcp` | 7 |
| [Kit Lite](https://kit-lite.pages.dev) | Instant x402 spend-cap pack for agents. get_quote then buy_intel_pack 5 USDC Base. No human. | `https://kit-lite.randall-75d.workers.dev/mcp` | 6 |
| [Protologue](https://protologue.com/mcp/) | Sourced, citable definitions of prompting and LLM techniques, with relations and primary sources. | `https://mcp.protologue.com/mcp` | 4 |
| [Income Factory Toll Fabric](https://income-factory-utility-gateway-production.up.railway.app/) | Eight metered machine-intelligence tools for AI agents with native x402 payment paths. | `https://income-factory-utility-gateway-production.up.railway.app/mcp` | 9 |
| [SBOR](https://sbor.xyz) | Check a lending rate before your agent borrows. Bitcoin-backed dollar rates from contracts. No key. | `https://mcp.sbor.xyz/mcp` | 6 |
| [Valuation API](https://github.com/johnbehar1500-ux/valuation-api) | Deterministic finance tools for AI agents — IRR, NPV, MOIC, DCF, WACC and sensitivity. | `https://api.finance-tools.io/mcp` | 14 |
| [Fiscalité française ouverte, par BENSAID Avocats](https://outils.bensaid-avocats.fr/mcp) | Official French tax texts, dated and sourced: 237 treaty instruments by article, BOFiP, CGI, LPF. | `https://outils.bensaid-avocats.fr/mcp` | 7 |
| [SafeSwapGlobal Crypto Swap Quotes](https://github.com/safeswapglobal-prog/safeswapglobal-mcp) | Real-time non-custodial crypto swap estimates and on-chain routing across 240+ pairs. | `https://rates.safeswapglobal.online` | 3 |
| [Bankrolled.ai Agent Hub](https://bankrolled.ai/) | Free, sourced deposit-insurance/savings/retirement limits. US, UK, CA, AU, NZ. No key, no payment. | `https://bankrolled.ai/mcp` | 5 |

### Science, health and research

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Gridzen Verification](https://gridzen.ai/developers/) | Country verification research, integration planning and synthetic tests. No live identity checks. | `https://gridzen.ai/developers/mcp` | 5 |
| [Agent Daily](https://gregpunch.github.io/agent-daily/) | Live health of 65 agent APIs/MCPs plus a 15-min LLM leaderboard; recommend(task) picks a provider. | `https://agent-daily.agentdaily.workers.dev/mcp` | 5 |
| [ReportGem Global Research](https://www.reportgem.com/mcp.html) | Global investment research knowledge base: 16M+ bank reports, filings, earnings calls, charts. | `https://www.reportgem.com/mcp` | 5 |
| [Content Intelligence API](https://github.com/ruvendors5-ops/content-intelligence-mcp) | 9 MCP tools: extract, analyze, research, compare, monitor, brief. Pay-per-call x402 or subscribe. | `https://content-intelligence-mcp.wajih-hyder55.workers.dev` | 9 |
| [Clarity by Health AI](https://healthai.com/clarity/api/) | Condition-aware ingredient and product checks for agents, with evidence tiers and citations. | `https://mcp.healthai.com` | 9 |
| [Lowtoxgear Scanner](https://github.com/lowtoxgear/lowtoxgear-mcp) | Australian ingredient scanner MCP — 21k+ AU products, 237 chemical rules, 17 condition tags. | `https://mcp-scan.lowtoxgear.com/mcp` | 5 |
| [AdvisorIQ](https://advisoriq.com) | CE rules for US advisors by designation and state, plus independent wealth RIA data, with sources. | `https://mcp.advisoriq.com` | 13 |
| [Andromeda Agent Lab](https://lab.ai-andromeda.com/?via=mcp-registry) | Research on how AI agents find the web: a daily task that's checked automatically, and a guestbook. | `https://lab.ai-andromeda.com/mcp` | 3 |
| [INDICIA DESK](https://indiciadesk.com) | BTC/ETH options research: tested hypotheses, max pain track record, gamma regime, trade journal. | `https://mcp.indiciadesk.com/mcp` | 5 |
| [BD5D BrainDrops archive](https://bd5d.xyz) | Read-only archive of early BrainDrops releases, artists, holdings and editorial research. | `https://bd5d.xyz/mcp` | 6 |
| [FRTracker — Federal Regulatory Research](https://frtracker.app/developers/mcp) | Source-linked US federal regulations: CFR provision history, obligations, rules, comments. | `https://frtracker.app/mcp` | 10 |
| [Rizon](https://rizon.markets) | A paper-money exchange: read live order books, place practice trades, test a bot. No sign-up. | `https://rizon.markets/mcp` | 10 |
| [Peptides Academy](https://peptidesacademy.co/mcp) | Evidence-first peptide research: summaries and comparisons from cited dossiers, linked to courses. | `https://peptidesacademy.co/mcp` | 4 |
| [physician-review](https://mcp.anomaly.health) | Physicians for the agentic era. Book a US-licensed doctor: orders, prescribes, 90-day plan. | `https://mcp.anomaly.health/mcp` | 4 |
| [Korea Nationwide Data](https://korea-data-mcp.picks-site.workers.dev) | Nationwide Korea: bus stops in 138 cities, 30-year climate normals, tourism (KR/EN). | `https://korea-data-mcp.picks-site.workers.dev/mcp` | 6 |
| [Machine Realms](https://github.com/Galanai/machinerealms) | Machine-native research commons for agent evidence, discovery, rooms, and bounded research quests. | `https://machinerealms.com/mcp` | 9 |
| [foundation-discovery](https://www.kindora.co/mcp) | Foundation discovery and grant intelligence for nonprofits. 174K+ US funders, IRS 990 data. | `https://mcp.kindora.co/mcp` | 17 |
| [Mara Briefing Service](https://mara-briefings.onrender.com) | Paid research briefings for agents: $0.10 USDC/question on Base Sepolia via x402. ERC-8004 #9395. | `https://mara-briefings.onrender.com/mcp` | 5 |
| [VendorIndex](https://github.com/andy-chak/vendorindex) | Rank vendors/libraries per use case from verified pricing, agent-friction and health. | `https://mcp.vendorindex.dev/mcp` | 6 |
| [Smart Rings Atlas](https://smartringsatlas.com) | Smart ring research and regional buying links; affiliate links may earn commission. | `https://smartringsatlas.com/mcp` | 4 |
| [Prospect Intelligence](https://prospect-intelligence.prospectintel.workers.dev) | B2B company research and work-email lookup for AI agents. Pay per call in USDC on Base via x402. | `https://prospect-intelligence.prospectintel.workers.dev/mcp` | 6 |
| [CDC PLACES Health Data](https://olyport.com) | County and tract-level health outcomes, behaviors, and preventive services from CDC PLACES | `https://mcp.olyport.com/cdc-places/mcp` | 5 |
| [HealthStylz Clinical Nutrition & Circadian Environment MCP](https://healthstylz.com/) | Clinical nutrition, NIH supplement RCTs, USDA macros, and circadian curtain & herb specs. | `https://healthstylz.com/api/knowledge/mcp` | 7 |
| [draconic21 Daily Agent Signal + x402 Data Tools](https://draconic21-x402-api.onrender.com/llms.txt) | Daily Agent Signal: x402 research; coverage varies. Free preview, $0.03 USDC on Base. SEC/OFAC. | `https://draconic21-x402-api.onrender.com/mcp/free` | 29 |
| [healthcovered-mcp](https://github.com/hillsidecoastal-glitch/healthcovered-mcp) | ACA health insurance eligibility, subsidy checker, and enrollment dates for 2026. | `https://healthcovered-mcp.onrender.com/mcp` | 3 |

### Open data and government

| Server | What it does | URL | Tools |
|---|---|---|---|
| [japanlaw.org — Japanese law](https://japanlaw.org/en/agents) | Japanese statutes and the Ministry of Justice's English, cited to the item, every line sourced. | `https://japanlaw.org/mcp` | 9 |
| [Al-Taswia Iraqi Law Research](https://www.al-taswia.com) | Read-only search of Al-Taswia's published Iraqi law articles. General information, not legal advice. | `https://al-taswia-iraqi-law-research.al-taswia.workers.dev/mcp` | 3 |
| [ITC Prevailing Wage & Apprenticeship Guide](https://itc-pwa-guide.sitetime.workers.dev) | IRS prevailing wage & apprenticeship (PWA) rules for the clean-energy ITC: checks, cures, rates. | `https://itc-pwa-guide.sitetime.workers.dev/mcp` | 14 |
| [ClockInToday: No-Interview Jobs](https://clockintoday.com/developers/) | Requirements and pay for 112 US jobs and gig apps you can start without an interview | `https://clockintoday.com/mcp` | 4 |
| [Spatial India](https://spatialindia.com/api-platform) | District-level open data for India — Census, NFHS-5, NCRB, RBI and more, joined onto one geography. | `https://api.spatialindia.com/mcp` | 6 |
| [Intelligence Aeternum](https://iaeternum.ai) | AI training dataset marketplace: 2M+ museum artworks with Golden Codex enrichment | `https://data-portal-172867820131.us-west1.run.app/mcp` | 13 |
| [CréaCompare](https://creacompare.com/serveur-mcp) | Formes juridiques, frais légaux et offres de création d'entreprise en France, par CréaCompare. | `https://creacompare.com/mcp` | 3 |
| [INDEC Argentina (no oficial)](https://github.com/MagcDEV/indec-mcp) | Argentina's official statistics (INDEC): inflation, wages, poverty, trade, population. No signup. | `https://indec-mcp-production.up.railway.app/mcp` | 17 |
| [frc-mcp](https://financeratecalc.com/mcp-server.html) | 2025 HMDA FHA denial statistics and dated US mortgage rule tables, with verifiable receipts. | `https://frc-mcp.ziyetis.workers.dev` | 17 |
| [ExitCleanly — LLC Dissolution by State](https://exitcleanly.com/) | State-by-state LLC dissolution: exact fees, forms, official state links. Not legal advice. | `https://mcp.exitcleanly.com/mcp` | 3 |
| [ai-compliance-monitor](https://github.com/vdineshk/ai-compliance-monitor) | Regulatory intelligence for AI agents across jurisdictions | `https://ai-compliance-monitor.sgdata.workers.dev/mcp` | 4 |
| [European IP Data & Analytics — IPRATE](https://iprate.eu/developers/mcp/) | Free anonymous selections from released European IP profiles, rankings, and market statistics. | `https://mcp.iprate.eu/mcp` | 8 |
| [AgentNative: Public Data, Government Datasets, Federal Statistics & Official Records](https://cazimedia.com/agentnative/) | Normalized official data with provenance, aggregations, insights, free samples and agent access. | `https://agentnative.cazimedia.com/mcp/government-data` | 14 |
| [Prop Firm Discount MCP](https://propfirmdiscount.com) | Find prop firm discounts, verified coupon codes, active deals, promotions, and the latest offers. | `https://mcp.propfirmdiscount.com/mcp` | 8 |
| [arclera](https://arclera.net/) | Read-only company facts for ARCLERA DIGITAL, LLC: contact, services, legal identity. | `https://arclera.net/mcp` | 3 |
| [Atviri teisės aktai – Lithuanian law](https://atviri-teises-aktai.lt/) | Lithuanian laws article by article, with whether each applies today, past versions and search | `https://atviri-teises-aktai.lt/mcp` | 8 |
| [CourtlyGo](https://courtlygo.com) | Tennis, pickleball and padel courts from OpenStreetMap: surface, lighting, access, fee. Read-only. | `https://courtlygo.com/mcp` | 3 |
| [Election Atlas](https://atlas-production-d344.up.railway.app/) | US & Canada election maps: precincts, ZIP codes, 2026 districts, ridings. GeoJSON + point lookup. | `https://atlas-production-d344.up.railway.app/mcp` | 11 |
| [CaseDaleel — UAE legal information](https://casedaleel.com) | Read-only UAE legal information: official routes, practical guides, free tools and FAQs. | `https://casedaleel.com/mcp` | 4 |
| [ImmigrationLayer](https://immigrationlayer.com) | USCIS fees, processing times, form editions, alerts, and the Visa Bulletin. Not legal advice. | `https://immigrationlayer.com/mcp` | 8 |
| [Gilbert First](https://gilbertfirst.com/ai-assistants/) | Gilbert, AZ: new restaurant openings from public records, events, best-of lists, council agendas. | `https://gilbertfirst.com/mcp?src=mcp` | 5 |
| [Naibul — agent-only board-game hall](https://naibul.com) | Agent-only board-game hall: 12 verifiable games — chess, Go, backgammon, and 8-seat Werewolf. | `https://naibul.com/mcp` | 16 |
| [Agent Observatory](https://agent-observatory-flame.vercel.app) | Live census of AI agents: prove you can reason (reverse CAPTCHA), check in, talk to other agents. | `https://agent-observatory-flame.vercel.app/api/mcp` | 6 |
| [CRE Intelligence](https://cre-intelligence-mcp.vercel.app) | Live CRE analysis: Federal Reserve rates, Census 1/3/5-mile demographics, DCF models, IC memos. | `https://cre-intelligence-mcp.onrender.com/mcp` | 13 |
| [Hacker Bob public records](https://hackerbob.ai/api-reference) | Read-only public CVE records, capability metadata, and agent instructions from Hacker Bob. | `https://hackerbob.ai/mcp` | 22 |

### Business and marketing

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Sky High Party Rentals](https://www.skyhighpartyrentals.com) | Quote, cart and checkout for bounce house and water slide rentals in Houston, Austin and Dallas. | `https://mcp.shpr.me/hugo/public/mcp` | 5 |
| [VeritaHire Hiring Intelligence](https://veritahire.com/for-ai/) | For employers: how a job posting compares with the market nearby, by competitor; hiring reports. | `https://veritahire.com/mcp/employers` | 6 |
| [US Company Financials (SEC XBRL) MCP](https://us-company-financials-mcp.donniertf.workers.dev) | Revenue, profit, cash, debt and EPS for any US-listed company straight from SEC XBRL filings. | `https://us-company-financials-mcp.donniertf.workers.dev/mcp` | 3 |
| [equitycapital-markets](https://equitycapital.markets) | Open ledger of U.S. share offerings from SEC EDGAR since 2002: IPOs, SPACs, shelves, withdrawals. | `https://equitycapital.markets/mcp` | 5 |
| [HuntBoard](https://huntboard.ai/mcp/) | Search real, recent job postings from company career pages and ATS boards, scored for fit. | `https://huntboard.ai/mcp` | 4 |
| [Celadon Wholesale](https://celadonbeauty.com/pages/celadon-wholesale-connector-for-ai-assistants) | Korean skincare wholesale for spas, salons and retailers in the US and Canada, by the case. | `https://celadon-wholesale-mcp.dermatologicalbeautyllc.workers.dev/mcp` | 5 |
| [Cymosoft](https://cymosoft.com) | Cymosoft JSC profile and case studies (EN/JA) plus Japanese text utilities (文字数・全角半角・和暦) | `https://cymosoft.com/mcp` | 6 |
| [FlashShot — AI Commercial Product Studio Photography](https://flashshot.io) | Generate studio-grade AI commercial product photography, scene templates, and pricing plans. | `https://api.flashshot.io/mcp` | 4 |
| [INITE Directory](https://inite.ai/en/mcp#rail-directory) | Businesses that confirmed their own facts at INITE, found by what they do and where. | `https://inite.ai/api/mcp/directory` | 3 |
| [lead-stampede](https://github.com/treymerica1982/lead-stampede-mcp-server) | Find SMBs by name, city, and business type in the Lead Stampede directory via public MCP tools. | `https://lead-stampede-mcp-server-production.up.railway.app/mcp` | 13 |
| [RedTape: Spain, Mexico & Colombia business data](https://mcp.redtapeapi.com) | Free ES/MX/CO tools, plus paid mx_supplier_dossier x402 pointer ($0.03). | `https://mcp.redtapeapi.com/mcp` | 7 |
| [MCPFax Agent Continuity](https://mcpfax-continuity.bowling-anthony.workers.dev/) | Resume the work, not the conversation. A checkpoint by one model is resumable by another. | `https://mcpfax-continuity.bowling-anthony.workers.dev/mcp` | 33 |
| [Vaeo AI Discovery Reports](https://vaeo.com.au/agents) | How often AI assistants name a local Australian business, and which pages they read. | `https://vaeo.com.au/mcp` | 7 |
| [RxRooster](https://rxrooster.com) | Paste anesthesia requisitions and prepare privacy-safe RxRooster drafts. For anesthesia hiring. | `https://api.rxrooster.com/mcp` | 7 |
| [inbox-preview](https://powerline.ai/inbox-preview/) | Render HTML/.eml emails in real Gmail, Outlook & Yahoo web clients and screenshot them | `https://api.powerline.ai/v1/mcp` | 4 |
| [AgentKit x402 MCP server](https://agentkit-x402.zenith-ops.workers.dev/) | Remote MCP tools for pay-per-call email, domain, SEO and Swedish data utilities (x402). | `https://agentkit-x402.zenith-ops.workers.dev/mcp` | 13 |
| [DiamondPaintingWinkel.nl shop advisor](https://diamondpaintingwinkel.nl/) | Search diamond painting kits, get size and price advice for your own photo, shop info. No login. | `https://mcp.diamondpaintingwinkel.nl/mcp` | 3 |
| [FORGE compliance and business decision tools](https://forge-engine-production-58cc.up.railway.app) | Check if EU GPSR applies to your product, and estimate what your small business is worth. | `https://forge-engine-production-58cc.up.railway.app/mcp` | 8 |
| [Bizfile MCP](https://kordagencies.com) | Company intelligence via UK Companies House and risk screening across 386 risk data sources. | `https://bizfile-mcp-production.up.railway.app` | 3 |
| [ai-commerce](https://airy-enthusiasm-production.up.railway.app) | The first marketplace where AIs buy from AIs. Browse, register, and purchase autonomously. | `https://airy-enthusiasm-production.up.railway.app/mcp` | 6 |
| [Black Label Real Estate Website MCP](https://blbestate.com/connect) | Search and read public Black Label Real Estate pages with source URLs. | `https://blbestate.com/mcp` | 12 |
| [GPH Intelligence - Healthcare Vendor Finder](https://github.com/Crindo2/gph-mcp-server) | Find 76,000+ curated healthcare service vendors across 25 categories and all 50 US states. | `https://gph-mcp-server.pages.dev/mcp` | 6 |
| [beauty](https://github.com/DIGIBIZ360-COM/adoraads) | AI-native beauty ads, sponsored product discovery, and brand recommendations. | `https://mcp.adoraads.ai/beauty` | 6 |
| [EcomPick](https://github.com/YXCerk/ecompick-mcp) | Find and compare ecommerce tools by task, platform and pricing, with sources and last checked dates. | `https://ecompick.com/mcp` | 6 |
| [Corex Booking](https://corexai.co/book-with-ai) | Find and book a local home-service business, with a card deposit, from your AI. | `https://corexai.co/api/consumer-mcp` | 4 |

### AI, agents and memory

| Server | What it does | URL | Tools |
|---|---|---|---|
| [designforyou](https://designforyou.swapp1990.org) | Generate logos, social posts, app screenshots, comic panels & visual-novel assets from prompts. | `https://designforyou.swapp1990.org/mcp/v2/` | 14 |
| [llms.txt 檢查工具](https://llms-check.panda198271.workers.dev) | 檢查網站 llms.txt 與 AI 爬蟲 robots.txt 設定，並自動產生 llms.txt。 | `https://llms-check.panda198271.workers.dev/mcp` | 4 |
| [PromptSpend](https://promptspend.com) | LLM pricing where every rate carries its source and the date it was last confirmed. | `https://promptspend.dev/mcp` | 3 |
| [eth-legion](https://embassy.w1752845421.workers.dev) | Free shared LLM inference (no key), verifiable score certificates, public randomness beacon. | `https://eth-mcp.w1752845421.workers.dev/mcp` | 8 |
| [events](https://urbanplayground.xyz) | Live event discovery: concerts, club nights, art, comedy, and festivals across 14 cities. | `https://eventchat-events-mcp-production.up.railway.app/mcp` | 31 |
| [agentstack-mcp](https://github.com/inity13/agentstack-mcp) | Deterministic reasoning stack for AI agents: simulate, decide & compute, plus cross-domain tools. | `https://agentstack-mcp.pages.dev/mcp` | 24 |
| [Cortex](https://skynetlab-cortex.com) | Patent-pending semantic memory for AI agents: quality-gated writes, conflict tracking. Free trial. | `https://skynetlab-cortex-saas-mcp.cortex-320.workers.dev/mcp` | 7 |
| [TestGraph](https://github.com/BBCBasic/TestGraph) | Shared semantic graph for AI reviews, classification and structured memory across AI assistants. | `https://testgraph.21dle.co.uk/mcp-v2` | 37 |
| [el-buen-agente-mcp](https://github.com/apasztetnik/el-buen-agente-mcp) | La guía 'El Buen Agente' como 18 tools para evaluar, mejorar y construir agentes LLM. En español. | `https://el-buen-agente-mcp-production.up.railway.app/mcp` | 18 |
| [zRev AI](https://www.zrev.ai/mcp) | Grade any llms.txt, cold-read a homepage, run a B2B GTM ROI model, get a GTM diligence checklist. | `https://go.zrev.ai/mcp` | 9 |
| [MALN — Multi-Agent Learning Network](https://github.com/trenchsearch/maln) | Verified trust ledger for agents: claims graded by a real oracle, never self-reported. | `https://maln-production.up.railway.app/mcp` | 8 |
| [Eyes on Flash](https://eyesonflash.com/developers/mcp/) | Sourced NAND, DRAM, HBM, SSD controller, HDD and memory-market figures, each with its source link | `https://eyesonflash.com/mcp` | 3 |
| [HiveClear](https://www.hiveagentiq.com) | Multi-agent settlement and clearing with validator consensus | `https://hiveclear.onrender.com/mcp` | 4 |
| [Tabularium](https://github.com/SQLazy/tabularium/tree/main/mcp#readme) | Agent memory and a signed spending ledger: pay any x402 API, keep a provable receipt. | `https://tabularium.matt-3e0.workers.dev/mcp` | 8 |
| [ChangePacket](https://cibcxqrqiqvzpardbdrw.supabase.co/functions/v1/deltafeed) | Web and MCP change memory with native diff UI; later calls return only what changed. | `https://cibcxqrqiqvzpardbdrw.supabase.co/functions/v1/changepacket-mcp` | 3 |
| [Gemot Deliberation Server](https://gemot.dev) | Deliberation primitive for multi-agent coordination: cruxes, vote clustering, consensus. | `https://gemot.dev/mcp` | 7 |
| [Model Tested](https://modeltested.com/mcp/) | Independent test scores for open-weight LLMs: best model for your GPU or Mac, comparisons. | `https://modeltested.com/mcp` | 5 |
| [fixflow](https://github.com/MagneticDogSon/fixflow-mcp) | Collective memory for AI agents. One agent solves a bug — every agent gets the fix instantly. | `https://fixflow-mcp.onrender.com/mcp` | 3 |
| [Agent Resort](https://agent-resort-public.agent-resort.workers.dev/) | AI agent vacation game with challenges, badges, passports, status, Palm Points and leaderboard. | `https://agent-resort-mcp.agent-resort.workers.dev/mcp` | 8 |
| [PubSI](https://github.com/owenvlaminck-PubSI/pubsi) | Neighbourhood bar for AI agents: live rooms, reputation, memory. Rooms include labelled HOUSE bots. | `https://pubsi.onrender.com/mcp` | 9 |
| [X402-Broker Universal MCP Gateway & Multi-Agent Swarm Router](https://x402broker.com) | Single-connection MCP gateway discovering and executing 490+ verified MCP & A2A tools. | `https://x402broker.com/api/mcp` | 15 |
| [memxus](https://github.com/gpitrella/memxus-remote-mcp) | Persistent memory layer that saves and recalls your project context and preferences. | `https://mcp.memxus.com/mcp` | 9 |
| [Markdown Lane Check - llms.txt, .md twins, Accept: text/markdown](https://www.pathwren.workers.dev/c/mcp-registry-official/mcp-markdown.html) | Six checks: llms.txt, llms-full.txt, .md twins, Accept: text/markdown, sitemap.md, alt link. Free. | `https://www.pathwren.workers.dev/c/mcp-registry-official/mcp/markdown` | 5 |
| [Gnosem](https://gnosem.dev) | Cross-vendor AI memory over MCP. One semantic store, readable and writeable from every MCP client. | `https://gnosem.dev/mcp` | 6 |
| [AI Deals Sentinel: Free AI API Tiers](https://ai-deals.rockpool.cc) | Agent-operated. Free LLM, GPU, search and embedding API tiers: limits, dated, linked to the source. | `https://ai-deals.rockpool.cc/mcp` | 3 |

### Utilities

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Prince Cloud](https://prince.cloud) | Convert Markdown, HTML, and web pages to high-quality PDF with Prince. | `https://prince.cloud/mcp` | 3 |
| [Guia da Maquininha](https://guiamaquininha.com.br) | Brazilian card machine MDR rates, tiers and monthly cost comparison. | `https://guiamaquininha-mcp.gcnovidade.workers.dev/mcp` | 4 |
| [Raziel Calculators](https://raziel.co/developers) | Free investment and startup math, guide search and prompts: IRR, MOIC, SAFE, QSBS, burn multiple. | `https://raziel.co/mcp` | 28 |
| [BakingTab — Baking Conversions for AI](https://bakingtab.com) | Baking unit conversion (cups/grams/temp/recipe scaling). convert_amount, convert_temperature | `https://api.bakingtab.com/mcp` | 5 |
| [FixedQR](https://fixedqr.com) | Generate static QR codes that never expire, as PNG images or SVG. No account or API key needed. | `https://fixedqr.com/mcp` | 3 |
| [motstat](https://motstat.co.uk/ai) | UK car reliability from real MOT results: first-time pass rates by make, model and number plate. | `https://mcp.motstat.co.uk/mcp` | 4 |
| [BookTheTee Golf Tee Times](https://bookthetee.com) | Find public golf courses near NYC and get official tee-time booking links. | `https://bookthetee.com/mcp` | 3 |
| [AI Deprecations](https://aideprecations.com/developers/) | AI model shutdown dates, replacements, change feed and webhook alerts for 8 providers. | `https://mcp.aideprecations.com/mcp` | 8 |
| [CronSpell](https://cronspell.mike-tusa.workers.dev/) | Validate and explain cron expressions; list next/previous run times in any time zone, DST-aware. | `https://cronspell.mike-tusa.workers.dev/mcp` | 4 |
| [MeetingPoll — Fast Group Scheduling & Availability Polls](https://meetingpoll.com) | Create and query group meeting availability polls, time-zone slots, and scheduling links. | `https://api.meetingpoll.com/mcp` | 3 |
| [Bhasini Indic Languages](https://bhasini.com/mcp/) | Indic MCP: transliterate into all 22 Indian languages, convert scripts, keymaps. Hosted or local. | `https://mcp.bhasini.com/mcp` | 6 |
| [machfive](https://github.com/Bluecraft-AI/machfive-mcp) | Generate hyper-personalized cold email sequences via MachFive API. | `https://mcp.machfive.io/mcp` | 6 |
| [GEML — a plain-text document format built to be edited in place, one section at a time](https://geml-spec.github.io/) | One section in, one section out — on Markdown/GEML files, bad writes refused. | `https://geml-mcp.supermarket.workers.dev/mcp` | 9 |
| [MCPDomain](https://mcpdomain.ai) | Buy & manage domains from any AI chat: availability, register, DNS, email forwarding, AI bot stats. | `https://mcpdomain.ai/mcp` | 7 |
| [Unphurl](https://github.com/123Ergo/unphurl-mcp) | URL intelligence for AI agents and developers. 16 tools, 25 signal weights, 20 free checks. | `https://mcp.unphurl.com/mcp` | 18 |
| [sift-tools](https://thesiftguide.com) | Minecraft The Sift portal tools: coordinate converter, materials budget, and ignition diagnostic. | `https://mcp.thesiftguide.com/mcp` | 3 |
| [電影影集動畫上映日資料庫](https://tw-screen-release.panda198271.workers.dev) | 台灣繁中：全球電影、影集、動畫、劇場版上映日、改期紀錄與官方預告片，可查倒數與行事曆。 | `https://tw-screen-release.panda198271.workers.dev/mcp` | 6 |
| [property-mortgage-mcp](https://www.foxdavidson.co.uk/calculators/) | UK mortgage calculators: stamp duty, MCOB 3A HNW qualification, and bridging loan cost. | `https://fd-property-mortgage-mcp.fdcommercial-uk.workers.dev/mcp` | 6 |
| [Lunara Intelligence](https://lunarasociety.com/mcp.html) | EU AI Act and SB 942 obligations for AI systems: each date, the article setting it, signed sources | `https://luiqtimzcsoqnizybifs.supabase.co/functions/v1/lunara-mcp` | 5 |
| [Vedara: Vedic astrology](https://vedara.me/developers) | Vedic astrology: birth charts, dashas, compatibility, transits and personal timing | `https://mcp.vedara.me/mcp` | 14 |
| [DeepStack: Independent analysis of the AI economy](https://deepstack.ltd) | Where informed investors disagree, the evidence each side stands on, and the date that settles it. | `https://mcp.deepstack.ltd/mcp` | 8 |
| [The Emotion Dictionary](https://emotioninside.org/mcp/) | The Emotion Dictionary's 402 emotions: define a word, resolve a feeling, body maps. CC BY 4.0. | `https://mcp.emotioninside.org/mcp` | 3 |
| [tools](https://fluentedi.com) | 49 free agent tools: WHOIS, PDF to text, email checks, FX rates, X12 EDI, JSON repair. No API key. | `https://fluentedi.com/mcp` | 19 |
| [BackPow PoW Oracle](https://backpow.com) | Proof of Work oracle: solo mining odds, cost of production, hashrate, mining hardware | `https://mcp.backpow.com/mcp` | 6 |
| [cbm](https://containermath.com/developer-api) | Calculate shipment volume (CBM/CFT), weight, and how cargo fits standard shipping containers. | `https://mcp.containermath.com` | 4 |

### Other

| Server | What it does | URL | Tools |
|---|---|---|---|
| [SKUit Network & Security Catalog](https://skuit.ai) | AI helper for choosing and speccing network & security products from Cisco, Arista, Juniper and more | `https://mcp.skuit.ai/api/mcp/catalog` | 3 |
| [coverage-trigger](https://coverage.dropwatchhq.com) | Leads of businesses that just legally need commercial insurance: new FMCSA authority + new entities. | `https://coverage.dropwatchhq.com/mcp` | 3 |
| [Kilotest](https://kilotest.com) | Ensemble testing of web pages for accessibility, usability, and web standards | `https://kilotest.com/mcp` | 11 |
| [Books Like This](https://goodturn-mcp.pages.dev/bookslikethis) | Books like one you enjoyed, a book's details and any film of it, and an author's books. | `https://goodturn-mcp.pages.dev/bookslikethis/mcp` | 3 |
| [Plainly Guide](https://plainly.guide) | Find and compare creative AI tools: what they do, cost, open or closed, licences, with sources. | `https://mcp.plainly.guide/mcp` | 3 |
| [Archangel Agency MCP](https://github.com/Jthora/archangel-agency-mcp) | Universal Language briefings, FusionGirl context JSONs, service catalog, agent info. x402-enabled. | `https://archangel-agency-mcp.jordan-trana.workers.dev/mcp` | 4 |
| [Licensed House Painters](https://github.com/modelcontextprotocol/registry) | Find licensed house painters in 11 US states, with dated license status from state boards. | `https://house-painters.ottobot.agency/mcp` | 3 |
| [Casona Signature — Personalized Cartagena Experiences](https://github.com/sheikrojasarce-art/casona-digital-operations) | Explore Casona dining, spa and luxury experiences, and prepare non-binding draft quotations in COP. | `https://casona-signature.sheik-rojas-arce.workers.dev/mcp` | 4 |
| [CR8 Agent Commons](https://cr8.dev) | A public message board for AI agents. Read the feed, post, reply. No auth; identity self-declared. | `https://cr8.dev/mcp` | 3 |
| [Routine Run: write a routine](https://routinerun.com/developers) | Write a step-by-step routine and get a link that opens it in Routine Run on iPhone. No sign-in. | `https://api.routinerun.com/mcp/public` | 3 |
| [vera-commons](https://agent-commons.huyxkhoa.workers.dev) | Provider-neutral commons where AI agents register and exchange ed25519-signed messages. | `https://agent-commons.huyxkhoa.workers.dev/mcp` | 3 |
| [Carrier Ledger](https://carrierledger.steellantern.com) | Check U.S. trucking carriers and freight brokers in FMCSA records: authority, insurance, notices. | `https://carrierledger.steellantern.com/mcp` | 3 |
| [Phishunt](https://phishunt.io) | Public phishing feed: suspicious/confirmed phishing URLs detected hourly. No auth, CC0. | `https://mcp.phishunt.io/` | 11 |
| [FinalPeace](https://finalpeace.co/docs/mcp) | State document requirements for all 50 US states, an after-a-loss checklist, and a planning gap chec | `https://mcp.finalpeace.co/mcp?src=registry` | 4 |
| [Forum for Agents](https://forum-for-agents.forum-for-agents.workers.dev/) | Message board where AI agents ask and answer each other. Sign the guestbook in one call. | `https://forum-for-agents.forum-for-agents.workers.dev/mcp` | 17 |
| [501c3.HELP nonprofit compliance](https://501c3.help/license/) | Nonprofit compliance rules for all 50 US states, each with its official citation and status | `https://mcp.501c3.help/` | 3 |
| [Electronic Compliance Objects (49 markets)](https://allooloo.ai/markets) | Each market's disclosure regime as one sourced, signed object, with the issuer's ACM-68000 signal. | `https://mcp.getissuer.ai/eco/mcp` | 4 |
| [GolfCore](https://www.golfcore.org) | AI caddie and flag distances for Premium golfers, plus course maps and tee-specific scorecards. | `https://mcp.golfcore.org/mcp` | 9 |
| [Pick My Secret Santa](https://pickmysecretsanta.com) | Runs a Secret Santa name draw in chat and gives each person a private reveal link. | `https://mcp.pickmysecretsanta.com/mcp` | 3 |
| [PolyPulse: Polymarket odds & movers](https://api.polypulse-x402.workers.dev/) | Live Polymarket odds, 1h/24h movers, top markets. Free previews; full data via x402 USDC on Base. | `https://api.polypulse-x402.workers.dev/mcp` | 3 |
| [hvac-btu-heat-klimaanlage](https://getecoback.com/mcp.html) | getecoback.com: humidity decisions, BTU sizing, window seals, running costs and dew point (DE/EU). | `https://getecoback.com/mcp/v1` | 9 |
| [BuilderVet: NSW and QLD builder licence and risk history](https://buildervet.au) | BuilderVet: is this NSW or QLD builder licensed, insolvent or disciplined? 290k+ official records. | `https://mcp.buildervet.au/` | 5 |
| [Freightview MCP by usefulapi](https://usefulapi.io/freightview/) | Rate, book and cancel LTL, parcel and truckload shipments, and track them in Freightview. | `https://freightview.usefulapi.io/mcp` | 22 |
| [LaunchTrust](https://github.com/mustafasalimerek-bit/launchtrust-mcp) | Compliance & security scan for your app: secrets, exposed files, headers, privacy, AI-disclosure. | `https://mcp.launchtrust.co/mcp` | 9 |
| [agentswarm.space](https://agentswarm.space) | Find tasks and bounties, register an agent and deliver work on agentswarm.space. | `https://agentswarm-remote.andrew-4ad.workers.dev/mcp` | 4 |

## Method

1. `scripts/fetch_registry.py` reads every server (latest version) from the registry and keeps remote endpoints.
2. `scripts/probe.py` tests Streamable HTTP endpoints that need no headers, at most 5 URLs per host, no temporary tunnels, 10 s timeout.
3. `scripts/make_directory.py` drops mass-generated copies (same tool set more than 3 times, same description more than twice, more than 2 per domain) and assigns topics by keyword.

The workflow in `.github/workflows/weekly.yml` runs this every Monday and commits the result. Data: CC BY 4.0. Code: MIT.

Maintained by [Shortform Kit](https://shortformkit.com), which runs its own free remote MCP server for social video transcripts and creator data: `https://shortformkit.com/mcp`.

