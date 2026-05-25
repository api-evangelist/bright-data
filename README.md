# Bright Data (bright-data)

Bright Data is an Israeli web data platform and operator of the world's largest legitimate residential proxy network (400M+ IPs across 195 countries). The platform combines proxy infrastructure (residential, ISP, datacenter, mobile) with higher-level web-access APIs — Web Unlocker, SERP API, Web Scraper API, Scraping Browser, Deep Lookup, and Web Archive — plus a 350-dataset marketplace and an MCP server that exposes 60+ web-access tools to AI agents. Serves 20,000+ customers across eCommerce, finance, real estate, ad-tech, and AI/ML, and is a primary supplier of training and grounding data for foundation-model providers.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Web Data, Web Scraping, Proxy, Residential Proxy, Datacenter Proxy, ISP Proxy, Mobile Proxy, SERP, Web Unlocker, Scraping Browser, Dataset Marketplace, MCP, AI Agents

## Timestamps

- **Created:** 2026-03-26
- **Modified:** 2026-05-25

## Headline Numbers

| Surface | Scale |
|---|---|
| Residential IPs | 400M+ across 195 countries |
| ISP IPs | 1.3M+ static residential |
| Mobile IPs | 7M+ 3G/4G/5G |
| Pre-built scrapers | 660+ |
| Marketplace datasets | 350+ across 250+ domains |
| MCP tools | 60+ |
| Uptime / Success | 99.99% / 99.95% |
| Customers | 20,000+ |

## APIs

### Bright Data Web Unlocker API
Single-endpoint unblocking with 98%+ success rate. Bright Data manages proxy selection, JavaScript rendering, CAPTCHA solving, fingerprinting, and anti-bot evasion. Supports synchronous (`POST /request`) and asynchronous (`POST /unblocker/req` + `GET /unblocker/get_result`) modes. Pay only for successful requests.

