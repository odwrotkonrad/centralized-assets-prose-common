# Purpose

## What It Is

Semver-tagged home of the prose written for agents: every repo's `AGENTS.md.ontoRepo.tpl` under `prose/repos/<repo-path>/`, and the AI toolchain payload (`ai-agents-docs`, claude rules, skills, output styles, LLM templates) under `prose/repos/ai-harness/ai-tools-configs/ai/`. Consumers render it through `centralized/assets/generic`'s `generic/filesUntracked` profile, `ai-tools-configs` loads the payload onto the host.

## Why It Exists

Agent prose changed on the README cadence in `cross-repo/prose/assets`. Apart, an agent rule edit releases nothing a human reads.

## Goals

- `prose/repos/<repo-path>/` mirrors the GitLab group tree.
- Every merge to main mints a semver tag, each release fans out through `cross-repo/automation`.
- Purpose docs live in `prose/common`, referenced, never copied.
