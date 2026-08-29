# Purpose

## What It Is

Generic repo assets every workspace repo consumes at `CENTRALIZED_ASSETS_GENERIC_REF`: the shared makefile (`generic-*` targets), the GitLab CI templates (`generic:*` jobs, included by ref, never rendered), the lefthook config, the toolchain dependency spec and the che specs for every conventional generated file. `consumer-repo-config/che.export.yml` exports `setup`, which renders `shared/generic/` and `lefthook.yml` into the consumer, and `deps`.

## Why It Exists

Every repo carried a copied Makefile, a copied `lefthook.yml`, copied CI jobs and a hand-written `env.tpl`. One repo authors each once, consumers keep two targets: `che-install` and `generic-setup`.

## Goals

- One home for the generic repo payload: makefile, CI templates, lefthook, deps, che specs.
- Consumers own nothing generic: `generic-setup` renders it all, gitignored.
- `.env` regeneration selective: missing keys, upstream pins, shell values or everything, never a needless `glab` call.
- Every merge to main mints a semver tag, each release fans out to consumers through `cross-repo/automation`.
