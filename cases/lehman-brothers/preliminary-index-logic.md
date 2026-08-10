# Frozen Index Logic — Lehman Brothers Application

This file records the frozen first-run logic used to apply the ITI–gITI–IDI framework to the Lehman Brothers case.

The purpose is to preserve the distinction between quantitative measurement, relational reconstruction, scale alignment, and final interpretation.

The framework is not a bankruptcy-prediction model.

Its empirical question is:

**Can observable quantitative institutional condition and the relational capacity required to reproduce that condition begin to diverge before terminal failure?**

## 1. Measurement Architecture

The empirical architecture contains three distinct stages:

1. independently generate ITI from admissible quantitative evidence;
2. independently generate gITI from contemporaneously documented institutional relationships;
3. align the two measures only after both have been generated and calculate IDI and signed divergence.

The two measurement paths must remain separate during construction.

No gITI coding may be influenced by the observed ITI trajectory, and no ITI specification may be selected because it produces a more persuasive divergence.

## 2. ITI — Institutional Tension Index

ITI represents tension visible through contemporaneously admissible quantitative institutional conditions.

For the Lehman Brothers application, the frozen candidate universe includes:

- gross leverage;
- net leverage;
- tangible equity capital;
- Holding Company liquidity pool;
- short-term or twelve-month funding burden;
- Level III exposure;
- rating-linked or additional collateral requirements.

The principal first-run ITI uses gross and net leverage because these are the frozen core variables with sufficient same-definition longitudinal coverage for a reproducible first-run estimator.

Both variables are standardized so that higher values indicate greater tension.

The principal ITI estimator is:

**principal component analysis of standardized gross and net leverage**

The first principal component is sign-oriented so that higher scores indicate greater leverage-visible tension.

The first-run principal component explains approximately **94.9%** of the standardized variation in the two leverage series.

The resulting standardized ITI trajectory is:

| Period | ITI |
|---|---:|
| 2006Q1 | −0.172 |
| 2006Q2 | −0.025 |
| 2006Q4 | 0.289 |
| 2007Q1 | 0.847 |
| 2008Q1 | 1.408 |
| 2008Q2 | −0.709 |
| 2008Q3 | −1.638 |

The principal ITI therefore reaches its maximum in **2008Q1** and falls sharply thereafter.

This decline is interpreted narrowly as a fall in leverage-visible tension.

It is not interpreted as proof that Lehman's overall institutional condition improved.

## 3. gITI — Geometric Institutional Tension Index

gITI represents tension reconstructed from contemporaneously documented institutional relationships.

It is not an outcome-side score and is not constructed from post-failure consequences.

The frozen principal relational architecture contains five edge families:

1. **ratings → unsecured funding access**
2. **ratings → collateral requirements**
3. **secured-funding conditions → Holding Company liquidity**
4. **legal-entity transferability → Holding Company liquidity**
5. **illiquid or concentrated assets → capital and funding pressure**

Each relationship is coded only where eligible contemporaneous evidence supports its existence and condition.

The frozen relational state protocol is:

- **0** — relationship is evidenced and functioning without material strain;
- **1** — relationship is trigger-sensitive or moderately constrained;
- **2** — relationship is materially constrained, concentrated, or increasingly backstop-dependent;
- **3** — relationship is functionally impaired, extraordinary-support dependent, or associated with structural separation or continuity threat;
- **N/O** — relationship is not observable from eligible contemporaneous evidence.

**N/O is not State 0.**

Missing evidence therefore cannot be interpreted as evidence of institutional normality.

## 4. gITI Aggregation Rule

The principal first-run gITI operator is:

**observed-edge ordinal strain intensity**

For each institution-period:

**gITI = mean observed edge state / 3**

A principal point score is reported only where at least **4 of the 5** frozen edge families are observable.

Where fewer than four edge families are observable, no point estimate is reported.

Instead, an uncertainty interval is calculated:

**Lower bound = observed state sum / 15**

**Upper bound = (observed state sum + 3 × missing edge families) / 15**

This rule preserves missingness rather than imputing unobserved relationships.

The principal first-run results are:

| Period | Observed edge families | gITI |
|---|---:|---:|
| 2007Q1 | 4/5 | 0.333 |
| 2008Q1 | 5/5 | 0.400 |
| 2008Q2 | 5/5 | 0.467 |

For 2008Q3, only one principal edge family is directly observable.

The admissible interval is:

**gITI ∈ [0.200, 1.000]**

No midpoint is used as a principal estimate.

## 5. Temporal Firewall

