# Contributing to Second Dawn

Thanks for helping! Second Dawn apps are MIT-licensed, free, offline and private. This guide applies to every repository in the organization.

## Setup

- Node 20+ and [pnpm](https://pnpm.io)
- Rust (stable) via [rustup](https://rustup.rs)
- Clone `dawn-core` and the app (e.g. `owll`) **side by side** in one folder; apps use `../dawn-core`.

```bash
pnpm install
pnpm lint
pnpm typecheck
cargo check
```

## Guidelines

- Keep changes small and focused; one topic per pull request.
- Run `pnpm format` before committing.
- Never commit model weights. Models are described in `dawn-core/models/catalog.json` and downloaded at runtime.
- Shared code belongs in `dawn-core`; app-specific code stays in the app.
- By contributing, you agree your work is licensed under the MIT license.
