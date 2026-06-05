# Bright Data (bright-data)

Bright Data is an Israeli web data platform and operator of the world's largest legitimate residential proxy network (400M+ IPs across 195 countries). The platform combines proxy infrastructure (residential, ISP, datacenter, mobile) with higher-level web-access APIs — Web Unlocker, SERP API, Web Scraper API, Scraping Browser, Deep Lookup, and Web Archive — plus a 350-dataset marketplace and an MCP server that exposes 60+ web-access tools to AI agents. Serves 20,000+ customers across eCommerce, finance, real estate, ad-tech, and AI/ML, and is a primary supplier of training and grounding data for foundation-model providers.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Web Data
- Web Scraping
- Proxy
- Residential Proxy
- Datacenter Proxy
- ISP Proxy
- Mobile Proxy
- SERP
- Web Unlocker
- Scraping Browser
- Dataset Marketplace
- MCP
- AI Agents

## Timestamps

- **Created:** 2026-03-26
- **Modified:** 2026-05-25

## APIs

### Bright Data Web Unlocker API

Single-endpoint web unblocking with a 98%+ success rate. Send any URL, Bright Data handles residential proxy selection, JavaScript rendering, CAPTCHA solving, fingerprint spoofing, and anti-bot evasion, returning the fully rendered page. Supports both synchronous and asynchronous modes via `/unblocker/req` with `/unblocker/get_result` for polling. Pay only for successful requests.

