# Failure of the Scalar Free-Fraction Closure of the Local Capacity-Metric Bridge (LC-O2-O1)

This repository contains the source of the paper
*Failure of the Scalar Free-Fraction Closure of the Local Capacity-Metric Bridge —
Trace Reduction, Co-Metric Inversion, and the Remaining Operator Problem
(LC-O2-O1 of the Lorentz-Capacity Sub-Programme)*
(`Beau2026lco2o1`).

## Overview

The paper **LC-O2** (`Beau2026lco2`) extends the temporal residual map
$\mathcal{P}_\tau^{\mathrm{Q5b}}$ to non-homogeneous fibrewise regimes through
a local Born-Infeld capacity radius $R(x)$, defined on two sides:

- **Capacity side:** $R_{\mathrm{capacity}}(x)^2 = 1 - \epsilon(x)$, with
  $\epsilon(x)$ the local spectral occupancy field.
- **Metric side:** $R_{\mathrm{metric}}(x)^2 = g_{\tau\tau}(x)/g_{\tau\tau}^\infty$,
  with $g_{\tau\tau}^\infty = -1/A_\tau^\infty$ and $A_\tau^\infty > 0$ postulated: Q11 leaves the temporal
  coefficient free, and the normalisation $g^{\mu\nu} = 2\eta^{\mu\nu}$ ($A_\tau^\infty = 2$) is a choice of
  units.

Their equivalence is stated in LC-O2 (Remark 3.2, Section 7.3) as an open
bridge, LC-O2-O1. This paper asks whether a scalar reduction of the local
admissibility weight closes it, and shows that it does not.

## Main Result (negative)

**Theorem (Failure of the free-fraction closure).** Assume the free-fraction law

$$A_\tau(x) = A_\tau^\infty\,(1 - \epsilon(x)),$$

with any postulated $A_\tau^\infty > 0$, together with the principal-symbol identification
$g^{\tau\tau} = -A_\tau$ (flat-space value $g^{\tau\tau,\infty} = -A_\tau^\infty$)
**and a diagonal temporal block** $g^{\tau i} = 0$ — without which
$g_{\tau\tau} \neq 1/g^{\tau\tau}$ in general. Then

$$R_{\mathrm{metric}}(x)^2 = \frac{1}{1 - \epsilon(x)},$$

so that $R_{\mathrm{metric}}^2 = R_{\mathrm{capacity}}^2$ requires
$(1-\epsilon)^2 = 1$, hence $\epsilon = 0$ in the physical range
$0 \le \epsilon < 1$. The value of $A_\tau^\infty$ cancels.

**The free-fraction law closes the homogeneous vacuum and nothing else.**

**Scope.** The result is deliberately narrow. A *reciprocal* scalar law
$A_\tau = A_\tau^\infty/(1-\epsilon)$ would close the bridge algebraically (it is not
derived here, and none is available in the corpus). What fails is therefore the
free-fraction law, **not scalar closure in general** — and the paper does not claim
that an operator-valued datum is necessary, that a covariantly transforming family
of local subspaces is impossible, or that the spatial components must be derived
jointly to close the temporal bridge.

The failure is one of *direction*, not of normalisation: a free-fraction law
makes the temporal co-metric coefficient *decrease* with occupancy, whereas a
Schwarzschild exterior requires it to *increase*
($A_\tau = A_\tau^\infty/(1-r_s/r)$, so that $|g_{\tau\tau}|$ decreases and clocks slow).

## No renormalisation repairs it

- **Constant rescaling is inert.** For $\widetilde g^{\mu\nu} = \kappa g^{\mu\nu}$
  the factor cancels in *both* normalised ratios (it scales numerator and
  denominator alike, and $\widetilde g_{\tau\tau} = \kappa^{-1} g_{\tau\tau}$).
  From $A_\tau^\infty = 2$, taking $\kappa = 1/4$ reproduces the flat-space value $-1/2$ used in the proposed
  derivation while leaving the no-go intact.
- **A local conformal factor would beg the question.** Agreement would require
  $\Omega^2(x) \propto (1-\epsilon(x))^{-2}$ — a new law read off the desired
  answer, which would also rescale the spatial components, and which appears in no
  source paper.
- **No densitised co-metric is available.** Q5b identifies the principal symbol
  directly as $\sigma_2(L_{\mathrm{eff}}) = g^{\mu\nu}k_\mu k_\nu$, leaving only a
  global scale freedom — already shown inert.

## What survives, and what remains open

$$\frac{g^{\tau\tau}}{g^{\tau\tau}_\infty} = 1-\epsilon \quad \text{(admissible ansatz)},
\qquad
\frac{g_{\tau\tau}}{g_{\tau\tau}^\infty} = 1-\epsilon \quad \text{(does not follow — the open bridge)}$$

The co-metric statement can be posed as an ansatz, but $R_{\mathrm{co}}$ is the
*metric inverse* of the capacity lapse and does not govern proper-time dilation.

## Three defects of the free-fraction derivation

