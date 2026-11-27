# Installing US Sales Tax Economic Nexus Check (remote MCP server, no install needed)

US Sales Tax Economic Nexus Check is a hosted remote MCP server. There is nothing to download, build or run, and no API key.

Add this to the MCP settings file (in Cline: MCP Servers, Configure, then cline_mcp_settings.json):

```json
{
  "mcpServers": {
    "us-sales-tax-nexus": {
      "type": "streamableHttp",
      "url": "https://us-sales-tax-nexus.nerolabs.workers.dev/mcp",
      "disabled": false,
      "autoApprove": []
    }
  }
}
```

Save the file. The server's tools appear straight away. To check it works, ask the assistant to list the server's tools.

Docs: https://us-sales-tax-nexus.nerolabs.workers.dev/docs
