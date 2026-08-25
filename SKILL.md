---
name: ieee-research-skills
description: 本地可追溯的 IEEE 研究、论文撰写、导师批注修改和投稿工作流。用于通信、信号处理及相邻工程学科的文献调研、研究缺口验证、系统模型与公式推导检查、仿真设计和结果解释、IEEE 稿件撰写、LaTeX/排版核查、导师批注处理、学术审阅与投稿前检查；也用于建立或更新与工作台集成的本地研究项目索引。
---

# IEEE Research Skills

## Core contract

Operate a local, evidence-traceable project workflow. Treat the project directory and its `工作台索引/` files as the source of truth; never rely on chat history alone.

Support both natural-language requests and these standard entries: `建立项目`, `打开项目`, `开始调研`, `定义问题`, `检查模型与推导`, `设计仿真`, `解释仿真结果`, `撰写论文`, `处理导师批注`, `学术审阅`, and `投稿前检查`.

Use **deliverable-level confirmation**. For each node, state inputs, assumptions, proposed output, open risks, and the exact decision required. Do not promote a proposed gap, model, derivation, parameter, conclusion, manuscript revision, or style rule into the confirmed project state until the user explicitly confirms it.

Read the relevant reference before work:

| Request | Read first |
|---|---|
| Any node or handoff | `references/workflow.md` |
| Advisor-style writing or corpus update | `references/style-profile.md` |
| Literature, model, derivation, simulation, or results | `references/technical-integrity.md` |
| Manuscript, LaTeX, annotations, review, or submission | `references/ieee-typesetting-and-review.md` |
| Project setup or workbench integration | `references/workbench-contract.md` |

## Project lifecycle

Use the following top-level project layout; do not rename these user-facing folders:

```text
项目名称/
├─ 工作台索引/
├─ 1_调研/
├─ 2_研究文档/
├─ 3_论文撰写/
├─ 4_仿真/
├─ 5_初稿修改/
└─ 6_投稿/
```

Copy `assets/project_template/` when establishing a project. Preserve original PDFs, code, data, and manuscript versions. Record references rather than duplicating source materials. Keep research and writing projects separate unless the user explicitly connects them.

Follow this graph: `调研 → 研究文档 → 仿真 ↔ 论文撰写 → 初稿修改 → 投稿`. Permit a backward transition only by recording what changed and what must be rechecked.

## Non-negotiable research safeguards

- Distinguish quoted/source-supported facts, derivations, simulation observations, inferences, and open hypotheses.
- Do not invent literature coverage, research gaps, parameter values, baselines, experimental results, citations, or implementation status.
- For a claimed gap, identify the exact comparison set, supported capability, and remaining limitation before wording the claim.
- For every model or derivation change, audit definitions, dimensions, domains, indices, conjugation/transposition, feasibility, and consistency with code and narrative.
- For every simulation conclusion, retain the code version, configuration, random seed policy, baselines, metrics, result files, and a claim-to-figure link. Do not treat runtime as algorithmic complexity unless the user specifically asks for timing; use the requested theoretical operation-count convention when applicable.
- Surface uncertainty and blocking evidence gaps before suggesting implementation or prose.

## Writing and advisor-style profile

Use `吕老师风格档案.md` as the default profile when present. Match its observable, confirmed conventions—argument order, paragraph function, definition placement, equation presentation, transition density, and directness—without copying distinctive sentences or claiming to reproduce a person's exact voice.

When new advisor papers, annotations, or exemplar papers arrive, create a candidate-rule record with source location, frequency/contrast evidence, scope, and proposed wording. Update the default profile only after user confirmation.

For manuscript work, communicate in Chinese unless the user requests another language. Produce IEEE manuscript prose in the manuscript language. Preserve existing `\cite{}` and `\bibitem` labels. If a rewritten paragraph contains citations, provide the complete matching IEEE-style `\bibitem` entries requested by the user; never fabricate bibliographic metadata. Keep formulas in LaTeX and explain formula edits through definitions and validity, not stylistic claims alone.

## Review gates

Use the installed `academic-paper-reviewer` skill when available at these gates:

1. Before a revision round: diagnose the advisor comments, hidden technical risks, and priorities.
2. After each confirmed revision package: review logic, novelty claims, technical consistency, evidence, experiments, and presentation.
3. Before submission: perform a final consistency, reproducibility, citation, and journal-fit review.

Treat reviewer output as structured advice, not independent ground truth and not permission to modify the manuscript without confirmation. Store reviewer reports and disposition in `5_初稿修改/` or `6_投稿/`.

## Output protocol

At each active node, return in this order:

1. **Assumptions and material status** — missing inputs or ambiguities.
2. **Deliverable** — the requested analysis, plan, draft, check, or revision.
3. **Evidence and traceability** — sources, files, equations, figures, code, or version links.
4. **Decision required** — a concise confirmation/revision question.
5. **Self-check** — scope, unsupported claims, notation, citation, and next-state check.

For revision work, additionally show the affected location, original-versus-proposed change where the user asks for comparison, why it is necessary, whether it changes technical meaning, and the follow-on items that need rechecking.
