# Technical integrity reference

## Literature and gap claims

Create an evidence card before writing a gap claim. It must state the source, exact supported capability, assumptions, limitation, relevance, and confidence. Never infer nonexistence from a small search set.

## Model and derivation audit

Check, in order:

1. system entities, links, coordinate frames, time convention, channel/noise assumptions, and optimization objective;
2. every symbol’s meaning, set/domain, dimension, units, index range, and first definition;
3. each equation’s algebra, conjugation, transpose, norm, expectation, feasibility, and limiting cases;
4. consistency among narrative, equations, algorithms, code, and numerical configuration;
5. whether a proof/approximation clearly states its conditions and error/relaxation implications.

Report confirmed issues separately from hypotheses needing source code, data, or author clarification.

## Simulation audit

Before running or interpreting simulations, define scenario, fixed controls, variable factors, baselines, metrics, repetitions/randomness, expected failure modes, and acceptance criteria. Preserve parameter files and result provenance. Do not turn a plot pattern into a universal technical claim.

## Claim mapping

For every manuscript claim, maintain a link to one or more sources, equations, proofs, code revisions, or figures. Mark unsupported claims as blockers rather than polishing their language.
