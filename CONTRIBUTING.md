# Contributing to AgentX

Thank you for helping improve AgentX. Small documentation fixes and focused bug reports are welcome, as are larger changes that include tests and a clear product rationale.

## Before opening a pull request

1. Search existing Issues and pull requests.
2. For a behavior change, open an Issue first so the intended contract is clear.
3. Keep a pull request focused on one change and explain the user-visible result.
4. Do not commit credentials, sessions, caches, generated build output, or personal machine paths.

## Local checks

Run the checks for the repository you changed:

```bash
# agentx-cli
cargo fmt --manifest-path Cargo.toml -- --check
cargo test --manifest-path Cargo.toml
cargo build --manifest-path Cargo.toml --release

# agentx-server
go test ./...
go vet ./...
go build ./cmd/app
go build ./cmd/migrate

# agentx-website
npm ci
npm run build
```

## Commit and review

Use a short imperative commit subject, such as `fix: reject invalid artifact paths`. Pull requests should describe the problem, the implementation, verification performed, and any migration or compatibility impact. Reviewers may request tests, documentation, or a change to the public API contract before merge.

## Community standard

Participation is governed by the [Code of Conduct](CODE_OF_CONDUCT.md). Please report security issues privately using the [Security Policy](SECURITY.md) instead of opening a public Issue.
