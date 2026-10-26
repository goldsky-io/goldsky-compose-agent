# Privacy Policy — Goldsky Compose Agent plugin

This notice describes the data flows of the **Goldsky Compose Agent plugin** in this repository. Use of Goldsky services is covered by the [Goldsky Privacy Policy](https://goldsky.com/privacy).

## Plugin components

The plugin contains Markdown skills and configuration for the remote Goldsky documentation MCP server. It contains no analytics, telemetry, or crash reporting.

## Data flows

| Flow | What happens |
| --- | --- |
| Skill instructions | Your agent may read and write local project files and run the Goldsky CLI as described by a skill. Compose CLI operations send app source, manifests, project identifiers, and secret values to Goldsky services. Compose apps send transactions to blockchain networks and may contact configured third-party providers. |
| Docs MCP server | Your agent host sends search queries to `https://docs.goldsky.com/mcp`. |

## Contact

<support@goldsky.com>
