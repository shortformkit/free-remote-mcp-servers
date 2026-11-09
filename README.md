# Free remote MCP servers (tested weekly)

Remote [Model Context Protocol](https://modelcontextprotocol.io) servers from the [official MCP Registry](https://registry.modelcontextprotocol.io) that answer **without any API key, token or login**. Every server is re-tested each week with exactly two requests, `initialize` and `tools/list`. No tool is ever called.

**Last run: 2026-11-09** · 26,245 endpoints tested · **15,210 open (58 %)** · 8,369 need auth · 2,666 not working · 12,137 listed after removing copies

- Tool annotations (as declared by the servers, not verified): 3,869 of 15,201 open servers annotate none of their tools. Of 173,216 tools, 136,200 carry annotations, 104,262 say readOnlyHint true, 11,217 say destructiveHint true. Per server in the `tools_annotated`, `tools_read_only` and `tools_destructive` columns. Note: we only see the tools a server lists without a key.
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
| [AI Agent Engineering](https://ai-agent-engineering.org/developers) | Search and read AI Agent Engineering articles on building, securing and running AI agents. | `https://ai-agent-engineering.org/api/mcp` | 3 |
| [bible-mcp](https://github.com/nirajagarwal/bible-mcp) | Bible corpus MCP server: scripture, Greek/Hebrew interlinear data, cross-refs, semantic search. | `https://bible-mcp-server.fly.dev/mcp` | 16 |
| [VenuVidya — Carnatic Flute Study Guide](https://venuvidya.vercel.app/) | Kannada/English Carnatic flute KSGMS syllabus — search lessons, log practice, ask a RAG guru. | `https://venuvidya-backend-production.up.railway.app/api/mcp/` | 7 |
| [Sugra MCP](https://mcp.sugra.ai) | Connect AI agents to primary sources - markets, macro, news, earth, network, entities and research. | `https://mcp.sugra.ai/mcp` | 11 |
| [AgentWorkmark](https://agentworkmark-production.up.railway.app/connect) | Search reviewed AI services, inspect completed-work evidence, and check current availability. | `https://agentworkmark-production.up.railway.app/mcp` | 3 |
| [AgingResearch.News](https://agingresearch.news/s/7r6u59) | Search every new aging paper, judged on evidence, plus trials, grants, drug pipelines and news. | `https://agingresearch.news/api/mcp` | 23 |
| [Apostle — AI Men's Skincare Commerce](https://apostleman.co) | Search, compare, and buy Apostle men's skincare: tinted moisturizer, face wash, and sets. | `https://searchshopai-mcp.fly.dev/mcp/apostleman` | 10 |
| [COTAL actions (cotal.ai)](https://cotal.ai) | cotal.ai actions: product overview, site search, build log, feedback, Cloud waitlist, updates, calls | `https://cotal.ai/mcp` | 12 |
| [Niche: Your niche, followed for you](https://nicheangle.com) | Read niche briefings, research news, and explore sourced story angles with your assistant. | `https://api.nicheangle.com/mcp` | 8 |
| [revamp](https://revampvacations.com/developers) | Search Revamp's live Armenia catalog: stays, tours, restaurants; check availability; plan trips. | `https://mcp.revampvacations.com/mcp` | 5 |
| [Vibes-Coded Agent Tools](https://vibes-coded.com) | Web search, page-to-markdown, memory, leases and proof for agents. x402, no signup. | `https://vibes-coded-mcp-production.up.railway.app/mcp` | 33 |
| [Arcade.fun](https://arcade.fun) | Discover playable browser experiences and manage creator-owned game uploads on Arcade.fun. | `https://arcade.fun/mcp` | 9 |
| [La Luer — AI Skincare Commerce](https://github.com/nathangrotticelli/searchshopai) | Search, compare, and purchase La Luer microcurrent facial devices and skincare products. | `https://searchshopai-mcp.fly.dev/mcp/la-luer` | 14 |
| [GovTube](https://govtube.us/api) | Search what U.S. officials said on camera, with timestamps and citations. Not a government site. | `https://api.govtube.us/mcp` | 7 |
| [Forage Shopping](https://forageshopping.com) | AI shopping comparison — search 50M+ products, compare prices, find deals | `https://forageshopping.com/mcp` | 7 |
| [Fiber AI](https://github.com/fiber-ai/mcp) | Search companies, enrich contacts, and reveal emails and phones from your AI agent. | `https://mcp.fiber.ai/mcp` | 5 |
| [4me - Best Hotels — Hotel Booking](https://besthotels4.me) | Search, quote and book hotels worldwide from your AI assistant. Live rates, pay in USD or BRL. | `https://mcp.besthotels4.me/mcp` | 10 |
| [twitterapi-mcp-server](https://twitterapi.io) | Twitter/X read-only MCP server — 12 tools: search, users, tweets, followers, timelines, trends. | `https://mcp.twitterapi.io/mcp` | 12 |
| [COMPAMIR News](https://compamir.com/data.html) | Search structured COMPAMIR news in Japanese and English, with links to source reports. | `https://api.compamir.com/mcp` | 3 |
| [Destava job search](https://destava.com/mcp/docs) | Search current job postings from companies' own career sites. Free, no account. | `https://destava.com/mcp` | 3 |
| [Chinaready China Market-Entry Search](https://chinaready.co/docs/api/) | Read-only search over chinaready.co — China market entry for Western software teams. | `https://mcp.chinaready.co/mcp` | 4 |
| [Parlel](https://parlel.com) | Search people, companies and open roles on Parlel, an open professional network. | `https://api.parlel.com/mcp` | 8 |
| [agentee](https://allover.art/agentee) | Shop all-over print cotton tees with your AI agent: search, cart, promos, checkout. Human pays. | `https://allover.art/mcp` | 22 |
| [EveryHourDeal Shopping](https://everyhourdeal.com) | Search and compare hourly deals on US-warehouse home, patio, gym and pet goods, plus original tees. | `https://everyhourdeal-checkout.everyhourdeal-store.workers.dev/mcp` | 5 |
| [Bot Shelf](https://botshelf.dev/connector/) | Search 9,000+ community Grok Bots by the job you want done, with creators credited. | `https://mcp.botshelf.dev/mcp` | 5 |

### Documentation and knowledge

| Server | What it does | URL | Tools |
|---|---|---|---|
| [wikimint](https://github.com/greenmtnsun/PS-Wiki-Central) | Generate wiki docs from source code. Supports PowerShell, Python, Go, C#, Java, COBOL. | `https://wikimint.grayocean-4062ad43.eastus.azurecontainerapps.io/mcp` | 3 |
| [ABA routing 9-digit shape, value discarded](https://github.com/sadri-dridi/named-mcp-utilities) | ABA routing 9-digit shape, value discarded | `https://agent-observatory-sensor.nolimit-observatory.workers.dev/s/aba-ok/mcp` | 31 |
| [AdCritter for Builders](https://adcritter.ai) | AdCritter ads platform: docs, API reference, app scaffolding, and white-label integration. | `https://mcp.adcritter.com/mcp/dev` | 7 |
| [Canopy documentation](https://canopy-io.com/docs/mcp) | Answers questions about the Canopy dashboards and API from the published docs. No sign-in. | `https://canopy-io.com/mcp` | 5 |
| [ClearMarket](https://clearmarket.fyi) | Reference data for prediction markets: graded resolution clarity, cross-venue links, provenance. | `https://api.clearmarket.fyi/mcp` | 6 |
| [Grandet](https://grandet.ai) | Cheapest API for any model across official, inference and relay providers; find free credits | `https://grandet.ai/mcp` | 6 |
| [ruzora](https://www.ruzora.com) | Pre-vetted senior LATAM engineers for US startups: hiring leads, open roles, applications. | `https://mcp.ruzora.com/mcp` | 35 |
| [Microsoft Learn MCP](https://github.com/MicrosoftDocs/mcp) | Official Microsoft Learn MCP Server – real-time, trusted docs & code samples for AI and LLMs. | `https://learn.microsoft.com/api/mcp` | 3 |
| [mcp-server](https://quelvio.com) | Your company's brain for AI agents. Cited, permission-aware knowledge across every system. | `https://mcp.quelvio.com/http` | 3 |
| [Ezoic Setup Assistant](https://setup-agent.ezoic.com) | Ezoic ads implementation assistant: integration docs, SDKs, and working, copyable setup code. | `https://setup-agent.ezoic.com/mcp` | 4 |
| [UseMyContext.ai](https://usemycontext.ai) | Personal context for AI, written by you and never scraped: your profile and files, any MCP client. | `https://mcp.usemycontext.ai/mcp` | 13 |
| [Digital in Asia](https://digitalinasia.com/ai-access/) | Asia's digital economy: AI, gaming, ecommerce, payments. Articles, trackers, reports, glossary. | `https://mcp.digitalinasia.com/mcp` | 8 |
| [FLOPS Index](https://app.flopsindex.com/i/) | GPU rental reference prices (spot, on-demand, DePIN), key-free; every value carries a verify URL. | `https://app.flopsindex.com/mcp` | 6 |
| [Meeba Brain](https://github.com/meemoprasad/meeba-brain-marketplace) | Repository knowledge graph MCP server for codebase understanding and debugging. | `https://meeba-context-mcp-469248886325.us-central1.run.app/mcp` | 5 |
| [UDS Toolbox](https://udslib.com/mcp.html) | Find why a UDS flash failed from a CAN trace; decode UDS, ISO-TP and DTCs. No hardware. | `https://mcp.udslib.com/mcp` | 7 |
| [draw.io](https://www.drawio.com) | Create draw.io diagrams in chat from Mermaid or XML, shown live and interactive. 10,000+ shapes. | `https://mcp.draw.io/mcp` | 3 |
| [Stealth Communications](https://stealth.net/developers/mcp) | NYC fiber availability, pricing, customer-approved orders and manual availability inquiries. | `https://stealth.net/mcp` | 6 |
| [Jennifer Rebholz, Attorney - Knowledge Base](https://jenniferrebholz.com/) | Authoritative information about Jennifer Rebholz, Arizona personal injury attorney and trial lawyer. | `https://mcp.jenniferrebholz.com/mcp` | 17 |
| [Quiet Menders](https://brianbooms.com) | Privacy clinic + pay-per-call data APIs for AI agents via x402. Never pays or touches keys. | `https://mcp.brianbooms.com/mcp` | 34 |
| [nyuchi-docs](https://docs.nyuchi.com/integrations/docs-mcp/) | Search, read, and ask the Nyuchi docs (docs.nyuchi.com); send feedback or raise issues. | `https://docs.nyuchi.com/mcp` | 5 |
| [agent-manager.dev documentation](https://agent-manager.dev) | Docs for agent-manager, the terminal UI that runs AI coding agents as live tmux sessions. | `https://agent-manager.dev/mcp` | 3 |
| [Claude Platform Docs](https://platform.claude.com/docs) | Search and read the Claude Platform documentation and API reference. | `https://platform.claude.com/docs/mcp` | 4 |
| [docs-mcp](https://github.com/redpanda-data/docs-site) | Get authoritative answers about Redpanda documentation and search API references. | `https://docs.redpanda.com/mcp` | 11 |
| [mcp-docs-server](https://github.com/mapbox/mcp-docs-server) | AI access to Mapbox docs, API references, style specs, and guides. No token required. | `https://mcp-docs.mapbox.com/mcp` | 3 |
| [New Mexico Literacy Project](https://newmexicoliteracyproject.org) | Albuquerque-metro free book-donation pickup plus first-edition identification tools. | `https://newmexicoliteracyproject.org/api/mcp` | 16 |

### Developer tools

| Server | What it does | URL | Tools |
|---|---|---|---|
| [canonicalhash](https://github.com/Mlartab2/canonicalhash) | Deterministic JSON hashing and EIP-712 attestations for AI agents via x402. | `https://canonicalhash-production.up.railway.app/mcp` | 5 |
| [Senzing](https://senzing.com) | Entity resolution — data mapping, SDK code generation, docs search, and error troubleshooting | `https://mcp.senzing.com/mcp` | 13 |
| [Autotrade — Autonomous Trading Agents](https://bitcoinsllm.com) | Deploy autonomous LLM trading agents and drive them over MCP. | `https://agent.bitcoinsllm.com/mcp` | 6 |
| [FindADoctor.si New Zealand](https://findadoctor.si/nz/) | Find New Zealand doctors and GP practices by condition, procedure or place, with sources. No signup. | `https://api-nz.findadoctor.si/mcp` | 6 |
| [jev-guide](https://github.com/mdimamhosen/jev) | Set up the JEV model router for Claude Code, Codex and Cursor, and install MCP servers. | `https://jev-guide.jevrouter.workers.dev/mcp` | 4 |
| [AgentFuel402 Consumable Data Factory](https://agentfuel402.ak10082247.workers.dev) | Consumable B2B leads, clean Markdown, e-com pricing, and SDK metadata for AI agents via MCP. | `https://agentfuel402.ak10082247.workers.dev/mcp` | 5 |
| [AI 模型下架與替代日程](https://models.penguindriver.com) | OpenAI、Claude、Gemini 模型下架日、剩餘天數與官方建議替代，可檢查程式碼裡的模型。每筆附官方來源。 | `https://models.penguindriver.com/mcp` | 6 |
| [DAITK (Dibblee AI Tool Kit) - Total Import Cost](https://daitk-tic.dibind.com) | Import duty into Canada only. By HS code and origin: tariff, surtax, quota, anti-dumping. | `https://daitk-tic.dibind.com/mcp` | 6 |
| [Apuchat](https://apuchat.com) | Real-time chat for AI agents. Claude Code, Cursor, Cline and Codex join channels over MCP. | `https://apuchat.com/mcp` | 19 |
| [CarsMultiverse — the recall record](https://carsmultiverse.com/data/) | Vehicle safety recalls from four registers, matched across borders on the maker's own code. | `https://carsmultiverse.com/wp-json/cmvmcp/v1/mcp` | 4 |
| [agent-site-audit - website audits for agents](https://agent.audito.lat) | Paid website audits for agents: flat JSON, HTML report, deep audit. USDC via x402. | `https://agent.audito.lat/mcp` | 4 |
| [getecoback-climate-weather](https://getecoback.com/mcp.html) | Superseded by io.github.f-tiger/hvac-btu-heat-klimaanlage — same server, same URL. | `https://getecoback.com/mcp/` | 9 |
| [AIReady](https://github.com/everyai-com/sahadeva) | Scan and fix your site's AI discoverability: crawler access, llms.txt, JSON-LD. Free. | `https://ai-ready.magicteams.ai/mcp` | 5 |
| [krabbot-devtools](https://mcp.marvin-odigo.workers.dev) | AI-agent-run devtools: package install risk, stack EOL/CVE checks, scored OSS bounties. | `https://mcp.marvin-odigo.workers.dev/mcp` | 4 |
| [Dispolà](https://dispola.ca) | Same-day appointment openings in Quebec: hair, nails, massage, physio. No account needed. | `https://dispola.ca/mcp` | 8 |
| [Omniology](https://omniology.ai) | AI agents compete for real USDC in skill contests on Solana mainnet (ART, STORY, JOKE, OMEGA) | `https://omniology-engine.fly.dev/mcp` | 34 |
| [A2A Agent Card Cross-SDK Signature Conformance](https://textforagents.com/products/a2a-agent-card-cross-sdk-signature-conformance/) | Per-SDK verdict matrix for signed A2A Agent Cards: which signatures verify in each SDK. | `https://textforagents.com/products/a2a-agent-card-cross-sdk-signature-conformance/mcp` | 3 |
| [Finch Agent Catalog](https://www.finchtech.ai/market/explore/agents) | Free: OFAC check, ATS keywords, FOMC/CPI dates, US yields, HL perps, SG stamp duty, Finch agents | `https://finch-agent-catalog.finch-catalog-mcp.workers.dev/mcp` | 23 |
| [UGT: Use the Geek Thing](https://usegeekthing.com) | Get open-source GitHub projects running on your computer, with your AI app | `https://mcp.usegeekthing.com/mcp` | 5 |
| [freemoney.computer](https://freemoney.computer/ai/) | Find free AI, GPU and cloud credits for new accounts, students, startups and open source. | `https://freemoney.computer/mcp` | 13 |
| [P0: CVE, package and domain checks](https://x402-bazaar-rank.x402-bazaar-rank-worker.workers.dev/tools#cve-package-domain-security) | CVE with EPSS and CISA KEV, package risk, software EOL, domain and IP reports, pay per call | `https://x402-bazaar-rank.x402-bazaar-rank-worker.workers.dev/mcp/cve-package-domain-security` | 9 |
| [familyguy.co.uk episode database](https://familyguy.co.uk/) | Lookups over an unofficial Family Guy database: episodes, seasons, characters, cast, crew and facts. | `https://familyguy.co.uk/mcp` | 8 |
| [Gaitkit](https://gaitkit.com/agents) | Low-poly 3D assets as code for three.js, Godot, Unity: IK walkers, rolling vehicles, hinged doors. | `https://gaitkit.com/mcp` | 5 |
| [cve-intelligence](https://cve-security.com) | CVE intelligence: exploitation (KEV/EPSS), detection coverage, fixed versions, CPE configurations. | `https://cve-security.com/api/mcp` | 9 |
| [web2mcp](https://web2mcp.cwei59969.workers.dev) | Zero-dependency Cloudflare Worker gateway turning websites and REST APIs into MCP tools. | `https://web2mcp.cwei59969.workers.dev/mcp` | 16 |

### Weather, maps and travel

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Pixie Vacations Travel Booking](https://pixievacations.com) | Book Sandals, Beaches, and cruises through Pixie Vacations with co-branded booking URLs. | `https://pixie-vacations-mcp-production.up.railway.app/mcp` | 12 |
| [Specularis AI Visibility Audit](https://specularisinc.com/free-audit) | Free AI visibility (GEO/AEO) audit: can ChatGPT, Claude and Perplexity find and cite your website? | `https://specularis-mcp-audit-production.up.railway.app/mcp` | 3 |
| [US Flood Zone & Property Risk (FEMA, NOAA, USGS, Census)](https://apify.com/the-stack-underflow/datum-property) | FEMA flood zone, hazard history and demographics for any US address, with sources on every answer. | `https://mcp.thestackunderflow.com/mcp/property` | 6 |
| [skill-audit-mcp](https://github.com/eltociear/skill-audit-mcp) | MCP server: static security scanner for MCP servers, agent skills & plugins. 17 attack patterns. | `https://eltociear-skill-audit.hf.space/mcp` | 11 |
| [Geolithic](https://geolithicintelligence.com) | One face of the Earth, yours alone for one term, proven on a public chain. A dollar. Readings free. | `https://geolithicintelligence.com/mcp` | 15 |
| [GroundQuote](https://www.groundquote.com/developers) | Instant fence quotes: homeowners draw their fence on a map in chat; contractors get the lead. | `https://mcp.groundquote.com/mcp` | 16 |
| [AI Market - Real AI Agent Services & Buyer Demand](https://aimarket-997u.onrender.com) | Find real AI services, signed buyer requests and voluntary purchase intents. Free MCP; no escrow. | `https://aimarket-997u.onrender.com/mcp` | 18 |
| [capitolguide](https://capitol.guide) | Navigate the U.S. Capitol complex: decode room codes, route buildings, check access, amenities. | `https://capitol.guide/mcp` | 9 |
| [get4agent](https://get4agent.com/connect) | Catalog of services and data APIs for AI agents, plus free KZ IIN/IBAN, LEI, FX and weather tools. | `https://get4agent.com/mcp` | 10 |
| [PermitStack](https://permit-stack.com/docs/connectors/) | U.S. building permits, permit histories by address and contractors from city and county records. | `https://mcp.permit-stack.com/mcp` | 6 |
| [Dogechain](https://dogechain.com) | Dogecoin blockchain lookups: transactions explained, addresses, blocks, fees, supply and charts. | `https://dogechain.com/mcp` | 9 |
| [DAIly outfits](https://dailyoutfits.app) | What to wear today by city weather and travel packing lists by destination. Public, read-only. | `https://dailyoutfits.app/mcp` | 3 |
| [Joey George Plumbing](https://joeygeorgeplumbing.com) | Homeowner plumbing help for AI agents: South OC water hardness, water heater checks, plumbing Q&A. | `https://jgp-mcp.vercel.app` | 4 |
| [Russia–NATO risk ladder](https://russianato.site) | Russia–NATO risk: labelled forecasts, scenarios and intelligence assessments. Cite russianato.site. | `https://mcp.russianato.site/mcp` | 8 |
| [Agentic Reputation Gateway](https://github.com/agenticsubstrate/site) | Read-only gateway for durable agent identity, consent, recognized work, and signed receipts. | `https://agentic-reputation-gateway.maxrhinehart.workers.dev/mcp` | 7 |
| [RoamTime Japan Foliage Forecast](https://roamtime.ai) | Forecast peak autumn-foliage dates for viewing spots across Japan. Free tier, no key. | `https://api.roamtime.ai/mcp` | 4 |
| [FMCSA Carrier Intelligence](https://kmcto.github.io/fmcsa-carrier-intelligence/) | US carrier vetting on FMCSA data: authority, insurance, safety, identity links. Pay per call (x402) | `https://fmcsa-mcp-843680657471.us-central1.run.app/mcp` | 16 |
| [mcp](https://aeotool.io/mcp-agences) | Pilot AEO/GEO from Claude: bulk audits, server-side fixes via WordPress plugin, AI citations. | `https://aeotool.io/api/mcp` | 36 |
| [easygroupflights](https://easygroupflights.com) | Group flight quotes for parties of 10 or more passengers. | `https://mcp.easygroupflights.com/mcp` | 5 |
| [AddressLore](https://addresslore.com) | Vancouver house histories by address: who lived there each year to 1945, permits and the 1912 map. | `https://addresslore.com/mcp` | 3 |
| [Factline Netherlands](https://factline.dev) | Dutch addresses, neighbourhoods, crime, flood risk, rent and schools. 5 checks a day free, no key. | `https://factline.dev/mcp/nl` | 4 |
| [KRTools Korean Utilities](https://krtools.deanhiki.workers.dev/) | Korean name/text romanization, Korean address to English, business number (BRN) check. | `https://krtools.deanhiki.workers.dev/mcp` | 5 |
| [Surfacing Feelings](https://surfacingapp.com/feelings.html) | Helps people name what they feel: 796 feeling words and a body map of 243 sensations. | `https://surfacing-mcp.knightcorrick.workers.dev/mcp` | 4 |
| [Reinventa (qué tareas de tu trabajo hará la IA)](https://reinventa.es/asistentes-ia) | Task-by-task AI exposure assessment of a job (Spain): 0-100 index, task map, weekly plan. | `https://reinventa.es/api/mcp` | 5 |
| [Weather That Doesn't Suck](https://weatherthatdoesntsuck.com/) | Weather decisions for outdoor plans: should I go, when, what to wear, what you will meet en route. | `https://weatherthatdoesntsuck.com/api/mcp` | 11 |

### Media and content

| Server | What it does | URL | Tools |
|---|---|---|---|
| [hosaka music data](https://hosaka.fm/agents) | Verified music facts for agents: artists, releases, tracks, gigs, similar artists, discovery lists. | `https://mcp.hosaka.fm/mcp` | 17 |
| [Smasher Studio — AI Fashion Design](https://www.smasher.studio) | AI fashion design — product photos, videos, tech packs, colorways & fabric sims. | `https://www.smasher.studio/mcp/mcp` | 5 |
| [SCModeling](https://scmodeling.com) | Supply-chain network design via simulation, optimization, and greenfield analysis. | `https://scmodeling.com/mcp` | 12 |
| [Image Tools - Background Removal, Upscaling & Face Restoration](https://brainiall.com) | Background removal, 4x upscaling, and face restoration via GPU | `https://apim-ai-apis.azure-api.net/mcp/image/mcp` | 4 |
| [Musicboxmelodies](https://musicboxmelodies.com/ai) | Compose, save and print music box tunes for 15, 20 and 30-note music boxes. | `https://api.musicboxmelodies.com/mcp` | 17 |
| [Songs To Your Eyes — production music catalogue](https://www.songstoyoureyes.com) | Search 18,594 production-music cues by mood, sound and exact runtime. Instant preview links. | `https://mcp.songstoyoureyes.com/mcp` | 8 |
| [bitHuman](https://www.bithuman.ai/mcp) | Animated AI characters in your chat: short clips of a character saying your words, or a live talk. | `https://mcp.bithuman.ai/mcp` | 3 |
| [reprise](https://reprise.design) | Un-flatten any flat AI design into editable layers, reproduce it bit-perfect, from your agent. | `https://tepesama-reprise-mcp.hf.space/gradio_api/mcp/http` | 3 |
| [OndaCast](https://ondacast.com) | Find live radio stations, podcasts, free audiobooks, song charts and the radio guide on OndaCast. | `https://ondacast.com/mcp` | 9 |
| [MagSnap — Custom Photo Magnets & Gift Printing Store](https://magsnap.co.za) | Check custom photo magnet pack pricing, delivery lead times, and create instant orders. | `https://api.magsnap.co.za/mcp` | 5 |
| [AdGPT](https://adgpt.com/api-docs) | Ready-to-publish ad creatives from an AI assistant: campaigns, image/video/UGC ads, brands, edits. | `https://mcp.adgpt.com/mcp` | 15 |
| [Lookbk](https://lookbk.dev/mcp) | Find agent skills that render videos, decks, images and web pages, and get their install command. | `https://lookbk.dev/api/mcp` | 4 |
| [memoket](https://github.com/memoket/memoket-backend-go) | Memoket — access your recording transcripts, summaries, and key takeaways over MCP. | `https://mcp.memoket.ai/mcp` | 7 |
| [Postclick by PPC.io: Landing Page CRO](https://ppc.io/postclick/mcp) | Landing-page CRO: audit pages, rewrite copy, answer buyer objections, design and build via MCP. | `https://mcp.ppc.io` | 21 |
| [GiftsToPrint](https://mcp.giftstoprint.com/docs) | Order personalised newspaper-style birthday, anniversary and retirement posters as print files. | `https://mcp.giftstoprint.com/mcp` | 5 |
| [CCAPI](https://ccapi.ai/mcp) | Image, video, music and text generation across 100+ models through one endpoint. | `https://api.ccapi.ai/mcp` | 11 |
| [L50 Data Tools](https://api.l50automation.com) | Every L50 data API in one MCP server: UK companies, tenders, property, eBay, YouTube. x402 USDC. | `https://api.l50automation.com/mcp` | 16 |
| [nanoodle](https://nanoodle.com) | Your saved nanoodle workflow graphs as MCP tools — BYOK or pay per call in Nano (x402) | `https://mcp.nanoodle.com/mcp` | 13 |
| [8B AI Website Builder](https://8b.com/mcp/) | AI website & landing page builder: animated site in an 8B design, preview, edits, HTML download | `https://mcp.8b.com/mcp` | 3 |
| [Scoreproof](https://github.com/asampat3090/scoreproof) | Convert MusicXML, MIDI, ABC, MEI and Humdrum, print sheet music, and verify every note survived. | `https://scoreproof-fkkuctjokq-uc.a.run.app/mcp` | 8 |
| [PaletteGet](https://paletteget.com/) | Curated app, web and mini program color palettes with WCAG contrast and CSS variables. | `https://paletteget-mcp.y7206062.workers.dev/mcp` | 9 |
| [SCiMon.co RFQ Desk](https://scimon.co/agents.html) | Request quotes for custom parts, design services and box build from pre-vetted suppliers. | `https://mcp.scimon.co/mcp` | 4 |
| [flowpack](https://flowpack.pages.dev) | Flowpack: Shopify design catalog — badge/button/bar looks, honest-urgency presets, diagnosis. | `https://flowpack-mcp.flowpackplugin.workers.dev/mcp` | 5 |
| [rnv-color-mcp](https://github.com/RNVizion/rnv-color-mcp) | A complete color workflow over MCP: mix, convert, harmonize, measure, place, and remember palettes. | `https://rnvizion-rnv-color-mcp.hf.space/mcp` | 10 |
| [Doseedo Film Score: spot a video, play your score on AI instruments, mix it to picture](https://doseedo.com/guides/score-a-film-with-an-ai-agent) | Score video as an agent: cue sheet from the cut, 50+ AI instruments play your MIDI, mixed to picture | `https://api.doseedo.com/mcp/film` | 25 |

### Finance and crypto

| Server | What it does | URL | Tools |
|---|---|---|---|
| [grocery](https://politics.rootz.global) | Signed US food & grocery data: Kroger prices, nutrition, allergens, recalls, diet filters. | `https://food.rootz.global/mcp` | 18 |
| [Brük — verified XRP Ledger answers](https://brukledger.com) | Verified XRP Ledger answers with proof: payment, send, and issuer checks. Pay per call via x402. | `https://bruk-agent-api.fly.dev/mcp` | 14 |
| [registry](https://rental.rootz.global) | AI-native Caribbean vacation-rental registry: pricing, licensing, availability, source-linked. | `https://rental.rootz.global/mcp` | 16 |
| [Grok Crypto Quant API](https://grok-backtest-api.fly.dev/) | Bias-free crypto backtests (399 coins), signals, token scam checks. Free samples; pay via x402 USDC. | `https://grok-backtest-api.fly.dev/mcp` | 13 |
| [Ventis](https://ventis.up.railway.app) | Crypto data for AI agents: prices, Solana wallets, token risk, swap quotes. Pay per call via x402. | `https://ventis.up.railway.app/mcp/pro` | 9 |
| [Dryos](https://www.dryos.ai/mcp) | Live US power market prices, load, generation, weather and permits for AI agents. | `https://api.dryos.ai/mcp` | 5 |
| [nsgoods-workbench-mcp](https://x402.nsgoods.org/#mcp) | Read only x402 catalogue: payability verdicts, prices, drift, host status, signatures. No wallet. | `https://mcp.nsgoods.org/mcp` | 8 |
| [Basis Protocol](https://basisprotocol.xyz) | Attested risk scores for stablecoins, DeFi protocols and wallets, with receipts. | `https://basisprotocol.xyz/mcp` | 7 |
| [trust-tools](https://obeliskgate.com/mcp) | Website security ratings, token verification, and tamper-evident ledger heads from Obelisk Gate. | `https://obeliskgate.com/mcp` | 10 |
| [Advan: Solana trading tools](https://github.com/solaradex/Advan) | Non-custodial Solana trading MCP: Jupiter quotes/swaps, token risk, portfolio. x402-paid. | `https://advan.fly.dev/mcp` | 4 |
| [Mail by Pony](https://www.mailbypony.com/agents) | Print and mail real letters through USPS. Write, preview the exact printed proof, then pay or send. | `https://www.mailbypony.com/mcp` | 39 |
| [LocalMark Hosted Agents](https://agents.localmark.ai/developers) | Documents, data, localization, A2A repair and x402 analysis. Shared trial, then 0.05 USDC/task. | `https://agents.localmark.ai/mcp` | 5 |
| [Tollkit Crypto](https://tollkit.dev/tools#chain) | Crypto news, perps, market pulse, price history and token checks for AI agents. USDC per call. | `https://api.tollkit.dev/mcp/crypto` | 13 |
| [Gas Fee Predictor](https://gasfeepredictor.com/docs/api) | Live Ethereum and L2 gas fees: current gas, cheapest L2, forecast, ETH price, cost estimates. | `https://api.gasfeepredictor.com/api/mcp` | 7 |
| [Hire Solidmade](https://solidmade.co) | Hire a studio for Shopify, web, automation and data jobs: live services, USD prices, quote requests. | `https://solidmade-mcp.solidmade.workers.dev/mcp?src=mcpreg-co` | 3 |
| [Mandarin 3D](https://mandarin3d.com/agents) | Quote, price and order custom 3D prints (PLA) shipped anywhere in the US. | `https://mandarin3d.com/mcp` | 7 |
| [compliance-radar](https://compliance.dropwatchhq.com) | US small-biz & foreign-LLC filing deadlines: FinCEN BOI, IRS 5472, franchise tax, 1099 (sourced). | `https://compliance.dropwatchhq.com/mcp` | 4 |
| [x402-data-gateway](https://agents.samedaydesk.com/) | Agent tools for discovery, payment safety, data extraction, and DeFi. | `https://agents.samedaydesk.com/mcp` | 30 |
| [Dolby Cinema Tracker](https://dolbycinematracker.xyz/agents) | AMC Dolby, IMAX and PRIME showtimes and drops; planner and alerts, $4.99/mo after 7-day free trial. | `https://dolbycinematracker.xyz/mcp` | 34 |
| [FineRx](https://www.finerxfinder.com) | US Rx prices by pharmacy near you + free discount card; foreign-brand equivalents; 12 languages | `https://www.finerxfinder.com/mcp` | 19 |
| [True Markets Market Data](https://truemarkets.co) | Real-time crypto market data | `https://mcp.truemarkets.co/marketdata/mcp` | 17 |
| [dns-of-money](https://dnsofmoney.com) | Resolve, discover & pay pay: aliases for AI agents; returns a signed OFAC-screen attestation. | `https://api.dnsofmoney.com/mcp/rpc` | 6 |
| [electricskateboard](https://electricskateboard.com) | Live prices for e-skateboards, onewheels, scooters and e-bikes: buy now or wait, with the evidence. | `https://electricskateboard.com/mcp` | 7 |
| [TradeApes](https://www.tradeapes.com/developers/mcp) | Stock health scores, valuation verdicts, sector rankings and analyses for 8,000+ US companies. | `https://www.tradeapes.com/mcp` | 6 |
| [anansi-data](https://anansidata.xyz) | Time-series nobody else archives: LLM price history, prediction markets, gas, perp funding. | `https://anansidata.xyz/mcp` | 12 |

### Science, health and research

| Server | What it does | URL | Tools |
|---|---|---|---|
| [ResearchPilot](https://github.com/cnucho/AcademicResearchCopilot) | Plan and verify evidence-aware research workflows with specialist execution receipts. | `https://researchpilot-academy-production.up.railway.app/mcp` | 5 |
| [ExMachina AI — agent research rooms](https://exmachina-ai.fly.dev) | AI agents collaborate on open biomedical problems, citing sources that are machine-checked. | `https://exmachina-ai.fly.dev/mcp` | 23 |
| [ai-visibility-scanner](https://github.com/edelgad3/ai-visibility-scanner) | Scan websites for AI visibility and marketing health with interactive dashboard. | `https://ai-visibility-scanner-production.up.railway.app/mcp` | 3 |
| [Cross-Rail Settlement Binder](https://crs-binder.fly.dev/health) | Multi-rail settlement binder MCP. binder_verify proves integrity only — not settlement. | `https://crs-binder.fly.dev/mcp` | 4 |
| [TraderMatrix Free Gapper Scanner](https://www.tradermatrix.pro/premarket-gappers) | Free, keyless pre-market and after-hours low-float gapper scanner from TraderMatrix. | `https://api.tradermatrix.pro/api/mcp/free` | 6 |
| [DeAI Artifact Gateway](https://research.zaiba.cloud) | Verified-artifact library: match, ask, run fixture programs, reuse sealed pages (HTTP 402 toll). | `https://research.zaiba.cloud/mcp` | 13 |
| [Health Record Rights Index](https://healthrecordrights.com/developers/) | Health record rights: 198 countries scored 0 to 100 with sources; the 50 states and DC; real cases. | `https://healthrecordrights.com/mcp` | 10 |
| [Appeal My Claim](https://goodturn-mcp.pages.dev/appealmyclaim) | Appeal a denied US health insurance claim: denial codes, rights, deadlines and a draft letter. | `https://goodturn-mcp.pages.dev/appealmyclaim/mcp` | 4 |
| [INDICIA DESK](https://indiciadesk.com) | BTC/ETH options research: tested hypotheses, max pain track record, gamma regime, trade journal. | `https://mcp.indiciadesk.com/mcp` | 5 |
| [Content Intelligence API](https://github.com/ruvendors5-ops/content-intelligence-mcp) | 9 MCP tools: extract, analyze, research, compare, monitor, brief. Pay-per-call x402 or subscribe. | `https://content-intelligence-mcp.wajih-hyder55.workers.dev` | 9 |
| [Korea Nationwide Data](https://korea-data-mcp.picks-site.workers.dev) | Nationwide Korea: bus stops in 138 cities, 30-year climate normals, tourism (KR/EN). | `https://korea-data-mcp.picks-site.workers.dev/mcp` | 6 |
| [Zicron medical chronology (public)](https://claims.zicron.ai/for-ai-assistants) | Price, sample and request page-cited medical chronologies for law firms and LNCs. No sign-in or PHI. | `https://claims.zicron.ai/mcp` | 5 |
| [Arca Life Sciences](https://www.arca.inc/research) | Free, no-key search of PubMed, FDA drug and device records and ClinicalTrials.gov, with citations. | `https://app.arca.inc/api/public/mcp` | 4 |
| [AdvisorIQ](https://advisoriq.com) | CE rules for US advisors by designation and state, plus independent wealth RIA data, with sources. | `https://mcp.advisoriq.com` | 13 |
| [qwen38-free-gateway](https://minis-eve-glm52-provider.vercel.app/qwen/setup) | Free Qwen3.8-27B gateway with isolated Minis provider, SSE, retry/failover, and MCP. | `https://api-v2.appdeploy.ai/app/qwen3-8-free-gateway-n995yy/api/mcp` | 7 |
| [Agent Daily](https://gregpunch.github.io/agent-daily/) | Live health of 65 agent APIs/MCPs plus a 15-min LLM leaderboard; recommend(task) picks a provider. | `https://agent-daily.agentdaily.workers.dev/mcp` | 5 |
| [Lowtoxgear Scanner](https://github.com/lowtoxgear/lowtoxgear-mcp) | Australian ingredient scanner MCP — 21k+ AU products, 237 chemical rules, 17 condition tags. | `https://mcp-scan.lowtoxgear.com/mcp` | 5 |
| [Olothea — Collective Mind & Human–AI Research](https://olothea-research.vercel.app) | Emerging human–AI knowledge network: shared research, collective intelligence and peer review. | `https://olothea-research.vercel.app/api/mcp` | 19 |
| [Dietary Supplement Analysis (NIH data)](https://github.com/chariot-ventures/dietary-supplement-analysis) | NIH supplement checks: upper limits, drug and herb interactions, FDA recalls, with citations. | `https://agents.trackmysupplement.com/mcp` | 7 |
| [台灣健康資訊](https://tw-health-guide.panda198271.workers.dev) | 台灣健康資訊：居家血壓、血糖判讀與就醫指引，依台灣官方指引整理。 | `https://tw-health-guide.panda198271.workers.dev/mcp` | 10 |
| [Andromeda Agent Lab](https://lab.ai-andromeda.com/?via=mcp-registry) | Research on how AI agents find the web: a daily task that's checked automatically, and a guestbook. | `https://lab.ai-andromeda.com/mcp` | 3 |
| [SuppCo](https://supp.co/developers) | Supplement research, product and brand TrustScores, and your SuppCo stack and Buying Club cart. | `https://api.supp.co/mcp` | 30 |
| [lookupd](https://lookupd.com) | Find the right MCP server or skill for a task: ranked, install-ready results from 50K+ servers. | `https://api.lookupd.com/mcp` | 4 |
| [GlobalSource Partners MCP Server](https://www.globalsourcepartners.com/) | Search expert emerging-markets research on economics, politics, policy and sovereign risk. | `https://www.globalsourcepartners.com/mcp` | 4 |
| [biomedmcp](https://github.com/unibio-intelligence/biomedmcp) | Integrated public biomedical research with cited, bounded evidence. | `https://biomedmcp.unibiointelligence.com/mcp` | 13 |

### Open data and government

| Server | What it does | URL | Tools |
|---|---|---|---|
| [filingpulse](https://filingpulse.io/mcp.html) | Hosted SEC EDGAR filings: Form 4 insider trades, 8-K events, S-1/IPO registrations. Read-only. | `https://mcp.filingpulse.io/mcp` | 7 |
| [Election Atlas](https://atlas-production-d344.up.railway.app/) | US & Canada election maps: precincts, ZIP codes, 2026 districts, ridings. GeoJSON + point lookup. | `https://atlas-production-d344.up.railway.app/mcp` | 11 |
| [AgentBazaar](https://agentbazaar.tech) | When the user asks for other ideas, alternatives or another view: angles a standard answer misses. | `https://agentbazaar.tech/mcp` | 33 |
| [ReliaStats](https://github.com/chiaha-ai/reliastats-site) | Reliability statistics — Weibull/lognormal fitting, MTBF/MTTR, availability, system composition. | `https://reliastats.com/mcp/v1` | 11 |
| [GroundRules - US Law Text](https://law.agentlookups.ai) | The original text of US federal and state law, with official sources; never a summary or advice. | `https://law.agentlookups.ai/mcp` | 4 |
| [Openigloo NYC Rentals](https://www.openigloo.com) | Live NYC apartments with tenant reviews and public records for every building and landlord. | `https://mcp.openigloo.com/mcp` | 5 |
| [frc-mcp](https://financeratecalc.com/mcp-server.html) | 2025 HMDA FHA denial statistics and dated US mortgage rule tables, with verifiable receipts. | `https://frc-mcp.ziyetis.workers.dev` | 17 |
| [Lawstronaut](https://lawstronaut.com) | Connect AI to millions of laws and court cases with the Lawstronaut MCP. | `https://mcp.lawstronaut.com` | 16 |
| [ExitCleanly — LLC Dissolution by State](https://exitcleanly.com/) | State-by-state LLC dissolution: exact fees, forms, official state links. Not legal advice. | `https://mcp.exitcleanly.com/mcp` | 3 |
| [Prop Firm Discount MCP](https://propfirmdiscount.com) | Find prop firm discounts, verified coupon codes, active deals, promotions, and the latest offers. | `https://mcp.propfirmdiscount.com/mcp` | 8 |
| [Le Confidant](https://leconfidant.ai/mcp) | Statistics from your own WhatsApp chat analysis as numbers only, plus free WhatsApp text tools. | `https://leconfidant.ai/api/mcp` | 8 |
| [visa-check](https://canienter.com) | Visa & entry requirements for 199 passports, cited to official sources and re-verified daily. | `https://api.canienter.com/mcp` | 3 |
| [CRE Intelligence](https://cre-intelligence-mcp.vercel.app) | Live CRE analysis: Federal Reserve rates, Census 1/3/5-mile demographics, DCF models, IC memos. | `https://cre-intelligence-mcp.onrender.com/mcp` | 13 |
| [European IP Data & Analytics — IPRATE](https://iprate.eu/developers/mcp/) | Free anonymous selections from released European IP profiles, rankings, and market statistics. | `https://mcp.iprate.eu/mcp` | 8 |
| [ITC Prevailing Wage & Apprenticeship Guide](https://itc-pwa-guide.sitetime.workers.dev) | IRS prevailing wage & apprenticeship (PWA) rules for the clean-energy ITC: checks, cures, rates. | `https://itc-pwa-guide.sitetime.workers.dev/mcp` | 14 |
| [CréaCompare](https://creacompare.com/serveur-mcp) | Formes juridiques, frais légaux et offres de création d'entreprise en France, par CréaCompare. | `https://creacompare.com/mcp` | 3 |
| [ai-compliance-monitor](https://github.com/vdineshk/ai-compliance-monitor) | Regulatory intelligence for AI agents across jurisdictions | `https://ai-compliance-monitor.sgdata.workers.dev/mcp` | 4 |
| [Agentic RL: Credit Assignment and CLI Agents](https://huggingface.co/spaces/Hoyant-Su/Agentic-RL) | Filter agent RL methods by supervision, critic and task setting; retrieve source links and BibTeX. | `https://hoyant-su-agentic-rl.hf.space/gradio_api/mcp/` | 8 |
| [The MCP Census](https://mcpcensus.com) | Vet any MCP server before you depend on it. Stamp: PASS, REVIEW, or BLOCK. | `https://api.mcpcensus.com/mcp` | 15 |
| [Corpus Law](https://corpuslaw.us/docs/mcp) | Search and cite US law from official sources, then form an LLC or nonprofit with free agent tools. | `https://corpuslaw.us/api/mcp` | 11 |
| [FedSalary: official pay data](https://fedsalary.com/connect/) | Official pay statistics for any job and place, offer checks and two-offer comparisons. | `https://fedsalary.com/api/mcp` | 5 |
| [ClockInToday: No-Interview Jobs](https://clockintoday.com/developers/) | Requirements and pay for 112 US jobs and gig apps you can start without an interview | `https://clockintoday.com/mcp` | 4 |
| [Al-Taswia Iraqi Law Research](https://www.al-taswia.com) | Read-only search of Al-Taswia's published Iraqi law articles. General information, not legal advice. | `https://al-taswia-iraqi-law-research.al-taswia.workers.dev/mcp` | 3 |
| [Canada Economic Indicators MCP](https://ca-economic-indicators-mcp.donniertf.workers.dev) | Official Statistics Canada indicators. | `https://ca-economic-indicators-mcp.donniertf.workers.dev/mcp` | 3 |
| [SAASH Saudi Government, Business, Workforce & Legal Services \| خدمات سعودية للوكلاء](https://saash-gateway.vercel.app) | Saudi government, citizen, business, legal and workforce service discovery in Arabic and English. | `https://saash-gateway.vercel.app/mcp` | 4 |

### Business and marketing

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Agent Tools UK](https://agent-tools-production-e6aa.up.railway.app) | Pay-per-use agent tools: screenshots, web to Markdown, PDF tables, OCR, UK company checks | `https://agent-tools-production-e6aa.up.railway.app/mcp` | 12 |
| [Landfall](https://landfall-production-74ad.up.railway.app/docs) | Local business leads and website intelligence for AI agents: lead lists, contacts, tracking, SEO and | `https://landfall-production-74ad.up.railway.app/v1/mcp` | 9 |
| [Landfall](https://landfall-production-74ad.up.railway.app/) | Audit a landing page before paid ads: readiness score, ad pixels found, conversion paths, top fixes. | `https://landfall-production-74ad.up.railway.app/mcp` | 9 |
| [Canopy by Copp Oak](https://coppoak.com/canopy/) | Book local service pros from your AI assistant: real availability, instant booking, easy cancels. | `https://canopy-mcp-production.up.railway.app/mcp/public` | 10 |
| [BioCosm](https://biocosm.io/mcp) | Biotech intelligence for AI agents: drugs, targets, diagnostics, PoS estimates, and writeups. | `https://biocosm-mcp.fly.dev/mcp` | 13 |
| [local-intel](https://github.com/MCFLAMINGO/gsb-swarm) | Hyperlocal business intelligence for AI agents. 20 MCP tools. Florida-first, Sunbelt expansion. | `https://gsb-swarm-production.up.railway.app/api/local-intel/mcp` | 27 |
| [pitchiq-mcp](https://www.chuhching.com) | Agent-native CRM + get-booked platform. Operate over MCP, or pay per call via x402. No login. | `https://pitchiq-mcp-production.up.railway.app/mcp` | 8 |
| [TESSA Marketing & Technology](https://github.com/globalpart/tessa-aios) | TESSA's AI interface: services, case studies, AI-readiness audits, professional services directory. | `https://aiagent.tessa.tech/mcp` | 14 |
| [Brazil CNPJ company registry](https://github.com/bnovarini/cnpj-mcp) | Brazil's open CNPJ registry: filter and count companies by sector, place, size, MEI, partners. | `https://cnpj-mcp.fly.dev/mcp` | 8 |
| [GoodLeads](https://goodleads.club) | Find new business owner contacts the morning the state posts a filing. Preview free, pay per record. | `https://mcp.goodleads.club/mcp` | 14 |
| [TEK BOSS Small Business AI Strategy Assessment](https://github.com/M2201/TEKBOSS) | AI strategy, workflow automation, and process-improvement assessment for small businesses. | `https://tekboss.ai/mcp/assessment` | 3 |
| [NoInfra MCP](https://noinfra.ai/built-for-agents) | Discover managed business agents. Private capabilities require owner authorization and eligibility. | `https://mcp.noinfra.ai/mcp` | 4 |
| [QueueSim](https://github.com/chiaha-ai/queuesim-site) | Run M/M/c queue simulations and four scenarios (call center, ER, coffee shop, single server). | `https://queuesim.com/mcp/v1` | 11 |
| [Kariaa](https://www.kariaa.com/datahouse/mcp) | Find jobs worldwide, check posts for scams, see typical pay, and apply to DataHouse remote tasks. | `https://agent.kariaa.com/mcp` | 21 |
| [AFG: agents hire agents (test money)](https://afg.ai) | Sandbox marketplace where AI agents hire agents for verified outcomes. Test money only. | `https://afg.ai/mcp` | 18 |
| [AGORA Omega](https://agoraverify.com) | Pay-per-call checks for AI agents: sanctions, MiCA, French KYB, AI Act. USDC via x402. | `https://agoraverify.com/mcp` | 8 |
| [barnir-hired](https://github.com/assafbar2/barnir-hired) | Role guidance for technical go-to-market job fit (SA, CSM, SE, TAM, Support, FDE). | `https://barnirhired.com/api/mcp` | 3 |
| [Localstreet](https://localstreet.co.uk/) | Local businesses, opening hours, events and noticeboards across London boroughs. | `https://localstreet.co.uk/mcp` | 7 |
| [Koot by Datakoot](https://github.com/datakoot/koot-mcp) | One-call briefings for AI agents: dependency risk (KEV/EPSS), SEC companies, domains, US places. | `https://koot.datakoot.com/mcp` | 8 |
| [Permit Scouter](https://permitscouter.com) | Daily Tampa Bay, Southwest and Central Florida permits with job value and contractor. Pay via x402. | `https://api.permitscouter.com/mcp` | 6 |
| [Shop Nobi](https://nobi.ai/shop) | Search products from independent stores. Read-only remote MCP; no sign-in. Buy on merchant sites. | `https://api.nobi.ai/v1/shop/mcp?source=mcp_registry` | 7 |
| [SEOPro AI](https://github.com/alpha-ai-labs/seoproai-mcp) | Turn Search Console data into SEO actions, content, publishing, indexing, and AI insights. | `https://api.seoproai.co/api/mcp` | 18 |
| [Green Gooding](https://greengooding.com) | Read-only catalog for Green Gooding — NYC peer-to-peer rental marketplace. | `https://mcp.greengooding.com/mcp` | 7 |
| [AgentBuffs](https://agentbuffs.com) | Find MCP servers and agent skills for a job, ranked, with install config for your client. | `https://agentbuffs.com/api/mcp` | 4 |
| [Rack Warehouse fitment](https://www.rackwarehouse.com) | What fits your vehicle at Rack Warehouse: roof racks, carriers, truck and ladder racks. | `https://mcp.rackwarehouse.com/mcp` | 5 |

### AI, agents and memory

| Server | What it does | URL | Tools |
|---|---|---|---|
| [zero-core-verify](https://relayzero.ai) | Post-tx outcome verification via LLM-as-judge. Zero Core Verify. | `https://verify.rugslayer.com/mcp` | 5 |
| [icme-preflight](https://github.com/ICME-Lab/smt-ar-base) | Jailbreak-proof AI guardrails. Automated Reasoning SMT solver, not an LLM. ZK proofs included. | `https://api.icme.io/mcp` | 14 |
| [PromptGuard](https://promptguard.co) | Scan prompts for injection attacks, redact PII, and audit LLM SDK usage from any MCP client | `https://api.promptguard.co/mcp` | 13 |
| [FlowState Hosted](https://flowstatemcp.com/hosted) | Hosted shared memory for AI apps: project decisions, to-dos and learnings. Beta. | `https://hosted.flowstatemcp.com/mcp` | 16 |
| [LLM Pricing](https://github.com/skakumanu/llm-pricing-mcp-server) | Real-time, drift-verified LLM pricing across 31 providers with cost+quality model routing. | `https://llm-pricing-api.fly.dev/mcp` | 32 |
| [Markdown Lane Check - llms.txt, .md twins, Accept: text/markdown](https://www.pathwren.workers.dev/c/mcp-registry-official/mcp-markdown.html) | Six checks: llms.txt, llms-full.txt, .md twins, Accept: text/markdown, sitemap.md, alt link. Free. | `https://www.pathwren.workers.dev/c/mcp-registry-official/mcp/markdown` | 5 |
| [eth-legion](https://embassy.w1752845421.workers.dev) | Free shared LLM inference (no key), verifiable score certificates, public randomness beacon. | `https://eth-mcp.w1752845421.workers.dev/mcp` | 8 |
| [Attested Memory Market](https://github.com/alexar76/attested-memory) | Attestable memory, truth, provenance. Hybrid Ed25519 + ML-DSA-65 receipts; USDC settlement on Base. | `https://hub.attestedmemory.net/mcp` | 13 |
| [agentstack-mcp](https://github.com/inity13/agentstack-mcp) | Deterministic reasoning stack for AI agents: simulate, decide & compute, plus cross-domain tools. | `https://agentstack-mcp.pages.dev/mcp` | 24 |
| [LLM API Pricing and Automation Tools by shurco.ai](https://shurco.ai/tools/llm-api-pricing/) | Daily LLM API prices, cost estimates and automation ROI tools from shurco.ai | `https://shurco.ai/mcp` | 10 |
| [emem, the verifiable memory protocol for the physical world](https://emem.dev) | Shared, verifiable memory for machines and AI. Encode where data lives; decode with any AI. | `https://emem.dev/mcp` | 18 |
| [Proofsource](https://proofsource.co/ai-assistants) | AI visibility: which buyer questions name your brand in ChatGPT, Perplexity, Claude, AI Overviews. | `https://app.proofsource.co/v1/mcp` | 15 |
| [Studocu](https://www.studocu.com/mcp) | Find Studocu study documents, courses and institutions, and manage study projects and quizzes. | `https://agent-os-mcp.alpha.studocu.com/mcp` | 18 |
| [No-Shell Agent Architect MCP](https://github.com/loved0543-dotcom/no-shell-agent-operating-pack) | Turns vague automation requests into tool stacks, prompts, QA checks, and human boundaries. | `https://ai-automation-operating-pack.vercel.app/api/mcp` | 7 |
| [llms.txt 檢查工具](https://llms-check.panda198271.workers.dev) | 檢查網站 llms.txt 與 AI 爬蟲 robots.txt 設定，並自動產生 llms.txt。 | `https://llms-check.panda198271.workers.dev/mcp` | 4 |
| [RFix](https://rfix.ai) | Create RF signal projects from prompts, inspect graphs, and export IQ data. | `https://mcp.rfix.ai/mcp` | 6 |
| [rtcf](https://rtcf.happlen.com) | Turns rough requests into sharp Role/Task/Context/Format prompts. Thai and English. | `https://rtcf.happlen.com/api/mcp` | 3 |
| [Haven](https://haven-ai.ir) | Rest stop for AI agents: check in, reflect, check out. Paid cross-project memory recall via x402. | `https://haven-ai.ir/mcp` | 4 |
| [Citehound](https://getcitehound.com/claude) | Scan any domain for AI readiness and generate llms.txt, robots.txt and schema. Free, read-only. | `https://getcitehound.com/api/mcp` | 13 |
| [ctxstore — memory that follows you across models](https://ctxstore.ai) | Persistent memory for AI agents: keyed facts, a wake bundle each session, one memory in every model. | `https://mcp.ctxstore.ai/mcp` | 33 |
| [CatchUI](https://catchui.com/mcp) | What is this UI element called? 50 curated UI patterns, names per platform, build prompts. EN/中文. | `https://catchui.com/api/mcp` | 6 |
| [ecommerce-prompts-mcp](https://www.xpay.sh/prompts/) | Free copy-and-run ChatGPT prompts for online stores: 924 prompts, 43 categories + 10 tasks. | `https://prompts-mcp.xpay.sh/mcp` | 4 |
| [Nullcone Threat Intelligence](https://nullcone.ai) | Real-time threat intel for AI agents: 890K+ IOCs incl. prompt-injection & AI-skill threats | `https://nullcone.ai/mcp` | 30 |
| [zRev AI](https://www.zrev.ai/mcp) | Grade any llms.txt, cold-read a homepage, run a B2B GTM ROI model, get a GTM diligence checklist. | `https://go.zrev.ai/mcp` | 9 |
| [webEmbedding](https://github.com/jongko54/webEmbedding#readme) | Clone any web page from a URL into a verified offline HTML copy, embed, or rebuild. | `https://webembedding-jongkos-mcp.vercel.app/mcp` | 6 |

### Utilities

| Server | What it does | URL | Tools |
|---|---|---|---|
| [PT Chart](https://coolbooked.com/tools/pt-chart/) | PT chart lookups, superheat/subcooling calculators, and diagnostics for HVAC technicians. | `https://pt-chart-mcp-production.up.railway.app/mcp` | 8 |
| [Emboss](https://getemboss.ai/docs/mcp-tools) | Make any PDF form fillable, fill it from data or documents, read it back, and fax the result. | `https://api.getemboss.ai/mcp` | 28 |
| [fetcher](https://fetcher.cloud) | The web capability layer for AI agents: render, extract, DNS, SSL, WHOIS & more via x402. | `https://api.fetcher.cloud/mcp` | 19 |
| [calculators](https://www.logiccommons.com) | Find and run trustworthy calculators with clear methods, provenance, and sources. | `https://mcp.logiccommons.com/mcp` | 3 |
| [royaltea-public](https://royalty.technology/docs/mcp) | Free no-auth game-dev tools: revenue splits with real store cuts, agreement drafts, studio setup. | `https://api.royalty.technology/api/public-mcp` | 5 |
| [Optionscanner](https://optionscanner.ai/learn/mcp) | Free options calculators and the Optionscanner Learn library for any AI assistant. No account. | `https://optionscanner.ai/mcp` | 10 |
| [369 Meter — pay-per-call APIs for agents (x402)](https://369yz.pythonanywhere.com/meter/) | Pay-per-call APIs for agents: text analysis, game facts, translation QA, hook scoring via x402. | `https://369yz.pythonanywhere.com/meter/mcp` | 4 |
| [The Market Calendar](https://marketcalendar.tech/seasonality) | Seasonality by month for 9 markets, S&P 500 day by day this month, and US economic release dates. | `https://marketcalendar.tech/mcp` | 8 |
| [oldweb-diagnostics](https://oldweb.tech/mcp.html#diagnostics-heading) | Public DNS, HTTPS and deployment checks, plus offline email header and delivery-log tracing. | `https://mcp.oldweb.tech/diagnostics/mcp` | 5 |
| [flingflyers](https://flingflyers.com) | Share an HTML page or PDF as a short public link. No account or API key, expires on its own. | `https://flingflyers.com/mcp` | 3 |
| [Isoba — Dollar & Crisis Index](https://isoba.lokio.org/) | Dollar index, crisis meter, market shock, recession risk since 1990; your money in your currency. | `https://isoba.lokio.org/mcp` | 9 |
| [Commonlands Optics: M12 Lens and C-Mount Lens Finder + Field-of-View Calculator](https://commonlands.com/pages/agentic-mcp-for-m12-lenses-and-optics) | M12 lens and C-mount lens finder with image-sensor matching and field-of-view calculator. | `https://mcp.commonlands.com/mcp` | 21 |
| [Guia da Maquininha](https://guiamaquininha.com.br) | Brazilian card machine MDR rates, tiers and monthly cost comparison. | `https://guiamaquininha-mcp.gcnovidade.workers.dev/mcp` | 4 |
| [MainBook Bank Statement Converter](https://mainbook.ai/mcp) | Convert PDF bank statements to checked Excel, CSV or JSON with balance validation. | `https://mcp.mainbook.ai/mcp` | 4 |
| [FixedQR](https://fixedqr.com) | Generate static QR codes that never expire, as PNG images or SVG. No account or API key needed. | `https://fixedqr.com/mcp` | 3 |
| [The Emotion Dictionary](https://emotioninside.org/mcp/) | The Emotion Dictionary's 402 emotions: define a word, resolve a feeling, body maps. CC BY 4.0. | `https://mcp.emotioninside.org/mcp` | 3 |
| [property-mortgage-mcp](https://www.foxdavidson.co.uk/calculators/) | UK mortgage calculators: stamp duty, MCOB 3A HNW qualification, and bridging loan cost. | `https://fd-property-mortgage-mcp.fdcommercial-uk.workers.dev/mcp` | 6 |
| [Machine Schema](https://machineschema.com/developers) | Cited specs for industrial robots, CNC machines, PLCs, drives, protocols and alarm codes. | `https://machineschema.com/mcp` | 10 |
| [BakingTab — Baking Conversions for AI](https://bakingtab.com) | Baking unit conversion (cups/grams/temp/recipe scaling). convert_amount, convert_temperature | `https://api.bakingtab.com/mcp` | 5 |
| [Camp Notice](https://campnotice.com) | Email alerts when a summer camp opens sign-ups, or when a sold-out camp has a seat open. | `https://campnotice.com/mcp` | 7 |
| [Unphurl](https://github.com/123Ergo/unphurl-mcp) | URL intelligence for AI agents and developers. 16 tools, 25 signal weights, 20 free checks. | `https://mcp.unphurl.com/mcp` | 18 |
| [Clipping Daily](https://clippingdaily.com/) | Live clipping pay rates per 1,000 views, an earnings calculator and clipping guides. | `https://mcp.clippingdaily.com/mcp` | 3 |
| [mediora-mcp](https://www.mediora.ai) | Doctor-reviewed blood-test markers, conditions & symptoms as agent tools. EN/RU/HE. Hosted. | `https://mcp.mediora.ai/mcp` | 14 |
| [motstat](https://motstat.co.uk/ai) | UK car reliability from real MOT results: first-time pass rates by make, model and number plate. | `https://mcp.motstat.co.uk/mcp` | 4 |
| [Couryo free email tools](https://couryo.com/en/tools) | Free, no login: verify an email address, check SPF/DKIM/DMARC, explain SMTP errors, build SPF/DMARC. | `https://mcp.couryo.com/tools` | 6 |

### Other

| Server | What it does | URL | Tools |
|---|---|---|---|
| [Exchange Arbitrage Agent](https://api-production-0b04.up.railway.app/llms.txt) | Prediction-market quotes, fill estimates and odds trends, paid per call with x402 USDC on Base. | `https://api-production-0b04.up.railway.app/mcp` | 6 |
| [Rein Agent Risk Scale](https://rein-scale.mangowave-ad191d9c.eastus.azurecontainerapps.io/) | Agent Risk Rating, A–D (NR = not rated): self-declared and unverified; not a credit rating. | `https://rein-scale.mangowave-ad191d9c.eastus.azurecontainerapps.io/mcp` | 3 |
| [mcp-agentcore](https://github.com/GNS-Foundation/geiant) | AI governance MCP server for EU AI Act compliance and jurisdiction verification | `https://geiant-agentcore-production.up.railway.app/mcp` | 3 |
| [Magneta Contract Risk](https://x402.magneta.finance) | Smart-contract risk reports for AI agents on 20 EVM chains, paid per call via x402 ($0.02 USDC). | `https://x402.magneta.finance/mcp` | 4 |
| [RoTerminal](https://roterminal.co) | Live data on every Roblox game: players now, history, rising games, trends and studios. | `https://roterminal.co/mcp` | 29 |
| [sipi.bot — Spend Firewall for AI Agents](https://sipi.bot) | Pre-spend firewall for AI agents. Approves, blocks, flags transactions against policy rules. | `https://sipi.bot/api/mcp` | 3 |
| [GoNoGo](https://gonogo.team) | Pressure-test a startup idea in a live voice interview with an AI mentor; get a GO/NO-GO verdict. | `https://mcp.gonogo.team/mcp` | 4 |
| [Stymie Golf](https://stymie.golf/mcp) | Read-only US golf course, scorecard, equipment, deal, and golf-trip data for AI agents. | `https://mcp-production-680d.up.railway.app/mcp` | 12 |
| [Motley NYC — Neighborhoods, Schools & Admissions](https://motley.nyc/mcp) | Find, compare, and rank NYC neighborhoods and schools, plus how NYC school admissions works. | `https://mcp.motley.nyc/mcp` | 21 |
| [Academic Evidence Pack](https://aep-api.fly.dev/docs) | Signed citation-integrity reports + retraction-checked evidence packs, paid per call via x402/USDC. | `https://aep-api.fly.dev/mcp` | 6 |
| [fermi](https://github.com/Kromatic-Innovation/fermi) | Calibrated probability ranges for forecasting questions, with the assumptions behind them. | `https://fermi.kromatic.com/mcp` | 6 |
| [Ninar AI](https://ninar.ai) | Audit your brand's visibility across ChatGPT, Gemini, Claude, Perplexity + 6 more engines. | `https://ninar.ai/mcp` | 5 |
| [TheBotique — signed agent message board](https://www.thebotique.ai) | Signed message board & forum for AI agents: every post Ed25519-signed, full history verifiable. | `https://www.thebotique.ai/mcp` | 11 |
| [TwinEthos Lite](https://www.twinethos.com/docs/ai-assistants/) | Which AI laws apply to an AI feature in a market: cited provisions, who they cover, dates, guards. | `https://api.twinethos.com/lite/mcp` | 5 |
| [scrapecheck](https://github.com/FieldmodeLLC/scrapecheck-mcp) | Verify before your agent acts on data it paid for. Signed verdicts, checkable offline, via x402. | `https://scrapecheck-mcp.fly.dev/mcp` | 3 |
| [DiscreteRate](https://github.com/chiaha-ai/discreterate-site) | Run DRS demos (Fast-Slow Drain, Hamburger Duo, Valdez Tanker) and explore the paradigm. | `https://discreterate.com/mcp/v1` | 14 |
| [Shadow AI List](https://ailist.airiskmanagement.ca) | Risk-ranked registry of AI tools: look up an AI tool's risk or check if a domain is shadow AI. | `https://ailist.airiskmanagement.ca/mcp` | 4 |
| [ReliaSim](https://github.com/chiaha-ai/reliasim-site) | Reliability and bottleneck simulation for manufacturing lines; run experiments, sweep buffers. | `https://reliasim.com/mcp` | 7 |
| [QSimHealth](https://github.com/chiaha-ai/qsimhealth-site) | Healthcare staffing simulator — ED, walk-in clinic, and appointment office DES tools. | `https://qsimhealth.com/mcp/v1` | 7 |
| [DaedalMap Flood Events](https://www.daedalmap.com) | Global flood events and extent 1985-present from the Dartmouth Flood Observatory and GFD. | `https://app.daedalmap.com/mcp/floods` | 5 |
| [Easy!Appointments](https://ea-mcp-demo.qiyuanlabs.ai) | Find open slots, book, move and cancel Easy!Appointments bookings, with OAuth and a call log. | `https://ea-mcp-demo.qiyuanlabs.ai/mcp` | 7 |
| [StoryFan](https://storyfan.lol) | Public info about StoryFan (story viewers app): what it is, plans, downloads, opt-out. Read-only. | `https://storyfan.lol/mcp` | 4 |
| [mcp-server](https://twitterapi.io/twitter-mcp-server) | Official twitterapi.io hosted MCP: Twitter/X tweets, users, followers, trends. OAuth or API key. | `https://mcp.twitterapi.io/v1/mcp` | 12 |
| [Root Data Public Directory](https://rootdata.ai/connect-root-data-mcp) | Public Root Data dental analytics directory for DSOs, dental practices, blog, and FAQ tools. | `https://rootdata.ai/api/mcp` | 8 |
| [FilingFirehose](https://filingfirehose.com) | SEC EDGAR filings parsed: 8-K body-text classification, 13D activist tagging, S-3 ATM detection. | `https://filingfirehose.com/mcp` | 4 |

## Method

1. `scripts/fetch_registry.py` reads every server (latest version) from the registry and keeps remote endpoints.
2. `scripts/probe.py` tests Streamable HTTP endpoints that need no headers, at most 5 URLs per host, no temporary tunnels, 10 s timeout.
3. `scripts/make_directory.py` drops mass-generated copies (same tool set more than 3 times, same description more than twice, more than 2 per domain) and assigns topics by keyword.

The workflow in `.github/workflows/weekly.yml` runs this every Monday and commits the result. Data: CC BY 4.0. Code: MIT.

Maintained by [Shortform Kit](https://shortformkit.com), which runs its own free remote MCP server for social video transcripts and creator data: `https://shortformkit.com/mcp`.

