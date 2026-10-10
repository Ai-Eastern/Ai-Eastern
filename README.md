<h1 align="center">Eastern</h1>

<p align="center">
  <b>Agent / RAG 工程 · 面向企业内部与政企场景</b><br>
  <sub>Agent / RAG engineering for on-prem enterprise and government scenarios</sub>
</p>

<p align="center">
  <a href="#open-source-contributions"><img alt="11 merged upstream PRs" src="https://img.shields.io/badge/merged%20upstream%20PRs-11-2EA44F?style=flat-square"></a>
  <a href="https://github.com/pandas-dev/pandas/pull/69015"><img alt="pandas PR #69015 merged" src="https://img.shields.io/badge/pandas-%2369015%20merged-2EA44F?style=flat-square"></a>
  <a href="https://github.com/pnpm/pnpm/pull/15152"><img alt="pnpm PR #15152 merged" src="https://img.shields.io/badge/pnpm-%2315152%20merged-2EA44F?style=flat-square"></a>
  <a href="https://github.com/NVIDIA/SkillSpector/pull/641"><img alt="NVIDIA SkillSpector PR #641 merged" src="https://img.shields.io/badge/NVIDIA%20SkillSpector-%23641%20merged-2EA44F?style=flat-square"></a>
  <a href="https://github.com/Ai-Eastern/reuse-before-build"><img alt="reuse-before-build stars" src="https://img.shields.io/github/stars/Ai-Eastern/reuse-before-build?style=flat-square&amp;label=reuse-before-build%20stars&amp;color=0969DA"></a>
</p>

<br>

权限感知的检索、工具边界、人工复核、可恢复的执行与评测回归。公开仓库包括个人复现、自研工具和开源贡献,每一项都标明证据边界。

> I prefer explicit evidence over broad claims: implementation, local verification, upstream acceptance, and real production use are different milestones.

**Stack** &nbsp;LangGraph · FastAPI · Pydantic · Chroma · MCP / A2A · OpenTelemetry · Python · TypeScript

## What I build

- **Reliable agent workflows** — tool boundaries, human review, failure handling, and observable execution.
- **Grounded retrieval systems** — evidence-carrying answers, access-aware retrieval, and explicit evaluation boundaries.
- **Developer tooling** — focused changes with regression coverage and reviewable behavior.

## Selected projects

**[enterprise-service-desk-agent-history](https://github.com/Ai-Eastern/enterprise-service-desk-agent-history)** — an internal service-desk agent evolved in four stages: RAG → MCP read-only tool → A2A local validation → multi-agent collaboration.<br>
Permission-aware retrieval · human-approval resume (LangGraph) · idempotent ticket creation · tests and version tags.<br>
<sub>Personal reproduction with fictional data. Scope and limits are documented in the repo.</sub>

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
