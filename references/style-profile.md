# IEEE journal style profile

## Purpose and boundary

This profile distils transferable engineering-writing conventions from the representative IEEE journal corpus in `ieee-journal-style-corpus.md`. It is a practical house style for communications-oriented research, with signal-processing and optimization methods where relevant; it is not an official IEEE rule set and not an imitation of any individual author.

## Confirmed baseline

### 1. Abstract: problem → gap → method → evidence → implication

- Name the technical setting and unresolved limitation before introducing the method.
- Describe the mechanism, not only a method name: identify the optimized variables, decomposition, estimator, proof device, or algorithmic step that closes the gap.
- Report the strongest supported result with its condition, metric, or baseline. Do not use unqualified claims such as “significant” or “superior.”
- End with the engineering implication; do not repeat the opening motivation.

### 2. Introduction: narrow the problem in explicit moves

Use the following paragraph functions unless the manuscript requires a justified variation:

1. establish the application and technical pressure;
2. organize the closest literature by capability rather than chronology;
3. identify a scoped limitation tied to cited work;
4. state the paper's response and why the chosen mechanism is suitable;
5. list contributions as method–evidence pairs;
6. give the paper organization only after the intellectual contribution is clear.

Each contribution item must point forward to a model, proposition, algorithm, experiment, or quantitative result in the manuscript.

### 3. System model: assumptions before algebra

- Introduce topology, entities, information flow, channel/data assumptions, and time-scale assumptions before the first derived expression.
- Define every symbol at first use, including dimension, domain, index range, and whether a quantity is known, estimated, optimized, or fixed.
- Separate physical assumptions from analytical simplifications. State where each simplification limits applicability.
- Use one term per concept and one symbol per quantity throughout text, equations, algorithms, and figures.

### 4. Problem formulation: expose the coupling

- Give the objective and constraints in a numbered formulation.
- Immediately explain each constraint in physical terms and identify the variables that create nonconvexity, discreteness, or coupling.
- State feasibility conditions and variable domains before presenting a solver.
- If the original problem is transformed, specify whether the new form is equivalent, a relaxation, a bound, or a local approximation.

### 5. Algorithm and theory: make the guarantee auditable

- Decompose the method into named subproblems or stages and explain why the sequence is valid.
- Place assumptions adjacent to the theorem, proposition, or convergence claim that depends on them.
- Distinguish monotonic improvement, convergence of iterates, convergence of objective values, and convergence to a stationary/global solution.
- Give an algorithm box or precise pseudocode with initialization, stopping rule, returned variables, and failure/feasibility handling.
- Report theoretical complexity in the stated operation-count convention; do not substitute runtime unless runtime is the measured quantity.

### 6. Numerical results: configure before interpreting

- State channel/data generation, dimensions, parameters, baselines, metrics, averaging procedure, and random-seed policy before the first result.
- Define every baseline fairly and identify which components are shared or disabled.
- Discuss each figure in the order: observed trend → mechanism → comparison → condition or limitation.
- Keep simulation observations distinct from theoretical conclusions and broader hypotheses.
- Use consistent precision and units. Avoid more significant digits than the experiment supports.

### 7. Sentence and paragraph style

- Prefer technically specific subjects and verbs over generic framing.
- Give each paragraph one dominant function and place the controlling claim early.
- Use transitions to express logic—cause, contrast, condition, or consequence—not merely sequence.
- Keep claims proportional to evidence. Prefer “under the considered setting” over universal wording when only simulations support the conclusion.
- Put citations next to the claim they support; avoid attaching one citation cluster to several distinct claims.

### 8. Figures, tables, equations, and references

- Captions should let a reader identify the scenario, varied quantity, metric, and key comparison without searching the main text.
- Tables compare like with like and disclose unavailable or inapplicable entries instead of forcing a value.
- Display equations that carry reasoning or are referenced later; keep simple definitions inline when readability improves.
- Treat notation, equation layout, baseline definitions, figure readability, and citation placement as technical integrity, not decoration.

## Evidence map

| Rule group | Primary corpus support |
|---|---|
| Framing, literature synthesis, research agenda | C01, C06, C07, C09, C11 |
| System model, optimization problem, alternating design | C02, C03, C04, C10, C12 |
| Tutorial sequencing and definition discipline | C05, C07 |
| Assumptions, convergence, algorithmic guarantees | C08, C10, C11, C12 |
| Simulation setup and claim-to-result linkage | C02, C03, C04, C10, C11, C12 |

Corpus IDs and DOI links are defined in `ieee-journal-style-corpus.md`. The map records provenance at rule-group level; it does not imply that every paper uses identical wording or structure.

## Candidate-rule method

For each candidate rule, record:

1. corpus ID, DOI, source version, and precise location;
2. observed pattern and a contrast/example count across at least two papers when possible;
3. scope: paragraph logic, wording, equation layout, figures, citations, or review preference;
4. safe generalized rule and known exceptions;
5. status: proposed, confirmed, rejected, or superseded.

## Update discipline

New corpus material may generate proposed rules only. Present the additions, cross-paper evidence, and any conflict with the confirmed baseline. Promote a rule to `IEEE期刊写作风格档案.md` only after explicit user confirmation.
