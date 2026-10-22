# Representative IEEE journal style corpus

## Scope

This corpus supports a communications-oriented writing profile with signal-processing and optimization methodology. It deliberately spans tutorial/survey, wireless-system analysis, system-and-optimization, and algorithm-theory papers so that neither one topic nor one author defines the house style. The repository stores bibliographic metadata, DOI links, and distilled observations only; it does not redistribute article full text.

The venue set is representative rather than exhaustive. Inclusion means that a paper is useful for studying technical organization and evidence presentation; it is not a ranking claim or an endorsement of every sentence-level choice.

## Corpus

| ID | Paper | Venue | Bibliographic record | Primary observation use |
|---|---|---|---|---|
| C01 | M. Di Renzo *et al.*, “Smart Radio Environments Empowered by Reconfigurable Intelligent Surfaces: How It Works, State of Research, and The Road Ahead” | IEEE JSAC, 2020, 38(11), 2450–2525 | [DOI: 10.1109/JSAC.2020.3007211](https://doi.org/10.1109/JSAC.2020.3007211) | Broad-field framing, taxonomy, research agenda, and explicit scope boundaries |
| C02 | Q. Wu and R. Zhang, “Intelligent Reflecting Surface Enhanced Wireless Network via Joint Active and Passive Beamforming” | IEEE TWC, 2019, 18(11), 5394–5409 | [DOI: 10.1109/TWC.2019.2936025](https://doi.org/10.1109/TWC.2019.2936025) | System model, coupled-variable formulation, alternating optimization, and baseline comparison |
| C03 | C. Huang *et al.*, “Reconfigurable Intelligent Surfaces for Energy Efficiency in Wireless Communication” | IEEE TWC, 2019, 18(8), 4157–4170 | [DOI: 10.1109/TWC.2019.2922609](https://doi.org/10.1109/TWC.2019.2922609) | Energy-efficiency objective, algorithm rationale, convergence/complexity discussion, and numerical validation |
| C04 | C. Pan *et al.*, “Multicell MIMO Communications Relying on Intelligent Reflecting Surfaces” | IEEE TWC, 2020, 19(8), 5218–5233 | [DOI: 10.1109/TWC.2020.2990766](https://doi.org/10.1109/TWC.2020.2990766) | Multi-entity notation, interference-aware formulation, subproblem decomposition, and simulation interpretation |
| C05 | Q. Wu *et al.*, “Intelligent Reflecting Surface-Aided Wireless Communications: A Tutorial” | IEEE TCOM, 2021, 69(5), 3313–3351 | [DOI: 10.1109/TCOMM.2021.3051897](https://doi.org/10.1109/TCOMM.2021.3051897) | Tutorial sequencing, definition discipline, model comparison, and bridge from principles to design |
| C06 | Y. Liu *et al.*, “Reconfigurable Intelligent Surfaces: Principles and Opportunities” | IEEE Communications Surveys & Tutorials, 2021, 23(3), 1546–1577 | [DOI: 10.1109/COMST.2021.3077737](https://doi.org/10.1109/COMST.2021.3077737) | Literature synthesis by capability, taxonomy, limitations, and future-opportunity wording |
| C07 | M. Di Renzo, F. H. Danufane, and S. Tretyakov, “Communication Models for Reconfigurable Intelligent Surfaces: From Surface Electromagnetics to Wireless Networks Optimization” | Proceedings of the IEEE, 2022, 110(9), 1164–1209 | [DOI: 10.1109/JPROC.2022.3195536](https://doi.org/10.1109/JPROC.2022.3195536) | Cross-domain definitions, assumption disclosure, model limitations, and stepwise technical exposition |
| C08 | G. Scutari, F. Facchinei, and L. Lampariello, “Parallel and Distributed Methods for Constrained Nonconvex Optimization—Part I: Theory” | IEEE TSP, 2017, 65(8), 1929–1944 | [DOI: 10.1109/TSP.2016.2637317](https://doi.org/10.1109/TSP.2016.2637317) | Assumption placement, theorem/guarantee boundaries, algorithm structure, and convergence language |
| C09 | T. L. Marzetta, “Noncooperative Cellular Wireless with Unlimited Numbers of Base Station Antennas” | IEEE TWC, 2010, 9(11), 3590–3600 | [DOI: 10.1109/TWC.2010.092810.091092](https://doi.org/10.1109/TWC.2010.092810.091092) | Asymptotic problem framing, model assumptions, analytical progression, and engineering interpretation |
| C10 | H. Q. Ngo *et al.*, “Cell-Free Massive MIMO Versus Small Cells” | IEEE TWC, 2017, 16(3), 1834–1850 | [DOI: 10.1109/TWC.2017.2655515](https://doi.org/10.1109/TWC.2017.2655515) | Architecture definition, theorem-to-algorithm flow, quantitative baseline comparison, and limitation disclosure |
| C11 | E. Björnson, J. Hoydis, and L. Sanguinetti, “Massive MIMO Has Unlimited Capacity” | IEEE TWC, 2018, 17(1), 574–590 | [DOI: 10.1109/TWC.2017.2768423](https://doi.org/10.1109/TWC.2017.2768423) | Correction of a prevailing claim, explicit conditions, theorem/proof structure, and bounded conclusion language |
| C12 | K. Shen and W. Yu, “Fractional Programming for Communication Systems—Part I: Power Control and Beamforming” | IEEE TSP, 2018, 66(10), 2616–2630 | [DOI: 10.1109/TSP.2018.2812733](https://doi.org/10.1109/TSP.2018.2812733) | Transform–equivalence explanation, theorem-to-application bridge, convergence statements, and relation to prior algorithms |

## Inspection anchors

The anchors below identify the document objects used for the initial rules. They make the distillation reproducible without copying source prose. Section numbering may differ between an accepted manuscript and the final IEEE version; use the named object together with the DOI record when rechecking.

| ID | Recheck these objects | Rule groups informed |
|---|---|---|
| C01 | Abstract; application overview; electromagnetic communication-theory framework; state-of-research synthesis; open research issues | Framing, taxonomy, scope limits, research agenda |
| C02 | Abstract; system model; joint active/passive beamforming formulation; alternating design; numerical-results discussion | Model order, coupled formulation, algorithm flow, baselines |
| C03 | Abstract; energy-efficiency formulation; solution-development and convergence/complexity discussion; numerical results | Objective explanation, guarantee boundaries, result claims |
| C04 | Abstract; multicell system model; interference-aware problem formulation; subproblem decomposition; simulation section | Multi-entity notation, decomposition, scenario comparison |
| C05 | Abstract and introduction; tutorial roadmap; canonical system models; design comparisons; concluding research directions | Tutorial sequence, definitions, comparison discipline |
| C06 | Abstract and introduction; principle/taxonomy sections; opportunity and challenge synthesis; conclusion | Literature grouping, taxonomy, limitation wording |
| C07 | Abstract; communication-model comparison; step-by-step surface-impedance formulation; local/global design comparison; numerical examples | Cross-domain definitions, assumptions, model validity |
| C08 | Abstract; problem class and assumptions; algorithmic framework; convergence results and proofs; Part-I/Part-II scope boundary | Assumption placement, theorem language, convergence scope |
| C09 | Abstract and introduction; propagation/training assumptions; asymptotic analysis; concluding engineering interpretation | Model assumptions, analytical progression, scoped implication |
| C10 | Abstract; Section I introduction; system and channel-estimation model; Theorem 1 and Appendix A; power-control algorithms; numerical comparison; Section VII conclusion | Definition order, theorem-to-algorithm trace, fair baseline reporting |
| C11 | Abstract and introduction; channel-covariance conditions; theorem/proof sequence; numerical examples; conclusion | Counterclaim framing, condition-first guarantees, bounded claims |
| C12 | Abstract and introduction; quadratic-transform statement and proof; communication applications; convergence discussion; relation to fixed-point/WMMSE methods | Transform status, theorem-to-application bridge, prior-work positioning |

## Distillation protocol

1. Treat DOI/publisher metadata as the identity record; record any preprint separately and never silently merge versions.
2. Observe document-level patterns: abstract moves, introduction functions, definition order, problem-formulation explanations, theorem assumptions, algorithm inputs/outputs, simulation setup, and claim-to-evidence links.
3. Generalize a rule only when it appears across at least two papers or label it as paper-/genre-specific.
4. Record counterexamples and venue/genre differences. A survey pattern must not automatically become a short technical-paper rule.
5. Do not copy distinctive phrasing. Express every accepted rule as an operational instruction that can be checked in a new manuscript.
6. Keep official IEEE templates and the target journal's current Author Guidelines authoritative for formatting and submission requirements.

## Coverage and limitations

- The corpus is strongest for wireless communications and communications-oriented optimization. Four non-RIS papers (C09–C12) provide independent checks on asymptotic analysis, distributed architectures, theorem-driven argument, and optimization methodology; domain transfer beyond communications still requires additional corpus material.
- It supports organization and technical communication; it cannot validate novelty, correctness, or journal fit by itself.
- DOI metadata confirms publication identity, not the interpretation of every stylistic choice.
- Before extending the profile to another engineering domain, add representative papers from that domain and repeat the cross-paper comparison.

## Update record

| Date | Change | Status |
|---|---|---|
| 2026-10-22 | Replaced the personal mentor-style source with a twelve-paper, cross-author IEEE corpus, added object-level inspection anchors, and established the initial transferable baseline | Confirmed by repository owner request |
