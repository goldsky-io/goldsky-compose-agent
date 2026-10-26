# Security Policy

## Reporting a vulnerability

Report security issues in this plugin to **security@goldsky.com**. Do not open a public GitHub issue for a vulnerability.

Include what you found, how to reproduce it, and the plugin version (`.claude-plugin/plugin.json` → `version`). We aim to acknowledge within two business days.

## Scope

In scope: the skill instructions and plugin manifests in this repository. Of particular interest:

- **Prompt injection** in skill text that could steer an agent into unintended transactions.
- **Credential exposure**: any path by which a skill could cause a Goldsky API token or a wallet private key to be printed, logged, or sent into a chat transcript.

Out of scope here: the Goldsky platform, CLI, and APIs. Report those through <https://goldsky.com/security> or the same address.
