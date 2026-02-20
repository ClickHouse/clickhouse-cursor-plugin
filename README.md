# ClickHouse Cursor plugin

Cursor plugin that adds **ClickHouse skills** and **MCP** support (starter-advanced style with minimal folders).

## What’s included

- **Skills** – ClickHouse best-practices guidance (schema, queries, ingestion) from [ClickHouse/agent-skills](https://github.com/ClickHouse/agent-skills).
- **MCP** – ClickHouse MCP server config in `mcp.json` (URL: wip); customize or remove as needed.

## How to use

After the plugin is installed, its skills and MCP are available to Cursor’s agent.

- **ClickHouse best-practices** – When you’re writing or editing ClickHouse SQL, schemas, or ingestion logic, the agent can use this skill automatically. You can also ask explicitly, e.g. *“Check this query against ClickHouse best practices.”*
- **MCP** – The plugin’s `mcp.json` configures the ClickHouse MCP server (HTTP endpoint). Once the plugin is installed, Cursor can use it to run queries, inspect schemas, or otherwise interact with ClickHouse when the agent needs it. Configure any required credentials or endpoints in Cursor’s MCP settings if your setup needs them.

## Install

- **From Cursor Marketplace** (when published): install the “ClickHouse Cursor” plugin from the marketplace.
- **From this repo**: clone or download the repo and add it as a local plugin in Cursor (see Cursor docs for loading a plugin from a folder).

If you clone the repo, use submodules so the ClickHouse best-practices skill is available:

```bash
git clone --recurse-submodules https://github.com/ClickHouse/clickhouse-cursor-plugin.git
```

## License

Apache 2.0. See [LICENSE](LICENSE).
