# US Sales Tax Economic Nexus Check

Which US states must a remote seller register in for sales tax? Every state's nexus rule. Sourced.

**Endpoint:** `https://us-sales-tax-nexus.nerolabs.workers.dev/mcp` (MCP, Streamable HTTP)
**Sign-in:** none
**About:** https://us-sales-tax-nexus.nerolabs.workers.dev/docs
**Privacy:** https://us-sales-tax-nexus.nerolabs.workers.dev/privacy
**Support:** founder@neroengine.com

## Tools

| Tool | What it does |
|---|---|
| `list_capabilities` | Lists coverage (45 sales tax states plus DC, and the 5 states with no statewide sales tax), the date the data was last checked, and related Nero Labs Rules servers. |
| `check_economic_nexus` | Checks which US states a remote seller (no office, staff or stock in the state) must register in to collect sales tax, from its sales into each state. |
| `list_nexus_thresholds` | Lists the economic nexus threshold of every US sales tax state (or one state) on a date: dollar and transaction thresholds, and/or logic, measurement period, what counts, marketplace rules, when to register and the official source. |
| `list_upcoming_nexus_changes` | Lists economic nexus threshold changes in a date window (for example states dropping the 200 transaction test), soonest first, with the old and new rule and source. |

## Connect

- **Claude (web or desktop):** Settings, Connectors, Add custom connector, paste the endpoint.
- **ChatGPT:** Settings, Apps and connectors, Advanced settings, switch on Developer mode, then Create, paste the endpoint, No authentication.
- **Claude Code:** `claude mcp add --transport http us-sales-tax-nexus https://us-sales-tax-nexus.nerolabs.workers.dev/mcp`
- **Gemini CLI:** `gemini extensions install https://github.com/Nero-Engine/us-sales-tax-nexus-mcp`
- **Cursor, VS Code, Windsurf and others:**

```json
{ "mcpServers": { "us-sales-tax-nexus": { "type": "http", "url": "https://us-sales-tax-nexus.nerolabs.workers.dev/mcp" } } }
```

This repository holds the listing only (README, server.json and the Gemini CLI extension manifest). The server runs at the endpoint above.

Built by Nero Labs (Nero Engine Group Ltd, UK).
