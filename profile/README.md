# TarnFS

Open-source, self-hosted drive: a Rust file system with its own content-addressed storage engine, exposed over S3, REST, MCP and WebDAV. It comes with a Svelte web app and a native Mac client, and runs on anything from a Raspberry Pi to a scaled-out cluster. AI agents work on files through scoped, auditable permissions.

## Repositories

| Repo | What |
| --- | --- |
| [TarnFS/tarnfs](https://github.com/TarnFS/tarnfs) | this repo: spec, shared rules, tooling |
| [TarnFS/server](https://github.com/TarnFS/server) | Rust workspace, CLI, Docker image |
| [TarnFS/web](https://github.com/TarnFS/web) | SvelteKit web app |
| [TarnFS/mac](https://github.com/TarnFS/mac) | native Mac app |

The spec lives in [`docs/spec.md`](docs/spec.md). Contributor and agent rules are in [`AGENTS.md`](AGENTS.md).

## Getting started

Clone this repo, then run the bootstrap script. It enables the commit hooks and clones the other repos next to it.

```sh
git clone https://github.com/TarnFS/tarnfs.git
cd tarnfs
scripts/bootstrap.sh
```

## License

AGPL-3.0-only. See [`LICENSE`](LICENSE).
