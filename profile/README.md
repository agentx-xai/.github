<p align="center">
  <img src="https://raw.githubusercontent.com/agentx-xai/.github/main/profile/agentx-mark.svg" alt="AgentX" width="112">
</p>

<h1 align="center">AgentX</h1>

<p align="center">Declarative, reproducible environments for AI agents.</p>

<p align="center">
  <a href="https://agentx-xai.github.io/agentx-website/">Website</a> ·
  <a href="https://github.com/agentx-xai/agentx-cli">CLI</a> ·
  <a href="https://github.com/agentx-xai/agentx-server">Registry Server</a> ·
  <a href="https://github.com/agentx-xai/agentx-website/tree/main/console">Web Console</a>
</p>

AgentX keeps AI agent environments reproducible across machines. Declare Skills, rules, MCP servers, policies, and versions once; compile them into each supported agent's native configuration; then inspect drift and reconcile devices from a local CLI or a team Registry.

### Repositories

| Repository | Responsibility |
| --- | --- |
| [`agentx-cli`](https://github.com/agentx-xai/agentx-cli) | Rust CLI for manifests, lockfiles, installation plans, eight agent adapters, Registry Device Flow, sync, drift, and rollback. |
| [`agentx-server`](https://github.com/agentx-xai/agentx-server) | Go Registry/API with PostgreSQL and S3 support, OIDC/JWKS authentication, workspace RBAC, audit, invitations, lifecycle controls, and production deployment templates. |
| [`agentx-website`](https://github.com/agentx-xai/agentx-website) | Vue product website and authenticated Registry Web Console with OIDC PKCE and workspace operations. |

The three repositories are independently versioned and released. For full-stack staging, clone them into the same parent directory:

```bash
git clone https://github.com/agentx-xai/agentx-cli.git
git clone https://github.com/agentx-xai/agentx-server.git
git clone https://github.com/agentx-xai/agentx-website.git
```

### Start with the CLI

```bash
cd agentx-cli
cargo run -- init
cargo run -- lock
cargo run -- install --yes --frozen
```

Read the [CLI guide](https://github.com/agentx-xai/agentx-cli#readme), [Server operations guide](https://github.com/agentx-xai/agentx-server/blob/main/docs/OPERATIONS.md), and [Website/Console guide](https://github.com/agentx-xai/agentx-website#readme). The public product site is at [agentx-xai.github.io/agentx-website](https://agentx-xai.github.io/agentx-website/).

### Project status

The source repositories are public and their `main` branches run component-specific CI. Hosted production deployments require operator-supplied identity, storage, secrets, observability, support, and legal configuration; the Server repository includes preflight checks and deployment guidance for those inputs.

### Contributing

Bug reports and feature proposals are welcome through GitHub Issues. Before opening a pull request, read the organization [contribution guide](https://github.com/agentx-xai/.github/blob/main/CONTRIBUTING.md). Security reports should follow the [security policy](https://github.com/agentx-xai/.github/blob/main/SECURITY.md).

AgentX is released under the [MIT License](https://github.com/agentx-xai/.github/blob/main/LICENSE).