The Lehman application uses a strict temporal firewall.

For a pre-failure institution-period observation:

- only evidence publicly available by the relevant cutoff may generate ITI;
- only contemporaneously available documentary evidence may generate gITI;
- post-event examiner reports, litigation records, or later disclosures may be used only for validation, interpretation, or falsification;
- later comparative figures cannot be used to backfill missing principal observations.

The objective is to prevent hindsight from determining the pre-failure measurement path.

## 6. Scale Alignment

ITI and gITI are aligned only after independent generation.

The principal ITI alignment maps the observed ITI support monotonically onto [0,1]:

**ITI* = (ITI − min ITI) / (max ITI − min ITI)**

gITI remains on its native [0,1] scale.

The principal alignment does not use gITI values to select the ITI transformation.

This prevents the alignment procedure from being chosen to maximize divergence.

## 7. IDI and Signed Divergence

After alignment:

**IDIₜ = |gITI*ₜ − ITI*ₜ|**

and:

**Dₜ = gITI*ₜ − ITI*ₜ**

IDI records the absolute distance between the two measurement paths.

Dₜ records the direction of the difference.

A positive D indicates that relational tension exceeds aligned quantitative tension.

A negative D indicates that aligned quantitative tension exceeds relational tension.

The principal aligned results are:

| Period | ITI* | gITI* | IDI | Dₜ |
|---|---:|---:|---:|---:|
| 2007Q1 | 0.816 | 0.333 | 0.482 | −0.482 |
| 2008Q1 | 1.000 | 0.400 | 0.600 | −0.600 |
| 2008Q2 | 0.305 | 0.467 | 0.162 | +0.162 |

The principal specification therefore produces an ordering reversal between 2008Q1 and 2008Q2.

For 2008Q3:

**Dₜ ∈ [0.200, 1.000]**

under the principal uncertainty bounds.

## 8. Robustness Rules

Robustness analysis varies one governed element at a time.

The principal first-run result is not replaced simply because another specification produces a larger divergence.

The robustness battery includes:

### Alternative ITI construction

Two alternative ITI constructions are used:

- equal-weight standardized gross and net leverage;
- average percentile-rank leverage composite.

Both preserve the Q1→Q2 ordering reversal.

### Alternative alignment

A common-period z-score alignment is used as a pre-specified monotone robustness check.

The Q1→Q2 sign reversal survives this alternative alignment.

### Conservative gITI coding

Each disputed relational state has a pre-recorded more conservative coding.

Under conservative coding:

- 2008Q1 gITI ≈ 0.067;
- 2008Q2 gITI ≈ 0.133.

The Q2 crossover no longer survives.

This is a material qualification.

The stronger finding is therefore the **directional separation** of the two measurement paths rather than a specification-invariant crossover date.

## 9. Interpretation Boundary

The framework does not treat ITI, gITI, or IDI as bankruptcy probabilities.

The current Lehman analysis does not establish:

- a universal failure threshold;
- a universal early-warning score;
- specification-invariant crossover timing;
- superiority of relational measures over all conventional indicators;
- portability of Lehman-specific variables to other institutional domains.

The strongest current empirical statement is:

**late-window reductions in leverage-visible institutional tension were not accompanied by an equivalent reduction in relational strain.**

The current empirical classification is:

**CONDITIONAL SUPPORT**

## 10. Fiscal-Geometric Relationship

The index architecture operates within the broader Fiscal-Geometric model:

**Fᴳᶜ = X × Y**

where:

- **X** denotes horizontal execution and carrying capacity across contemporaneous institutional space;
- **Y** denotes vertical carrying capacity through time.

ITI is not identical to X.

gITI is not identical to Y.

The indices are measurement instruments used to examine manifestations of the underlying institutional capacities.

The Lehman application therefore does not claim to estimate X and Y directly.

It tests whether continued institutional execution can coexist with deterioration or constraint in the relationships required to carry institutional operation forward through time.

## 11. First-Run Status

The following elements are now frozen or completed:

- ITI candidate universe;
- ITI principal estimator;
- gITI node and edge taxonomy;
- gITI state protocol;
- gITI first-run operator;
- temporal firewall;
- principal ITI alignment;
- principal IDI and signed-divergence calculation;
- alternative alignment;
- alternative ITI constructions;
- conservative gITI robustness coding.

The current first-run conclusion is:

**The ITI–gITI–IDI architecture produces a measurable late-window separation between leverage-visible tension and relational institutional tension in the Lehman Brothers case, but the precise timing and magnitude of the crossover remain sensitive to conservative relational coding.**
