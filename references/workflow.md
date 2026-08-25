# Workflow reference

## Node contract

Every node produces one inspectable deliverable. Mark it `proposed`, `confirmed`, `rejected`, or `superseded`; do not silently overwrite a confirmed decision.

| Node | Minimum inputs | Deliverable for confirmation | Record location |
|---|---|---|---|
| Task intake | goal, materials, constraints | scope card and next node | `工作台索引/当前状态.md` |
| Literature research | question, search set, sources | evidence map and gap card | `1_调研/` |
| Research definition | confirmed gap, target setting | problem-definition card | `2_研究文档/` |
| Model and derivation | assumptions, notation, sources | model/derivation verification package | `2_研究文档/` |
| Simulation | confirmed model, code/data availability | experiment matrix and acceptance criteria | `4_仿真/` |
| Results | result files, configurations | result explanation and claim map | `4_仿真/` |
| Manuscript | accepted technical inputs, target venue | structure or revision package | `3_论文撰写/` |
| Draft revision | annotated draft, clean draft, style profile | comment disposition and revised package | `5_初稿修改/` |
| Submission | frozen manuscript, journal requirements | submission readiness package | `6_投稿/` |

## Transition rules

- Require confirmation before moving forward.
- When a model, parameter, or claim changes, identify every downstream artifact that needs revalidation.
- Keep draft-writing activity from creating new scientific conclusions; return to research or simulation when evidence is missing.
- Use the user’s requested granularity. The default is a complete deliverable, not one confirmation per sentence.

## Standard entries

| Entry | First response |
|---|---|
| `建立项目` | propose the six folders, index files, scope and profile setup |
| `打开项目` | summarize state, confirmed decisions, blockers, and next deliverable |
| `开始调研` | propose a search/selection strategy and evidence-card schema |
| `定义问题` | separate known facts, constraints, candidate problem statements, and validation needs |
| `检查模型与推导` | map symbols, assumptions, equations, code correspondence, and proof obligations |
| `设计仿真` | propose baselines, factors, metrics, controls, and acceptance criteria |
| `解释仿真结果` | link each claim to an artifact; distinguish observation from interpretation |
| `撰写论文` | propose section purpose, logic and evidence prerequisites before prose |
| `处理导师批注` | extract comments, cluster issues, propose priority and traceable responses |
| `学术审阅` | invoke the reviewer gate and create a disposition plan |
| `投稿前检查` | audit frozen files, venue requirements, consistency and reply materials |
