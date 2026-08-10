# Lehman Brothers Variable and Relational Map

This file records the empirical objects used in the Lehman Brothers application of the ITI–gITI–IDI framework.

The purpose is not to assign every observed data point mechanically to ITI, gITI, or IDI.

The current architecture distinguishes between:

- quantitative candidates used to generate ITI;
- relational objects used to reconstruct gITI;
- aligned outputs used to calculate IDI and signed divergence;
- contextual or validation evidence that does not directly enter either principal index.

This distinction replaces the earlier expected-versus-realized variable map.

## 1. Quantitative Candidates for ITI

ITI is generated from contemporaneously admissible quantitative observations.

The frozen Lehman candidate universe includes:

| Candidate | Direction of Tension | Principal Role | Current Status |
|---|---|---|---|
| Gross leverage | Higher = greater tension | Core quantitative candidate | Principal first-run variable |
| Net leverage | Higher = greater tension | Core quantitative candidate | Principal first-run variable |
| Tangible equity capital | Lower = greater tension | Capital support candidate | Secondary / late-window |
| Holding Company liquidity pool | Lower = greater tension | Liquidity support candidate | Late-window core candidate |
| Short-term / 12-month funding burden | Higher = greater tension | Funding continuity candidate | Secondary |
| Level III exposure | Higher = greater tension | Valuation / illiquidity candidate | Late-window robustness |
| Rating-linked additional collateral requirement | Higher = greater tension | Liquidity sensitivity candidate | Robustness only |

The principal first-run ITI uses gross and net leverage because they provide the most consistent same-definition longitudinal coverage.

The other candidates remain part of the frozen empirical universe but are not forced into the principal long-window estimator where coverage is insufficient.

## 2. Principal ITI Inputs

The principal ITI estimator uses:

- gross leverage;
- net leverage.

Both are standardized so that higher values indicate greater observable institutional tension.

The estimator is:

**PCA on standardized gross and net leverage**

The first principal component explains approximately **94.9%** of the standardized variation in the two series.

The principal standardized ITI trajectory is:

| Period | ITI |
|---|---:|
| 2006Q1 | −0.172 |
| 2006Q2 | −0.025 |
| 2006Q4 | 0.289 |
| 2007Q1 | 0.847 |
| 2008Q1 | 1.408 |
| 2008Q2 | −0.709 |
| 2008Q3 | −1.638 |

The first-run ITI therefore represents leverage-visible institutional tension.

It is not a complete measure of Lehman's total institutional condition.

## 3. Relational Objects for gITI

gITI is not constructed from a second list of outcome variables.

It is reconstructed from documented institutional relationships.

The frozen principal relational architecture contains five edge families:

| Relational Edge Family | Source Node | Target Node | Institutional Meaning |
|---|---|---|---|
| Ratings → Unsecured Funding | Credit Ratings | Unsecured Funding Access | Whether rating deterioration affects access or cost of unsecured financing |
| Ratings → Collateral | Credit Ratings | Collateral Requirements | Whether rating changes trigger additional collateral demands |
| Secured Funding → Liquidity | Secured Funding Capacity | Holding Company Liquidity | Whether funding terms, haircuts, or repo capacity affect usable liquidity |
| Legal Transferability → Liquidity | Legal-Entity Transferability | Holding Company Liquidity | Whether resources located in subsidiaries can actually support Holdings |
| Illiquid Assets → Capital/Funding Pressure | Illiquid / Concentrated Assets | Capital and Funding Capacity | Whether difficult-to-carry assets create capital, funding, or monetization pressure |

These relationships are coded only where contemporaneous documentary evidence supports them.

## 4. Canonical gITI Nodes

The current Lehman graph ontology uses the following canonical nodes:

- Credit Ratings
- Unsecured Funding Access
- Collateral Requirements
- Secured Funding Capacity
- Holding Company Liquidity
- Legal-Entity Transferability
- Illiquid / Concentrated Assets
- Cash Capital / Long-Term Capital
- Investor / Creditor Confidence

Additional nodes may be introduced only through a declared robustness or later-version expansion.

Period-specific nodes should not be created simply to fit the evidence of a particular quarter.

## 5. Relational State Coding

Each observable principal relationship is coded using the frozen state protocol:

- **0** — functioning without material strain;
- **1** — trigger-sensitive or moderately constrained;
- **2** — materially constrained, concentrated, or increasingly backstop-dependent;
- **3** — functionally impaired, extraordinary-support dependent, or associated with structural separation or continuity threat;
- **N/O** — not observable from eligible contemporaneous evidence.

