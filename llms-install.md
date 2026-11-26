# Install maps-agent (instructions for agents)

Remote MCP server, Streamable HTTP, no sign-in, no API key, nothing to build or download.

Server URL: `https://maps-agent.com/mcp`

## Cline

```sh
cline mcp install maps-agent https://maps-agent.com/mcp --transport http --yes
```

Or add this to `cline_mcp_settings.json`, keeping the servers already listed there:

```json
{
  "mcpServers": {
    "maps-agent": {
      "transport": {
        "type": "streamableHttp",
        "url": "https://maps-agent.com/mcp"
      }
    }
  }
}
```

## Check

The client lists the tools `search` and `fetch`.