- **Human URL:** [https://docs.brightdata.com/scraping-automation/web-unlocker/introduction](https://docs.brightdata.com/scraping-automation/web-unlocker/introduction)

#### Tags

- Web Unlocker
- Unblocking
- Anti-Bot
- CAPTCHA

#### Properties

- [Documentation](https://docs.brightdata.com/scraping-automation/web-unlocker/introduction)
- [Documentation](https://docs.brightdata.com/scraping-automation/web-unlocker/async-requests)
- [OpenAPI](openapi/bright-data-web-unlocker-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bright-data-web-unlocker-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-web-unlocker-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bright Data SERP API

Real-time SERP data from Google, Bing, Yandex, and DuckDuckGo across 31 languages and 195 countries. Supports organic, news, images, videos, shopping, jobs, hotels, flights, lens, trends, reviews, maps, and AI Overview result types. Submit asynchronous requests via `/serp/req` and poll `/serp/get_result`, or stream synchronously over the proxy on port 33335. Geolocation, device, browser, pagination, and localization parameters supported.

- **Human URL:** [https://docs.brightdata.com/scraping-automation/serp-api/introduction](https://docs.brightdata.com/scraping-automation/serp-api/introduction)

#### Tags

- SERP
- Search
- Google
- Bing

#### Properties

- [Documentation](https://docs.brightdata.com/scraping-automation/serp-api/introduction)
- [Documentation](https://docs.brightdata.com/scraping-automation/serp-api/send-your-first-request)
- [OpenAPI](openapi/bright-data-serp-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bright-data-serp-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-serp-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bright Data Web Scraper API

Asynchronous snapshot-based scraping over 660+ pre-built dataset endpoints (Amazon, Walmart, LinkedIn, Instagram, TikTok, YouTube, Reddit, Google Maps, Airbnb, Booking, Zillow, and many more) plus custom collectors. Trigger via `POST /datasets/v3/scrape`, poll `/datasets/v3/progress/{snapshot_id}`, and download via `/datasets/v3/snapshot/{snapshot_id}`. Returns JSON, NDJSON, CSV, or Parquet; supports direct delivery to S3, Azure Blob, GCS, Snowflake, and webhooks.

- **Human URL:** [https://docs.brightdata.com/scraping-automation/web-scraper-api/overview](https://docs.brightdata.com/scraping-automation/web-scraper-api/overview)

#### Tags

- Web Scraping
- Datasets
- Structured Data

#### Properties

- [Documentation](https://docs.brightdata.com/scraping-automation/web-scraper-api/overview)
- [Documentation](https://docs.brightdata.com/scraping-automation/web-scraper-api/trigger-a-collection)
- [OpenAPI](openapi/bright-data-web-scraper-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bright-data-web-scraper-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-web-scraper-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/bright-data-snapshot-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Bright Data Scraping Browser API

Fully managed remote Chromium browsers driven over CDP/WebSocket from Puppeteer, Playwright, or Selenium. Each session ships with built-in unlocker logic, residential proxy egress, CAPTCHA solving, and fingerprint management so JavaScript-heavy and interactive flows complete reliably. REST endpoints expose session inventory (`GET /browser_sessions`) for observability and lifecycle inspection.

- **Human URL:** [https://docs.brightdata.com/scraping-automation/scraping-browser/introduction](https://docs.brightdata.com/scraping-automation/scraping-browser/introduction)

#### Tags

- Browser Automation
- Headless Browser
- Puppeteer
- Playwright
- Selenium

#### Properties

- [Documentation](https://docs.brightdata.com/scraping-automation/scraping-browser/introduction)
- [Documentation](https://docs.brightdata.com/scraping-automation/scraping-browser/quickstart)
- [OpenAPI](openapi/bright-data-scraping-browser-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bright-data-scraping-browser-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-scraping-browser-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bright Data Deep Lookup API

Find companies and professionals across 1,000+ public sources with 95%+ accuracy. Submit a natural-language description or structured query via `POST /trigger`, preview row counts with `/preview`, optimize the query with `/enhance_query`, and enrich existing columns with `/request/{id}/enrich`. Results are downloaded via `/request/{id}/download`. Billed per result.

- **Human URL:** [https://docs.brightdata.com/api-reference/deep-lookup/Deep-Lookup-API-Overview](https://docs.brightdata.com/api-reference/deep-lookup/Deep-Lookup-API-Overview)

#### Tags

- Entity Resolution
- People Search
- Company Search
- Enrichment

#### Properties

- [Documentation](https://docs.brightdata.com/api-reference/deep-lookup/Deep-Lookup-API-Overview)
- [OpenAPI](openapi/bright-data-deep-lookup-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bright-data-deep-lookup-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-deep-lookup-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bright Data Web Archive API

Search and deliver petabyte-scale historical web snapshots across 250+ domains. Submit a query via `POST /webarchive/search`, monitor with `GET /webarchive/search/{search_id}`, list all searches via `GET /webarchive/searches`, and deliver matching corpora to S3/Azure/GCS via `POST /deliver-to-cloud`.

- **Human URL:** [https://docs.brightdata.com/api-reference/web-archive-api/Web-Archive-API-Overview](https://docs.brightdata.com/api-reference/web-archive-api/Web-Archive-API-Overview)

#### Tags

- Historical Data
- Web Archive
- Time Series

#### Properties

- [Documentation](https://docs.brightdata.com/api-reference/web-archive-api/Web-Archive-API-Overview)
- [OpenAPI](openapi/bright-data-web-archive-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bright-data-web-archive-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-web-archive-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bright Data Dataset Marketplace API

Programmatic access to 350+ ready-to-use datasets across 250+ domains (eCommerce, social, real estate, travel, business). List available datasets via `GET /datasets`, inspect schemas via `GET /datasets/{dataset_id}/metadata`, retrieve snapshots via `GET /datasets/snapshots/{id}`, and push deliveries to S3, Azure, GCS, Snowflake, or webhooks via `POST /datasets/snapshots/{id}/deliver`.

- **Human URL:** [https://docs.brightdata.com/datasets/marketplace](https://docs.brightdata.com/datasets/marketplace)

#### Tags

- Datasets
- Marketplace
- Bulk Data

#### Properties

- [Documentation](https://docs.brightdata.com/datasets/marketplace)
- [OpenAPI](openapi/bright-data-dataset-marketplace-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bright-data-dataset-marketplace-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-dataset-marketplace-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bright Data Account Management API

Manage Bright Data zones (proxy pools and product entitlements), IP allocations, access control, and billing programmatically. Endpoints include `POST/GET/DELETE /zone`, `/zone/change_disable`, `/zone/ips` (add/remove/refresh/migrate/statistics), `/zone/whitelist`, `/zone/blacklist`, `/zone/domain_perm`, plus `/customer/balance` and `/zone/bw` for balance and bandwidth reporting.

- **Human URL:** [https://docs.brightdata.com/api-reference/account-management-api/Account-Management-API-Overview](https://docs.brightdata.com/api-reference/account-management-api/Account-Management-API-Overview)

#### Tags

- Administrative
- Zones
- Billing

#### Properties

- [Documentation](https://docs.brightdata.com/api-reference/account-management-api/Account-Management-API-Overview)
- [OpenAPI](openapi/bright-data-account-management-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bright-data-account-management-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-account-management-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/bright-data-zone-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Bright Data Proxy Manager API

Local self-hosted REST control plane (port 22999) for the Bright Data Proxy Manager. Programmatically create and configure proxy ports (`/api/proxies`, `/api/proxies/{PORT}`), ban offending IPs (`/api/proxies/{PORT}/banip`), refresh IP pools (`/api/refresh_ips`), and read zone configuration (`/api/zones`). Supports SSL, logging, statistics, and remote upgrade/restart endpoints.

- **Human URL:** [https://docs.brightdata.com/proxy-networks/proxy-manager/api](https://docs.brightdata.com/proxy-networks/proxy-manager/api)

#### Tags

- Proxy Manager
- Local API
- Self-Hosted

#### Properties

- [Documentation](https://docs.brightdata.com/proxy-networks/proxy-manager/api)
- [OpenAPI](openapi/bright-data-proxy-manager-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bright-data-proxy-manager-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-proxy-manager-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bright Data Scraping Shield API

Compliance-focused classification API that exposes Bright Data's allowlist/blocklist taxonomy. `GET /shield/class` lists every classification, `/shield/domains_by_class` returns domains by category, `/shield/samples` returns sample classifications, and `/shield/zones_by_class` reports the zones cleared for each class.

- **Human URL:** [https://docs.brightdata.com/api-reference/scraping-shield-api/Scraping-Shield-API-Overview](https://docs.brightdata.com/api-reference/scraping-shield-api/Scraping-Shield-API-Overview)

#### Tags

- Compliance
- Domain Classification
- Trust and Safety

#### Properties

- [Documentation](https://docs.brightdata.com/api-reference/scraping-shield-api/Scraping-Shield-API-Overview)
- [OpenAPI](openapi/bright-data-scraping-shield-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bright-data-scraping-shield-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-scraping-shield-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Bright Data MCP Server

Bright Data's Model Context Protocol server exposes 60+ web-access tools (search, scrape, structured extraction, browser automation, datasets) to MCP-compatible clients including Claude Desktop, Claude Code, ChatGPT, Cursor, LangChain, LangGraph, LlamaIndex, CrewAI, n8n, Google ADK, NVIDIA NeMo, and Cloudflare Agents. Available as a hosted endpoint (5,000 free requests/month), self-hosted, and remote.

- **Human URL:** [https://docs.brightdata.com/mcp-server/overview](https://docs.brightdata.com/mcp-server/overview)

#### Tags

- MCP
- Model Context Protocol
- AI Agents
- Tools

#### Properties

- [Documentation](https://docs.brightdata.com/mcp-server/overview)
- [Source Code](https://github.com/brightdata/brightdata-mcp)
- [Postman Collection](collections/bright-data-account-management-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-account-management-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/bright-data-dataset-marketplace-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-dataset-marketplace-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/bright-data-deep-lookup-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-deep-lookup-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/bright-data-proxy-manager-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-proxy-manager-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/bright-data-scraping-browser-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-scraping-browser-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/bright-data-scraping-shield-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-scraping-shield-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/bright-data-serp-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-serp-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/bright-data-web-archive-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-web-archive-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/bright-data-web-scraper-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-web-scraper-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/bright-data-web-unlocker-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data-web-unlocker-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/bright-data.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bright-data.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://brightdata.com)
- [Documentation](https://docs.brightdata.com)
- [Getting Started](https://docs.brightdata.com/quickstart)
- [Sign Up](https://brightdata.com/cp/start)
- [Login](https://brightdata.com/cp/zones)
- [Pricing](https://brightdata.com/pricing)
- [Plans](plans/bright-data-plans-pricing.yml)
- [Rate Limits](rate-limits/bright-data-rate-limits.yml)
- [Fin Ops](finops/bright-data-finops.yml)
- [Blog](https://brightdata.com/blog)
- [Status Page](https://status.brightdata.com)
- [Terms of Service](https://brightdata.com/legal/tos)
- [Privacy Policy](https://brightdata.com/legal/privacy-policy)
- [Trust Center](https://brightdata.com/trust-center)
- [Support](https://brightdata.com/contact)
- [LinkedIn](https://www.linkedin.com/company/bright-data)
- [GitHub Organization](https://github.com/luminati-io)
- [GitHub Organization](https://github.com/brightdata)
- [SDK](https://github.com/brightdata/sdk-python)
- [SDK](https://github.com/brightdata/sdk-js)
- [SDK](https://github.com/brightdata/ai-sdk)
- [Command Line Interface](https://github.com/brightdata/cli)
- [Tool](https://github.com/brightdata/brightdata-mcp)
- [Tool](https://github.com/brightdata/openclaw-plugin)
- [Tool](https://github.com/brightdata/brightdata-cursor-plugin)
- [Code Examples](https://github.com/brightdata/bright-data-quickstart-templates)
- [Code Examples](https://github.com/luminati-io/sbr-examples)
- [Integrations](https://brightdata.com/integrations)
- [L L Ms Txt](https://docs.brightdata.com/llms.txt)
- [Documentation](https://docs.brightdata.com/api-reference)
- [Forum](https://discord.gg/brightdata)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
**URL:** https://apievangelist.com
