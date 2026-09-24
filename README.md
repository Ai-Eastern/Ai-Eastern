# Eastern

**I build small, verifiable systems around AI agents.**

My work focuses on grounded retrieval, tool integration, backend reliability, and developer workflows. I prefer explicit evidence over broad claims: implementation, local verification, upstream acceptance, and real production use are different milestones.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat&logo=nodedotjs&logoColor=white)
[![pandas PR #69015 merged](https://img.shields.io/badge/pandas-PR%20%2369015%20merged-2EA44F?style=flat&logo=pandas&logoColor=white&labelColor=150458)](https://github.com/pandas-dev/pandas/pull/69015)
[![pnpm PR #15152 merged](https://img.shields.io/badge/pnpm-PR%20%2315152%20merged-2EA44F?style=flat&logo=pnpm&logoColor=white&labelColor=F69220)](https://github.com/pnpm/pnpm/pull/15152)
[![ECC PR #3184 merged](assets/ecc-pr-3184-merged.svg)](https://github.com/affaan-m/ECC/pull/3184)
[![Open source: 7 merged upstream PRs](https://img.shields.io/badge/Open%20Source-7%20merged%20upstream%20PRs-2EA44F?style=flat&logo=github&logoColor=white)](#verified-open-source-work)

## What I build

- **Reliable agent workflows** — tool boundaries, human review, failure handling, and observable execution.
- **Grounded retrieval systems** — evidence-carrying answers, access-aware retrieval, and explicit evaluation boundaries.
- **Developer tooling** — focused changes with regression coverage and reviewable behavior.

## Verified open-source work

| Project | Contribution |
| --- | --- |
| [pandas](https://github.com/pandas-dev/pandas) | Preserved assertion diagnostics for nested sequence length mismatches so unhashable nested values no longer mask the intended `AssertionError`, with regression coverage across low-level assertions, Series, and DataFrame comparisons. [Merged PR #69015](https://github.com/pandas-dev/pandas/pull/69015) |
| [pnpm](https://github.com/pnpm/pnpm) | Fixed configured `.js` pnpmfile loading so the module format follows the nearest `package.json`, with CommonJS and ES module regression coverage. [Merged PR #15152](https://github.com/pnpm/pnpm/pull/15152) |
| [Docling](https://github.com/docling-project/docling) | Fixed the AsciiDoc backend so incomplete tables no longer emit an extra empty table, and unified end-of-document table flushing to preserve captions, with regression coverage. [Merged PR #4300](https://github.com/docling-project/docling/pull/4300) |
| [OpenMAIC](https://github.com/THU-MAIC/OpenMAIC) | Added request-ID correlation and server-side 5xx logging for persistence routes. [Merged PR #1601](https://github.com/THU-MAIC/OpenMAIC/pull/1601) |
| [ECC](https://github.com/affaan-m/ECC) | Fixed project-scoped Claude hooks in ESM projects by adding managed CommonJS boundaries while preserving user-owned package manifests, with install, reinstall, and uninstall regression coverage. [Merged PR #3184](https://github.com/affaan-m/ECC/pull/3184) |
| [Archify](https://github.com/tt-a1i/archify) | Fixed resolved quality-profile reporting in exported SVG metadata. [Merged PR #437](https://github.com/tt-a1i/archify/pull/437) |
| [Laya](https://github.com/NandhaKishorM/laya) | Fixed `Router.preload([])` unexpectedly loading all three checkpoints when the selection is empty, with a regression check that no model loads occur. [Merged PR #240](https://github.com/NandhaKishorM/laya/pull/240) |

## Selected projects

### [reuse-before-build](https://github.com/Ai-Eastern/reuse-before-build)

A dependency-free Agent Skill that helps coding agents inspect existing implementations, tests, and prior decisions before choosing what to **Take, Borrow, or Build**. The repository includes dated evaluation records, diffs, test replays, compatibility notes, and documented failures rather than a success-rate claim.

### [codex-agent-workbench](https://github.com/Ai-Eastern/codex-agent-workbench)

Codex-native orchestration for multi-project development, scoped context, and traceable handoffs. Prototype.

## Engineering principles

- Evidence before claims.
- Reuse before building.
- Small changes with explicit verification.
- Human review at consequential boundaries.
- A passing demo is not production evidence.
