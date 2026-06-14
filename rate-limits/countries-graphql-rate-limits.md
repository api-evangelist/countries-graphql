# Countries GraphQL API - Rate Limits

## Overview

Formal rate limit information for the Countries GraphQL API is not publicly documented. The API is a free, open-source public service and does not publish explicit rate-limit thresholds.

## Known Details

- The API is powered by **Stellate** (formerly GraphCDN), which provides GraphQL edge caching and can implicitly throttle abusive traffic patterns.
- No API key or authentication is required, so limits are enforced at the infrastructure level rather than per-user.
- The project README and GitHub repository do not specify request-per-second or daily quota limits.

## Recommendations

- Implement client-side caching of responses where possible to reduce repeated identical queries.
- Avoid high-frequency polling; country data changes infrequently and is well-suited to long cache TTLs.
- If building a production application, consider self-hosting the open-source repository to avoid dependency on the shared public endpoint.

## Status

Rate limit details are **not publicly available** as of 2026-06-14.

## Source

- https://github.com/trevorblades/countries
