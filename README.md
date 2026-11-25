# Sayod 111 B2B and E-Commerce Intelligence MCP Server

[![Listed on mcpservers.org](https://mcpservers.org/badge.svg)](https://mcpservers.org/servers/sayod111/sayod111-mcp-servers)
[![mcptry](https://mcptry.com/badge/io.github.sayod111/sayod111-intelligence-mcp)](https://mcptry.com/servers/io.github.sayod111/sayod111-intelligence-mcp)

Production remote MCP server by Sayod 111 providing pure Async HTTP/2 commercial data extraction and diagnostics for Claude, ChatGPT, Cursor, VS Code, Clay, n8n, and Make workflows. Apify authentication and usage charges may apply.

## Remote MCP Endpoint (Streamable HTTP)

https://mcp.apify.com/?tools=sayod111/commercepulse-pro,sayod111/b2b-revenue-lead-enricher-mcp,sayod111/b2b-hiring-intent-ats-mcp

## Tools

### 1. CommercePulse Pro (sayod111/commercepulse-pro)
Audits Shopify, WooCommerce, BigCommerce, Magento, PrestaShop, Salla, and Zid storefronts. Returns 78 structured fields including platform, theme, 85+ app and ad-pixel fingerprints with IDs, SEO/CRO technical defects, MX-verified merchant emails, product catalogs, and Clay-ready flat columns.
- Apify Store: https://apify.com/sayod111/commercepulse-pro

### 2. B2B Revenue Intelligence (sayod111/b2b-revenue-lead-enricher-mcp)
Enriches B2B company domains with 97 fields: publicly listed corporate emails, DNS MX/SPF/DMARC verification, 110 technology fingerprints, agency ICP fit scores, and structured outreach notes.
- Apify Store: https://apify.com/sayod111/b2b-revenue-lead-enricher-mcp

### 3. B2B Hiring Intent 7-ATS Scanner (sayod111/b2b-hiring-intent-ats-mcp)
Extracts live open roles across Greenhouse, Lever, Ashby, Workable, SmartRecruiters, Recruitee, and BreezyHR alongside 6 B2B buying intent categories, hiring velocity scores, and corporate contacts.
- Apify Store: https://apify.com/sayod111/b2b-hiring-intent-ats-mcp

## Quick Setup (Claude Desktop / Cursor / VS Code)

```json
{
  "mcpServers": {
    "sayod111-intelligence": {
      "url": "https://mcp.apify.com/?tools=sayod111/commercepulse-pro,sayod111/b2b-revenue-lead-enricher-mcp,sayod111/b2b-hiring-intent-ats-mcp"
    }
  }
}
```

See [Apify MCP documentation](https://docs.apify.com/platform/integrations/mcp) for authentication.

## Cloudflare gateway

Connect to https://sayod111-mcp-gateway.sayodyalawi.workers.dev/mcp and call `tools/list` to discover the active tools. Live Actor calls require your Apify token in the Authorization Bearer header. Access to the WealthPulse and Trust Center Actors is restricted until their Store publication.

### Version 1.2.0

The prepared gateway exposes ten tools. The four additions read public data. Discovery needs no credentials. Calls use `Authorization: Bearer <APIFY_TOKEN>` and can incur Apify charges. Availability depends on gateway deployment and the caller's access to each Actor.

| MCP tool | Apify Actor |
|---|---|
| `us_healthcare_kol_cms_enricher` | `us-healthcare-kol-cms-enricher` |
| `us_sled_gov_bids_monitor` | `us-sled-gov-bids-monitor` |
| `us_ucc_1_secured_loan_leads` | `us-ucc-1-secured-loan-leads` |
| `us_biotech_grants_trials_fda510k` | `us-biotech-grants-trials-fda510k` |

## REST API Discovery
- Postman Public Workspace: https://www.postman.com/s-ali-mohamed-bh-2153051/sayod-111-intelligence-apis/overview
- Apify Creator Profile: https://apify.com/sayod111
