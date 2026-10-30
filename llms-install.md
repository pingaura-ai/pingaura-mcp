# Installing the PingAura MCP server

PingAura is a hosted (remote) MCP server. There is nothing to clone, build or run locally.

1. Add a remote MCP server with this URL, using the Streamable HTTP transport:
   `https://www.pingaura.ai/api/mcp`
2. Authentication is OAuth 2.1 with dynamic client registration. On first use the client opens a browser window; the user signs in to PingAura and approves access. No API key is needed in config.
3. Example `mcp.json` / Cline config:

```json
{
  "mcpServers": {
    "pingaura": {
      "url": "https://www.pingaura.ai/api/mcp"
    }
  }
}
```

4. Verify by calling `get-account-info` or `list-domains`.

A PingAura account is required: https://www.pingaura.ai
