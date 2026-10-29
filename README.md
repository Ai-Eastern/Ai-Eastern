<h1 align="center">Eastern</h1>

<p align="center">
  <b>I build small, verifiable systems around AI agents.</b>
</p>

<p align="center">
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat&amp;logo=python&amp;logoColor=white">
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&amp;logo=typescript&amp;logoColor=white">
  <img alt="Node.js" src="https://img.shields.io/badge/Node.js-5FA04E?style=flat&amp;logo=nodedotjs&amp;logoColor=white">
</p>

<p align="center">
  <a href="https://github.com/pandas-dev/pandas/pull/69015"><img alt="pandas PR #69015 merged" src="https://img.shields.io/badge/pandas-PR%20%2369015%20merged-2EA44F?style=flat&amp;logo=pandas&amp;logoColor=white&amp;labelColor=150458"></a>
  <a href="https://github.com/pnpm/pnpm/pull/15152"><img alt="pnpm PR #15152 merged" src="https://img.shields.io/badge/pnpm-PR%20%2315152%20merged-2EA44F?style=flat&amp;logo=pnpm&amp;logoColor=white&amp;labelColor=F69220"></a>
  <a href="https://github.com/NVIDIA/SkillSpector/pull/641"><img alt="NVIDIA SkillSpector PR #641 merged" src="https://img.shields.io/badge/NVIDIA%20SkillSpector-PR%20%23641%20merged-2EA44F?style=flat&amp;logo=nvidia&amp;logoColor=white&amp;labelColor=76B900"></a>
  <a href="https://github.com/affaan-m/ECC/pull/3184"><img alt="ECC PR #3184 merged" src="https://raw.githubusercontent.com/Ai-Eastern/Ai-Eastern/main/assets/ecc-pr-3184-merged.svg"></a>
  <a href="#open-source-contributions"><img alt="Open source: 11 merged upstream PRs" src="https://img.shields.io/badge/Open%20Source-11%20merged%20upstream%20PRs-2EA44F?style=flat&amp;logo=github&amp;logoColor=white"></a>
  <a href="https://github.com/Ai-Eastern/reuse-before-build"><img alt="reuse-before-build stars" src="https://img.shields.io/github/stars/Ai-Eastern/reuse-before-build?style=flat&amp;logo=github&amp;logoColor=white&amp;label=reuse-before-build&amp;color=0969DA"></a>
</p>

<br>

权限感知的检索、工具边界、人工复核、可恢复的执行与评测回归。公开仓库包括个人复现、自研工具和开源贡献,每一项都标明证据边界。

> I prefer explicit evidence over broad claims: implementation, local verification, upstream acceptance, and real production use are different milestones.

**Stack** &nbsp;LangGraph · FastAPI · Pydantic · Chroma · MCP / A2A · OpenTelemetry

## What I build

- **Reliable agent workflows** — tool boundaries, human review, failure handling, and observable execution.
- **Grounded retrieval systems** — evidence-carrying answers, access-aware retrieval, and explicit evaluation boundaries.
- **Developer tooling** — focused changes with regression coverage and reviewable behavior.

## Selected projects

**[codex-agent-workbench](https://github.com/Ai-Eastern/codex-agent-workbench)** — a Codex-native framework for multi-agent coding and multi-project orchestration.<br>
Direct execution · native subagents · scoped project context · traceable handoffs and recovery.<br>
<sub>Runnable prototype with bounded live validation. Full three-project acceptance remains pending.</sub>

**[reuse-before-build](https://github.com/Ai-Eastern/reuse-before-build)** — a dependency-free Agent Skill that helps coding agents inspect existing implementations, tests, and prior decisions before choosing what to **Take, Borrow, or Build**.<br>
Dated evaluation records, diffs, test replays, compatibility notes, and documented failures — rather than a success-rate claim.

## Open-source contributions

Merged upstream pull requests across 11 projects. Highlights:

| Project | Contribution | PR |
| :-- | :-- | :-: |
| [pandas](https://github.com/pandas-dev/pandas) | Preserved the intended `AssertionError` for nested sequence length mismatches, so unhashable nested values no longer mask it. Regression tests across low-level assertions, Series, and DataFrame. | [#69015](https://github.com/pandas-dev/pandas/pull/69015) |
| [pnpm](https://github.com/pnpm/pnpm) | Fixed configured `.js` pnpmfile loading so the module format follows the nearest `package.json`. CommonJS and ES module regression tests. | [#15152](https://github.com/pnpm/pnpm/pull/15152) |
| [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) | Exposed MCP rug-pull and least-privilege match details in JSON reports; redacted URL credentials in `pattern` across report formats. Regression tests. | [#641](https://github.com/NVIDIA/SkillSpector/pull/641) |
| [PR-Agent](https://github.com/The-PR-Agent/pr-agent) | Preserved request-specific `extra_instructions` during code-suggestion reflection, so scoring sees the context used in generation. Passed as untrusted user-prompt data; tests for context transport, empty-context compatibility, and token-budget enforcement. | [#3987](https://github.com/The-PR-Agent/pr-agent/pull/3987) |
| [Docling](https://github.com/docling-project/docling) | Fixed the AsciiDoc backend emitting an extra empty table for incomplete tables; unified end-of-document table flushing to preserve captions. Regression tests. | [#4300](https://github.com/docling-project/docling/pull/4300) |

<details>
<summary>Other merged PRs (6)</summary>

<br>

- [Headroom #3778](https://github.com/headroomlabs-ai/headroom/pull/3778) — keep unmarked HTML tool output intact when no retrieval marker exists.
- [Kornia #5300](https://github.com/kornia/kornia/pull/5300) — keep inverse mask sampling overrides local, so state does not leak across images.
- [OpenMAIC #1601](https://github.com/THU-MAIC/OpenMAIC/pull/1601) — request-ID correlation and server-side 5xx logging for persistence routes.
- [ECC #3184](https://github.com/affaan-m/ECC/pull/3184) — fix project-scoped Claude hooks in ESM projects via managed CommonJS boundaries.
- [Archify #437](https://github.com/tt-a1i/archify/pull/437) — report the resolved quality profile in exported SVG metadata.
- [Laya #240](https://github.com/NandhaKishorM/laya/pull/240) — keep an empty `Router.preload([])` selection from loading all checkpoints.

</details>

## Engineering principles

- Evidence before claims.
- Reuse before building.
- Small changes with explicit verification.
- Human review at consequential boundaries.
- A passing demo is not production evidence.