1. **The trace form is a fresh postulate.** W1 (`Beau2026w1`) supplies cumulative
   admissibility weights $a_q(s)$ of a filtered *Dirichlet form* — a coefficient
   multiplying squared increments, not a partial trace, and with no dependence on
   any occupancy field. Q11 fixes no value of $A_\tau$: spatial $\mathrm{SU}(2)$ invariance leaves it free, and
   its Casimir value $2$ is a choice of units, not a normalised trace over a variable subspace.

2. **Type mismatch: vector versus subspace.** The occupancy is defined by the
   *norms of vectors* $C_{\mathrm{occ}}, C_{\mathrm{max}} \in \mathrm{Sym}^2(V_\rho)$,
   but the proof treats them as *subspaces* carrying a partial trace. For a genuine
   subspace, $\mathrm{tr}_C(\lambda I) = \lambda \dim C$ — quantised in
   $\{0,\tfrac13,\tfrac23,1\}$ since $\dim \mathrm{Sym}^2(V_\rho) = 3$ — whereas the
   argument requires $\lambda\|C\|^2$, continuous on $[0,1)$. A norm-valued occupancy
   cannot be a trace fraction without an additional occupation operator, density
   matrix, or weighted projector; none is defined.

3. **No local covariance law is stated.** A proper subspace of an irreducible
   module is not invariant, so restricting the weight to $C_{\mathrm{free}}(x)$ is
   not by itself equivariant. This is an *absence*, not an impossibility: a family
   $C_{\mathrm{free}}(x)$ may well transform covariantly, with invariant scalars
   (its rank, or the norm of a distinguished vector) well defined. What is missing
   is any such transformation rule, without which the homogeneous form of Q11 cannot
   be transported pointwise. Schur's lemma forces *scalarity* only.

Defects 2 and 3 are independent of the inversion: they would persist even if the
monotonicity were correct.

## Status

- Free-fraction closure of the capacity-metric bridge: **disproved** (Theorem 3.1)
- Attribution of the partial-trace form to W1: **not supported**; the trace step is
  additionally **mistyped**
- Local covariance law for $C_{\mathrm{free}}(x)$: **missing** (an absence, not an
  impossibility)
- Co-metric statement $g^{\tau\tau}/g^{\tau\tau}_\infty = 1-\epsilon$: **survives**
  as an admissible ansatz
- **LC-O2-O1: open**
- Remark 3.2 of LC-O2 states the equivalence as an explicitly declared
  postulate, physically coherent and consistent with a supplied Schwarzschild weak-field
  metric, but **not derived**

Results of LC-O2 that take $R(x)$ as given — the local Born-Infeld sphere, the
fibrewise temporal residual map, the gravitational time-dilation corollary — are
**unaffected**.

## Open content

Open questions, listed as candidate routes rather than established requirements:

1. **Monotonicity.** Any closure must make the temporal co-metric coefficient
   increase where capacity is consumed, and this should follow from the
   construction rather than be imposed. Whether a *derived* scalar law with this
   property exists is open.
2. **Local covariance.** A transformation rule for the local admissible sector,
   allowing the homogeneous form of Q11 to be applied pointwise.
3. **Typing of the occupancy.** If occupancy is to enter through a trace, the
   corresponding occupation operator or weighted projector must be defined.
4. **Candidate: an operator-valued datum.** The local projector
   $P_{\mathrm{free}}(x)$ is *one* candidate, with the reduction derived rather
   than posited. We do not claim a scalar datum is insufficient.
5. **Relation to the spatial components.** Schwarzschild requires $g^{\tau\tau}$
   and $g^{rr}$ to vary differently; whether closing the *temporal* bridge alone
   requires a joint law is **not settled here**.

## Position in the sub-programme

```
LorCap -> TempProj -> LC-O2 -> LC-O2-O1 (no-go)
```

## Dependencies

| Paper | Role |
|-------|------|
| LC-O2 (`Beau2026lco2`) | Open problem statement (Remark 3.2, Section 7.3) |
| W1 (`Beau2026w1`) | Admissibility weights (Dirichlet form); no partial-trace form |
| Q5b (`Beau2026q5b`) | Principal symbol $\sigma_2(L_{\mathrm{eff}}) = g^{\mu\nu}k_\mu k_\nu$, under [H-L] and [H-lift] |
| Q11 (`Beau2026q11`) | Conditional homogeneous form; $A_\tau$ free, so $A_\tau^\infty$ is postulated |

## Repository Contents

```
lc-o2-o1/
|-- out/              # Compiled PDF
|-- tex/
|   |-- lc-o2-o1.tex
|   |-- cosmochrony-bibliography.bib
|-- compile.sh
|-- zenodo.json
|-- README.md
```

## Compilation

```bash
bash compile.sh
```

## Citation

> J. Beau, *Failure of the Scalar Free-Fraction Closure of the Local Capacity-Metric Bridge*,
> Preprint, 2026.

## Acknowledgements

Portions of the editorial refinement benefited from iterative interactions with
large language models used as analytical assistants.
All claims, interpretations, and final formulations remain the sole
responsibility of the author.
