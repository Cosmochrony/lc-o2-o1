# Local Spectral Closure of the Capacity-Metric Bridge (LC-O2-O1)

This repository contains the source of the paper
*Local Spectral Closure of the Capacity-Metric Bridge
(LC-O2-O1 of the Lorentz-Capacity Sub-Programme)*
(`Beau2026lco2o1`).

## Overview

The paper **LC-O2** (`Beau2026lco2`) extends the temporal residual map
$\mathcal{P}_\tau^{\mathrm{Q5b}}$ to non-homogeneous fibrewise regimes through
a local Born-Infeld capacity radius $R(x)$, defined simultaneously on two sides:

- **Capacity side:** $R(x)^2 = 1 - \epsilon(x)$, with $\epsilon(x)$ the local
  spectral occupancy field.
- **Metric side:** $R(x)^2 = -2\,g^{\tau\tau}(x)$.

Their equivalence was stated in LC-O2 (Remark 3.2, Section 7.3) as an open
analytic bridge: it could only be checked through the Einstein equations
imported from the Gravity branch. The present paper (LC-O2-O1) closes this
bridge purely spectrally, from local admissibility data alone.

## Main Result

The local capacity radius and the metric radius coincide:

$$R(x)^2 = 1 - \epsilon(x) = -2\,g^{\tau\tau}(x),$$

equivalently,

$$\epsilon(x) = 1 + 2\,g^{\tau\tau}(x).$$

The proof proceeds through two steps.

1. **Local admissibility-weight reduction (Lemma).** If $\epsilon(x)$ is defined
   as a quadratic occupancy in the rank-three sector $\mathrm{Sym}^2(V_\rho)$,
   then the local temporal coefficient of the effective admissibility operator
   satisfies
   $$A_\tau(x) = A_\tau^\infty \,(1 - \epsilon(x)) = 2\,(1 - \epsilon(x)).$$
   This follows from $\mathrm{SU}(2)$-invariance of the admissibility weight
   (Schur's lemma) and orthogonality of the occupied/free decomposition in
   $\mathrm{Sym}^2(V_\rho)$.

2. **Principal-symbol identification.** The principal-symbol reconstruction of
   the effective operator $L_{\mathrm{eff}}$, applied locally with the flat-space
   normalisation $A_\tau^\infty = 2$, $g^{\tau\tau,\infty} = -\tfrac{1}{2}$, gives
   $$g^{\tau\tau}(x) = -\frac{A_\tau(x)}{4}.$$

Combining the two yields $R(x)^2 = 1 - \epsilon(x) = -2\,g^{\tau\tau}(x)$.
The bridge is closed spectrally, without invoking the Einstein equation.

## Key features

- **No Einstein equation required.** The capacity-metric identity is derived
  from local admissibility data alone.
- **Quadratic occupancy is essential.** The Schur-lemma step requires
  $\epsilon(x)$ to be a quadratic norm on $\mathrm{Sym}^2(V_\rho)$, not an
  arbitrary additive scalar density.
- **Upgrade of Remark 3.2 of LC-O2.** What was previously an open postulate
  becomes a theorem.
- **Gravitational time dilation reinterpreted.** Near a mass source, the local
  capacity budget is more occupied, the residual radius
  $R(x) = \sqrt{1 - \epsilon(x)} < 1$ slows local clocks, consistently with
  the standard gravitational redshift.

## Status

- Local admissibility-weight reduction: **proved**
- Principal-symbol identification: **structural** (imports the symbol formula
  of Q5b/Q11)
- Spectral closure of the capacity-metric bridge: **proved**

## Position in the sub-programme

```
LorCap -> TempProj -> LC-O2 -> LC-O2-O1
```

## Dependencies

| Paper | Role |
|-------|------|
| LC-O2 (`Beau2026lco2`) | Open problem statement (Remark 3.2, Section 7.3) |
| W1 (`Beau2026w1`) | Admissibility-weight reduction argument |
| Q5b (`Beau2026q6b`) | Principal-symbol reconstruction of the effective metric |
| Q11 (`Beau2026q11`) | Flat-space normalisation $A_\tau^\infty = 2$ |

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

> J. Beau, *Local Spectral Closure of the Capacity-Metric Bridge*,
> Preprint, 2026.

## Acknowledgements

Portions of the editorial refinement benefited from iterative interactions with
large language models used as analytical assistants.
All claims, interpretations, and final formulations remain the sole
responsibility of the author.