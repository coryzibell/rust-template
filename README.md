# Rust Template

A Rust project template with Matrix-themed CI workflows.

## Usage

1. Click "Use this template" on GitHub
2. Update `Cargo.toml` with your project name, description, and author
3. Start coding

## CI Workflows

| Workflow | Trigger | Purpose |
|----------|---------|---------|
| `wake up.` | PR or push to main | Orchestrates everything - gates drafts, runs tests, bumps version |
| `the matrix has you.` | Called by wake up | Format, clippy, tests across platforms |
| `follow the white rabbit.` | Tag push (v*) | Builds release binaries for all targets |
| `knock, knock.` | Release published | Publishes to crates.io |

## Why Matrix?

[Why the Matrix theming?](https://github.com/coryzibell/dotmatrix/blob/main/zion/insight/matrix-philosophy.md)

## Secrets

Set these in your repo settings:

- `PAT_TOKEN` - Personal access token for tag creation
- `CARGO_REGISTRY_TOKEN` - For crates.io publishing (optional)

## License

MIT OR Apache-2.0
