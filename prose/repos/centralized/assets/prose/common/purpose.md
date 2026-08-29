# Purpose

## What It Is

Semver-tagged home of the prose components both audiences reuse: every repo's `purpose.md` under `prose/repos/<repo-path>/` and the repo data templates under `templates/data/` (`makefile.agents.md`, `repo-structure.md`).

## Why It Exists

`purpose.md` feeds both `README.md` and `AGENTS.md`: it belongs to neither audience repo.

## Goals

- `prose/repos/<repo-path>/` mirrors the GitLab group tree.
- Every merge to main mints a semver tag, each release fans out through `cross-repo/automation`.
