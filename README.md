# Quotient-Group Obstructions in the Erdős–Straus Equation

**An open, AI-assisted mathematical research project by the Asscoin Institute for Advanced Mathematics.**

*Independent research. Questionable funding. Reproducible results.*

## Overview

This repository contains a preliminary investigation of quotient-group obstructions for a restricted class of Type II divisor constructions associated with the **Erdős–Straus conjecture**.

The conjecture asks whether, for every integer \(n\ge2\), there exist positive integers \(x,y,z\) satisfying

\[
\frac4n=\frac1x+\frac1y+\frac1z.
\]

Our investigation does **not** claim to resolve this conjecture.

Instead, we examine when particular modular constructions admit Type II solutions while excluding Type I solutions, and how the resulting restrictions depend on the structure of finite multiplicative groups.

The underlying divisor-square parametrization is established mathematics. Our focus is on the sharpness of certain quotient-group obstructions and constrained minimum-modulus classifications.

**Mathematical novelty remains unconfirmed.** We welcome independent verification, counterexamples, corrections, and references to equivalent results in the existing literature.

## The central research question

For a denominator of the form

\[
x_m=q_1^m q_2^r q_3^s,
\]

where the \(q_i\) are distinct primes and \(r,s\) are fixed positive integers, consider a residual modulus

\[
a=4x_m-p\equiv3\pmod4.
\]

Under what conditions can a Type II quadratic-divisor construction persist for every sufficiently large \(m\), while Type I constructions are excluded throughout the full divisor set \(D(x_m^2)\)?

The research studies this question through the quotient group

\[
Q=(\mathbb Z/a\mathbb Z)^\times/\langle q_1\rangle.
\]

The preliminary note establishes a finite quotient-group criterion and an index obstruction for these *pure Type II* modular constructions.

## Main results presented

The manuscript develops:

- **A quotient-group criterion:** Necessary and sufficient conditions for eventual pure Type II modular families.
- **An index-eight obstruction:** Such families require the relevant quotient group to have at least eight elements.
- **A base-2 classification:** A characterization of the equality case when the growing prime base is 2 and the quotient index is eight.
- **Four constrained minimum moduli:** The values 11, 31, 127, and 195, each under explicitly stated restrictions.

These are statements about modular admissibility. They do not establish infinitely many prime values of \(p=4x_m-a\), universal coverage of primes, or a solution to the Erdős–Straus conjecture.

The precise hypotheses, proofs, and scope of each minimum appear in the manuscript.

## Research materials

| Resource | Contents |
|---|---|
| [Research note](./assignment13_research_note.pdf) | Five-page manuscript with definitions, theorems, proofs, and references |
| [Verification appendix](./assignment13_verification_appendix.pdf) | Four-page companion documenting finite search domains, quotient certificates, and numerical checks |
| [Verification script] | Reproducible exact-arithmetic verification |
| [Printed certificate] | Checks the finite certificate included in the manuscript |
| [Certificate outputs]| Deterministic verification results |

*Links should be updated to match the actual repository paths. Include only files that have been committed.*

## Reproducing the verification

The verification suite uses Python 3.8 or later and requires no external packages.

```bash
python3 verify.py --output-dir rerun
python3 printed_certificate.py
```

The scripts check finite modulus domains, subgroup and quotient calculations, explicit divisor conditions, and exact unit-fraction identities.

The computational checks support the finite certificates. The general mathematical statements rely on the proofs in the research note, not on finite sampling alone.

## Open questions and requests for review

We are particularly interested in feedback on the following:

1. **Prior art:** Is the sharp index-eight obstruction already established in an equivalent formulation?
2. **Mathematical significance:** Do the constrained minimum-modulus classifications add a useful distinction to existing Erdős–Straus parametrizations?
3. **Proof correctness:** Are there missing hypotheses, invalid deductions, or counterexamples to the stated results?
4. **Verification:** Do the finite certificates cover their claimed domains, and can the computations be independently reproduced?

Critical feedback is explicitly welcome. A counterexample or a relevant earlier theorem is a valuable research outcome.

Please open a GitHub Issue or Discussion with the relevant theorem, calculation, or reference.

## Research process and AI disclosure

This project originated as an exploratory experiment using advanced AI reasoning systems to investigate an open mathematical problem.

The research involved iterative conjecture generation, computational experimentation, adversarial model review, correction of false claims, and a separate prior-art investigation.

The manuscript and verification materials were prepared with substantial AI assistance. Independent model audits identified errors in earlier drafts, including incorrect modular calculations and overbroad theorem statements.

The current note reflects those corrections but has **not undergone formal human peer review**.

Agreement between AI systems is not treated as proof. We encourage independent mathematical and computational scrutiny.

## Related literature

The investigation builds on established work, including:

- Elsholtz and Tao, *Counting the number of solutions to the Erdős–Straus equation on unit fractions* (2013; corrected arXiv version 2015).
- Bradford, *Elementary Patterns from the Erdős–Straus Conjecture*, *Integers* 25 (2025), A54.
- Other references on divisor parametrizations and modular constructions cited in the manuscript.

Please consult the research note for the full bibliography.

## About the Asscoin Institute

The **Asscoin Institute for Advanced Mathematics** is an independent, pseudonymous, AI-assisted research initiative established in 2026.

Its mission is to explore mathematical questions with curiosity, computational tools, and a willingness to be proven wrong.

No academic affiliation, institutional endorsement, or formal peer-review status is claimed.

*Founded on curiosity. Sustained by questionable tokenomics. Correctable by anyone.*
