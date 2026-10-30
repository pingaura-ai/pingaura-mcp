# PingAura MCP server

Connect AI assistants and coding agents to [PingAura](https://www.pingaura.ai), the AI visibility platform. Ask about your brand's AI visibility score, share of voice against competitors, which prompts mention you, site health for AI crawlers, and draft or publish articles, all from your assistant.

This repository holds install instructions and client configs. The server itself is hosted by PingAura.

- **Endpoint:** `https://www.pingaura.ai/api/mcp` (Streamable HTTP)
- **Auth:** OAuth 2.1 with dynamic client registration and PKCE. Your client opens a browser to sign in; no API keys in config.
- **Docs:** https://www.pingaura.ai/docs/mcp/mcp-server
- **Also listed in:** the official MCP Registry (`ai.pingaura/pingaura`), Claude, ChatGPT and Microsoft 365 Copilot directories.

## Install

**Claude Code**

```bash
claude mcp add --transport http pingaura https://www.pingaura.ai/api/mcp
```

**Cursor, VS Code, Cline and other `mcp.json` clients**

```json
{
  "mcpServers": {
    "pingaura": {
      "url": "https://www.pingaura.ai/api/mcp"
    }
  }
}
```

**Gemini CLI**

```bash
gemini extensions install https://github.com/pingaura-ai/pingaura-mcp
```

**Claude.ai / ChatGPT:** add the URL under Settings, Connectors.

## What you can do

- Visibility: AI visibility score, per-engine summaries, run comparisons
- Competitors: list, add and update the competitors you track
- Prompts: browse prompt scores, organise prompts into topics and filters
- Site health: audits, issues and sitemap sync
- Content: list, draft, update and publish articles

Write tools are marked so your assistant asks before changing anything.

## Support

support@pingaura.ai · Security: https://www.pingaura.ai/security
