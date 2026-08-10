# Project Roadmap

This repository develops the ITI–gITI–IDI framework through a staged empirical research programme.

The Lehman Brothers application has now progressed beyond preliminary variable mapping and index design. The first independent ITI and gITI runs, scale alignment, IDI calculation, and core robustness tests have been completed.

The roadmap therefore distinguishes between:

- completed foundational work;
- current empirical consolidation;
- next-stage comparative validation;
- cross-domain extension.

## Phase 1 — Public Source and Evidence Architecture

**Status: COMPLETED**

The first phase established the evidentiary foundation for the Lehman Brothers application.

Completed work includes:

- collection of contemporaneously available public disclosures;
- SEC filing and accession registration;
- construction of a source register;
- creation of an evidence ledger;
- separation of principal and validation-only evidence;
- implementation of a temporal firewall;
- documentation of unresolved source gaps.

The governing rule is:

**later knowledge does not become earlier evidence.**

Post-event materials may be used for validation, interpretation, or falsification but cannot generate principal pre-failure ITI or gITI values.

## Phase 2 — Measurement Architecture

**Status: COMPLETED**

The second phase separated quantitative and relational measurement.

### ITI path

ITI is generated from contemporaneously admissible quantitative observations.

The frozen candidate universe includes:

- gross leverage;
- net leverage;
- tangible equity capital;
- Holding Company liquidity;
- short-term funding burden;
- Level III exposure;
- rating-linked collateral requirements.

The principal first-run specification uses gross and net leverage because they provide the most consistent same-definition longitudinal coverage.

### gITI path

gITI is reconstructed independently from documented institutional relationships.

The frozen principal relationship families are:

1. ratings → unsecured funding access;
2. ratings → collateral requirements;
3. secured-funding conditions → Holding Company liquidity;
4. legal-entity transferability → Holding Company liquidity;
5. illiquid or concentrated assets → capital and funding pressure.

N/O denotes an unobservable relationship and is not treated as zero.

## Phase 3 — First Independent Index Generation

**Status: COMPLETED**

### ITI

The principal first-run ITI uses principal component analysis of standardized gross and net leverage.

The first principal component explains approximately **94.9%** of the standardized variation in the two series.

The ITI trajectory reaches its maximum in **2008Q1** and declines sharply thereafter.

### gITI

The principal first-run gITI uses observed-edge ordinal strain intensity.

Point estimates are reported only where at least four of five frozen relationship families are observable.

Principal point estimates include:

- 2007Q1: 0.333;
- 2008Q1: 0.400;
- 2008Q2: 0.467.

The final pre-failure 2008Q3 observation is reported as an uncertainty interval because relational coverage is incomplete.

## Phase 4 — Alignment and Institutional Distortion

**Status: COMPLETED**

ITI and gITI are aligned only after independent generation.

The principal formulas are:

**IDIₜ = |gITI*ₜ − ITI*ₜ|**

**Dₜ = gITI*ₜ − ITI*ₜ**

The principal aligned results are:

| Period | ITI* | gITI* | IDI | Dₜ |
|---|---:|---:|---:|---:|
| 2007Q1 | 0.816 | 0.333 | 0.482 | −0.482 |
| 2008Q1 | 1.000 | 0.400 | 0.600 | −0.600 |
| 2008Q2 | 0.305 | 0.467 | 0.162 | +0.162 |

The principal specification therefore produces an ordering reversal between 2008Q1 and 2008Q2.

For 2008Q3, signed divergence remains positive throughout the admissible uncertainty interval.

## Phase 5 — Robustness and Claim Control

**Status: COMPLETED**

The first robustness battery includes:

- alternative ITI construction;
- rank-based ITI construction;
- alternative monotone scale alignment;
- conservative gITI coding.

The Q1→Q2 ordering reversal survives alternative ITI construction and alternative alignment.

However, the most conservative gITI coding removes the precise Q2 crossover.

The current empirical classification is therefore:

**CONDITIONAL SUPPORT**

The strongest current conclusion is:

**the late-window direction of separation is better supported than the precise timing or magnitude of the crossover.**

The framework is not interpreted as a bankruptcy-prediction system or universal failure threshold.

## Phase 6 — Empirical Consolidation

**Status: CURRENT**

The current stage focuses on consolidating the Lehman application into a fully reproducible empirical record.

Current tasks include:

- finalizing the empirical manuscript;
- maintaining the frozen evidence and coding record;
- improving unresolved early-period source coverage where possible;
- preserving a public technical record of the ITI, gITI, and IDI procedures;
- documenting the difference between principal and conservative specifications;
- preparing figures and tables for scholarly publication.

The objective is reproducibility rather than expansion of the claim.

## Phase 7 — Failed-Institution Comparative Validation

**Status: NEXT**

The next major empirical step is to apply the same architecture to additional failed financial institutions.

Potential cases may include:

- Bear Stearns;
- Merrill Lynch;
- other financial institutions with sufficient contemporaneous public evidence.

The purpose is not to search retrospectively for a visually similar failure pattern.

The comparative test is whether the same frozen architecture identifies comparable late-window divergence without redesigning the framework for each institution.

Key questions include:

- Does ITI fall or stabilize while gITI remains elevated?
- Does signed divergence become positive?
- Is the divergence persistent?
- Does the timing differ across institutions?
- Which relational mechanisms are institution-specific and which are recurrent?

## Phase 8 — Surviving-Peer Comparison

**Status: PLANNED**

A stronger test requires institutions exposed to the same crisis environment that did not fail.

Potential surviving peers may include functionally comparable institutions such as:

- Goldman Sachs;
- JPMorgan Chase;
- other institutions with sufficiently comparable public evidence.

The central question is not whether surviving institutions avoid all divergence.

It is whether divergence:

- compresses;
- reverses;
- stabilizes;
- or is followed by restoration of institutional carrying capacity.

A surviving-peer comparison is necessary to determine whether the Lehman pattern reflects general crisis stress or a more specific deterioration in institutional continuity.

## Phase 9 — Comparative Calibration

**Status: PLANNED**

Once multiple financial institutions have been reconstructed, comparative analysis can examine:

- timing of divergence;
- duration of divergence;
- sign persistence;
- recovery versus continued deterioration;
- sensitivity to graph coding;
- relationship between relational strain and conventional financial indicators.

At this stage the project may begin testing whether common empirical regularities exist.

No universal ITI, gITI, or IDI threshold will be assumed in advance.

## Phase 10 — Cross-Domain Extension

**Status: LONGER-TERM**

The framework may later be applied beyond financial institutions.

Potential domains include:

- pension systems;
- sovereign and public funds;
- public authorities;
- administrative systems;
- educational institutions;
- regulatory institutions.

Cross-domain applications must preserve:

### Architectural invariance

The separation between ITI, gITI, and their subsequent comparison remains constant.

### Functional translation

Each domain must define its own manifestations of horizontal execution and vertical carrying capacity.

### Empirical calibration

Variables, relationships, reporting intervals, evidentiary rules, and reference populations must be calibrated to the institution being studied.

Common numerical thresholds should not be assumed across domains without comparative validation.

## Long-Term Research Objective

The long-term objective is not to create another generalized failure-prediction score.

The research programme asks a different question:

**When does an institution that remains operational begin to lose the relational capacity required to reproduce that operation through time?**

The ITI–gITI–IDI framework provides one empirical architecture for investigating that question.
