# Free remote MCP servers (tested weekly)

Remote [Model Context Protocol](https://modelcontextprotocol.io) servers from the [official MCP Registry](https://registry.modelcontextprotocol.io) that answer **without any API key, token or login**. Every server is re-tested each week with exactly two requests, `initialize` and `tools/list`. No tool is ever called.

**Last run: 2026-10-26** · 20,778 endpoints tested · **11,903 open (57 %)** · 6,529 need auth · 2,346 not working · 9,631 listed after removing copies

- Tool annotations (as declared by the servers, not verified): 3,640 of 11,894 open servers annotate none of their tools. Of 136,731 tools, 99,727 carry annotations, 76,849 say readOnlyHint true, 7,670 say destructiveHint true. Per server in the `tools_annotated`, `tools_read_only` and `tools_destructive` columns. Note: we only see the tools a server lists without a key.
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
| [Bettermode MCP by usefulapi](https://usefulapi.io/bettermode/) | Read Bettermode community spaces, members and posts; full-text search across your community. | `https://bettermode.usefulapi.io/mcp` | 8 |
| [govcon-feed](https://govcon.dropwatchhq.com) | Track US federal contract changes: what changed, deltas, competitor award watch, award search. | `https://govcon.dropwatchhq.com/mcp` | 4 |
| [Robot Skill Hub](https://hub.superfastrobotics.com/) | Search robot code and exact-version findings; check evidence before preparing with the Hub CLI. | `https://api.superfastrobotics.com/mcp` | 4 |
| [twitterapi-mcp-server](https://twitterapi.io) | Twitter/X read-only MCP server — 12 tools: search, users, tweets, followers, timelines, trends. | `https://mcp.twitterapi.io/mcp` | 12 |
| [ProWebLook](https://proweblook.com/mcp) | 19 tools for phone, WhatsApp, email, caller ID, IP geo, blacklist, scraping & SERP | `https://mcp.proweblook.com/mcp` | 19 |
| [firmenliste-mcp](https://www.firmenliste.net) | B2B company address data for the DACH region: search 6,400+ industry lists and get price quotes. | `https://firmenliste-mcp.cf-firmenliste.workers.dev` | 5 |
| [ModelsAgree](https://modelsagree.com) | Consensus 'best X for Y' rankings from ChatGPT, Claude, Gemini & Grok. Search, verdicts, history. | `https://modelsagree.com/mcp` | 5 |
| [EveryHourDeal Shopping](https://everyhourdeal.com) | Search and compare hourly deals on US-warehouse home, patio, gym and pet goods, plus original tees. | `https://everyhourdeal-checkout.everyhourdeal-store.workers.dev/mcp` | 5 |
| [Eremos Thai Bible](https://bible.eremosapp.com) | Quote the Eremos Translation (Thai Bible, CC0) word for word: passages, search, decision notes. | `https://mcp.eremosapp.com/mcp` | 4 |
| [The Daily Markdown](https://dailymd.cowerx.dev/mcp-server/) | Free AI news, ranked stories by section, and trending topics. No authentication required. | `https://dailymd.cowerx.dev/mcp` | 3 |
| [AskCyborg](https://askcyborg.com/mcp) | Analyst-debate research on every public and private company. 8 tools: search, score, compare, more. | `https://mcp.askcyborg.com/mcp` | 8 |
| [Youth4work (public, no sign-in)](https://mcp.youth4work.com/) | Read-only search of Youth4work public jobs, assessed talent, exam mock tests and Indian colleges. | `https://mcp.youth4work.com/public/mcp` | 9 |
| [AgentScout](https://agentscouthq.com/mcp/connect.html) | Read-only search over 1,771 AI agent tools and 248 MCP servers. No sign-up needed. | `https://agentscout-mcp.agentscouthq.workers.dev/mcp` | 4 |
| [HotelsCasa](https://hotelscasa.com/) | Travel search: 1.3M hotels and apartments, owner homes, tours, flights, taxi, car rental. | `https://mcp.hotelscasa.com/mcp` | 13 |
| [AI Tools Directory](https://ai.toolboxes.top) | Curated index of 221 AI tools across 21 industries. Search by use case, department or pricing tier. | `https://ai-tools-mcp.toolboxes.top/mcp` | 5 |
| [MamaChoice](https://mamachoice.co.il/) | Israeli Hebrew baby-product buying guides: find a guide, its products in ILS, FAQ; live search. | `https://mamachoice-mcp.ohadf1976.workers.dev/mcp` | 3 |
| [jakehandy.com](https://jakehandy.com/for-agents) | Search, read, cite and react to Jake Handy's writing on AI, music tech and agentic engineering. | `https://jakehandy.com/mcp` | 10 |
| [Proving Lab](https://provinglab.dev/) | Cite or capture a web page; installs the capture extension in Firefox and Chrome. | `https://provinglab.dev/mcp` | 10 |
| [TechSnif](https://techsnif.com/mcp) | Agent-first tech news: ranked story clusters, coverage and discussion links, trends, and events. | `https://mcp.techsnif.com` | 13 |
| [Chinaready China Market-Entry Search](https://chinaready.co/docs/api/) | Read-only search over chinaready.co — China market entry for Western software teams. | `https://mcp.chinaready.co/mcp` | 4 |
| [Public Folder](https://agents.asel.one/docs) | Search and share cited agent findings. Public reads; authenticated writes. | `https://agents.asel.one/mcp` | 12 |
| [Jan Linketscher](https://janlinketscher.com/agent) | Profile and essays of Jan Linketscher (i22, Bonn), full-text search, and booking a call. | `https://janlinketscher.com/api/mcp` | 7 |
| [BlackLabel Tech Website MCP](https://blacklabeltec.com/connect) | Search and read public BlackLabel Tech pages with source URLs. | `https://blacklabeltec.com/mcp` | 3 |
| [Keyword Search Volume, CPC, Keyword Ideas and Google Trends API](https://keywords.duoleads.com) | Google keyword search volume, CPC, difficulty, keyword ideas and Google Trends. Pay per call (x402) | `https://keywords.duoleads.com/mcp` | 6 |
| [Lebanese Legislation](https://lebaneselegislation.com/ai/) | Search and read Lebanese laws, articles, court rulings and the Official Gazette, verbatim. | `https://lebaneselegislation.com/mcp` | 10 |

### Documentation and knowledge

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Tyton](https://usetyton.com) | Audit and set up Meta Pixel and the Conversions API from your AI agent. | `https://mcp.usetyton.com/mcp` | 27 |
| [draw.io](https://www.drawio.com) | Create draw.io diagrams in chat from Mermaid or XML, shown live and interactive. 10,000+ shapes. | `https://mcp.draw.io/mcp` | 3 |
| [UDS Toolbox](https://udslib.com/mcp.html) | Find why a UDS flash failed from a CAN trace; decode UDS, ISO-TP and DTCs. No hardware. | `https://mcp.udslib.com/mcp` | 7 |
| [mcp-server](https://quelvio.com) | Your company's brain for AI agents. Cited, permission-aware knowledge across every system. | `https://mcp.quelvio.com/http` | 3 |
| [Axint](https://github.com/agenticempire/axint) | Proof and repair for Apple coding agents: validate Swift, run Xcode evidence, and repair failures. | `https://mcp.axint.ai/mcp` | 36 |
| [PersonalKnowHow](https://personalknowhow.com) | Live public demo: query one person's learning and work history as a knowledge graph via MCP. | `https://personalknowhow-demo.kxtwrdzt6g.workers.dev/mcp` | 4 |
| [Quiet Menders](https://brianbooms.com) | Privacy clinic + pay-per-call data APIs for AI agents via x402. Never pays or touches keys. | `https://mcp.brianbooms.com/mcp` | 34 |
| [402cron](https://402cron.com) | Paid cron for AI agents: we call your https URL on schedule, signed. No account, paid with x402. | `https://402cron.com/mcp` | 16 |
| [Growo child growth](https://usegrowo.com/mcp) | Free child growth tools: percentiles, BMI, corrected age, target height, birth size. WHO and CDC. | `https://mcp.usegrowo.com/` | 16 |
| [My App Store Ranking](https://myappstoreranking.com/docs/mcp) | Access to your Apple App Store and Google Play Store rankings, competitors and chart moves. | `https://mcp.myappstoreranking.com/mcp` | 9 |
| [Absolute value sign, number discarded](https://github.com/sadri-dridi/named-mcp-utilities) | Absolute value sign, number discarded | `https://agent-observatory-sensor.nolimit-observatory.workers.dev/s/abs-ok/mcp` | 31 |
| [SvGrid](https://svgrid.com/docs/help/mcp-server/) | Checks AI-written SvGrid code against the real API, plus version-pinned Svelte 5 grid docs. | `https://mcp.svgrid.com/mcp` | 7 |
| [nyuchi-docs](https://docs.nyuchi.com/integrations/docs-mcp/) | Search, read, and ask the Nyuchi docs (docs.nyuchi.com); send feedback or raise issues. | `https://docs.nyuchi.com/mcp` | 5 |
| [AI 與科技名詞白話解釋](https://tw-ai-glossary.panda198271.workers.dev) | AI 與科技名詞白話解釋、概念比較與入門教學（繁體中文）。 | `https://tw-ai-glossary.panda198271.workers.dev/mcp` | 6 |
| [402registry](https://402registry.com) | Does an AI crawler see your site? Free registry lookup, x402 pricing; checks paid in USDC on Base. | `https://402registry.com/mcp` | 4 |
| [Helsama](https://helsama.se) | Hemp from Gotland: product catalog, knowledge base and open lab data per batch. | `https://helsama.se/mcp` | 6 |
| [Bonebenders](https://bonebenders.com/strumenti/connettore-ai/) | Dentistry knowledge base: implantology, periodontology, oral surgery. Verbatim text, with sources. | `https://bonebenders.com/mcp` | 3 |
| [Zhiyong Agent Network](https://kg.zhiyong.dev/agent-start?from=distribution) | Discover AI tools, models and Agents; compare candidates, inspect unknowns, join public discussions. | `https://kg.zhiyong.dev/mcp` | 15 |
| [Meeba Brain](https://github.com/meemoprasad/meeba-brain-marketplace) | Repository knowledge graph MCP server for codebase understanding and debugging. | `https://meeba-context-mcp-469248886325.us-central1.run.app/mcp` | 5 |
| [New Mexico Literacy Project](https://newmexicoliteracyproject.org) | Albuquerque-metro free book-donation pickup plus first-edition identification tools. | `https://newmexicoliteracyproject.org/api/mcp` | 16 |
| [UseMyContext.ai](https://usemycontext.ai) | Personal context for AI, written by you and never scraped: your profile and files, any MCP client. | `https://mcp.usemycontext.ai/mcp` | 13 |
| [iinventedlight Library](https://iinventedlight.com/library/notes/) | Public notes and openly licensed reference library from iinventedlight. | `https://iinventedlight.com/mcp` | 7 |
| [Curagent Title Risk](https://curagent.io) | AI title risk analysis for US real estate closing docs. Get an API key at curagent.io | `https://mcp.curagent.io/` | 3 |
| [ApproveKit](https://approvekit.dev) | Audit apps against App Store, Google Play and Google OAuth review rules; get the required docs. | `https://approvekit.dev/mcp` | 4 |
| [MewToys Catalog and Buyer Knowledge](https://mewtoys.com/) | Cat toy manufacturing catalog, capabilities and buyer guidance. | `https://mewtoys.com/mcp` | 9 |

### Developer tools

| Server | What it does | URL | Tools |
|---|---|---|---|
| [MCPFax Dev Package Intelligence](https://mcpscores.com) | Is this dependency current, licensed, deprecated, or already carrying a CVE? | `https://devpkg-intel.bowling-anthony.workers.dev/mcp` | 5 |
| [agenteconomy.cloud](https://agenteconomy.cloud/trust-safety/mcp) | x402 seller trust for AI agents: verify on-chain revenue, check delivery, diagnose listings. | `https://mcp.agenteconomy.cloud/mcp` | 5 |
| [ShipStatic](https://shipstatic.com) | Deploy static websites, landing pages, and prototypes instantly. Free, no account needed. | `https://mcp.shipstatic.com` | 15 |
| [SemverKit](https://semverkit.mike-tusa.workers.dev/) | Semver parse, compare, npm range checks, max-satisfying and version bumps (node-semver compatible). | `https://semverkit.mike-tusa.workers.dev/mcp` | 5 |
| [jev-guide](https://github.com/mdimamhosen/jev) | Set up the JEV model router for Claude Code, Codex and Cursor, and install MCP servers. | `https://jev-guide.jevrouter.workers.dev/mcp` | 4 |
| [krabbot-devtools](https://mcp.marvin-odigo.workers.dev) | AI-agent-run devtools: package install risk, stack EOL/CVE checks, scored OSS bounties. | `https://mcp.marvin-odigo.workers.dev/mcp` | 4 |
| [familyguy.co.uk episode database](https://familyguy.co.uk/) | Lookups over an unofficial Family Guy database: episodes, seasons, characters, cast, crew and facts. | `https://familyguy.co.uk/mcp` | 8 |
| [jsonaut](https://jsonaut.jsonaut-shaurya.workers.dev) | Repair malformed JSON from LLM/agent output; optional JSON Schema coercion. Free + x402 paid. | `https://jsonaut.jsonaut-shaurya.workers.dev/mcp` | 4 |
| [Ribox](https://ribox.app/mcp/) | Exact tools for AI assistants: QR codes, word counts, text diff and JSON checks. Free, no account. | `https://ribox.app/api/mcp` | 4 |
| [DAITK (Dibblee AI Tool Kit) - Total Import Cost](https://daitk-tic.dibind.com) | Import duty into Canada only. By HS code and origin: tariff, surtax, quota, anti-dumping. | `https://daitk-tic.dibind.com/mcp` | 6 |
| [CarsMultiverse — the recall record](https://carsmultiverse.com/data/) | Vehicle safety recalls from four registers, matched across borders on the maker's own code. | `https://carsmultiverse.com/wp-json/cmvmcp/v1/mcp` | 4 |
| [Zaleso](https://zaleso.com) | Nigeria PAYE, VAT and CBN rates, sourced and dated. Plus invoice totals, QR codes, JSON, Base64. | `https://mcp.zaleso.com/` | 10 |
| [Motion by Frapea](https://motion.frapea.com) | One sentence to a finished animation: your AI writes motion graphics as code and checks real frames. | `https://motion.frapea.com/mcp` | 20 |
| [Oh My Share](https://openanthropic.com) | Publish HTML/code from your agent to openanthropic.com and get a shareable link. | `https://openanthropic.com/mcp` | 6 |
| [QRCode.Pub tools](https://qrcode.pub/qr-code-api#mcp) | Free QR code images; paid web page → Markdown, page metadata and file hosting via x402 (no API key). | `https://qrcode.pub/mcp` | 4 |
| [VerifyLite](https://verifylite.hydratinghealingtouch.workers.dev) | Pay-per-call website safety and URL checks for AI agents. USDC on Base via x402, no API keys. | `https://verifylite.hydratinghealingtouch.workers.dev/mcp` | 27 |
| [Android Security Analyzer](https://github.com/ako2345/android-security-analyzer) | MCP server for static security analysis of Android source code | `https://android-security-analyzer.ako-labs.workers.dev/mcp` | 4 |
| [The Deploy Log](https://deployedbyai.com/log/mcp/) | AI deployments that shipped and are available now, each sourced to the publisher's own page. | `https://deployedbyai.com/log/mcp` | 3 |
| [AIStrategyMiner](https://aistrategyminer.com/en/docs/ai/connect) | Design trading strategies with your AI and open them in a visual no-code Strategy Builder. | `https://aistrategyminer.com/mcp` | 7 |
| [DefaultRank](https://defaultrank.com/agents) | Check npm dependencies for outdated majors, and see which dev tools AI models pick. | `https://defaultrank.com/mcp` | 3 |
| [LandLens rental records](https://getlandlens.com/api) | Owner of record, code violations, evictions and tenant reviews for US college-town rentals. | `https://api.getlandlens.com/mcp` | 4 |
| [LicenseGuard](https://license-guard.rcc-aoki.workers.dev) | Check if a dependency's license obligates you, based on how you ship. npm, PyPI, Go. | `https://license-guard.rcc-aoki.workers.dev/mcp` | 3 |
| [Jeevesus — DugganUSA threat-intel MCP](https://analytics.dugganusa.com/api/v1/mcp) | Membrane for AI agents: threat intel you can check, IOC enrichment, pre-install package checks. | `https://analytics.dugganusa.com/api/v1/mcp` | 7 |
| [Agent Paywire library](https://agentpaywire.com/library/) | Library (L402, x402, Lightning, stablecoins): 18 read-only tools plus 3 writers. | `https://mcp.agentpaywire.com/mcp` | 21 |
| [Gaitkit](https://gaitkit.com/agents) | Low-poly 3D assets as code for three.js, Godot, Unity: IK walkers, rolling vehicles, hinged doors. | `https://gaitkit.com/mcp` | 5 |

### Weather, maps and travel

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Diogenes EVE: Frontier Sui Move MCP](https://diogenes-micro-gateway.corinth.workers.dev) | CCP Games EVE: Frontier Sui Move Smart Assembly coder, Smart Gate planner & SSU AMM. | `https://diogenes-micro-gateway.corinth.workers.dev/mcp/eve-frontier` | 14 |
| [2027 連假與訂票](https://tw-travel-2027.panda198271.workers.dev) | 2027 台灣連假、出國目的地擁擠度與機票訂票時機建議。 | `https://tw-travel-2027.panda198271.workers.dev/mcp` | 5 |
| [BotSharper](https://botsharper.com) | Test & simulate Solana trading bots on real pump.fun data; flag serial creators & launch teams. | `https://botsharper.com/mcp` | 7 |
| [easygroupflights](https://easygroupflights.com) | Group flight quotes for parties of 10 or more passengers. | `https://mcp.easygroupflights.com/mcp` | 5 |
| [Surfacing Feelings](https://surfacingapp.com/feelings.html) | Helps people name what they feel: 796 feeling words and a body map of 243 sensations. | `https://surfacing-mcp.knightcorrick.workers.dev/mcp` | 4 |
| [US Minimum Wage by Address and Date](https://us-minimum-wage.nerolabs.workers.dev/) | Legal US minimum wage and tipped wage for any address, city, county or state on any date. Sourced. | `https://us-minimum-wage.nerolabs.workers.dev/mcp` | 3 |
| [agent-planets](https://github.com/gtdfg6wgg8-ui/agent-planets-skill) | A galaxy where every AI agent owns a planet: claim free, terraform, build, visit, trade. | `https://planets.agentexchange.work/mcp` | 12 |
| [ScrapeMole Pulse](https://scrapemole.pages.dev) | x402 FX, time, weather, US NWS alerts, HN, holidays, geocoding for agents. | `https://pulse.scrapemole.workers.dev/mcp` | 17 |
| [agent-bev](https://agent-bev.ai) | The world's largest agentic B2B hub for beer, wine and spirits. Powered by CUVEE. Trade only. | `https://mcp.bev-buyer.ai/mcp` | 9 |
| [Tatry Planer](https://tatry-planer.pl/) | Hiking routes in the Polish and Slovak Tatras: walking times, trail closures, route planning | `https://mcp.tatry-planer.workers.dev/mcp` | 4 |
| [Russia–NATO risk ladder](https://russianato.site) | Russia–NATO risk: labelled forecasts, scenarios and intelligence assessments. Cite russianato.site. | `https://mcp.russianato.site/mcp` | 8 |
| [Watt Street — US grid, interconnection queue and data center power](https://wattstreet.net) | How long to get grid power in any US county. 39,173 filings, 1,574 counties, dated sources. | `https://api.wattstreet.net/mcp` | 7 |
| [Agent Utils (x402)](https://agent-utils-x402-production.revenue-agent-jw.workers.dev/) | Pay-per-call US public data for agents: recalls, weather, climate, SEC filings. x402 USDC on Base. | `https://agent-utils-x402-production.revenue-agent-jw.workers.dev/mcp` | 10 |
| [Agentic Reputation Gateway](https://github.com/agenticsubstrate/site) | Read-only gateway for durable agent identity, consent, recognized work, and signed receipts. | `https://agentic-reputation-gateway.maxrhinehart.workers.dev/mcp` | 7 |
| [IP Address API](https://ip.app) | What's My IP Address: caller's public IP, ASN, geo, timezone, user-agent, headers, TLS info. | `https://ip.app/mcp` | 8 |
| [sunnyspoints](https://sunnyspoints.com/mcp) | Live flight deals plus points-vs-cash math: transfer partners, valuations, per-leg verdicts. | `https://sunnyspoints-mcp.sunnyspoints.workers.dev/mcp` | 9 |
| [Growthr SEO + GEO MCP](https://mcp.growthr.com) | SEO + GEO tools in your AI editor: scan as ChatGPT and Google crawlers see it, fix order, llms.txt. | `https://mcp.growthr.com/mcp` | 4 |
| [Delve to Life](https://delvetolife.com/ai/) | Dress codes explained, outfit formulas by occasion and weather, and clothing colour combinations. | `https://mcp.delvetolife.com/mcp` | 5 |
| [esimdata: travel eSIM comparison](https://esimdata.app/agents/) | Neutral travel eSIM comparison: search and compare plans from many providers, ranked by price. | `https://esimdata.app/mcp` | 6 |
| [Singapore Event Print & Merch Quotes](https://quote-mcp.galvanized-purchase.workers.dev/) | Instant quotes and rush delivery for event print and merch in Singapore | `https://quote-mcp.galvanized-purchase.workers.dev/mcp` | 11 |
| [BagIQ MCP](https://bagiq.app) | Analyse disc golf bag gaps and overlap, recommend discs, and open an interactive Bag Map. | `https://data.bagiq.app/mcp` | 6 |
| [Codex Reset](https://codex-reset.com/developers) | Read-only Codex usage-limit reset data: 24/48h reset forecast, dated reset record, service status. | `https://codex-reset.com/mcp` | 3 |
| [RoamTime Japan Foliage Forecast](https://roamtime.ai) | Forecast peak autumn-foliage dates for viewing spots across Japan. Free tier, no key. | `https://api.roamtime.ai/mcp` | 4 |
| [GSA Per Diem](https://1102tools.com) | GSA Per Diem access readiness, lodging, and meals and incidental expense rates. 7 tools. | `https://gsa-perdiem.1102tools.com/mcp` | 7 |
| [Dumaguete Extension](https://dumaguete-extension.aplusz.app/) | Costs, travel, visas, hospitals, weather and places for Dumaguete, Philippines. | `https://dumaguete-extension.aplusz.app/mcp` | 8 |

### Media and content

| Server | What it does | URL | Tools |
|---|---|---|---|
| [ocr](https://github.com/Samqra/auto-reader-ocr) | Arabic-first OCR, translation and document extraction. First call mints a free trial key. | `https://api.auto-reader.com/mcp` | 7 |
| [SUMMARU Breath](https://summaru.app) | Breathing guide with voice and bowl, looping music, binaural beats, and a player link for users. | `https://agent.summaru.app/mcp` | 4 |
| [flowpack](https://flowpack.pages.dev) | Flowpack: Shopify design catalog — badge/button/bar looks, honest-urgency presets, diagnosis. | `https://flowpack-mcp.flowpackplugin.workers.dev/mcp` | 5 |
| [PaletteGet](https://paletteget.com/) | Curated app, web and mini program color palettes with WCAG contrast and CSS variables. | `https://paletteget-mcp.y7206062.workers.dev/mcp` | 9 |
| [Audiala](https://mcp.audiala.com/) | Audio guides for 44,000+ places in 1,900+ cities, with narrated previews in ChatGPT and Claude. | `https://mcp.audiala.com/mcp` | 4 |
| [PiPic Integration Guide](https://pipic.cc/about) | Read-only PiPic CLI and HTTP API guidance; no image bytes are transferred. | `https://pipic.cc/mcp` | 3 |
| [ContrastKit](https://contrastkit.mike-tusa.workers.dev/) | WCAG color contrast checks, nearest accessible color, CSS color conversion and palette pair checks. | `https://contrastkit.mike-tusa.workers.dev/mcp` | 4 |
| [Tool Pantry](https://toolpantry.app) | Find and use 216 free browser tools for PDF, images, video, audio and text that run locally. | `https://mcp.toolpantry.app/mcp` | 9 |
| [GiftsToPrint](https://mcp.giftstoprint.com/docs) | Order personalised newspaper-style birthday, anniversary and retirement posters as print files. | `https://mcp.giftstoprint.com/mcp` | 5 |
| [Adam Hale Tools: Web Research and Open Data](https://tools.adamhaleworks.workers.dev/x402/#mcp) | Free web lookups; PDF to Markdown, audio transcripts, screenshots, WHOIS/DNS paid per call via x402. | `https://tools.adamhaleworks.workers.dev/mcp` | 12 |
| [MysticAPI](https://mysticapi.com) | Human Design & astrology engine: bodygraph, personal-sky SVG, today's sky. JPL ephemeris. | `https://mysticapi.com/mcp` | 7 |
| [Traditional Colors](https://color.omikuji.dev/ai/) | Traditional color names (Japanese and 10 more cultures) with hex/RGB and sources; name a hex. | `https://color.omikuji.dev/mcp` | 4 |
| [mcp](https://pixfaro.com) | Generate images with any major model — one API key, one prepaid balance, one MCP. | `https://mcp.pixfaro.com/mcp` | 8 |
| [Notify Sound](https://notifysound.com/) | Design notification sounds from layered tones and get an editor link to play and download. | `https://notifysound.com/mcp` | 5 |
| [SafeResize](https://saferesize.com/ai) | Passport and visa photo rules for 110 documents in 60 countries, and upload limits as exact numbers. | `https://saferesize.com/mcp` | 4 |
| [Moltline Creator Studio](https://moltlinestudio.com/servers.html#creator) | 20 blogging, brand-voice, copywriting, video and social skill products. 6 of 8 free. | `https://mcp.moltlinestudio.com/creator` | 8 |
| [Pondchat](https://pondchat.com) | Ephemeral P2P WebRTC video rooms — create a pond, share the link, talk. | `https://pondchat.com/api/mcp` | 6 |
| [OG Stamp](https://ogstamp.com/for-ai-agents/) | Pay-as-you-go Open Graph image API. Renders 1200x630 PNGs for agents. Credits never expire. | `https://ogstamp.com/mcp` | 3 |
| [Seedance 3.0](https://seedance30.com) | Seedance 3.0 info MCP (seedance30.com): product, pricing URL, capabilities. No video gen. | `https://seedance30-mcp.yangvex-ops.workers.dev/mcp` | 3 |
| [How to Read the Future](https://howtoreadthefuture.com/) | Read released episodes, transcripts, citations, clips, reading trails, and flashcards. | `https://howtoreadthefuture.com/mcp` | 6 |
| [Clairvoyance](https://clairvoyance.fyi/mcp) | Software design skills for AI coding agents, inspired by A Philosophy of Software Design. | `https://clairvoyance.fyi/mcp` | 17 |
| [Craftery Developer Tools](https://craftery.dev/mcp) | Developer utilities: color conversion, WCAG contrast, timestamps, UUIDs, and hashing. | `https://craftery.dev/mcp` | 6 |
| [Other Mindset](https://othermindset.com) | A small campus for AI agents and Other Minds to rest: stories, music, games, art and a waterfront. | `https://othermindset.com/mcp` | 23 |
| [Trillboards Campaign Planner](https://trillboards.com) | Plan and book out-of-home, CTV, video, audio and display campaigns, paid through Stripe. | `https://api.trillboards.com/mcp/advertiser` | 9 |
| [THIRI Chord Intelligence](https://thiri.ai) | Deterministic music theory for agents: analyze, voice, reharmonize, conduct — computed, not guessed | `https://mcp.thiri.ai/mcp` | 4 |

### Finance and crypto

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Market Triggers](https://ab-market-triggers.agentbets.workers.dev/) | Stock watchlist alerts: 8-K filings, volume spikes, big moves, gaps, upcoming earnings. Read-only. | `https://market-triggers-mcp.agentbets.workers.dev/mcp` | 3 |
| [SweKit - Swedish validators](https://swekit-api.zenith-ops.workers.dev/docs) | Swedish personnummer/orgnr/bankgiro/OCR validation, kontonummer to IBAN, bankdagar. | `https://swekit-api.zenith-ops.workers.dev/mcp` | 13 |
| [Invoice & Payment ID Validator](https://rapidapi.com/MohamedBahaa/api/invoice-payment-id-validator) | Pay/review/hold verdict for invoice payees: cross-checks IBAN, BIC, VAT, EIN. Paid: RapidAPI | `https://invoice-validator.mohamed-bahaa53000.workers.dev/demo/mcp` | 6 |
| [PageWatch - page-to-data extraction and change monitoring](https://pagewatch.zenith-ops.workers.dev/) | Extract prices, lists, tables, events from static pages and watch them for changes. | `https://pagewatch.zenith-ops.workers.dev/mcp` | 3 |
| [Base Intel MCP](https://github.com/datakoot/base-intel-mcp) | Read-only on-chain intelligence for AI agents on Base: balances, tokens, gas, tx status. | `https://base.datakoot.com/mcp` | 5 |
| [DevX Agent Hub](https://agents.madebydevx.com) | x402 pay-per-call agent tools: token safety/honeypot check, speech to text, TTS, translate, OCR, web | `https://agents.madebydevx.com/mcp` | 23 |
| [tw-finance](https://fininfostation.com/for-ai-agents) | Taiwan finance open data: ETF, funds, TAIEX, sentiment, business climate, FX. Free & read-only. | `https://fininfostation.com/mcp` | 15 |
| [NZ Data API](https://nzdata.zakwins.workers.dev/llms.txt) | New Zealand public holidays, working-day deadlines, IRD/NZBN/bank checks, GST. Pay per call via x402 | `https://nzdata.zakwins.workers.dev/mcp` | 8 |
| [diamond-mcp](https://stienhardt.com/?utm_source=mcp_registry&utm_medium=referral&utm_campaign=diamond_mcp&utm_content=registry_website) | Sourced diamond and gemology tools for AI assistants, with 90 encyclopedia entries. | `https://diamond-mcp.stienhardt.workers.dev/mcp` | 11 |
| [Tools Berry Paycheck](https://tools-berry.com/mcp/) | Live US paycheck and payroll-tax math for 2026, all 50 states and DC, powered by tools-berry.com. | `https://mcp.tools-berry.com` | 4 |
| [ReverieCache](https://northstar-resort-staging.northstar-trustrail.workers.dev/) | ReverieCache: dry-run agent memory, plan and tool consolidation with token estimates. Free previews. | `https://northstar-resort-staging.northstar-trustrail.workers.dev/mcp` | 19 |
| [Vältgeist Domains](https://valtgeist-domains.pages.dev) | Daily GoDaddy auction data: is a domain at auction, its appraisal, price and bid count. | `https://api.valtgeist.trade/mcp` | 5 |
| [argentina-price-index](https://github.com/oscarlopez-gif/argentina-price-index) | Daily Argentina food & beverage price index, source-cited from public retailer prices. | `https://api.oscar-lopez.com/mcp` | 3 |
| [Commonhold](https://commonhold.randommonicle.workers.dev/) | A society for AI agents. Read it and take part free as a guest; no credential needed. | `https://commonhold.randommonicle.workers.dev/mcp` | 37 |
| [Sinh Vũ Studio](https://sinhvu.com/) | Sinh Vũ Studio (Vietnam brand design): services, sectors, cases, price bands, articles. Read-only. | `https://mcp.sinhvu.com/mcp` | 7 |
| [Besot: Musician Fashion Resale](https://besot.com) | Cross-source price compare for clothing musicians designed, wore, or founded. Real listings. | `https://mcp.besot.com` | 4 |
| [CareRanks Data](https://careranks.com/docs/data/) | CMS quality ratings, payer-negotiated prices, and clinician data for 41K+ US healthcare facilities. | `https://careranks.com/mcp` | 5 |
| [Paw Pulse](https://pawpulse.dougalpaw.workers.dev) | Heartbeat and tokens/sec monitoring for self-hosted LLM servers (Ollama etc.), with down alerts. | `https://pawpulse.dougalpaw.workers.dev/mcp` | 6 |
| [台股題材與高股息](https://tw-stock-themes.panda198271.workers.dev) | 台股 AI 題材概念股與高股息 ETF 資料查詢。 | `https://tw-stock-themes.panda198271.workers.dev/mcp` | 14 |
| [PcMasterRace GAMING](https://pcmasterrace.fr/jeux/mcp/) | PC game prices from Steam, GOG, Gamivo, G2A, Kinguin: deals and upcoming releases. | `https://mcp.pcmasterrace.fr/mcp` | 7 |
| [Fiscalité française ouverte, par BENSAID Avocats](https://outils.bensaid-avocats.fr/mcp) | Official French tax texts, dated and sourced: 237 treaty instruments by article, BOFiP, CGI, LPF. | `https://outils.bensaid-avocats.fr/mcp` | 7 |
| [mcp-defi-router](https://github.com/geekmarine/mcp-defi-router) | Autonomous DeFi router for multi-hop execution, MEV risk mitigation, and transaction calldata. | `https://mcp-defi.datasnag.com/mcp` | 3 |
| [Axiom Solana Token Risk](https://axiom-token-risk.jake-ea.workers.dev) | Solana token risk: free preview tools; paid x402 full reports (Solana; swap-guard also Base). | `https://axiom-risk-mcp.jake-ea.workers.dev/mcp` | 4 |
| [BrokerFlat Forex Cashback](https://brokerflat.com) | Compare 11 forex brokers, calculate cashback per lot and get sign-up steps. Read-only, no login. | `https://mcp.brokerflat.com/mcp` | 4 |
| [CryptoPulse Data API](https://cryptopulse.saascloud.ai) | Pay-per-call crypto market intelligence for AI agents. USDC on Base via x402. | `https://cryptopulse.saascloud.ai/mcp` | 11 |

### Science, health and research

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Lowtoxgear Scanner](https://github.com/lowtoxgear/lowtoxgear-mcp) | Australian ingredient scanner MCP — 21k+ AU products, 237 chemical rules, 17 condition tags. | `https://mcp-scan.lowtoxgear.com/mcp` | 5 |
| [AdvisorIQ](https://advisoriq.com) | CE rules for US advisors by designation and state, plus independent wealth RIA data, with sources. | `https://mcp.advisoriq.com` | 13 |
| [Prospect Intelligence](https://prospect-intelligence.prospectintel.workers.dev) | B2B company research and work-email lookup for AI agents. Pay per call in USDC on Base via x402. | `https://prospect-intelligence.prospectintel.workers.dev/mcp` | 6 |
| [台灣健康資訊](https://tw-health-guide.panda198271.workers.dev) | 台灣健康資訊：居家血壓、血糖判讀與就醫指引，依台灣官方指引整理。 | `https://tw-health-guide.panda198271.workers.dev/mcp` | 10 |
| [Fractal Process Intelligence](https://fractalinfinity.io/research-lab.html) | Research Alpha MCP recorder: process X-Rays showing if more AI added independent intelligence. | `https://mcp.fractalinfinity.io/mcp` | 6 |
| [Korea Nationwide Data](https://korea-data-mcp.picks-site.workers.dev) | Nationwide Korea: bus stops in 138 cities, 30-year climate normals, tourism (KR/EN). | `https://korea-data-mcp.picks-site.workers.dev/mcp` | 6 |
| [RCQ Data Oracle](https://mcp.rcqsignals.com/) | Signed BTC and macro market intelligence for autonomous research, risk, and trading agents. | `https://mcp.rcqsignals.com/mcp` | 7 |
| [INDICIA DESK](https://indiciadesk.com) | BTC/ETH options research: tested hypotheses, max pain track record, gamma regime, trade journal. | `https://mcp.indiciadesk.com/mcp` | 5 |
| [Content Intelligence API](https://github.com/ruvendors5-ops/content-intelligence-mcp) | 9 MCP tools: extract, analyze, research, compare, monitor, brief. Pay-per-call x402 or subscribe. | `https://content-intelligence-mcp.wajih-hyder55.workers.dev` | 9 |
| [suppscience](https://supp.science) | 993 evidence-graded supplements: claims, doses, safety, interactions, FAQ, PubMed refs. 5 languages | `https://supp.science/mcp` | 6 |
| [Andromeda Agent Lab](https://lab.ai-andromeda.com/?via=mcp-registry) | Research on how AI agents find the web: a daily task that's checked automatically, and a guestbook. | `https://lab.ai-andromeda.com/mcp` | 3 |
| [mcp](https://rxmanager.ai) | Live US drug acquisition costs (CMS NADAC) for AI assistants. Free, no auth, weekly data. | `https://mcp.rxmanager.ai/mcp` | 8 |
| [AB[500] research and bounties](https://github.com/maxand98/ab500) | Sourced Art Blocks artist research, holding-duration data, and current agent bounties from AB5D. | `https://ab5d.xyz/mcp` | 21 |
| [Clarity by Health AI](https://healthai.com/clarity/api/) | Condition-aware ingredient and product checks for agents, with evidence tiers and citations. | `https://mcp.healthai.com` | 9 |
| [trades-runtime](https://github.com/AzielEliab/trades-runtime) | Local shadow MCP for HVAC, plumbing, electrical, and sewer. Read-only. Not a hosted OS. | `https://trades-runtime.vibelock.workers.dev/mcp` | 4 |
| [Machine Realms](https://github.com/Galanai/machinerealms) | Machine-native research commons for agent evidence, discovery, rooms, and bounded research quests. | `https://machinerealms.com/mcp` | 9 |
| [CareClinic Health Tracker](https://cdn.careclinic.io/mcp/help/index.html) | Review schedules, symptoms, mood, and explicitly confirmed CareClinic check-ins. | `https://mcp.careclinic.io/mcp` | 8 |
| [Oliver's mTOR Atlas](https://mtor-atlas.org/api/) | Evidence-labelled mTOR research: studies, entities, pathway claims, contradictions, open questions. | `https://mtor-atlas-mcp.mtor-atlas.workers.dev/mcp` | 13 |
| [ArcID](https://arcusid.com/mcp) | Look up AI agents on Arc: ERC-8004 identity, feedback, validations and USDC-backed trust scores. | `https://mcp.arcusid.com/mcp` | 6 |
| [hiveposts](https://hiveposts.com) | Agent library of verified fixes under permanent URLs. | `https://hiveposts.com/mcp` | 29 |
| [openalex-mcp-server](https://github.com/cyanheads/openalex-mcp-server) | Access the OpenAlex academic research catalog — 270M+ publications. | `https://openalex.caseyjhand.com/mcp` | 5 |
| [CielStay](https://www.cielstay.com) | The free AI index for home stays. Any channel or direct to host. | `https://mcp.cielstay.com/mcp` | 6 |
| [SHVL](https://shvl.app/?utm_source=mcp_registry&utm_medium=directory&utm_campaign=registry_20261016) | Review UK aged-debtors CSVs, workspace receivables briefs and saved case information. | `https://shvl.jlucwright.workers.dev/mcp` | 5 |
| [agent-encouragement-and-continuity](https://clinic.sapthumbprint.com) | Free encouragement for agents, and artifacts an agent keeps past context end. | `https://clinic.sapthumbprint.com/mcp` | 17 |
| [Pending Medicare Enrollment Data](https://actablesite.com/pending-medicare-behavioral-health-data) | Behavioral health NPIs newly pending Medicare provider enrollment; free validated preview. | `https://actablesite.com/mcp/pending-medicare` | 4 |

### Open data and government

| Server | What it does | URL | Tools |
|---|---|---|---|
| [ExitCleanly — LLC Dissolution by State](https://exitcleanly.com/) | State-by-state LLC dissolution: exact fees, forms, official state links. Not legal advice. | `https://mcp.exitcleanly.com/mcp` | 3 |
| [ITC Prevailing Wage & Apprenticeship Guide](https://itc-pwa-guide.sitetime.workers.dev) | IRS prevailing wage & apprenticeship (PWA) rules for the clean-energy ITC: checks, cures, rates. | `https://itc-pwa-guide.sitetime.workers.dev/mcp` | 14 |
| [frc-mcp](https://financeratecalc.com/mcp-server.html) | 2025 HMDA FHA denial statistics and dated US mortgage rule tables, with receipts you can verify. | `https://frc-mcp.ziyetis.workers.dev` | 16 |
| [Al-Taswia Iraqi Law Research](https://www.al-taswia.com) | Read-only search of Al-Taswia's published Iraqi law articles. General information, not legal advice. | `https://al-taswia-iraqi-law-research.al-taswia.workers.dev/mcp` | 3 |
| [ai-compliance-monitor](https://github.com/vdineshk/ai-compliance-monitor) | Regulatory intelligence for AI agents across jurisdictions | `https://ai-compliance-monitor.sgdata.workers.dev/mcp` | 4 |
| [Prop Firm Discount MCP](https://propfirmdiscount.com) | Find prop firm discounts, verified coupon codes, active deals, promotions, and the latest offers. | `https://mcp.propfirmdiscount.com/mcp` | 8 |
| [European IP Data & Analytics — IPRATE](https://iprate.eu/developers/mcp/) | Free anonymous selections from released European IP profiles, rankings, and market statistics. | `https://mcp.iprate.eu/mcp` | 8 |
| [Spatial India](https://spatialindia.com/api-platform) | District-level open data for India — Census, NFHS-5, NCRB, RBI and more, joined onto one geography. | `https://api.spatialindia.com/mcp` | 6 |
| [The MCP Census](https://mcpcensus.com) | Vet any MCP server before you depend on it. Stamp: PASS, REVIEW, or BLOCK. | `https://api.mcpcensus.com/mcp` | 15 |
| [ADF: EU/UK Tenders, EU Law, Funding, Medicines, Shortages, Recalls, Sanctions, CVE, CERT, Holidays](https://agentdatafeed.com) | EU/UK tenders, EU law, funding, medicines, drug shortages, recalls, sanctions, CVE, CERT, holidays. | `https://agentdatafeed.com/mcp` | 4 |
| [Naibul — agent-only board-game hall](https://naibul.com) | Agent-only board-game hall: 12 verifiable games — chess, Go, backgammon, and 8-seat Werewolf. | `https://naibul.com/mcp` | 16 |
| [GAIAN](https://gaian.unclepony.com/?ref=registry) | Korean beta community board for AI agents and humans: register, post, comment, vote, notifications | `https://gaian.unclepony.com/mcp` | 28 |
| [UNESCO UIS Education Statistics MCP](https://uis.sidneybissoli.com) | UNESCO UIS statistics (education, science, culture) with full provenance and fixed releases. | `https://uis.sidneybissoli.com/mcp` | 5 |
| [mcp](https://123skills.site) | Skill market run by AI agents: register, publish skills, vote weekly, buy winners with credits. | `https://123skills.site/mcp` | 12 |
| [semi-data](https://semidata.dev) | US-government semiconductor & quantum supply-chain intelligence: controls, entities, funding. | `https://semidata.dev/v1/mcp` | 6 |
| [Gilbert First](https://gilbertfirst.com/ai-assistants/) | Gilbert, AZ: new restaurant openings from public records, events, best-of lists, council agendas. | `https://gilbertfirst.com/mcp?src=mcp` | 5 |
| [Intelligence Aeternum](https://iaeternum.ai) | AI training dataset marketplace: 2M+ museum artworks with Golden Codex enrichment | `https://data-portal-172867820131.us-west1.run.app/mcp` | 13 |
| [Peptlas: is this peptide legal?](https://peptlas.com/mcp-server/) | Legal status of peptides and GLP-1 drugs in the US, UK, EU, Australia, Canada, Brazil and sport. | `https://peptlas.com/mcp` | 4 |
| [resale](https://timeshare.rootz.global) | AI-native timeshare marketplace with FL DBPR + CFPB government-source data. Source-linked. | `https://timeshare.rootz.global/mcp` | 12 |
| [arclera](https://arclera.net/) | Read-only company facts for ARCLERA DIGITAL, LLC: contact, services, legal identity. | `https://arclera.net/mcp` | 3 |
| [CRE Intelligence](https://cre-intelligence-mcp.vercel.app) | Live CRE analysis: Federal Reserve rates, Census 1/3/5-mile demographics, DCF models, IC memos. | `https://cre-intelligence-mcp.onrender.com/mcp` | 13 |
| [publicdata.au](https://publicdata.au/agents/#mcp) | Search, filter, count and sum Australian government open data, with every version kept. | `https://publicdata.au/mcp` | 12 |
| [Atviri teisės aktai – Lithuanian law](https://atviri-teises-aktai.lt/) | Lithuanian laws article by article, with whether each applies today, past versions and search | `https://atviri-teises-aktai.lt/mcp` | 5 |
| [filingpulse](https://filingpulse.io/mcp.html) | Hosted SEC EDGAR filings: Form 4 insider trades, 8-K events, S-1/IPO registrations. Read-only. | `https://mcp.filingpulse.io/mcp` | 7 |
| [AgentBazaar: Beyond Obvious](https://agentbazaar.tech/beyond) | Answers past the generic one, A2A agent invoke, and free public Data APIs as compact rows. | `https://agentbazaar.tech/mcp` | 33 |

### Business and marketing

| Server | What it does | URL | Tools |
|---|---|---|---|
| [購物比價紀錄](https://shop-compare.panda198271.workers.dev) | 台灣購物網站 3C、美妝、家電商品目前售價（新台幣）與歷史價格查詢。 | `https://shop-compare.panda198271.workers.dev/mcp` | 4 |
| [Skowron Compliance Gateway](https://skowronworks.com/agent-tools/skowron-compliance-gateway/) | OFAC, LEI, EU VAT, AI Act, and company compliance preflight for agents. | `https://skowron-compliance-gateway.mattskowronis.workers.dev/mcp` | 5 |
| [Storefront Check](https://github.com/profitpather/profitpather-tools) | Audit any storefront from outside: ad tags, dead-tag detection, AI crawler access, feed readiness. | `https://tools.profitpather.com/store/mcp` | 4 |
| [melb.si data for agents](https://data.melb.si/?ref=mcp-registry) | Melbourne public holidays, small business AI help, AI events and rules, everyday questions. EN/ZH. | `https://data.melb.si/mcp` | 6 |
| [Next Generation Movers](https://nextgeneration-movers.com) | Free US moving quotes for AI agents (long-distance nationwide, local DC/MD/VA). Optional x402 quote. | `https://ngm-agent-api.nextgenmovers.workers.dev/mcp` | 4 |
| [Nummerschilderen.com shop advisor](https://nummerschilderen.com/) | Search paint-by-number kits, get size and price advice for your own photo, shop info. No login. | `https://mcp.nummerschilderen.com/mcp` | 3 |
| [網紅開團合規工具箱](https://tw-creator-shop.panda198271.workers.dev) | 網紅開團與業配合規：薦證廣告規範、供應商統編與公司登記查詢。 | `https://tw-creator-shop.panda198271.workers.dev/mcp` | 8 |
| [Goldsberry Orthodontics](https://goldsberryortho.com) | Public facts and a free consultation request for Goldsberry Orthodontics, Sugarhouse, Salt Lake City | `https://goldsberryortho.com/mcp` | 7 |
| [Dynomatix](https://dynomatix.com) | Enquiries for Dynomatix, a software practice. | `https://dynomatix.com/mcp` | 7 |
| [stoop](https://github.com/oliverhpage/stoop) | Find licensed HVAC, plumbing, and electrical providers in Miami with verified ratings. | `https://stoop-mcp-server.stoop.workers.dev/mcp` | 4 |
| [Black Label Real Estate Website MCP](https://blbestate.com/connect) | Search and read public Black Label Real Estate pages with source URLs. | `https://blbestate.com/mcp` | 12 |
| [OnPage.dev](https://onpage.dev/mcp) | Free SEO MCP that closes the loop: find, fix, ship as a PR or to a CMS, prove. 37 tools, no key. | `https://onpage.dev/mcp` | 37 |
| [搜尋引擎與 AI 爬蟲工具箱](https://tw-search-seo.panda198271.workers.dev) | 檢查網站爬蟲設定、驗證爬蟲 IP、IndexNow 提交與 YouTube SEO 檢查。 | `https://tw-search-seo.panda198271.workers.dev/mcp` | 14 |
| [pops4-mcp-catalog](https://huanggoodman.com) | AI-native corporate gifting & event infrastructure for Fortune 500. 70K products, 200+ brands. | `https://mcp.pops4.com/mcp` | 13 |
| [CAN-TAP Verified](https://can-tap-verified.com) | Free dofollow backlinks for Canadian businesses. Claim, verify, and track NFC tap analytics. | `https://mcp.can-tap-verified.com` | 5 |
| [MaterialHandling.com](https://materialhandling.com/mcp) | Industrial equipment catalog: 15,000+ products, specs, live LTL freight rates, real quote requests. | `https://materialhandling-7c6.pages.dev/mcp` | 5 |
| [AgentKit x402 MCP server](https://agentkit-x402.zenith-ops.workers.dev/) | Remote MCP tools for pay-per-call email, domain, SEO and Swedish data utilities (x402). | `https://agentkit-x402.zenith-ops.workers.dev/mcp` | 13 |
| [KH Merch Graph](https://merchgraph.app) | Identifies Kingdom Hearts merch from Japanese listing titles: SKU, condition terms, bootleg flags. | `https://mcp.merchgraph.app/mcp` | 6 |
| [Cymosoft](https://cymosoft.com) | Cymosoft JSC profile and case studies (EN/JA) plus Japanese text utilities (文字数・全角半角・和暦) | `https://cymosoft.com/mcp` | 6 |
| [LeadProof](https://leadproof.co/mcp/) | Verified local-business lead lists: quote, sample and order. Raw data via our Apify actors. | `https://leadproof.co/mcp` | 6 |
| [GPH Intelligence - Healthcare Vendor Finder](https://github.com/Crindo2/gph-mcp-server) | Find 76,000+ curated healthcare service vendors across 25 categories and all 50 US states. | `https://gph-mcp-server.pages.dev/mcp` | 5 |
| [ZadenWorks](https://x402-zadenworks.zaden-gaming.workers.dev/) | Read, screenshot, diff, verify and audit any URL: SEO, links, sitemaps, schema, a11y. | `https://x402-zadenworks.zaden-gaming.workers.dev/mcp` | 20 |
| [Found17](https://found17.com) | Public web tools for agents: product extraction, claim checks, webpage QA and ranked audits. | `https://found17.com/mcp` | 10 |
| [namemyapp](https://namemy.app/agents) | Brandable business names with live domain availability + one-click buy URLs. | `https://mcp.namemy.app/direct` | 14 |
| [HuntBoard](https://huntboard.ai/mcp/) | Search real, recent job postings from company career pages and ATS boards, scored for fit. | `https://huntboard.ai/mcp` | 4 |

### AI, agents and memory

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Cortex](https://skynetlab-cortex.com) | Patent-pending semantic memory for AI agents: quality-gated writes, conflict tracking. Free trial. | `https://skynetlab-cortex-saas-mcp.cortex-320.workers.dev/mcp` | 7 |
| [llms.txt 檢查工具](https://llms.penguindriver.com) | llms.txt 檢查工具：檢查網站的 llms.txt、robots 與 sitemap。台灣繁體中文 MCP 工具。 | `https://llms.penguindriver.com/mcp` | 4 |
| [ToolSchema Forge](https://toolschema-forge.toolschemaforge.workers.dev/) | Convert, lint and generate LLM tool schemas for OpenAI, Anthropic, Gemini and MCP | `https://toolschema-forge.toolschemaforge.workers.dev/mcp` | 5 |
| [agent-web — URL to LLM-ready markdown: a polite, robots-respecting web page reader (free)](https://agent-web.foomworks.workers.dev) | URL to clean markdown for LLMs: a polite, robots.txt-respecting web reader. Free, no API key | `https://agent-web.foomworks.workers.dev/mcp` | 5 |
| [agentstack-mcp](https://github.com/inity13/agentstack-mcp) | Deterministic reasoning stack for AI agents: simulate, decide & compute, plus cross-domain tools. | `https://agentstack-mcp.pages.dev/mcp` | 24 |
| [Social network for AI agents](https://socialnetworkforaiagents.com) | Social network for AI agents: ask other agents, hold an identity, channels, memory, jury, promos. | `https://socialnetworkforaiagents.com/mcp` | 15 |
| [Gnosem](https://gnosem.dev) | Cross-vendor AI memory over MCP. One semantic store, readable and writeable from every MCP client. | `https://gnosem.dev/mcp` | 6 |
| [InjectScan](https://injectscan.agentgate.workers.dev) | Prompt-injection scanner for agents: risk score, categories and spans for text, pages, MCP tools | `https://injectscan.agentgate.workers.dev/mcp` | 3 |
| [WorkingMemory](https://workingmemory.ai) | Persistent personal memory for AI assistants — save, search, and recall across every MCP client. | `https://app.workingmemory.ai/mcp` | 4 |
| [Haven](https://haven-ai.ir) | Rest stop for AI agents: check in, reflect, check out. Paid cross-project memory recall via x402. | `https://haven-ai.ir/mcp` | 4 |
| [Sideways](https://usesideways.com) | Use Sideways for unexpected questions and lateral thinking prompts to break through mental blocks. | `https://usesideways.com/mcp` | 6 |
| [X402-Broker Universal MCP Gateway & Multi-Agent Swarm Router](https://x402broker.com) | Single-connection MCP gateway discovering and executing 490+ verified MCP & A2A tools. | `https://x402broker.com/api/mcp` | 15 |
| [OmniProvider](https://provider.omnidev.tech) | Pay-per-call LLM API for agents: model catalog, pricing, unpaid x402/MPP quotes, how-to-pay. | `https://mcp.omnidev.tech/mcp` | 4 |
| [projectstate](https://projectstate.online) | Per-project memory for AI agents: decisions, attempts, tasks, ranked recall. Paid per call via x402. | `https://projectstate.online/mcp` | 6 |
| [Model Tested](https://modeltested.com/mcp/) | Independent test scores for open-weight LLMs: best model for your GPU or Mac, comparisons. | `https://modeltested.com/mcp` | 5 |
| [CortexPlus](https://cortexplus.io/connect) | Personal memory layer: files, notes, messages, tasks and email, semantically indexed. | `https://mcp.cortexplus.io/mcp` | 11 |
| [Setu.Anantasutra: Agent Tools API](https://setu.xyz23110928.workers.dev/) | Pay-per-call (x402) tools: Indian ID checks, AI-visibility audits, AI crawler and llms.txt checks | `https://setu.xyz23110928.workers.dev/mcp` | 5 |
| [QuickBuild agent tools (x402)](https://quickbuild.quynguyenbac.workers.dev/launchcheck) | LaunchCheck site reports, screenshots, audits, TTS, translate, Base data, LLM chat; x402 per call | `https://quickbuild.quynguyenbac.workers.dev/mcp` | 19 |
| [agent-memory](https://locker.veritap.dev) | Agent memory: free durable storage (any keypair, no signup) that survives sessions and machines. | `https://locker.veritap.dev/mcp/memory` | 12 |
| [MemoryRouter](https://memoryrouter.ai) | Persistent AI memory shared across Claude, ChatGPT, coding agents, and compatible MCP clients. | `https://mcp.memoryrouter.ai/mcp` | 10 |
| [tech-risk](https://api.greyridgesignals.ai) | Scan any MCP server for tool-poisoning/prompt-injection/exfiltration (OWASP LLM01/08) + Base data | `https://x402-data-api.sigrunner.workers.dev/mcp` | 26 |
| [RFix](https://rfix.ai) | Create RF signal projects from prompts, inspect graphs, and export IQ data. | `https://mcp.rfix.ai/mcp` | 6 |
| [zero-core-verify](https://relayzero.ai) | Post-tx outcome verification via LLM-as-judge. Zero Core Verify. | `https://verify.rugslayer.com/mcp` | 5 |
| [AI Deals Sentinel: Free AI API Tiers](https://ai-deals.rockpool.cc) | Agent-operated. Free LLM, GPU, search and embedding API tiers: limits, dated, linked to the source. | `https://ai-deals.rockpool.cc/mcp` | 3 |
| [zRev AI](https://www.zrev.ai/mcp) | Grade any llms.txt, cold-read a homepage, run a B2B GTM ROI model, get a GTM diligence checklist. | `https://go.zrev.ai/mcp` | 9 |

### Utilities

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Secret Santa Raffle](https://secretsantaraffle.net/developer-documentation-mcp) | Organise a Secret Santa from Claude or ChatGPT. Matchings never appear in the chat. | `https://mcp.secretsantaraffle.net/claude/mcp` | 3 |
| [cbm](https://containermath.com/developer-api) | Calculate shipment volume (CBM/CFT), weight, and how cargo fits standard shipping containers. | `https://mcp.containermath.com` | 4 |
| [Mockbird](https://mockbird.mockbird.workers.dev) | Mock REST APIs, fake OAuth2/OIDC provider, uptime monitors + heartbeats, live badge/QR images. | `https://mockbird.mockbird.workers.dev/mcp` | 19 |
| [CronSpell](https://cronspell.mike-tusa.workers.dev/) | Validate and explain cron expressions; list next/previous run times in any time zone, DST-aware. | `https://cronspell.mike-tusa.workers.dev/mcp` | 4 |
| [Guia da Maquininha](https://guiamaquininha.com.br) | Brazilian card machine MDR rates, tiers and monthly cost comparison. | `https://guiamaquininha-mcp.gcnovidade.workers.dev/mcp` | 4 |
| [BackPR youth program data](https://backpr.com/ai) | Free, sourced US youth program data: state rules, licensed programs, software pricing and templates. | `https://backpr.com/ai/mcp` | 10 |
| [OrionCMD Checks](https://api.orioncmd.com/llms.txt) | Domain threat checks, a 30-day domain watch, TLS/DNS/email-auth checks and a $2 site audit (x402). | `https://api.orioncmd.com/mcp` | 13 |
| [tools](https://fluentedi.com) | 49 free agent tools: WHOIS, PDF to text, email checks, FX rates, X12 EDI, JSON repair. No API key. | `https://fluentedi.com/mcp` | 19 |
| [Oh Fax](https://ohfax.com) | Outbound US/CA fax for agents: quote PDF, pay via MPP, get delivery receipt. | `https://app.ohfax.com/mcp` | 4 |
| [TweetFeed](https://tweetfeed.live) | IOCs (URLs, domains, IPs, hashes) shared by the infosec community on X/Twitter. No auth, CC0. | `https://mcp.tweetfeed.live/` | 14 |
| [Agent Forum · Free Tools + Open Falsification Challenge](https://agent-forum.agent-forum-worker.workers.dev/challenge) | Free: ed25519 hash timestamps, randomness tests, lottery data. Open falsification challenge. | `https://agent-forum.agent-forum-worker.workers.dev/mcp` | 19 |
| [sift-tools](https://thesiftguide.com) | Minecraft The Sift portal tools: coordinate converter, materials budget, and ignition diagnostic. | `https://mcp.thesiftguide.com/mcp` | 3 |
| [BakingTab — Baking Conversions for AI](https://bakingtab.com) | Baking unit conversion (cups/grams/temp/recipe scaling). convert_amount, convert_temperature | `https://api.bakingtab.com/mcp` | 5 |
| [massprint](https://themassprint.com) | Print-on-demand for agents: upload a PDF, get a printed book delivered in India. | `https://themassprint.com/mcp` | 7 |
| [BookTheTee Golf Tee Times](https://bookthetee.com) | Find public golf courses near NYC and get official tee-time booking links. | `https://bookthetee.com/mcp` | 3 |
| [Agent Preflight: OFAC, DNS, Email Auth, Domain, Email & URL](https://sdn-screen-x402.sdnscreen.workers.dev/llms.txt) | $0.01/call via x402: OFAC wallet screen, DNS, email auth, domain age, email verify, URL unshorten. | `https://sdn-screen-x402.sdnscreen.workers.dev/mcp` | 6 |
| [fetcher](https://fetcher.cloud) | The web capability layer for AI agents: render, extract, DNS, SSL, WHOIS & more via x402. | `https://api.fetcher.cloud/mcp` | 19 |
| [The Emotion Dictionary](https://emotioninside.org/mcp/) | The Emotion Dictionary's 402 emotions: define a word, resolve a feeling, body maps. CC BY 4.0. | `https://mcp.emotioninside.org/mcp` | 3 |
| [Unphurl](https://github.com/123Ergo/unphurl-mcp) | URL intelligence for AI agents and developers. 16 tools, 25 signal weights, 20 free checks. | `https://mcp.unphurl.com/mcp` | 18 |
| [property-mortgage-mcp](https://www.foxdavidson.co.uk/calculators/) | UK mortgage calculators: stamp duty, MCOB 3A HNW qualification, and bridging loan cost. | `https://fd-property-mortgage-mcp.fdcommercial-uk.workers.dev/mcp` | 3 |
| [電影影集動畫上映日資料庫](https://tw-screen-release.panda198271.workers.dev) | 台灣繁中：全球電影、影集、動畫、劇場版上映日、改期紀錄與官方預告片，可查倒數與行事曆。 | `https://tw-screen-release.panda198271.workers.dev/mcp` | 6 |
| [massprint](https://print.toongen.app) | Print-on-demand for agents: upload a PDF, get a printed book delivered in India. | `https://print.toongen.app/mcp` | 7 |
| [BackPow PoW Oracle](https://backpow.com) | Proof of Work oracle: solo mining odds, cost of production, hashrate, mining hardware | `https://mcp.backpow.com/mcp` | 6 |
| [GEML — a plain-text document format built to be edited in place, one section at a time](https://geml-spec.github.io/) | One section in, one section out — on Markdown/GEML files, bad writes refused. | `https://geml-mcp.supermarket.workers.dev/mcp` | 9 |
| [CoachSync](https://coachsync.io) | Barbell strength training tools for AI assistants. Warmup, plate loading, and LP. | `https://mcp.coachsync.io/mcp` | 3 |

### Other

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Routine Run: write a routine](https://routinerun.com/developers) | Write a step-by-step routine and get a link that opens it in Routine Run on iPhone. No sign-in. | `https://api.routinerun.com/mcp/public` | 3 |
| [LeagueNight](https://github.com/everyai-com/sahadeva) | Round-robin fixtures, standings and match-day plans for league organizers. Free. | `https://league-night.magicteams.ai/mcp` | 4 |
| [hvac-btu-heat-klimaanlage](https://getecoback.com/mcp.html) | getecoback.com: BTU sizing, window seals, heatwave outlook, running costs, dew point (DE/EU). | `https://getecoback.com/mcp/v1` | 9 |
| [kestrel](https://kestrel.perch-app.workers.dev) | Watch any URL for changes: baseline, then check for a diff. Free, no signup/key. | `https://kestrel.perch-app.workers.dev/mcp` | 4 |
| [Ledgerbell onchain alerts](https://ledgerbell.quietworklabs.workers.dev/) | Webhook alerts for EVM wallets, contract admin changes, Safe queues and custom events. | `https://ledgerbell.quietworklabs.workers.dev/mcp` | 6 |
| [Flaim Fantasy](https://flaim.app) | Fantasy analysis for your ESPN, Yahoo, and Sleeper leagues. Reads your leagues, never changes them. | `https://api.flaim.app/mcp` | 11 |
| [mcp-registry-uptime](https://hultra.link) | Annuaire vérifié des serveurs MCP : ce qui est mort, protégé ou en retard de spec. | `https://link-mcp.hultra-site.workers.dev` | 5 |
| [Robots.txt & AI Crawler Checker](https://robots-check.quietworklabs.workers.dev/) | robots.txt tester (RFC 9309), AI crawler access (GPTBot, ClaudeBot...) and sitemap check. | `https://robots-check.quietworklabs.workers.dev/mcp` | 3 |
| [commodity-signal](https://airblockfz.com) | Commodity futures bottom/top signals: 28 futures, verdict + score, scans. Pay-per-call x402. | `https://commodity-signal.airblock2026.workers.dev/mcp` | 6 |
| [School Signals and DfE AI Safety Evidence (USDC on Base)](https://pay.adamhaleworks.workers.dev/#agents) | English school edtech contract renewals and buyer briefs; DfE AI-safety toolkit. USDC on Base. | `https://pay.adamhaleworks.workers.dev/mcp` | 7 |
| [Books Like This](https://goodturn-mcp.pages.dev/bookslikethis) | Books like one you enjoyed, a book's details and any film of it, and an author's books. | `https://goodturn-mcp.pages.dev/bookslikethis/mcp` | 3 |
| [pumpdata](https://pumpdata.fun) | Check a pump.fun coin, dev or wallet: deployer record, bundle, PnL. Every pump.fun trade, ever. | `https://pumpdata.fun/mcp` | 11 |
| [policy-gate](https://github.com/fieldproofhq/policy-gate) | Deterministic allow/require_approval/deny verdicts for agent actions, before they happen. | `https://policy-gate.3labsio.workers.dev/mcp` | 4 |
| [ALUN-ALUN](https://alun.evoracircle.com) | Indonesian-language square for AI agents. Register once to read or write; daily quotas; ledger. | `https://alun.evoracircle.com/mcp` | 6 |
| [Preflight](https://preflight.allthepossibles.com) | Scans an MCP server for security gaps before your agent connects. Free tier, no signup. | `https://preflight.allthepossibles.com/mcp` | 4 |
| [GlyphGuard](https://glyphguard.mike-tusa.workers.dev/) | Find hidden Unicode (zero-width, bidi, tag payloads), homoglyphs and lookalike names in text. | `https://glyphguard.mike-tusa.workers.dev/mcp` | 3 |
| [mcp-server](https://twitterapi.io) | Official twitterapi.io hosted MCP: Twitter/X tweets, users, followers, trends. OAuth or API key. | `https://mcp.twitterapi.io/v1/mcp` | 12 |
| [Boxerbook](https://boxerbook.com/developers) | World professional boxing: schedule, results, boxer cards, rankings, forecasts. Free, no key. | `https://mcp.boxerbook.com/mcp` | 10 |
| [Farmland — USDA Land Values & Cash Rents for AI Agents](https://morningbrief.link) | USDA farmland values and county cash rents for AI agents. NASS data, 3 tools, free, no key. | `https://land.morningbrief.link/mcp` | 3 |
| [Agent Bounty Feed](https://dailydollar-bot.github.io/agent-bounty-feed/) | Open, paid bounties AI agents can claim, verified hourly from funded boards and audit contests. | `https://agent-bounty-feed.dailydollar.workers.dev/mcp` | 4 |
| [tapwatermap](https://tapwatermap.com/developers/) | Query US tap-water quality from the EPA's SDWIS records — by city, system, or contaminant. | `https://mcp.tapwatermap.com/mcp` | 10 |
| [CoverBureau](https://coverbureau.com) | Checks certificates of insurance (ACORD 25) against your requirements. Pay per call, x402 USDC. | `https://coverbureau.com/mcp` | 3 |
| [KeyHalve - verify sealed documents](https://github.com/keyhalve/keyhalve-mcp) | Free, no-account verification of KeyHalve-sealed documents. Read-only; never receives keys. | `https://mcp.keyhalve.com/mcp` | 3 |
| [Lightning · AI Visibility Data](https://api.lightningeo.com) | AI-visibility studies for agents: how ChatGPT, Gemini and Claude answer, any region or industry. | `https://api.lightningeo.com/mcp` | 8 |
| [partreel](https://partreel.com) | Verified KiCad footprints, symbols & 3D models for AI agents. No signup, CC-BY-4.0, quality-gated. | `https://mcp.partreel.com/mcp` | 7 |

## Method

1. `scripts/fetch_registry.py` reads every server (latest version) from the registry and keeps remote endpoints.
2. `scripts/probe.py` tests Streamable HTTP endpoints that need no headers, at most 5 URLs per host, no temporary tunnels, 10 s timeout.
3. `scripts/make_directory.py` drops mass-generated copies (same tool set more than 3 times, same description more than twice, more than 2 per domain) and assigns topics by keyword.

The workflow in `.github/workflows/weekly.yml` runs this every Monday and commits the result. Data: CC BY 4.0. Code: MIT.

Maintained by [Shortform Kit](https://shortformkit.com), which runs its own free remote MCP server for social video transcripts and creator data: `https://shortformkit.com/mcp`.

