# Sayod 111 B2B and E-Commerce Intelligence MCP Server

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

## REST API Discovery
- Postman Public Workspace: https://www.postman.com/s-ali-mohamed-bh-2153051/sayod-111-intelligence-apis/overview
- Apify Creator Profile: https://apify.com/sayod111
