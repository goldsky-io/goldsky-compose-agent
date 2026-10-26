# Goldsky Compose Agent

Agent skills for [Goldsky Compose](https://docs.goldsky.com/compose/introduction): TypeScript apps that run on cron, HTTP, or onchain triggers and write back onchain from managed smart wallets.

These skills send onchain transactions that can spend real funds and gas. They are kept apart from the [Goldsky Agent](https://github.com/goldsky-io/goldsky-agent) plugin, which reads, indexes, and streams onchain data and sends no transactions.

## Skills

| Skill | Use it to |
| --- | --- |
| `compose` | Build and deploy a Compose app (oracle, keeper, automation). Manifest, CLI, and API references and worked examples are in `skills/compose/references/` |
| `compose-doctor` | Diagnose a Compose app that crashloops, misses events, or fails tasks |
| `onchain-automation` | Plan a detect, decide, execute workflow across Turbo, Subgraphs, and Compose |

The skills hand off to `auth-setup`, `secrets`, `turbo-builder`, `subgraph-builder`, and `edge` from the Goldsky Agent plugin. Install both.

## Installation

**Claude Code**

```
/plugin marketplace add goldsky-io/goldsky-agent
/plugin marketplace add goldsky-io/goldsky-compose-agent
/plugin install goldsky-compose@goldsky-compose-agent
```

`goldsky-compose` declares `goldsky@goldsky-agent` as a dependency, so Claude Code installs it too.

**Any agent**

```bash
npx skills add goldsky-io/goldsky-agent
npx skills add goldsky-io/goldsky-compose-agent
```

**Cursor**

Clone both repositories and add both paths to `plugins.local` in your Cursor settings.

## Review what the agent does

Compose skills deploy contracts and send transactions. Every skill asks for your confirmation before a `deploy`, `deployContract`, `writeContract`, or `secret set`. Read the command before you approve it.

## Policies

- [Terms of Use](./TERMS.md)
- [Privacy Policy](./PRIVACY.md)
- [Security Policy](./SECURITY.md) — report issues to security@goldsky.com
- [MIT License](./LICENSE)
