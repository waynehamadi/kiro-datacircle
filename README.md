# Datacircle power for Kiro

Find the best GTM APIs. We benchmark all the GTM APIs and we put the results on our website: https://datacircle.dev

This power adds our MCP server to Kiro: `https://api.datacircle.dev/mcp`, Streamable HTTP, open to anyone, with no key. It answers from the sheet. `list_apis` lists the GTM APIs on it, and `search_plans` finds their plans by API, provider or price. Each plan comes with its score, and the best come first, as on the sheet.

## Install

In Kiro: Powers panel, **Add Custom Power**, **Import power from a repository URL**, then `https://github.com/waynehamadi/kiro-datacircle`.

In Kiro CLI:

```
git clone https://github.com/waynehamadi/kiro-datacircle
kiro-cli powers install ./kiro-datacircle
```

The power turns on when you talk about GTM APIs, email finders, enrichment or API prices.

## What it has

- `plugin.json`: the power's manifest, in the Agent Plugins format.
- `mcp.json`: our MCP server.
- `skills/datacircle/SKILL.md`: how to use its two tools.

The same data is a REST API with no key, https://api.datacircle.dev/v1 (spec: https://api.datacircle.dev/v1/openapi.json).

Docs: https://datacircle.dev/docs/mcp. Privacy: https://datacircle.dev/privacy. Support: https://datacircle.dev/support or wayne@datacircle.dev. MIT license.
