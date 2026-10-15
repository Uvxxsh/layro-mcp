# Layro MCP

Layro's remote MCP server gives Cursor access to 89 production React + Tailwind components (53 free).
Your agent can search the library, read each component's props and usage, and install the tested component with pinned packages.

## Install

Add to `~/.cursor/mcp.json` (or `.cursor/mcp.json` in a project):

```json
{
  "mcpServers": {
    "layro": { "url": "https://layropro.com/api/mcp" }
  }
}
```

Free components work with no account. For Pro components, add your token from https://layropro.com/account:

```json
{
  "mcpServers": {
    "layro": {
      "url": "https://layropro.com/api/mcp",
      "headers": { "Authorization": "Bearer YOUR_LAYRO_TOKEN" }
    }
  }
}
```

Docs: https://layropro.com/mcp
