<p align="center">
  <img src="assets/gateformer-banner.svg" width="100%" alt="GateFormer — Forecast-space decomposition for solar irradiance forecasting">
</p>

<h1 align="center">GateFormer</h1>

<p align="center">
  <strong>Forecast-space decomposition for intra-hour solar irradiance prediction from sky images</strong>
</p>

<p align="center">
  <a href="https://github.com/DavidHamlyn">David Hamlyn</a> · Sunny Chaudhary · Jonathon Hare · Tasmiat Rahman<br>
  University of Southampton<br>
  <em>Energy and AI · 2026</em>
</p>

<p align="center">
  <a href="https://doi.org/10.1016/j.egyai.2026.100917"><strong>Read the paper ↗</strong></a>
  &nbsp;·&nbsp;
  <a href="https://davidhamlyn.github.io/GateFormer/">Project page</a>
  &nbsp;·&nbsp;
  <a href="#citation">Citation</a>
  &nbsp;·&nbsp;
  <a href="#code-release">Code release</a>
</p>

<p align="center">
  <a href="https://doi.org/10.1016/j.egyai.2026.100917"><img src="https://img.shields.io/badge/DOI-10.1016%2Fj.egyai.2026.100917-245c72" alt="DOI: 10.1016/j.egyai.2026.100917"></a>
  <a href="https://www.sciencedirect.com/journal/energy-and-ai"><img src="https://img.shields.io/badge/Published_in-Energy_and_AI-d49b38" alt="Published in Energy and AI"></a>
  <a href="#code-release"><img src="https://img.shields.io/badge/Code-coming_soon-697687" alt="Code coming soon"></a>
</p>

---

## Overview

GateFormer forecasts global horizontal irradiance (GHI) from sky imagery and recent irradiance measurements. A shared, GHI-conditioned Vision Transformer feeds two complementary predictors: one forecasts the future trajectory, while the other predicts change at the final horizon. A learned gate blends their forecasts, followed by a residual correction.

<p align="center">
  <img src="assets/gateformer-overview.svg" width="100%" alt="Simplified method: sky images and GHI enter a shared Vision Transformer; trajectory and delta forecasts are adaptively blended, then refined with residual correction.">
</p>

<p align="center"><sub>Conceptual overview. See the paper for the full architecture and conditioning inputs.</sub></p>

## Results at a glance

| Evaluation | Reported result |
| :--- | :--- |
| NREL-TSI · +30 minutes | **125.01 W/m² RMSE** |
| Comparison with SIAT · paired timestamps | **9.6% lower RMSE** |
| Forecast skill over smart persistence · three sites | **22.97–28.86%** |

Evaluated on **NREL-TSI, Chilbolton, and SIRTA**. Figures are from the [published paper](https://doi.org/10.1016/j.egyai.2026.100917); comparisons follow its evaluation protocol.

## Code release

**Code coming soon.** This repository currently serves as the paper’s project page. The implementation will be added here in a future update.

Star this repository to bookmark the project, or use **Watch → Custom → Releases** to follow future releases.

## Citation

If this work is useful to your research, please cite:

```bibtex
@article{hamlyn2026gateformer,
  title   = {{GateFormer}: Forecast-space decomposition for intra-hour solar irradiance prediction from sky images},
  author  = {Hamlyn, David and Chaudhary, Sunny and Hare, Jonathon and Rahman, Tasmiat},
  journal = {Energy and AI},
  volume  = {26},
  pages   = {100917},
  year    = {2026},
  doi     = {10.1016/j.egyai.2026.100917},
  url     = {https://doi.org/10.1016/j.egyai.2026.100917}
}
```

Download the [BibTeX entry](citation.bib), or use GitHub’s **Cite this repository** button.

## Related research

[Vision Transformers for Estimating Irradiance Using Data-Scarce Sky Images](https://github.com/DavidHamlyn/solar-irradiance-vision-transformer) — our earlier work on solar irradiance estimation, published in *Energy and AI* (2025).
