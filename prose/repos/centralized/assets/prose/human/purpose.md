# Purpose

## What It Is

Semver-tagged home of the prose written for humans: every repo's `README.md.ontoRepo.tpl` and its supplemental docs under `prose/repos/<repo-path>/`. Consumers render it through `centralized/assets/generic`'s `generic/filesTracked` profile.

## Why It Exists

Human and agent prose changed on one cadence in `cross-repo/prose/assets`: a README edit re-released every agent rule. Apart, each audience releases on its own.

## Goals

- `prose/repos/<repo-path>/` mirrors the GitLab group tree.
- Every merge to main mints a semver tag, each release fans out through `cross-repo/automation`.
- Purpose docs and the license live in `prose/common`, referenced, never copied.
