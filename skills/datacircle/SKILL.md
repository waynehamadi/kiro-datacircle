---
name: datacircle
description: "Find the best GTM API for a job, from Datacircle's sheet of every plan of every GTM API: price per 1,000, score, rate limits, speed and the fields it returns. Use when the user asks which API to use, what an API costs, or to compare GTM APIs (email finders, enrichment, people and company data)."
---

# Datacircle

Find the best GTM APIs. We benchmark all the GTM APIs and we put the results on our website. The `datacircle` MCP server of this power is open to anyone, with no key, and answers from the sheet.

## Tools

- `list_apis`: lists the APIs on the sheet and the number of plans and providers for each. Call it first, and pass an API's name to `search_plans`.
- `search_plans`: the sheet's rows, one for each plan of each call, best first. Pass `api` (a name from `list_apis`), `query` for a provider or a plan, `sort` (`price` for the cheapest first), `limit` and `offset`. Each plan has its provider, plan, billing, $ per 1,000 (`perThousand`), score out of 100 (`score`), rate limits, speed, the fields it returns and its page on datacircle.dev. What each key means: https://datacircle.dev/fields

## How to answer

- Say the plan's price per 1,000 and its score, and link its page.
- The best plans come first, as on the sheet. Compare a few of them, not the whole list.
- With `api`, the answer links the API's best page (`bestPage`), which ranks its providers on our benchmark. Give it.
- The same data is a REST API with no key, https://api.datacircle.dev/v1 (spec: https://api.datacircle.dev/v1/openapi.json), and one file with no sign-up: https://datacircle.dev/datacircle.json.