**Human URL:** [https://docs.brightdata.com/scraping-automation/web-unlocker/introduction](https://docs.brightdata.com/scraping-automation/web-unlocker/introduction)

- [OpenAPI](openapi/bright-data-web-unlocker-api-openapi.yml)
- [Naftiko Capability — Web Unlocker](capabilities/web-unlocker.yaml)

### Bright Data SERP API
Real-time Google, Bing, Yandex, and DuckDuckGo SERPs across 31 languages and 195 countries. Result types include organic, news, images, videos, shopping, jobs, hotels, flights, lens, trends, reviews, maps, and AI Overview. Async via `POST /serp/req` + `GET /serp/get_result`; synchronous via proxy on port 33335.

**Human URL:** [https://docs.brightdata.com/scraping-automation/serp-api/introduction](https://docs.brightdata.com/scraping-automation/serp-api/introduction)

- [OpenAPI](openapi/bright-data-serp-api-openapi.yml)
- [Naftiko Capability — SERP](capabilities/serp.yaml)

### Bright Data Web Scraper API
Asynchronous snapshot-based scraping over 660+ pre-built dataset endpoints (Amazon, Walmart, LinkedIn, Instagram, TikTok, YouTube, Reddit, Google Maps, Airbnb, Booking, Zillow, and many more) plus custom collectors. Trigger jobs, poll progress, list/cancel/rerun snapshots, and download or deliver results (JSON, NDJSON, CSV, Parquet) to S3, Azure, GCS, Snowflake, or a webhook.

**Human URL:** [https://docs.brightdata.com/scraping-automation/web-scraper-api/overview](https://docs.brightdata.com/scraping-automation/web-scraper-api/overview)

- [OpenAPI](openapi/bright-data-web-scraper-api-openapi.yml)
- [JSON Schema — Snapshot](json-schema/bright-data-snapshot-schema.json)
- [Naftiko Capability — Web Scraper](capabilities/web-scraper.yaml)

### Bright Data Scraping Browser API
Managed remote Chromium browsers driven over CDP/WebSocket from Puppeteer, Playwright, or Selenium. Each session includes built-in unlocker logic, residential egress, CAPTCHA solving, and fingerprint management. The REST surface exposes session inventory and lifecycle inspection.

**Human URL:** [https://docs.brightdata.com/scraping-automation/scraping-browser/introduction](https://docs.brightdata.com/scraping-automation/scraping-browser/introduction)

- [OpenAPI](openapi/bright-data-scraping-browser-api-openapi.yml)
- [Naftiko Capability — Scraping Browser](capabilities/scraping-browser.yaml)

### Bright Data Deep Lookup API
Natural-language entity research across 1,000+ public sources for companies and professionals with 95%+ accuracy. Trigger, preview, enhance, enrich, monitor, and download. Billed per delivered result.

**Human URL:** [https://docs.brightdata.com/api-reference/deep-lookup/Deep-Lookup-API-Overview](https://docs.brightdata.com/api-reference/deep-lookup/Deep-Lookup-API-Overview)

- [OpenAPI](openapi/bright-data-deep-lookup-api-openapi.yml)
- [Naftiko Capability — Deep Lookup](capabilities/deep-lookup.yaml)

### Bright Data Web Archive API
Petabyte-scale historical web search over 250+ domains. Submit searches, monitor, and deliver matching corpora to cloud storage.

**Human URL:** [https://docs.brightdata.com/api-reference/web-archive-api/Web-Archive-API-Overview](https://docs.brightdata.com/api-reference/web-archive-api/Web-Archive-API-Overview)

- [OpenAPI](openapi/bright-data-web-archive-api-openapi.yml)
- [Naftiko Capability — Web Archive](capabilities/web-archive.yaml)

### Bright Data Dataset Marketplace API
Programmatic access to 350+ ready-to-use datasets across 250+ domains. List, inspect, retrieve snapshots, and deliver to S3, Azure, GCS, Snowflake, or a webhook.

**Human URL:** [https://docs.brightdata.com/datasets/marketplace](https://docs.brightdata.com/datasets/marketplace)

- [OpenAPI](openapi/bright-data-dataset-marketplace-api-openapi.yml)
- [Naftiko Capability — Dataset Marketplace](capabilities/dataset-marketplace.yaml)

### Bright Data Account Management API
Manage zones (proxy pools and product entitlements), IP allocations, access control, passwords, and billing/bandwidth reporting. Includes `/zone`, `/zone/ips`, `/zone/whitelist`, `/zone/blacklist`, `/zone/domain_perm`, `/customer/balance`, and `/zone/bw`.

**Human URL:** [https://docs.brightdata.com/api-reference/account-management-api/Account-Management-API-Overview](https://docs.brightdata.com/api-reference/account-management-api/Account-Management-API-Overview)

- [OpenAPI](openapi/bright-data-account-management-api-openapi.yml)
- [JSON Schema — Zone](json-schema/bright-data-zone-schema.json)
- [Naftiko Capability — Account Management](capabilities/account-management.yaml)

### Bright Data Proxy Manager API
Local self-hosted REST control plane (`http://localhost:22999`) for routing, banning, refreshing IPs, and inspecting zone configuration on the Bright Data Proxy Manager.

**Human URL:** [https://docs.brightdata.com/proxy-networks/proxy-manager/api](https://docs.brightdata.com/proxy-networks/proxy-manager/api)

- [OpenAPI](openapi/bright-data-proxy-manager-api-openapi.yml)
- [JSON Schema — Proxy Port](json-schema/bright-data-proxy-port-schema.json)
- [Naftiko Capability — Proxy Manager](capabilities/proxy-manager.yaml)

### Bright Data Scraping Shield API
Compliance-focused domain classification API. Surfaces `class`, `domains_by_class`, `samples`, and `zones_by_class` so teams can verify a target domain's eligibility against Bright Data's allowlist taxonomy.

**Human URL:** [https://docs.brightdata.com/api-reference/scraping-shield-api/Scraping-Shield-API-Overview](https://docs.brightdata.com/api-reference/scraping-shield-api/Scraping-Shield-API-Overview)

- [OpenAPI](openapi/bright-data-scraping-shield-api-openapi.yml)
- [Naftiko Capability — Scraping Shield](capabilities/scraping-shield.yaml)

### Bright Data MCP Server
Model Context Protocol server exposing 60+ web-access tools (search, scrape, structured extraction, browser automation, datasets) to MCP-compatible clients including Claude Desktop, Claude Code, ChatGPT, Cursor, LangChain, LangGraph, LlamaIndex, CrewAI, n8n, Google ADK, NVIDIA NeMo, Cloudflare Agents, Snowflake Cortex, and Vapi. Available hosted (5,000 free requests/month), self-hosted, or remote.

**Human URL:** [https://docs.brightdata.com/mcp-server/overview](https://docs.brightdata.com/mcp-server/overview)

- [Source — brightdata/brightdata-mcp](https://github.com/brightdata/brightdata-mcp)
- [Naftiko Capability — MCP Server](capabilities/mcp-server.yaml)

## Pricing (Self-Serve)

| Product | Tier | Monthly | Quota / IPs | Unit Rate |
|---|---|---|---|---|
| Web Unlocker | Pay As You Go | $0 | — | $1.50 / 1K results |
| Web Unlocker | Growth | $499 | 380K results | $1.30 / 1K |
| Web Unlocker | Business | $999 | 900K results | $1.10 / 1K |
| Web Unlocker | Premium | $1,999 | 2M results | $1.00 / 1K |
| SERP API | Pay As You Go | $0 | — | $1.50 / 1K results |
| SERP API | Growth | $499 | 380K results | $1.30 / 1K |
| Web Scraper API | Pay As You Go | $0 | — | $1.50 / 1K records |
| Web Scraper API | Scale | $499 | 384K records | $1.30 / 1K |
| Residential Proxies | Pay As You Go | $0 | — | $4.00 / GB |
| Residential Proxies | Growth | $499 | 141 GB | $3.50 / GB |
| Residential Proxies | Business | $999 | 332 GB | $3.00 / GB |
| Residential Proxies | Premium | $1,999 | 798 GB | $2.50 / GB |
| ISP Proxies | Starter | $18 | 10 IPs | $1.80 / IP |
| ISP Proxies | Growth | $145 | 100 IPs | $1.45 / IP |
| Datacenter Proxies | Starter | $14 | 10 IPs | $1.40 / IP |
| Datacenter Proxies | Growth | $100 | 100 IPs | $1.00 / IP |
| Enterprise | All Products | Custom | Custom | Custom + SLA + SSO + AM |

See [`plans/bright-data-plans-pricing.yml`](plans/bright-data-plans-pricing.yml) for the machine-readable plan document, [`rate-limits/bright-data-rate-limits.yml`](rate-limits/bright-data-rate-limits.yml) for rate-limit posture, and [`finops/bright-data-finops.yml`](finops/bright-data-finops.yml) for the FOCUS-aligned FinOps mapping.

## SDKs and Tooling

- [Python SDK — brightdata/sdk-python](https://github.com/brightdata/sdk-python)
- [JavaScript SDK — brightdata/sdk-js](https://github.com/brightdata/sdk-js)
- [AI SDK — brightdata/ai-sdk](https://github.com/brightdata/ai-sdk)
- [CLI — brightdata/cli](https://github.com/brightdata/cli)
- [MCP Server — brightdata/brightdata-mcp](https://github.com/brightdata/brightdata-mcp)
- [OpenClaw Plugin — brightdata/openclaw-plugin](https://github.com/brightdata/openclaw-plugin)
- [Cursor Plugin — brightdata/brightdata-cursor-plugin](https://github.com/brightdata/brightdata-cursor-plugin)
- [Quickstart Templates — brightdata/bright-data-quickstart-templates](https://github.com/brightdata/bright-data-quickstart-templates)
- [Scraping Browser Examples — luminati-io/sbr-examples](https://github.com/luminati-io/sbr-examples)

## Other Artifacts

- [JSON-LD Context](json-ld/bright-data-context.jsonld)
- [Spectral Ruleset](rules/bright-data-rules.yml)
- [Vocabulary](vocabulary/bright-data-vocabulary.yml)

## Links

- [Bright Data](https://brightdata.com)
- [Documentation](https://docs.brightdata.com)
- [API Reference](https://docs.brightdata.com/api-reference)
- [Pricing](https://brightdata.com/pricing)
- [Status](https://status.brightdata.com)
- [Trust Center](https://brightdata.com/trust-center)
- [Sign Up](https://brightdata.com/cp/start)
- [Control Panel](https://brightdata.com/cp/zones)
- [Blog](https://brightdata.com/blog)
- [GitHub — brightdata](https://github.com/brightdata)
- [GitHub — luminati-io](https://github.com/luminati-io)
- [LinkedIn](https://www.linkedin.com/company/bright-data)
- [llms.txt](https://docs.brightdata.com/llms.txt)
