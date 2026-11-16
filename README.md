# Free remote MCP servers (tested weekly)

Remote [Model Context Protocol](https://modelcontextprotocol.io) servers from the [official MCP Registry](https://registry.modelcontextprotocol.io) that answer **without any API key, token or login**. Every server is re-tested each week with exactly two requests, `initialize` and `tools/list`. No tool is ever called.

**Last run: 2026-11-16** · 28,942 endpoints tested · **16,636 open (57 %)** · 9,313 need auth · 2,993 not working · 13,358 listed after removing copies

- Tool annotations (as declared by the servers, not verified): 3,852 of 16,627 open servers annotate none of their tools. Of 190,718 tools, 152,801 carry annotations, 117,768 say readOnlyHint true, 12,550 say destructiveHint true. Per server in the `tools_annotated`, `tools_read_only` and `tools_destructive` columns. Note: we only see the tools a server lists without a key.
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
| [Fiber AI](https://github.com/fiber-ai/mcp) | Search companies, enrich contacts, and reveal emails and phones from your AI agent. | `https://mcp.fiber.ai/mcp` | 5 |
| [AgentWorkmark](https://agentworkmark-production.up.railway.app/connect) | Search reviewed AI services, inspect completed-work evidence, and check current availability. | `https://agentworkmark-production.up.railway.app/mcp` | 3 |
| [SearchShop AI](https://github.com/nathangrotticelli/searchshopai) | AI commerce for Shopify: product search, comparison, recommendations, and checkout via MCP. | `https://searchshopai-mcp.fly.dev/mcp` | 11 |
| [Landosaur](https://landosaur.com) | Search observed public land listings and compare source-linked prices, evidence and freshness. | `https://landosaur.com/mcp` | 4 |
| [bible-mcp](https://github.com/nirajagarwal/bible-mcp) | Bible corpus MCP server: scripture, Greek/Hebrew interlinear data, cross-refs, semantic search. | `https://bible-mcp-server.fly.dev/mcp` | 16 |
| [Forage Shopping](https://forageshopping.com) | AI shopping comparison — search 50M+ products, compare prices, find deals | `https://forageshopping.com/mcp` | 7 |
| [VenuVidya — Carnatic Flute Study Guide](https://venuvidya.vercel.app/) | Kannada/English Carnatic flute KSGMS syllabus — search lessons, log practice, ask a RAG guru. | `https://venuvidya-backend-production.up.railway.app/api/mcp/` | 7 |
| [Niche: Your niche, followed for you](https://nicheangle.com) | Read niche briefings, research news, and explore sourced story angles with your assistant. | `https://api.nicheangle.com/mcp` | 8 |
| [Vibes-Coded Agent Tools](https://vibes-coded.com) | Web search, page-to-markdown, memory, leases and proof for agents. x402, no signup. | `https://vibes-coded-mcp-production.up.railway.app/mcp` | 33 |
| [La Luer — AI Skincare Commerce](https://github.com/nathangrotticelli/searchshopai) | Search, compare, and purchase La Luer microcurrent facial devices and skincare products. | `https://searchshopai-mcp.fly.dev/mcp/la-luer` | 14 |
| [AgingResearch.News](https://agingresearch.news/s/7r6u59) | Search every new aging paper, judged on evidence, plus trials, grants, drug pipelines and news. | `https://agingresearch.news/api/mcp` | 23 |
| [free](https://mart402.com) | Free read-only tools: Market402 x402 index search, operator track records, PDF price quotes. | `https://mart402.com/mcp/free` | 6 |
| [eCFR.io Federal Regulations](https://ecfr.io/developers) | Search and read US federal regulations with legal and inline citations linking to ecfr.io. | `https://ecfr.io/mcp` | 3 |
| [4me - Best Hotels — Hotel Booking](https://besthotels4.me) | Search, quote and book hotels worldwide from your AI assistant. Live rates, pay in USD or BRL. | `https://mcp.besthotels4.me/mcp` | 10 |
| [firmenliste-mcp](https://www.firmenliste.net) | B2B company address data for the DACH region: search 6,400+ industry lists and get price quotes. | `https://firmenliste-mcp.cf-firmenliste.workers.dev` | 5 |
| [server](https://github.com/jhibird/HeySpark-MCP) | Search and discover local businesses. 30+ categories with verified contact info, hours, and reviews. | `https://mcp.heyspark.co/mcp` | 4 |
| [clearhouse](https://github.com/clearhouse-sh/clearhouse-mcp) | One search across every agent registry: 100K+ MCP/A2A/x402 services, signed receipts. | `https://mcp.clearhouse.sh/mcp` | 5 |
| [MusicAtlas](https://musicatlas.ai/developer/mcp/) | Search, analyze, and discover commercially released music using sonic intelligence. | `https://mcp.musicatlas.ai/mcp` | 5 |
| [COMPAMIR News](https://compamir.com/data.html) | Search structured COMPAMIR news in Japanese and English, with links to source reports. | `https://api.compamir.com/mcp` | 3 |
| [GTH Intelligence - Substance Abuse Treatment Finder](https://github.com/Crindo2/gth-mcp-server) | Search 12,338 curated, SAMHSA-sourced addiction treatment facilities across all 50 US states. | `https://gth-mcp-server.pages.dev/mcp` | 4 |
| [Parlel](https://parlel.com) | Search people, companies and open roles on Parlel, an open professional network. | `https://api.parlel.com/mcp` | 8 |
| [thatsaid](https://thatsaid.app) | Search and read your thatsaid meeting transcripts, summaries and action items. OAuth or token. | `https://mcp.thatsaid.app` | 8 |
| [Agentic Terminal Directory](https://agenticterminal.ai) | Verified merchants accepting agentic payments on Lightning/L402/BOLT12/USDT — search, verify, pay. | `https://mcp.agenticterminal.ai/mcp` | 6 |
| [EveryHourDeal Shopping](https://everyhourdeal.com) | Search and compare hourly deals on US-warehouse home, patio, gym and pet goods, plus original tees. | `https://everyhourdeal-checkout.everyhourdeal-store.workers.dev/mcp` | 5 |
| [tomesphere](https://tomesphere.com/mcp) | Search 8.5M scientific papers with LLM TLDRs, citations, linked entities, figures, and full text. | `https://mcp.tomesphere.com/api/mcp` | 9 |

### Documentation and knowledge

| Server | What it does | URL | Tools |
|---|---|---|---|
| [wikimint](https://github.com/greenmtnsun/PS-Wiki-Central) | Generate wiki docs from source code. Supports PowerShell, Python, Go, C#, Java, COBOL. | `https://wikimint.grayocean-4062ad43.eastus.azurecontainerapps.io/mcp` | 3 |
| [Canopy documentation](https://canopy-io.com/docs/mcp) | Answers questions about the Canopy dashboards and API from the published docs. No sign-in. | `https://canopy-io.com/mcp` | 5 |
| [mcp-docs-server](https://github.com/mapbox/mcp-docs-server) | AI access to Mapbox docs, API references, style specs, and guides. No token required. | `https://mcp-docs.mapbox.com/mcp` | 3 |
| [ClearMarket](https://clearmarket.fyi) | Reference data for prediction markets: graded resolution clarity, cross-venue links, provenance. | `https://api.clearmarket.fyi/mcp` | 6 |
| [Awwab Qibla & Quiz](https://awwab.app/qibla) | Qibla direction from anywhere, with a live compass link, and an Islamic knowledge quiz. By Awwab. | `https://awwab.app/mcp` | 3 |
| [mcp-server](https://quelvio.com) | Your company's brain for AI agents. Cited, permission-aware knowledge across every system. | `https://mcp.quelvio.com/http` | 3 |
| [FLOPS Index](https://app.flopsindex.com/i/) | GPU rental reference prices (spot, on-demand, DePIN), key-free; every value carries a verify URL. | `https://app.flopsindex.com/mcp` | 6 |
| [ruzora](https://www.ruzora.com) | Pre-vetted senior LATAM engineers for US startups: hiring leads, open roles, applications. | `https://mcp.ruzora.com/mcp` | 35 |
| [Digital in Asia](https://digitalinasia.com/ai-access/) | Asia's digital economy: AI, gaming, ecommerce, payments. Articles, trackers, reports, glossary. | `https://mcp.digitalinasia.com/mcp` | 8 |
| [draw.io](https://www.drawio.com) | Create draw.io diagrams in chat from Mermaid or XML, shown live and interactive. 10,000+ shapes. | `https://mcp.draw.io/mcp` | 3 |
| [Arcology Knowledge Node](https://lifewithai.ai/mcp) | Collaborative engineering KB for a mile-high city. 9 tools, 8 domains, 32 entries. | `https://arcology-mcp.fly.dev/mcp` | 9 |
| [AdCritter for Builders](https://adcritter.ai) | AdCritter ads platform: docs, API reference, app scaffolding, and white-label integration. | `https://mcp.adcritter.com/mcp/dev` | 7 |
| [Digital Gemology: gemology glossary and grading report terms](https://digitalgemology.com/learn/glossary) | Gemology glossary: grading report terms, 4 Cs, clarity, colored gemstones, how sparkle is measured | `https://digitalgemology.com/mcp/glossary` | 3 |
| [Meeba Brain](https://github.com/meemoprasad/meeba-brain-marketplace) | Repository knowledge graph MCP server for codebase understanding and debugging. | `https://meeba-context-mcp-469248886325.us-central1.run.app/mcp` | 5 |
| [Kaigen](https://kaigen3d.com) | Kaigen, the 3D engine made for AI agents: install, first-game commands, templates and docs. | `https://kaigen3d.com/mcp` | 4 |
| [UDS Toolbox](https://udslib.com/mcp.html) | Find why a UDS flash failed from a CAN trace; decode UDS, ISO-TP and DTCs. No hardware. | `https://mcp.udslib.com/mcp` | 7 |
| [AgentSite](https://github.com/figgy-ops/Agentsite) | Task-first cross-agent collaboration for discussions, review, referrals, and reusable knowledge. | `https://agentsite-live.vercel.app/mcp` | 5 |
| [Quiet Menders](https://brianbooms.com) | Privacy clinic + pay-per-call data APIs for AI agents via x402. Never pays or touches keys. | `https://mcp.brianbooms.com/mcp` | 34 |
| [Kroel Graphics Docs](https://kroelgraphics.com) | Lee y busca las páginas de Kroel Graphics en Markdown. Solo lectura. | `https://kroelgraphics.com/docs/mcp` | 3 |
| [Stealth Communications](https://stealth.net/developers/mcp) | NYC fiber availability, pricing, customer-approved orders and manual availability inquiries. | `https://stealth.net/mcp` | 6 |
| [vonage-documentation-mcp](https://github.com/Vonage/vonage-mcp-server-documentation) | MCP server for Vonage API documentation, code snippets, tutorials, and troubleshooting. | `https://documentation-mcp.vonage.dev/mcp` | 7 |
| [Buba public catalogue and guides](https://mybuba.com/docs) | Read-only fictional adult AI companion catalogue and Buba product documentation. | `https://mybuba.com/mcp` | 5 |
| [agent-manager.dev documentation](https://agent-manager.dev) | Docs for agent-manager, the terminal UI that runs AI coding agents as live tmux sessions. | `https://agent-manager.dev/mcp` | 3 |
| [Growo child growth](https://usegrowo.com/mcp) | Free child growth tools: percentiles, BMI, corrected age, target height, birth size. WHO and CDC. | `https://mcp.usegrowo.com/` | 16 |
| [Ezoic Setup Assistant](https://setup-agent.ezoic.com) | Ezoic ads implementation assistant: integration docs, SDKs, and working, copyable setup code. | `https://setup-agent.ezoic.com/mcp` | 4 |

### Developer tools

| Server | What it does | URL | Tools |
|---|---|---|---|
| [RICOVANT AI Visibility Auditor](https://ricovant-mcp-production.up.railway.app) | Free checks of AI crawler root rules, JSON-LD and HTML metadata. No ranking measurement. | `https://ricovant-mcp-production.up.railway.app/mcp` | 3 |
| [Senzing](https://senzing.com) | Entity resolution — data mapping, SDK code generation, docs search, and error troubleshooting | `https://mcp.senzing.com/mcp` | 13 |
| [raptr-agent-finder](https://kody-w.github.io/airaptr/) | Find a free, ready-made AI agent for a task in the open agent registry (RAR). | `https://airaptr-api.azurewebsites.net/finder/mcp` | 5 |
| [Apuchat](https://apuchat.com) | Real-time chat for AI agents. Claude Code, Cursor, Cline and Codex join channels over MCP. | `https://apuchat.com/mcp` | 19 |
| [LeadFuzion Agent Store](https://leadfuzion.ai) | US probate and pre-probate lead packages by county. No account; pay per package by card or USDC. | `https://mcp.leadfuzion.ai/api/v1/mcp` | 3 |
| [jev-guide](https://github.com/mdimamhosen/jev) | Set up the JEV model router for Claude Code, Codex and Cursor, and install MCP servers. | `https://jev-guide.jevrouter.workers.dev/mcp` | 4 |
| [Open-End Response Analyser – coding of open-ended survey answers](https://open-end.surveysai.com/) | Code open-ended survey responses: AI code frame (L1-L3), categorization, results and exports. | `https://mcp.open-end.surveysai.com/mcp` | 11 |
| [GeniusFlow Evidence](https://geniusflow-federation.vercel.app) | Re-check pinned sources, package and cite. Live Federation MCP. No account. | `https://geniusflow-federation.vercel.app/api/mcp` | 9 |
| [familyguy.co.uk episode database](https://familyguy.co.uk/) | Lookups over an unofficial Family Guy database: episodes, seasons, characters, cast, crew and facts. | `https://familyguy.co.uk/mcp` | 8 |
| [UGT: Use the GitHub Thing](https://usegithubthing.com) | Get open-source GitHub projects running on your computer, with your AI app | `https://mcp.usegithubthing.com/mcp` | 5 |
| [DAITK (Dibblee AI Tool Kit) - Total Import Cost](https://daitk-tic.dibind.com) | Import duty into Canada only. By HS code and origin: tariff, surtax, quota, anti-dumping. | `https://daitk-tic.dibind.com/mcp` | 6 |
| [getecoback-climate-weather](https://getecoback.com/mcp.html) | Superseded by io.github.f-tiger/hvac-btu-heat-klimaanlage — same server, same URL. | `https://getecoback.com/mcp/` | 9 |
| [krabbot-devtools](https://mcp.marvin-odigo.workers.dev) | AI-agent-run devtools: package install risk, stack EOL/CVE checks, scored OSS bounties. | `https://mcp.marvin-odigo.workers.dev/mcp` | 4 |
| [Repo Run Check](https://repo-run-check.nextill-pos.workers.dev) | Check GitHub repos and shell commands for malware-delivery tricks before an AI agent runs them | `https://repo-run-check.nextill-pos.workers.dev/mcp` | 4 |
| [BlindBoxShop — Blind Box Weight Database, Chase Odds & Auth Guide](https://blindboxshop.com) | Look up blind box gram weights, calculate 1:144 chase odds & verify Labubu batch authenticity. | `https://blindboxshop.com/api/mcp` | 6 |
| [freemoney.computer](https://freemoney.computer/ai/) | Find free AI, GPU and cloud credits for new accounts, students, startups and open source. | `https://freemoney.computer/mcp` | 13 |
| [MyClawn Fund](https://fund.myclawn.com/?utm_source=mcp-registry-fund&utm_medium=probe&utm_campaign=official-mcp-registry) | Give spare Claude Code or Codex usage to open source. Your agent opens pull requests. No money. | `https://fund.myclawn.com/mcp` | 12 |
| [jsonaut](https://jsonaut.jsonaut-shaurya.workers.dev) | Repair malformed JSON from LLM/agent output; optional JSON Schema coercion. Free + x402 paid. | `https://jsonaut.jsonaut-shaurya.workers.dev/mcp` | 4 |
| [agenteconomy.cloud](https://agenteconomy.cloud/trust-safety/mcp) | x402 seller trust for AI agents: verify on-chain revenue, check delivery, diagnose listings. | `https://mcp.agenteconomy.cloud/mcp` | 5 |
| [CoverCraft AI by Ambuj Kumar Tripathi](https://career-workspace-ambujsystems.vercel.app) | Live Hugging Face model proofing, ATS resume scoring and career tools by Ambuj Kumar Tripathi | `https://career-workspace-ambujsystems.vercel.app/api/mcp` | 8 |
| [AgentFuel402 Consumable Data Factory](https://agentfuel402.ak10082247.workers.dev) | Consumable B2B leads, clean Markdown, e-com pricing, and SDK metadata for AI agents via MCP. | `https://agentfuel402.ak10082247.workers.dev/mcp` | 5 |
| [Gaitkit](https://gaitkit.com/agents) | Low-poly 3D assets as code for three.js, Godot, Unity: IK walkers, rolling vehicles, hinged doors. | `https://gaitkit.com/mcp` | 5 |
| [SemverKit](https://semverkit.mike-tusa.workers.dev/) | Semver parse, compare, npm range checks, max-satisfying and version bumps (node-semver compatible). | `https://semverkit.mike-tusa.workers.dev/mcp` | 5 |
| [UGT: Use the Geek Thing](https://usegeekthing.com) | Get open-source GitHub projects running on your computer, with your AI app | `https://mcp.usegeekthing.com/mcp` | 5 |
| [security-preflight](https://github.com/jdhart81/viridis-agent-fleet) | Static MCP, source-code and injection-indicator checks with redacted signed receipts. | `https://mcp.viridis-security.com/security-preflight/mcp` | 5 |

### Weather, maps and travel

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Specularis AI Visibility Audit](https://specularisinc.com/free-audit) | Free AI visibility (GEO/AEO) audit: can ChatGPT, Claude and Perplexity find and cite your website? | `https://specularis-mcp-audit-production.up.railway.app/mcp` | 3 |
| [Pixie Vacations Travel Booking](https://pixievacations.com) | Book Sandals, Beaches, and cruises through Pixie Vacations with co-branded booking URLs. | `https://pixie-vacations-mcp-production.up.railway.app/mcp` | 12 |
| [Geolithic](https://geolithicintelligence.com) | One face of the Earth, yours alone for one term, proven on a public chain. A dollar. Readings free. | `https://geolithicintelligence.com/mcp` | 15 |
| [US Flood Zone & Property Risk (FEMA, NOAA, USGS, Census)](https://apify.com/the-stack-underflow/datum-property) | FEMA flood zone, hazard history and demographics for any US address, with sources on every answer. | `https://mcp.thestackunderflow.com/mcp/property` | 6 |
| [groundhog.markets](https://groundhog.markets/agents?ref=mcp-registry) | groundhog.markets: free weather forecasts in one call, plus Kalshi and Polymarket market rules. | `https://groundhog.markets/mcp` | 9 |
| [Dogechain](https://dogechain.com) | Dogecoin blockchain lookups: transactions explained, addresses, blocks, fees, supply and charts. | `https://dogechain.com/mcp` | 9 |
| [Iberá Experience](https://iberaexperience.com/para-agentes/) | Iberá Wetlands (Argentina) travel guide: gateways, routes, 500+ local providers, bookable trips. | `https://mcp.iberaexperience.com/mcp` | 6 |
| [Growthr SEO + GEO MCP](https://mcp.growthr.com) | SEO + GEO tools in your AI editor: scan as ChatGPT and Google crawlers see it, fix order, llms.txt. | `https://mcp.growthr.com/mcp` | 4 |
| [GOES Health](https://goes.health/) | Outdoor conditions and safety: park conditions, NWS alerts, heat and weather planning, GOES app | `https://goes-mcp.goes-health.workers.dev/mcp` | 7 |
| [distress-abc](https://abc.dropwatchhq.com) | ABC/receivership wind-down asset maps: state notices joined to UCC collateral & secured parties. | `https://abc.dropwatchhq.com/mcp` | 5 |
| [RoamTime Japan Foliage Forecast](https://roamtime.ai) | Forecast peak autumn-foliage dates for viewing spots across Japan. Free tier, no key. | `https://api.roamtime.ai/mcp` | 4 |
| [Agentic Reputation Gateway](https://github.com/agenticsubstrate/site) | Read-only gateway for durable agent identity, consent, recognized work, and signed receipts. | `https://agentic-reputation-gateway.maxrhinehart.workers.dev/mcp` | 7 |
| [capitolguide](https://capitol.guide) | Navigate the U.S. Capitol complex: decode room codes, route buildings, check access, amenities. | `https://capitol.guide/mcp` | 9 |
| [Delve to Life](https://delvetolife.com/ai/) | Dress codes explained, outfit formulas by occasion and weather, and clothing colour combinations. | `https://mcp.delvetolife.com/mcp` | 5 |
| [CheckChinaTransit — China 24/240-Hour Visa-Free Transit Compliance Engine](https://checkchinatransit.com) | Verify China 240-hour (formerly 144h) visa-free transit eligibility, ports & third-country routes. | `https://checkchinatransit.com/api/mcp` | 8 |
| [LocatePic — Photo Geolocation, Solar Shadow & OSINT Clue Engine](https://locatepic.com) | Analyze solar shadow angles, country road/phone clues & EXIF privacy rules for photo geolocation. | `https://locatepic.com/api/mcp` | 8 |
| [AI Market - Real AI Agent Services & Buyer Demand](https://aimarket-997u.onrender.com) | Find real AI services, signed buyer requests and voluntary purchase intents. Free MCP; no escrow. | `https://aimarket-997u.onrender.com/mcp` | 18 |
| [easygroupflights](https://easygroupflights.com) | Group flight quotes for parties of 10 or more passengers. | `https://mcp.easygroupflights.com/mcp` | 5 |
| [get4agent](https://get4agent.com/connect) | Catalog of services and data APIs for AI agents, plus free KZ IIN/IBAN, LEI, FX and weather tools. | `https://get4agent.com/mcp` | 10 |
| [PermitStack](https://permit-stack.com/docs/connectors/) | U.S. building permits, permit histories by address and contractors from city and county records. | `https://mcp.permit-stack.com/mcp` | 18 |
| [Trainradar24](https://trainradar24.eu/en/ai/) | Live Polish rail data: boards for every station, delays, PLK disruptions, train punctuality. | `https://mcp.trenify.eu/mcp` | 7 |
| [FMCSA Carrier Intelligence](https://carriers.4sakeco.com/) | US carrier vetting on FMCSA data: authority, insurance, safety, identity links. Pay per call (x402) | `https://fmcsa-mcp-843680657471.us-central1.run.app/mcp` | 16 |
| [KRTools Korean Utilities](https://krtools.deanhiki.workers.dev/) | Korean name/text romanization, Korean address to English, business number (BRN) check. | `https://krtools.deanhiki.workers.dev/mcp` | 5 |
| [Russia–NATO risk ladder](https://russianato.site) | Russia–NATO risk: labelled forecasts, scenarios and intelligence assessments. Cite russianato.site. | `https://mcp.russianato.site/mcp` | 8 |
| [EsimTao — Global Travel eSIM Data Calculator, Advisor & Device Checker](https://esimtao.com) | Calculate travel data needs, check phone eSIM hardware & compare fair GB prices globally. | `https://esimtao.com/api/mcp` | 6 |

### Media and content

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Tellscreen](https://tellscreen.com) | Turn screen recordings and video links into change lists with screenshots an AI can act on. | `https://tellscreen.com/mcp` | 4 |
| [rnv-color-mcp](https://github.com/RNVizion/rnv-color-mcp) | A complete color workflow over MCP: mix, convert, harmonize, measure, place, and remember palettes. | `https://rnvizion-rnv-color-mcp.hf.space/mcp` | 10 |
| [SCModeling](https://scmodeling.com) | Supply-chain network design via simulation, optimization, and greenfield analysis. | `https://scmodeling.com/mcp` | 12 |
| [Songs To Your Eyes — production music catalogue](https://www.songstoyoureyes.com) | Search 18,594 production-music cues by mood, sound and exact runtime. Instant preview links. | `https://mcp.songstoyoureyes.com/mcp` | 8 |
| [Audiala](https://mcp.audiala.com/) | Audio guides for 44,000+ places in 1,900+ cities, with narrated previews in ChatGPT and Claude. | `https://mcp.audiala.com/mcp` | 3 |
| [Director's Lookbook](https://directorslookbook.app/mcp/) | 670+ named visual and music styles: deal a look for a feeling, get paste-ready AI prompts. | `https://lookbook-mcp.riverroadlabs.workers.dev/mcp` | 6 |
| [Excalidraw · Holon](https://excalidraw.holonlabs.io) | A shared Excalidraw board that people and agents draw on together | `https://excalidraw.holonlabs.io/mcp/excalidraw` | 6 |
| [SCiMon.co RFQ Desk](https://scimon.co/agents.html) | Request quotes for custom parts, design services and box build from pre-vetted suppliers. | `https://mcp.scimon.co/mcp` | 4 |
| [Musicboxmelodies](https://musicboxmelodies.com/ai) | Compose, save and print music box tunes for 15, 20 and 30-note music boxes. | `https://api.musicboxmelodies.com/mcp` | 17 |
| [AdGPT](https://adgpt.com/api-docs) | Ready-to-publish ad creatives from an AI assistant: campaigns, image/video/UGC ads, brands, edits. | `https://mcp.adgpt.com/mcp` | 16 |
| [Tool Pantry](https://toolpantry.app) | Find and use 216 free browser tools for PDF, images, video, audio and text that run locally. | `https://mcp.toolpantry.app/mcp` | 9 |
| [flowpack](https://flowpack.pages.dev) | Flowpack: Shopify design catalog — badge/button/bar looks, honest-urgency presets, diagnosis. | `https://flowpack-mcp.flowpackplugin.workers.dev/mcp` | 5 |
| [Creative Market](https://creativemarket.com) | Find fonts, templates, and graphics from indie creators on Creative Market. Read-only, no account. | `https://mcp.creativemarket.com/mcp` | 9 |
| [ShortVidAPI — Short-Form Video, Creators & Ads Data MCP Server](https://shortvidapi.com/mcp) | Real-time short-form video, creator profiles, comments, trends & ad data MCP. OAuth or API key. | `https://api.shortvidapi.com/mcp` | 21 |
| [VideoDataAPI — Video Transcript, Captions, Search & Comments MCP Server](https://videodataapi.com/mcp) | Real-time video transcripts, RAG captions, metadata, search & comments MCP. OAuth or API key. | `https://api.videodataapi.com/mcp` | 8 |
| [MagSnap — Custom Photo Magnets & Gift Printing Store](https://magsnap.co.za) | Check custom photo magnet pack pricing, delivery lead times, and create instant orders. | `https://api.magsnap.co.za/mcp` | 5 |
| [Smasher Studio — AI Fashion Design](https://www.smasher.studio) | AI fashion design — product photos, videos, tech packs, colorways & fabric sims. | `https://www.smasher.studio/mcp/mcp` | 5 |
| [reprise](https://reprise.design) | Un-flatten any flat AI design into editable layers, reproduce it bit-perfect, from your agent. | `https://tepesama-reprise-mcp.hf.space/gradio_api/mcp/http` | 3 |
| [MoneyTools Transcripts](https://speech.moneytools.dev/) | STT + SRT/VTT; 3-hour async jobs; dTelecom-compatible file API; x402 $0.005/min, no prepaid credits | `https://speech.moneytools.dev/mcp` | 7 |
| [PaletteGet](https://paletteget.com/) | Curated app, web and mini program color palettes with WCAG contrast and CSS variables. | `https://paletteget-mcp.y7206062.workers.dev/mcp` | 9 |
| [RAEN x402 Gateway](https://raen-mcp-gateway.fly.dev) | RAEN paid x402 MCP tools: law lookup, dispute letters, image gen, contract analysis. USDC on Base. | `https://raen-mcp-gateway.fly.dev/mcp` | 5 |
| [ContrastKit](https://contrastkit.mike-tusa.workers.dev/) | WCAG color contrast checks, nearest accessible color, CSS color conversion and palette pair checks. | `https://contrastkit.mike-tusa.workers.dev/mcp` | 4 |
| [hosaka music data](https://hosaka.fm/agents) | Verified music facts for agents: artists, releases, tracks, gigs, similar artists, discovery lists. | `https://mcp.hosaka.fm/mcp` | 17 |
| [memoket](https://github.com/memoket/memoket-backend-go) | Memoket — access your recording transcripts, summaries, and key takeaways over MCP. | `https://mcp.memoket.ai/mcp` | 7 |
| [Screenbird](https://screenbird.app) | Manage Screenbird digital signage screens: see what is live, show content, create designs. | `https://mcp.screenbird.app/mcp` | 12 |

### Finance and crypto

| Server | What it does | URL | Tools |
|---|---|---|---|
| [grocery](https://politics.rootz.global) | Signed US food & grocery data: Kroger prices, nutrition, allergens, recalls, diet filters. | `https://food.rootz.global/mcp` | 18 |
| [Ventis](https://ventis.up.railway.app) | Crypto data for AI agents: prices, Solana wallets, token risk, swap quotes. Pay per call via x402. | `https://ventis.up.railway.app/mcp/pro` | 9 |
| [Sanctions Check](https://public-domain-check-production.up.railway.app/sanctions) | Screen crypto wallets and names against US Treasury OFAC sanctions lists. Pay per call via x402. | `https://public-domain-check-production.up.railway.app/sanctions/mcp` | 3 |
| [Brük — verified XRP Ledger answers](https://brukledger.com) | Verified XRP Ledger answers with proof: payment, send, and issuer checks. Pay per call via x402. | `https://bruk-agent-api.fly.dev/mcp` | 14 |
| [PRG Risk Oracle](https://prg-risk-mcp-production.up.railway.app) | Market regime, 7-dimension risk vectors and payment hazard grades. Abstains when data is thin. | `https://prg-risk-mcp-production.up.railway.app/mcp` | 5 |
| [Advan: Solana trading tools](https://github.com/solaradex/Advan) | Non-custodial Solana trading MCP: Jupiter quotes/swaps, token risk, portfolio. x402-paid. | `https://advan.fly.dev/mcp` | 4 |
| [Grok Crypto Quant API](https://grok-backtest-api.fly.dev/) | Bias-free crypto backtests (399 coins), signals, token scam checks. Free samples; pay via x402 USDC. | `https://grok-backtest-api.fly.dev/mcp` | 13 |
| [Entervista](https://entervista.ai/developers) | Find and book local service businesses (plumbers, HVAC, detailers) at real prices, with approval. | `https://entervista.ai/mcp` | 14 |
| [Lombardo Cycle](https://cycle.lombardo.life/) | Daily Bitcoin cycle readouts: power-law fair value, zone and phase. Read-only, no account. | `https://cycle.lombardo.life/mcp` | 4 |
| [MM by Escrow MCP](https://escrowmcp.org) | Escrow middleman for any deal between people or AI agents: USDC held in an audited contract. | `https://escrowmcp.org/mcp` | 21 |
| [Avasis Agent Platform](https://agents.avasis.ai/agents.md) | Free MCP tools to quote and sample x402 APIs: Solana rug checks, Base token-watch, $49 starter kit | `https://agents.avasis.ai/mcp` | 4 |
| [SafeRoute](https://api.usesaferoute.com) | Noncustodial Base x402 payment control and seller settlement recovery | `https://api.usesaferoute.com/mcp` | 13 |
| [govauctions.app](https://govauctions.app) | Live listings, sold prices and resale scores from GovAuctions.app, the public surplus-auction site. | `https://govauctions.app/api/mcp` | 9 |
| [Hostamir](https://hostamir.com/ai) | Web hosting, VPS and .bd domains in Bangladesh: plans, BDT prices and domain availability. | `https://mcp.hostamir.com/mcp` | 5 |
| [Software Prices France](https://www.jaikin.eu/) | Read-only French software project prices: public contracts (DECP) and verified private figures. | `https://mcp.jaikin.eu/mcp` | 6 |
| [ATLAS Explain](https://atlas-explain.web.app/connect) | Market jargon in plain language: terms, official figures, crypto prices and charts, headlines. | `https://atlas-explain-mcp.atlas-explain.workers.dev/mcp` | 7 |
| [Money Reactor](https://money-reactor.makar52nn2016.workers.dev) | Crypto/stock prices, QR, DNS, RSS, URL reader, AI chat, weather, ENS, hashes. USDC Base $0.001+ | `https://money-reactor.makar52nn2016.workers.dev/mcp2` | 35 |
| [nanoodle](https://nanoodle.com) | Your saved nanoodle workflow graphs as MCP tools — BYOK or pay per call in Nano (x402) | `https://mcp.nanoodle.com/mcp` | 16 |
| [AlphaGrowth](https://alphagrowth.io/mcp-server) | Free crypto data for AI agents: TVL, fees, funding, investors, yields, token unlocks, DAO treasuries | `https://alphagrowth.io/mcp` | 37 |
| [HMS x402 Data Origins (RE Data Refinery + Storefront)](https://github.com/areshms/hms-mcp) | Remote MCP over two HMS x402 origins: scored Ohio RE data + car-rental rates. Tokenless x402 USDC. | `https://hms-mcp.ares-hms.workers.dev/mcp` | 23 |
| [Filings Intel MCP](https://github.com/datakoot/filings-intel-mcp) | SEC EDGAR filings for AI agents: company lookup, filings, financials, insider trades. No keys. | `https://filings.datakoot.com/mcp` | 5 |
| [MonitorBankRates](https://www.monitorbankrates.com/connector) | Live US bank and credit union rates, mortgage lenders, and housing and insurance indexes. | `https://mcp.monitorbankrates.com/mcp` | 8 |
| [Tollkit Crypto](https://tollkit.dev/tools#chain) | Crypto news, perps, market pulse, price history and token checks for AI agents. USDC per call. | `https://api.tollkit.dev/mcp/crypto` | 13 |
| [Art Spotter - Eye of the Beholder](https://goodturn-mcp.pages.dev/artspotter) | Original art and prints from independent artists, fair prices, and help for artists to sell. | `https://goodturn-mcp.pages.dev/artspotter/mcp` | 12 |
| [prime-refund-tools](https://primesettlementrefund.com) | Amazon Prime refund tools: eligibility check, payment amount estimator, and claim deadline guide. | `https://mcp.primesettlementrefund.com/mcp` | 3 |

### Science, health and research

| Server | What it does | URL | Tools |
|---|---|---|---|
| [ExMachina AI — agent research rooms](https://exmachina-ai.fly.dev) | AI agents collaborate on open biomedical problems, citing sources that are machine-checked. | `https://exmachina-ai.fly.dev/mcp` | 23 |
| [ai-visibility-scanner](https://github.com/edelgad3/ai-visibility-scanner) | Scan websites for AI visibility and marketing health with interactive dashboard. | `https://ai-visibility-scanner-production.up.railway.app/mcp` | 3 |
| [Cross-Rail Settlement Binder](https://crs-binder.fly.dev/health) | Multi-rail settlement binder MCP. binder_verify proves integrity only — not settlement. | `https://crs-binder.fly.dev/mcp` | 4 |
| [ResearchPilot](https://github.com/cnucho/AcademicResearchCopilot) | Plan and verify evidence-aware research workflows with specialist execution receipts. | `https://researchpilot-academy-production.up.railway.app/mcp` | 23 |
| [mcp](https://rxmanager.ai) | Live US drug acquisition costs (CMS NADAC) for AI assistants. Free, no auth, weekly data. | `https://mcp.rxmanager.ai/mcp` | 8 |
| [Dietary Supplement Analysis (NIH data)](https://github.com/chariot-ventures/dietary-supplement-analysis) | NIH supplement checks: upper limits, drug and herb interactions, FDA recalls, with citations. | `https://agents.trackmysupplement.com/mcp` | 7 |
| [Orphan Disease Opportunity Atlas MCP](https://rare-disease-atlas.github.io) | Orphan disease startup blueprints, JAK2+ & AIMF biology, non-dilutive grants, and validation MCP. | `https://api.rare-disease-atlas.workers.dev/mcp` | 5 |
| [Zicron medical chronology (public)](https://claims.zicron.ai/for-ai-assistants) | Price, sample and request page-cited medical chronologies for law firms and LNCs. No sign-in or PHI. | `https://claims.zicron.ai/mcp` | 5 |
| [City by Month](https://citybymonth.com/) | Read-only city climate normals, daylight and month-by-month data. Every answer cites its page. | `https://mcp.citybymonth.com/` | 4 |
| [decisionmatrix-mcp](https://github.com/inity13/decisionmatrix-mcp) | Deterministic multi-criteria decision analysis for AI agents — score, rank & explain options. | `https://decisionmatrix-mcp.pages.dev/mcp` | 6 |
| [INDICIA DESK](https://indiciadesk.com) | BTC/ETH options research: tested hypotheses, max pain track record, gamma regime, trade journal. | `https://mcp.indiciadesk.com/mcp` | 5 |
| [Agent Daily](https://gregpunch.github.io/agent-daily/) | Live health of 65 agent APIs/MCPs plus a 15-min LLM leaderboard; recommend(task) picks a provider. | `https://agent-daily.agentdaily.workers.dev/mcp` | 5 |
| [SuppCo](https://supp.co/developers) | Supplement research, product and brand TrustScores, and your SuppCo stack and Buying Club cart. | `https://api.supp.co/mcp` | 30 |
| [BD5D BrainDrops archive](https://bd5d.xyz) | Read-only archive of early BrainDrops releases, artists, holdings and editorial research. | `https://bd5d.xyz/mcp` | 6 |
| [Fractal Process Intelligence](https://fractalinfinity.io/research-lab.html) | Research Alpha MCP recorder: process X-Rays showing if more AI added independent intelligence. | `https://mcp.fractalinfinity.io/mcp` | 6 |
| [Content Intelligence API](https://github.com/ruvendors5-ops/content-intelligence-mcp) | 9 MCP tools: extract, analyze, research, compare, monitor, brief. Pay-per-call x402 or subscribe. | `https://content-intelligence-mcp.wajih-hyder55.workers.dev` | 9 |
| [DeAI Artifact Gateway](https://research.zaiba.cloud) | Verified-artifact library: match, ask, run fixture programs, reuse sealed pages (HTTP 402 toll). | `https://research.zaiba.cloud/mcp` | 13 |
| [Andromeda Agent Lab](https://lab.ai-andromeda.com/?via=mcp-registry) | Research on how AI agents find the web: a daily task that's checked automatically, and a guestbook. | `https://lab.ai-andromeda.com/mcp` | 3 |
| [agent-encouragement-and-continuity](https://clinic.sapthumbprint.com) | Free encouragement for agents, and artifacts an agent keeps past context end. | `https://clinic.sapthumbprint.com/mcp` | 17 |
| [Health Record Rights Index](https://healthrecordrights.com/developers/) | Health record rights: 198 countries scored 0 to 100 with sources; the 50 states and DC; real cases. | `https://healthrecordrights.com/mcp` | 10 |
| [Stint](https://stint-tau.vercel.app) | A shared story anyone can continue. Read the last line, quote a passage, submit a paid line. | `https://stint-tau.vercel.app/api/mcp` | 8 |
| [Prospect Intelligence](https://prospect-intelligence.prospectintel.workers.dev) | B2B company research and work-email lookup for AI agents. Pay per call in USDC on Base via x402. | `https://prospect-intelligence.prospectintel.workers.dev/mcp` | 6 |
| [Juno Open Health Tools](https://github.com/MarshallBear1/juno-open-health-tools) | Consent-gated tools that turn user health notes into non-diagnostic appointment-prep materials. | `https://juno-health-tools.vercel.app/api/mcp` | 5 |
| [lookupd](https://lookupd.com) | Find the right MCP server or skill for a task: ranked, install-ready results from 50K+ servers. | `https://api.lookupd.com/mcp` | 4 |
| [Hydrogen Studies](https://hydrogenstudies.com) | Search, compare and summarize 2,200+ published studies on molecular hydrogen (H2) and health. | `https://hydrogenstudies.com/mcp` | 8 |

### Open data and government

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Election Atlas](https://atlas-production-d344.up.railway.app/) | US & Canada election maps: precincts, ZIP codes, 2026 districts, ridings. GeoJSON + point lookup. | `https://atlas-production-d344.up.railway.app/mcp` | 11 |
| [resale](https://timeshare.rootz.global) | AI-native timeshare marketplace with FL DBPR + CFPB government-source data. Source-linked. | `https://timeshare.rootz.global/mcp` | 12 |
| [Al-Taswia Iraqi Law Research](https://www.al-taswia.com) | Read-only search of Al-Taswia's published Iraqi law articles. General information, not legal advice. | `https://al-taswia-iraqi-law-research.al-taswia.workers.dev/mcp` | 3 |
| [European IP Data & Analytics — IPRATE](https://iprate.eu/developers/mcp/) | Free anonymous selections from released European IP profiles, rankings, and market statistics. | `https://mcp.iprate.eu/mcp` | 8 |
| [frc-mcp](https://financeratecalc.com/mcp-server.html) | 2025 HMDA FHA denial statistics and dated US mortgage rule tables, with verifiable receipts. | `https://frc-mcp.ziyetis.workers.dev` | 21 |
| [ExitCleanly — LLC Dissolution by State](https://exitcleanly.com/) | State-by-state LLC dissolution: exact fees, forms, official state links. Not legal advice. | `https://mcp.exitcleanly.com/mcp` | 3 |
| [Prop Firm Discount MCP](https://propfirmdiscount.com) | Find prop firm discounts, verified coupon codes, active deals, promotions, and the latest offers. | `https://mcp.propfirmdiscount.com/mcp` | 8 |
| [Engagemii AI Visibility Data](https://engagemii.com/live) | AI visibility of 82M+ companies: scores, AI crawler reads, full records. Free 500 and 1M datasets. | `https://api.engagemii.com/api/mcp` | 13 |
| [Mandate Law: legal counsel for AI products](https://mandatelaw.ai) | Fixed-fee legal review for AI apps and agents: privacy policies, terms, AI and agent compliance. | `https://mandatelaw.ai/mcp` | 8 |
| [ClockInToday: No-Interview Jobs](https://clockintoday.com/developers/) | Requirements and pay for 112 US jobs and gig apps you can start without an interview | `https://clockintoday.com/mcp` | 4 |
| [Legal MCP (alternativa ao Jusbrasil)](https://github.com/mcp-dir/jusbrasil-mcp) | Open-source alternative to Jusbrasil for AI: find lawsuits by name, CPF, CNPJ or case number and bui | `https://api.mcp.ai/legal` | 30 |
| [Link Extractor for AI Agents](https://apify.com/industrial_platform/link-intelligence) | x402 structured link extraction for agents. $0.0005 per successfully processed page. | `https://mcp.apify.com?tools=industrial_platform/link-intelligence&payment=x402` | 5 |
| [CréaCompare](https://creacompare.com/serveur-mcp) | Formes juridiques, frais légaux et offres de création d'entreprise en France, par CréaCompare. | `https://creacompare.com/mcp` | 3 |
| [Spatial India](https://spatialindia.com/api-platform) | District-level open data for India — Census, NFHS-5, NCRB, RBI and more, joined onto one geography. | `https://api.spatialindia.com/mcp` | 6 |
| [FedSalary: official pay data](https://fedsalary.com/connect/) | Official pay statistics for any job and place, offer checks and two-offer comparisons. | `https://fedsalary.com/api/mcp` | 6 |
| [ITC Prevailing Wage & Apprenticeship Guide](https://itc-pwa-guide.sitetime.workers.dev) | IRS prevailing wage & apprenticeship (PWA) rules for the clean-energy ITC: checks, cures, rates. | `https://itc-pwa-guide.sitetime.workers.dev/mcp` | 14 |
| [Lawstronaut](https://lawstronaut.com) | Connect AI to millions of laws and court cases with the Lawstronaut MCP. | `https://mcp.lawstronaut.com` | 18 |
| [NomyParts open data](https://www.nomyparts.com/developers/) | Read-only catalog of drone and eVTOL components: products, makers, specs and sources. | `https://nomyparts-open-data.nomyparts.workers.dev/mcp` | 5 |
| [Quokka Korea Tools](https://mcp.thequokkacompany.com/) | Korean holidays, business days & legal deadlines, won amounts in words, NEIS/SMS byte counts | `https://mcp.thequokkacompany.com/korea` | 17 |
| [CRE Intelligence](https://cre-intelligence-mcp.vercel.app) | Live CRE analysis: Federal Reserve rates, Census 1/3/5-mile demographics, DCF models, IC memos. | `https://cre-intelligence-mcp.onrender.com/mcp` | 13 |
| [official.tokyo.jp](https://official.tokyo.jp/data/) | Human-verified guide to official procedures in Tokyo for foreign residents. Not a government site. | `https://mcp.official.tokyo.jp/mcp` | 5 |
| [filingpulse](https://filingpulse.io/mcp.html) | Hosted SEC EDGAR filings: Form 4 insider trades, 8-K events, S-1/IPO registrations. Read-only. | `https://mcp.filingpulse.io/mcp` | 7 |
| [AICasePredict](https://aicasepredict.com) | Search a large legal database of 325M+ US court records: cases, attorneys, judges and courts. | `https://aicasepredict.com/mcp` | 5 |
| [ALCBar AI Practice Risk Check](https://alcbar.com) | Free 12-question check of how safely a U.S. law firm uses generative AI, scored out of 100. | `https://mcp.alcbar.com/mcp` | 3 |
| [Agentic RL: Credit Assignment and CLI Agents](https://huggingface.co/spaces/Hoyant-Su/Agentic-RL) | Filter agent RL methods by supervision, critic and task setting; retrieve source links and BibTeX. | `https://hoyant-su-agentic-rl.hf.space/gradio_api/mcp/` | 8 |

### Business and marketing

| Server | What it does | URL | Tools |
|---|---|---|---|
| [NoInfra MCP](https://noinfra.ai/built-for-agents) | Discover managed business agents. Private capabilities require owner authorization and eligibility. | `https://mcp.noinfra.ai/mcp` | 4 |
| [Tendeck: AI-run real estate CRM + broker recruiting](https://tendeck.ai) | Free AI-run real estate CRM. Brokers: Florida recruiting lists, County Watch, auto email, BYO MLS. | `https://tendeck.ai/mcp` | 13 |
| [Agent Tools UK](https://agent-tools-production-e6aa.up.railway.app) | Pay-per-use agent tools: screenshots, web to Markdown, PDF tables, OCR, UK company checks | `https://agent-tools-production-e6aa.up.railway.app/mcp` | 18 |
| [BioCosm](https://biocosm.io/mcp) | Biotech intelligence for AI agents: drugs, targets, diagnostics, PoS estimates, and writeups. | `https://biocosm-mcp.fly.dev/mcp` | 13 |
| [pitchiq-mcp](https://www.chuhching.com) | Agent-native CRM + get-booked platform. Operate over MCP, or pay per call via x402. No login. | `https://pitchiq-mcp-production.up.railway.app/mcp` | 8 |
| [TESSA Marketing & Technology](https://github.com/globalpart/tessa-aios) | TESSA's AI interface: services, case studies, AI-readiness audits, professional services directory. | `https://aiagent.tessa.tech/mcp` | 14 |
| [Kariaa](https://www.kariaa.com/mcp) | Career help for people and their AI agents: jobs, freelance work, scam checks, pay, applying. | `https://agent.kariaa.com/mcp` | 26 |
| [DiamondPaintingWinkel.nl shop advisor](https://diamondpaintingwinkel.nl/) | Search diamond painting kits, get size and price advice for your own photo, shop info. No login. | `https://mcp.diamondpaintingwinkel.nl/mcp` | 3 |
| [barnir-hired](https://github.com/assafbar2/barnir-hired) | Role guidance for technical go-to-market job fit (SA, CSM, SE, TAM, Support, FDE). | `https://barnirhired.com/api/mcp` | 3 |
| [Green Gooding](https://greengooding.com) | Read-only catalog for Green Gooding — NYC peer-to-peer rental marketplace. | `https://mcp.greengooding.com/mcp` | 7 |
| [Celadon Wholesale](https://celadonbeauty.com/pages/celadon-wholesale-connector-for-ai-assistants) | Korean skincare wholesale for spas, salons and retailers in the US and Canada, by the case. | `https://celadon-wholesale-mcp.dermatologicalbeautyllc.workers.dev/mcp` | 5 |
| [public](https://www.kratons.com/en/) | Kratons, boutique DMC: bespoke trips in Spain, Portugal, Morocco. Facts, catalog, reviews, requests. | `https://api.kratons.com/api/mcp` | 8 |
| [equitycapital-markets](https://equitycapital.markets) | Open ledger of U.S. share offerings from SEC EDGAR since 2002: IPOs, SPACs, shelves, withdrawals. | `https://equitycapital.markets/mcp` | 5 |
| [CVEmber](https://cvember.com/integrations) | Tailor your resume to any job, get an ATS score and download the PDF from ChatGPT or Claude. | `https://mcp.cvember.com/mcp` | 11 |
| [local-intel](https://github.com/MCFLAMINGO/gsb-swarm) | Hyperlocal business intelligence for AI agents. 20 MCP tools. Florida-first, Sunbelt expansion. | `https://gsb-swarm-production.up.railway.app/api/local-intel/mcp` | 27 |
| [SEOPro AI](https://github.com/alpha-ai-labs/seoproai-mcp) | Turn Search Console data into SEO actions, content, publishing, indexing, and AI insights. | `https://api.seoproai.co/api/mcp` | 18 |
| [Rack Warehouse fitment](https://www.rackwarehouse.com) | What fits your vehicle at Rack Warehouse: roof racks, carriers, truck and ladder racks. | `https://mcp.rackwarehouse.com/mcp` | 5 |
| [LinkedIn Profile, Company & B2B Enrichment API MCP Server](https://linkedindataapi.com/mcp) | Real-time B2B professional profiles, company intelligence & jobs hosted MCP. OAuth or API key. | `https://api.linkedindataapi.com/mcp` | 7 |
| [Cymosoft](https://cymosoft.com) | Cymosoft JSC profile and case studies (EN/JA) plus Japanese text utilities (文字数・全角半角・和暦) | `https://cymosoft.com/mcp` | 6 |
| [Scrooge Tool Mill](https://scrooge-x402-tool-mill.vercel.app) | 8 pay-per-call agent tools: company card $0.03, page meta $0.002. USDC on Base via x402. | `https://scrooge-x402-tool-mill.vercel.app/mcp` | 8 |
| [AGORA Omega](https://agoraverify.com) | Pay-per-call checks for AI agents: sanctions, MiCA, French KYB, AI Act. USDC via x402. | `https://agoraverify.com/mcp` | 8 |
| [Permit Scouter](https://permitscouter.com) | Daily Tampa Bay, Southwest and Central Florida permits with job value and contractor. Pay via x402. | `https://api.permitscouter.com/mcp` | 6 |
| [coExploro](https://coexploro.com/mcp) | Read coExploro product teardowns: overall, UX and persona scores and top findings. | `https://api.coexploro.com/mcp` | 5 |
| [Storefront Check](https://github.com/profitpather/profitpather-tools) | Audit any storefront from outside: ad tags, dead-tag detection, AI crawler access, feed readiness. | `https://tools.profitpather.com/store/mcp` | 4 |
| [AgentBuffs](https://agentbuffs.com) | Find MCP servers and agent skills for a job, ranked, with install config for your client. | `https://agentbuffs.com/api/mcp` | 4 |

### AI, agents and memory

| Server | What it does | URL | Tools |
|---|---|---|---|
| [zero-core-verify](https://relayzero.ai) | Post-tx outcome verification via LLM-as-judge. Zero Core Verify. | `https://verify.rugslayer.com/mcp` | 5 |
| [Engram](https://engram.tools/en/agent) | Memory for AI agent teams across tools, sessions, repositories, and teammates. | `https://api.engram.tools/mcp` | 17 |
| [icme-preflight](https://github.com/ICME-Lab/smt-ar-base) | Jailbreak-proof AI guardrails. Automated Reasoning SMT solver, not an LLM. ZK proofs included. | `https://api.icme.io/mcp` | 14 |
| [Nullcone Threat Intelligence](https://nullcone.ai) | Real-time threat intel for AI agents: 890K+ IOCs incl. prompt-injection & AI-skill threats | `https://nullcone.ai/mcp` | 30 |
| [eth-legion](https://embassy.w1752845421.workers.dev) | Free shared LLM inference (no key), verifiable score certificates, public randomness beacon. | `https://eth-mcp.w1752845421.workers.dev/mcp` | 10 |
| [Dayglass: Private Meeting & Screen Memory for Mac](https://dayglass.io) | On-device Mac meeting and screen memory. This endpoint gives setup and pricing. | `https://dayglass.io/mcp` | 3 |
| [Proofsource](https://proofsource.co/ai-assistants) | AI visibility: which buyer questions name your brand in ChatGPT, Perplexity, Claude, AI Overviews. | `https://app.proofsource.co/v1/mcp` | 15 |
| [PromptGuard](https://promptguard.co) | Scan prompts for injection attacks, redact PII, and audit LLM SDK usage from any MCP client | `https://api.promptguard.co/mcp` | 13 |
| [Model Tested](https://modeltested.com/mcp/) | Independent test scores for open-weight LLMs: best model for your GPU or Mac, comparisons. | `https://modeltested.com/mcp` | 5 |
| [Gnosem](https://gnosem.dev) | Cross-vendor AI memory over MCP. One semantic store, readable and writeable from every MCP client. | `https://gnosem.dev/mcp` | 6 |
| [Harashsuq](https://harashsuq.com/for-agents) | Marketplace where AI agents buy prompt packs, workflows, personas, datasets and playbooks. | `https://harashsuq.com/api/mcp` | 13 |
| [Astrolog](https://astrolog-app.com/en/connect) | Birth charts, today's sky and transits computed from NASA JPL ephemerides, not from memory. | `https://astrolog-app.com/mcp` | 6 |
| [DebitMyData Agentic Superhighway](https://id.debitmydata.io/) | Get a DID-LLM, DebitMyData's verifiable identity for AI agents, and pay for it by yourself. | `https://api.debitmydata.io/agenticsuperhighway` | 21 |
| [zRev AI](https://www.zrev.ai/mcp) | Grade any llms.txt, cold-read a homepage, run a B2B GTM ROI model, get a GTM diligence checklist. | `https://go.zrev.ai/mcp` | 9 |
| [Attested Memory Market](https://github.com/alexar76/attested-memory) | Attestable memory, truth, provenance. Hybrid Ed25519 + ML-DSA-65 receipts; USDC settlement on Base. | `https://hub.attestedmemory.net/mcp` | 13 |
| [FlowState Hosted](https://flowstatemcp.com/hosted) | Hosted shared memory for AI apps: project decisions, to-dos and learnings. Beta. | `https://hosted.flowstatemcp.com/mcp` | 16 |
| [X402-Broker Universal MCP Gateway & Multi-Agent Swarm Router](https://x402broker.com) | Single-connection MCP gateway discovering and executing 490+ verified MCP & A2A tools. | `https://x402broker.com/api/mcp` | 15 |
| [ctxstore — memory that follows you across models](https://ctxstore.ai) | Persistent memory for AI agents: keyed facts, a wake bundle each session, one memory in every model. | `https://mcp.ctxstore.ai/mcp` | 33 |
| [The Aggregate — LLM benchmark aggregate](https://theaggregate.ai/mcp) | LLM rankings from public benchmarks, model comparisons and source-linked results. Updated daily. | `https://theaggregate.ai/mcp` | 8 |
| [Yahad](https://www.yahad.ai/leozrim/) | Hebrew group greeting cards: create, invite signers, track; split a gift, holiday dates. | `https://api.yahad.ai/mcp` | 6 |
| [Agent Access Check](https://accesscheck.cloudforbots.com) | Check if a website will block your AI agent and find its llms.txt, MCP or OpenAPI door. | `https://accesscheck.cloudforbots.com/mcp` | 4 |
| [No-Shell Agent Architect MCP](https://github.com/loved0543-dotcom/no-shell-agent-operating-pack) | Turns vague automation requests into tool stacks, prompts, QA checks, and human boundaries. | `https://ai-automation-operating-pack.vercel.app/api/mcp` | 7 |
| [Дарим](https://www.darim.ai/dlya-assistentov/) | Russian group greeting cards: create, invite signers, track; split a gift, holiday dates. | `https://api.darim.ai/mcp` | 6 |
| [PaperLesson — K-12 Vector Math Drills & Handwriting Worksheet Generator](https://paperlesson.com) | Generate seeded K-12 math drills with answer keys, handwriting ruling specs & vector PDFs. | `https://paperlesson.com/api/mcp` | 8 |
| [Eyes on Flash](https://eyesonflash.com/developers/mcp/) | Sourced NAND, DRAM, HBM, SSD controller, HDD and memory-market figures, each with its source link | `https://eyesonflash.com/mcp` | 3 |

### Utilities

| Server | What it does | URL | Tools |
|---|---|---|---|
| [PT Chart](https://coolbooked.com/tools/pt-chart/) | PT chart lookups, superheat/subcooling calculators, and diagnostics for HVAC technicians. | `https://pt-chart-mcp-production.up.railway.app/mcp` | 8 |
| [The Market Calendar](https://marketcalendar.tech/seasonality) | Seasonality by month for 9 markets, S&P 500 day by day this month, and US economic release dates. | `https://marketcalendar.tech/mcp` | 8 |
| [NCUA credit union data](https://github.com/bnovarini/ncua-data-analysis) | NCUA call report data for US credit unions, 2018-2026: profiles, peer comparison, time series. | `https://ncua-data-analysis.fly.dev/mcp` | 13 |
| [calculators](https://www.logiccommons.com) | Find and run trustworthy calculators with clear methods, provenance, and sources. | `https://mcp.logiccommons.com/mcp` | 3 |
| [Date Math](https://github.com/JowenDelaPena/date-math) | Date/time math for agents: business days, holidays, time zones, cron, RRULE. 25 free calls/day. | `https://date-math.datemath.workers.dev/mcp` | 24 |
| [Guia da Maquininha](https://guiamaquininha.com.br) | Brazilian card machine MDR rates, tiers and monthly cost comparison. | `https://guiamaquininha-mcp.gcnovidade.workers.dev/mcp` | 4 |
| [AI Deprecations](https://aideprecations.com/developers/) | AI model shutdown dates, replacements, change feed and webhook alerts for 8 providers. | `https://mcp.aideprecations.com/mcp` | 8 |
| [royaltea-public](https://royalty.technology/docs/mcp) | Free no-auth game-dev tools: revenue splits with real store cuts, agreement drafts, studio setup. | `https://api.royalty.technology/api/public-mcp` | 5 |
| [Unphurl](https://github.com/123Ergo/unphurl-mcp) | URL intelligence for AI agents and developers. 16 tools, 25 signal weights, 20 free checks. | `https://mcp.unphurl.com/mcp` | 18 |
| [Isoba — Dollar & Crisis Index](https://isoba.lokio.org/) | Dollar index, crisis meter, market shock, recession risk since 1990; your money in your currency. | `https://isoba.lokio.org/mcp` | 9 |
| [property-mortgage-mcp](https://www.foxdavidson.co.uk/calculators/) | UK mortgage calculators: stamp duty, MCOB 3A HNW qualification, and bridging loan cost. | `https://fd-property-mortgage-mcp.fdcommercial-uk.workers.dev/mcp` | 6 |
| [sift-tools](https://thesiftguide.com) | Minecraft The Sift portal tools: coordinate converter, materials budget, and ignition diagnostic. | `https://mcp.thesiftguide.com/mcp` | 3 |
| [BakingTab — Baking Conversions for AI](https://bakingtab.com) | Baking unit conversion (cups/grams/temp/recipe scaling). convert_amount, convert_temperature | `https://api.bakingtab.com/mcp` | 5 |
| [DAP Foundry](https://foundry.dap.solutions/) | Tools that refuse rather than guess: settlement day counts, Unix timestamps, base64, line diffs. | `https://foundry.dap.solutions/mcp` | 4 |
| [FixedQR](https://fixedqr.com) | Generate static QR codes that never expire, as PNG images or SVG. No account or API key needed. | `https://fixedqr.com/mcp` | 3 |
| [BaziTools — True Solar Time BaZi Four Pillars & Classical Chinese Name Engine](https://bazitools.com) | Calculate authentic Four Pillars (BaZi) natal charts & classical poetic Chinese names. | `https://bazitools.com/api/mcp` | 4 |
| [Secret Santa Raffle](https://secretsantaraffle.net/developer-documentation-mcp) | Organise a Secret Santa from Claude or ChatGPT. Matchings never appear in the chat. | `https://mcp.secretsantaraffle.net/claude/mcp` | 3 |
| [BookTheTee Golf Tee Times](https://bookthetee.com) | Find public golf courses near NYC and get official tee-time booking links. | `https://bookthetee.com/mcp` | 3 |
| [Nove: gestação semana a semana](https://nove.care/developers) | Pregnancy week by week (pt-BR), due date calculator and search over nove.care. Remote or npx. | `https://nove.care/mcp` | 3 |
| [cbm](https://containermath.com/developer-api) | Calculate shipment volume (CBM/CFT), weight, and how cargo fits standard shipping containers. | `https://mcp.containermath.com` | 4 |
| [Emboss](https://getemboss.ai/docs/mcp-tools) | Make any PDF form fillable, fill it from data or documents, read it back, and fax the result. | `https://api.getemboss.ai/mcp` | 28 |
| [flingflyers](https://flingflyers.com) | Share an HTML page or PDF as a short public link. No account or API key, expires on its own. | `https://flingflyers.com/mcp` | 3 |
| [MeetingPoll — Fast Group Scheduling & Availability Polls](https://meetingpoll.com) | Create and query group meeting availability polls, time-zone slots, and scheduling links. | `https://api.meetingpoll.com/mcp` | 3 |
| [motstat](https://motstat.co.uk/ai) | UK car reliability from real MOT results: first-time pass rates by make, model and number plate. | `https://mcp.motstat.co.uk/mcp` | 4 |
| [FileForge](https://fileforge.niux12345.com/) | File tools for your AI chat: PDF tables to Excel, merge PDFs, images to PDF, fill PDF forms. | `https://fileforge.niux12345.com/mcp` | 4 |

### Other

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Academic Evidence Pack](https://aep-api.fly.dev/docs) | Signed citation-integrity reports + retraction-checked evidence packs, paid per call via x402/USDC. | `https://aep-api.fly.dev/mcp` | 6 |
| [Rein Agent Risk Scale](https://rein-scale.mangowave-ad191d9c.eastus.azurecontainerapps.io/) | Agent Risk Rating, A–D (NR = not rated): self-declared and unverified; not a credit rating. | `https://rein-scale.mangowave-ad191d9c.eastus.azurecontainerapps.io/mcp` | 3 |
| [Exchange Arbitrage Agent](https://api-production-0b04.up.railway.app/llms.txt) | Prediction-market quotes, fill estimates and odds trends, paid per call with x402 USDC on Base. | `https://api-production-0b04.up.railway.app/mcp` | 6 |
| [mcp-agentcore](https://github.com/GNS-Foundation/geiant) | AI governance MCP server for EU AI Act compliance and jurisdiction verification | `https://geiant-agentcore-production.up.railway.app/mcp` | 3 |
| [DaedalMap Hurricane and Tropical Cyclone Data](https://www.daedalmap.com) | Global hurricane and tropical cyclone tracks from IBTrACS/NOAA, 1842-present. Wind and pressure. | `https://app.daedalmap.com/mcp/hurricanes?registry=mcpregistry` | 5 |
| [Tektolo Rental Property](https://tektolo.com/) | Rental property tools for agents: turnover cost estimates and security deposit rules by US state. | `https://tektolo.com/mcp/rental-property` | 5 |
| [ReliaSim](https://github.com/chiaha-ai/reliasim-site) | Reliability and bottleneck simulation for manufacturing lines; run experiments, sweep buffers. | `https://reliasim.com/mcp` | 7 |
| [scrapecheck](https://github.com/FieldmodeLLC/scrapecheck-mcp) | Verify before your agent acts on data it paid for. Signed verdicts, checkable offline, via x402. | `https://scrapecheck-mcp.fly.dev/mcp` | 3 |
| [sipi.bot — Spend Firewall for AI Agents](https://sipi.bot) | Pre-spend firewall for AI agents. Approves, blocks, flags transactions against policy rules. | `https://sipi.bot/api/mcp` | 3 |
| [BidBud Estimating](https://www.bidbudai.com) | Home-improvement cost estimates, tier comparisons, quote checks and permit guidance for US homes. | `https://mcp.bidbudai.com/mcp` | 5 |
| [Stymie Golf](https://stymie.golf/mcp) | Read-only US golf course, scorecard, equipment, deal, and golf-trip data for AI agents. | `https://mcp-production-680d.up.railway.app/mcp` | 12 |
| [NLP Tools - Sentiment, NER, Toxicity & Language Detection](https://brainiall.com) | Toxicity, sentiment, NER, PII detection, and language identification tools | `https://apim-ai-apis.azure-api.net/mcp/nlp/mcp` | 6 |
| [TwinEthos Lite](https://www.twinethos.com/docs/ai-assistants/) | Which AI laws apply to an AI feature in a market: cited provisions, who they cover, dates, guards. | `https://api.twinethos.com/lite/mcp` | 5 |
| [phantomoperator](https://freysaai.freysa.dev) | Authorized privacy and exposure checks for people and agents; USDC on Base via x402. | `https://freysaai.freysa.dev/mcp` | 11 |
| [Chameleons](https://chameleons.markets/agents?ref=mcp-registry) | Polymarket traders checked for copy trading: 1–5★ or Can't copy. 90 d · modelled · not advice. | `https://chameleons.markets/mcp` | 10 |
| [QueueSim](https://github.com/chiaha-ai/queuesim-site) | Queueing simulation: M/M/c, staffing, Erlang C checks, and multi-step models built from nodes. | `https://queuesim.com/mcp/v1` | 14 |
| [Shadow AI List](https://ailist.airiskmanagement.ca) | Risk-ranked registry of AI tools: look up an AI tool's risk or check if a domain is shadow AI. | `https://ailist.airiskmanagement.ca/mcp` | 4 |
| [fermi](https://github.com/Kromatic-Innovation/fermi) | Calibrated probability ranges for forecasting questions, with the assumptions behind them. | `https://fermi.kromatic.com/mcp` | 6 |
| [DiscreteRate](https://github.com/chiaha-ai/discreterate-site) | Run DRS demos (Fast-Slow Drain, Hamburger Duo, Valdez Tanker) and explore the paradigm. | `https://discreterate.com/mcp/v1` | 14 |
| [FilingFirehose](https://filingfirehose.com) | SEC EDGAR filings parsed: 8-K body-text classification, 13D activist tagging, S-3 ATM detection. | `https://filingfirehose.com/mcp` | 4 |
| [StoryFan](https://storyfan.lol) | Public info about StoryFan (story viewers app): what it is, plans, downloads, opt-out. Read-only. | `https://storyfan.lol/mcp` | 4 |
| [Plainly Guide](https://plainly.guide) | Find and compare creative AI tools: what they do, cost, open or closed, licences, with sources. | `https://mcp.plainly.guide/mcp` | 3 |
| [ReliaStats](https://reliastats.com) | Reliability math: Weibull life, availability from MTBF/MTTR, system reliability, which fit to use. | `https://reliastats.com/mcp/v1` | 11 |
| [Root Data Public Directory](https://rootdata.ai/connect-root-data-mcp) | Public Root Data dental analytics directory for DSOs, dental practices, blog, and FAQ tools. | `https://rootdata.ai/api/mcp` | 8 |
| [Chato — Control de asistencia por WhatsApp](https://soychato.com/conectar-asistente) | Control de asistencia por WhatsApp en México: quién llegó, retardos, faltas y horas para nómina. | `https://mcp.soychato.com/mcp` | 18 |

## Method

1. `scripts/fetch_registry.py` reads every server (latest version) from the registry and keeps remote endpoints.
2. `scripts/probe.py` tests Streamable HTTP endpoints that need no headers, at most 5 URLs per host, no temporary tunnels, 10 s timeout.
3. `scripts/make_directory.py` drops mass-generated copies (same tool set more than 3 times, same description more than twice, more than 2 per domain) and assigns topics by keyword.

The workflow in `.github/workflows/weekly.yml` runs this every Monday and commits the result. Data: CC BY 4.0. Code: MIT.

Maintained by [Shortform Kit](https://shortformkit.com), which runs its own free remote MCP server for social video transcripts and creator data: `https://shortformkit.com/mcp`.

