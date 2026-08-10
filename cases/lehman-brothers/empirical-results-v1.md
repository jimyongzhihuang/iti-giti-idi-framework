# Lehman Brothers Empirical Results — v1

This file records the first frozen empirical results of the Lehman Brothers application of the ITI–gITI–IDI framework.

The purpose is to provide a compact public record of the principal first-run outputs, alignment, signed divergence, uncertainty bounds, and robustness boundary.

The framework is not interpreted as a bankruptcy-prediction system.

## 1. Principal ITI Result

The principal first-run ITI is generated from standardized gross and net leverage using principal component analysis.

The first principal component explains approximately **94.9%** of the standardized variation in the two leverage series.

The standardized ITI trajectory is:

| Period | ITI |
|---|---:|
| 2006Q1 | −0.172 |
| 2006Q2 | −0.025 |
| 2006Q4 | 0.289 |
| 2007Q1 | 0.847 |
| 2008Q1 | 1.408 |
| 2008Q2 | −0.709 |
| 2008Q3 | −1.638 |

ITI reaches its maximum in **2008Q1** and declines sharply thereafter as reported gross and net leverage fall.

This result is interpreted narrowly as a decline in leverage-visible institutional tension.

It is not interpreted as evidence that Lehman's total institutional condition improved.

## 2. Principal gITI Result

The principal gITI architecture contains five frozen relationship families:

1. ratings → unsecured funding access;
2. ratings → collateral requirements;
3. secured-funding conditions → Holding Company liquidity;
4. legal-entity transferability → Holding Company liquidity;
5. illiquid or concentrated assets → capital and funding pressure.

Each relationship is coded from 0 to 3 only where contemporaneous evidence supports the relationship.

**N/O denotes not observable and is not treated as zero.**

The principal point estimates are:

| Period | Observable Edge Families | gITI |
|---|---:|---:|
| 2007Q1 | 4/5 | 0.333 |
| 2008Q1 | 5/5 | 0.400 |
| 2008Q2 | 5/5 | 0.467 |

For 2008Q3, only one of the five principal relationship families is directly observable.

No precise point estimate is reported.

The admissible interval is:

**gITI ∈ [0.200, 1.000]**

## 3. Alignment

ITI and gITI are aligned only after independent generation.

The principal ITI alignment is:

**ITI* = (ITI − min ITI) / (max ITI − min ITI)**

gITI remains on its native [0,1] scale.

The alignment rule is frozen independently of the observed divergence pattern.

## 4. IDI and Signed Divergence

The Institutional Distortion Index is:

**IDIₜ = |gITI*ₜ − ITI*ₜ|**

The corresponding signed divergence is:

**Dₜ = gITI*ₜ − ITI*ₜ**

The principal aligned results are:

| Period | ITI* | gITI* | IDI | Dₜ |
|---|---:|---:|---:|---:|
| 2007Q1 | 0.816 | 0.333 | 0.482 | −0.482 |
| 2008Q1 | 1.000 | 0.400 | 0.600 | −0.600 |
| 2008Q2 | 0.305 | 0.467 | 0.162 | +0.162 |

The principal specification therefore produces an ordering reversal between **2008Q1 and 2008Q2**.

In 2008Q1, aligned leverage-visible tension exceeds relational tension.

By 2008Q2, aligned leverage-visible tension falls sharply while relational tension rises modestly.

Signed divergence changes from:

**−0.600 → +0.162**

For 2008Q3:

**Dₜ ∈ [0.200, 1.000]**

under the principal uncertainty bounds.

Because only one principal relational edge family is directly observable, this is an interval result rather than a point estimate.

## 5. Alternative ITI Robustness

The principal ITI result was compared with two transparent alternatives:

- equal-weight standardized gross and net leverage;
- average percentile-rank leverage composite.

Both preserve the Q1→Q2 ordering reversal.

Under the equal-weight standardized specification:

- 2008Q1 D = −0.600;
- 2008Q2 D = +0.162.

Under the rank-based specification:

- 2008Q1 D = −0.600;
- 2008Q2 D = +0.300.

The principal reversal is therefore not dependent on PCA weighting.

## 6. Alignment Robustness

An alternative common-period z-score alignment was also tested.

The Q1→Q2 sign reversal survives:

- 2008Q1 D remains negative;
- 2008Q2 D becomes positive.

The result is therefore not generated solely by the principal min-max alignment.

Because only three common principal point-score periods are available, this robustness result remains limited in scope.

## 7. Conservative gITI Robustness

The most consequential sensitivity test uses pre-recorded conservative relational coding.

Under the conservative specification:

- 2008Q1 gITI ≈ 0.067;
- 2008Q2 gITI ≈ 0.133.

Against the principal aligned ITI:

- 2008Q1 D ≈ −0.933;
- 2008Q2 D ≈ −0.172.

The precise Q2 crossover therefore does **not** survive conservative gITI coding.

This is a material qualification.

However, the direction of movement remains different:

- leverage-visible ITI falls sharply;
- conservative gITI rises.

The stronger empirical finding is therefore separation in direction rather than specification-invariant crossover timing.

## 8. Q3 Uncertainty

Under the principal Q3 bounds:

**Dₜ ∈ [0.200, 1.000]**

Under conservative gITI coding:

**Dₜ ∈ approximately [0.133, 0.933]**

The sign remains positive under both specifications.

However, Q3 has only one of five principal relational edge families directly observable.

The result is therefore directional rather than precise.

## 9. Empirical Classification

The current empirical classification is:

**CONDITIONAL SUPPORT**

The evidence supports the proposition that observable quantitative institutional condition and relational institutional condition can move apart before terminal failure.

The evidence does not establish:

- a universal bankruptcy threshold;
- a general failure-prediction rule;
- specification-invariant crossover timing;
- universal superiority of gITI over conventional indicators;
- common numerical thresholds across institutions.

## 10. Strongest Supported Finding

The strongest supported empirical statement is:

**Late-window reductions in leverage-visible institutional tension were not accompanied by an equivalent reduction in relational strain.**

The principal specification identifies a Q1→Q2 ordering reversal.

Alternative ITI constructions and alternative alignment preserve that reversal.

Conservative relational coding removes the precise Q2 crossover but preserves the directional separation.

The late-window direction of separation is therefore better supported than the precise timing or magnitude of the crossover.

## 11. Fiscal-Geometric Interpretation

The empirical results operate within the broader Fiscal-Geometric model:

**Fᴳᶜ = X × Y**

where:

- **X** denotes horizontal execution and carrying capacity across contemporaneous institutional space;
- **Y** denotes vertical carrying capacity through time.

ITI is not identical to X.

gITI is not identical to Y.

The indices are measurement instruments for examining observable manifestations of institutional condition.

The Lehman result supports the narrower proposition that substantial current execution can coexist with strain in the relationships required to reproduce that execution through time.

## 12. Current Research Boundary

This file records the first frozen Lehman result.

Future work should not rewrite the principal first-run specification simply because a later specification produces stronger divergence.

Subsequent work should be identified as:

- source correction;
- pre-declared robustness;
- comparative validation;
- later-version methodological extension.

The next major empirical stage is comparison with additional failed institutions and surviving peers.
