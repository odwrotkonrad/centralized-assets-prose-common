# Purpose

## What It Is

Semver-tagged home of the prose both audiences share: every repo's `purpose.md` under `prose/repos/<repo-path>/`, the canonical MIT `license/LICENSE`, and the repo data templates under `templates/data/` (`makefile.agents.md`, `repo-structure.md`).

## Why It Exists

`purpose.md` feeds both `README.md` and `AGENTS.md`: it belongs to neither audience repo. The license is copied verbatim into every repo and must have one source.

## Goals

- `prose/repos/<repo-path>/` mirrors the GitLab group tree.
- Every merge to main mints a semver tag, each release fans out through `cross-repo/automation`.
- `LICENSE` copied byte for byte (`makeCopies`), never rendered.
