<p align="center">
  <img src="https://raw.githubusercontent.com/agentx-xai/.github/main/profile/agentx-mark.svg" alt="AgentX" width="112">
</p>

<h1 align="center">AgentX</h1>

<p align="center">Declarative, reproducible environments for AI agents.</p>

<p align="center">
  <a href="https://agentx-xai.github.io/agentx-website/">Website</a> ·
  <a href="https://github.com/agentx-xai/agentx-cli">CLI</a> ·
  <a href="https://github.com/agentx-xai/agentx-server">Registry Server</a> ·
  <a href="https://github.com/agentx-xai/agentx-website">Console</a>
</p>

AgentX keeps an AI agent environment reproducible across machines. Declare Skills, rules, MCP servers, policies, and versions once; compile them into the native configuration of each supported agent; then inspect drift and reconcile devices from a local CLI or a team Registry.

### What is included

- **CLI**: local-first initialization, lockfiles, install plans, adapters, Registry sync, device reconciliation, drift and rollback.
- **Registry Server**: workspace-scoped manifests, immutable artifacts, policies, approvals, audit events, devices, and OpenAPI APIs.
- **Website and Console**: product documentation, architecture overview, and the web entry point for Registry operations.
- **Adapters**: Codex, Claude Code, Cursor, Windsurf, Gemini CLI, GitHub Copilot, Cline, and Grok Build.

### Start here

```bash
git clone https://github.com/agentx-xai/agentx-cli.git
cd agentx-cli
cargo run -- init
cargo run -- lock
cargo run -- install --yes --frozen
```

Read the [CLI README](https://github.com/agentx-xai/agentx-cli#readme) for local installation and the [product guide](https://github.com/agentx-xai/agentx-cli/blob/main/PRODUCT.md) for the full workflow. Server deployment is documented in the [Server README](https://github.com/agentx-xai/agentx-server#readme); the public product site is at [agentx-xai.github.io/agentx-website](https://agentx-xai.github.io/agentx-website/).

### Project status

The repositories are public and ship tagged releases. Every pull request runs formatting, tests, static checks, and production builds. A version tag such as `v0.1.2` produces a GitHub Release with the relevant binaries or website artifact.

### Contributing

Bug reports and feature proposals are welcome through GitHub Issues. Before opening a pull request, read the organization [contribution guide](https://github.com/agentx-xai/.github/blob/main/CONTRIBUTING.md). Security reports should follow the [security policy](https://github.com/agentx-xai/.github/blob/main/SECURITY.md).

AgentX is released under the [MIT License](https://github.com/agentx-xai/.github/blob/main/LICENSE).
