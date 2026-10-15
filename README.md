# Layro MCP

Layro is a library of 112 production React UI components written in TypeScript and styled with Tailwind CSS (62 free).
Its remote MCP server gives Cursor, Claude Code, VS Code, Windsurf, Codex and other MCP clients access to the whole library.
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

Search and component details work with no account. To install components, add the CLI token from https://layropro.com/account. A free account's token unlocks the 62 free components; lifetime access unlocks Pro:

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
