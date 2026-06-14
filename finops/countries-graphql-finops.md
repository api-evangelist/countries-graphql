# Countries GraphQL API - FinOps

## Overview

The Countries GraphQL API is a free, open-source public API. There are no direct costs associated with consuming the public endpoint.

## Cost Structure

| Item | Cost |
|---|---|
| Public API usage | $0 |
| Authentication / API keys | Not required |
| Paid tiers or quotas | None |

## Self-Hosting Costs

If your organization requires SLA guarantees or higher reliability than a community-maintained free API provides, you can self-host the open-source project. Estimated infrastructure costs for self-hosting:

- **Compute:** Minimal — the API serves static country data; a small serverless function or low-tier container is sufficient.
- **Hosting options:** Vercel, Netlify, Fly.io, or any Node.js-compatible platform.
- **Data:** Country data is bundled from the `countries-list` npm package; no external database is needed.

## FinOps Recommendations

- Use the free public endpoint for development and low-traffic production workloads.
- Cache GraphQL responses aggressively — country data rarely changes, making it ideal for long-TTL edge caching.
- If self-hosting via Stellate/GraphCDN, review that platform's pricing for caching and analytics features.

## Pricing Transparency

Pricing details for the managed public endpoint are **not publicly available** — the API is offered as a free community service with no documented monetization model as of 2026-06-14.

## Source

- https://github.com/trevorblades/countries