**N/O must never be treated as zero.**

The absence of documentary evidence does not establish that the relationship was functioning normally.

## 6. gITI Point-Score Rule

The principal first-run gITI is:

**mean observed edge state / 3**

A point estimate is reported only if at least **4 of the 5** frozen principal edge families are observable.

The current principal point estimates are:

| Period | Observable Edge Families | gITI |
|---|---:|---:|
| 2007Q1 | 4/5 | 0.333 |
| 2008Q1 | 5/5 | 0.400 |
| 2008Q2 | 5/5 | 0.467 |

For 2008Q3, only one principal edge family is directly observable.

No precise point score is reported.

The admissible interval is:

**gITI ∈ [0.200, 1.000]**

## 7. Contextual Quantitative Evidence

The following variables may inform institutional interpretation without automatically entering the principal ITI:

- total assets;
- total stockholders' equity;
- long-term capital;
- cash;
- collateralized financing;
- unencumbered assets;
- cash-capital surplus;
- mortgage and commercial real-estate exposure;
- quarterly net income or loss;
- mark-to-market adjustments;
- strategic asset sales or proposed separation transactions.

These observations can support interpretation of X, Y, liquidity conditions, capital pressure, asset-carrying burden, or robustness tests.

They do not enter ITI merely because they are numerically available.

## 8. Contextual Market and Outcome Evidence

The following evidence does not form the principal gITI merely because it reflects market stress or realized outcomes:

- stock-price decline;
- CDS spread movement;
- rating downgrade events;
- bankruptcy filing;
- post-failure contagion;
- examiner findings;
- litigation evidence.

Such evidence may be used for:

- timing comparison;
- validation;
- interpretation;
- falsification;
- external benchmarking.

Post-event evidence cannot generate a pre-failure principal ITI or gITI observation.

## 9. Temporal Admissibility

Every empirical object must retain:

- source;
- public date;
- reporting period;
- page or document location where available;
- admission status;
- evidence identifier;
- contemporaneous / validation-only classification.

Later disclosures cannot be substituted for missing earlier principal observations.

If a same-period value cannot be verified from contemporaneously eligible evidence, the principal cell remains missing.

## 10. IDI and Signed Divergence

IDI does not have its own independent input variables.

It is generated only after ITI and gITI have been independently calculated and aligned.

The formulas are:

**IDIₜ = |gITI*ₜ − ITI*ₜ|**

**Dₜ = gITI*ₜ − ITI*ₜ**

The principal aligned results are:

| Period | ITI* | gITI* | IDI | Dₜ |
|---|---:|---:|---:|---:|
| 2007Q1 | 0.816 | 0.333 | 0.482 | −0.482 |
| 2008Q1 | 1.000 | 0.400 | 0.600 | −0.600 |
| 2008Q2 | 0.305 | 0.467 | 0.162 | +0.162 |

For 2008Q3:

**Dₜ ∈ [0.200, 1.000]**

under the principal uncertainty bounds.

## 11. Mapping Rule

The current empirical mapping is therefore:

**quantitative observation → ITI candidate**

**documented institutional relationship → gITI edge/state**

**independently generated ITI and gITI → IDI and D**

The same source document may contribute to both ITI and gITI only where it supports two separately defined empirical objects.

For example:

- a reported liquidity amount may be an ITI candidate;
- a statement that liquidity must backstop loss of repo capacity may support a gITI relationship.

The number and the relationship must not be collapsed into a single observation.

## 12. Fiscal-Geometric Interpretation

The empirical map operates within:

**Fᴳᶜ = X × Y**

where:

- **X** = horizontal execution and carrying capacity across contemporaneous institutional space;
- **Y** = vertical carrying capacity through time.

Quantitative candidates and relational objects are observable manifestations used to examine these institutional capacities.

ITI is not X.

gITI is not Y.

IDI is not a bankruptcy probability.

The framework instead tests whether different observable representations of institutional condition begin to separate while the institution remains operational.

## 13. Current Empirical Status

The current Lehman result is classified as:

**CONDITIONAL SUPPORT**

The principal Q1→Q2 ordering reversal survives:

- alternative ITI construction;
- rank-based ITI construction;
- alternative scale alignment.

It does not survive the most conservative gITI coding.

The strongest current conclusion is therefore:

**the late-window direction of separation is better supported than the precise timing or magnitude of the crossover.**
