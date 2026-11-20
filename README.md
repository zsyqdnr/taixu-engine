# taixu-engine
Closed research API for SLC‑C EEG metric, meditation & altered‑state research

# Taixu‑Engine API
> Spatiotemporal Limit‑Cycle Crystallinity (**SLC‑C**) — Model‑free EEG scalar metric for meditation & altered‑states‑of‑consciousness research

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24377579.svg)](https://doi.org/10.5281/zenodo.24377579)

## Overview
Taixu‑Engine provides a closed‑research API for computing **SLC‑C (Spatiotemporal Limit‑Cycle Crystallinity)**, a composite EEG metric built from the Sync × Coverage two‑dimensional signature.

SLC‑C quantifies whole‑brain spatiotemporal dynamical integration from BDF EEG recordings. It distinguishes **local high synchrony** from genuine **whole‑brain functional coordination**, and outputs continuous scalar values.
A falsifiable hypothesis is proposed in the preprint: extreme SLC‑C values may serve as neurophysiological proxies for flow‑state and deep meditative altered states of consciousness.

> ⚠️ **Important note**: This is an exploratory research‑only tool.
>‑ It is NOT a medical device, no medical certification in any jurisdiction.
>‑ Not for clinical diagnosis, disease screening or therapeutic decision‑making.
>‑ Results are signal statistics of your recording, not clinical measurements.

Preprint: https://doi.org/10.5281/zenodo.24377579

## Intellectual‑property statement
The preprint publishes theoretical framework and qualitative descriptions only.
Exact mathematical formulations, internal parameters and the anchor‑score algorithm are **proprietary commercial assets**. No source code is released.
Only top‑level scalar outputs and percentile‑based demonstrative profiles are made available for research use.

## Input requirements
‑ Input format: BDF / BDF+ (BioSemi standard format)
‑ Minimum recording length: > 6 minutes
‑ Recommended: 64‑channel high‑density EEG recordings; results degrade with fewer channels or noisy recordings.
‑ Poor electrode contact, motion artifacts and line‑noise will bias metric outputs.

## What you receive from the API
Three primary scalar return values (always available for research screening):
1. `SLC‑C`: Spatiotemporal Limit‑Cycle Crystallinity scalar
2. `Sync`: Cross‑channel spatial synchrony percentile (reference‑cohort)
3. `Coverage`: Spatial feature‑spread percentile (reference‑cohort)

> Full demonstrative PDF reports (containing radar‑plot, percentile bar‑chart and qualitative signal reading) are **only shared under formal research collaboration arrangements**, not for ad‑hoc single‑file screening requests.

## Usage tiers
### Tier 1 — Academic screening (free, exploratory)
For researchers wanting a quick feasibility check on their existing BDF datasets.
‑ Deliverables: Only three scalar numbers (`SLC‑C`, `Sync`, `Coverage`). No PDF report.
‑ Limits: small volume of test files per research group.
‑ Expectation: please cite the preprint in any resulting manuscripts or preprints if you use these scalar outputs.

### Tier 2 — Formal research collaboration (free / negotiated)
Eligibility: you intend to produce peer‑reviewed work or preprint, and agree to cite the Zenodo preprint. Joint authorship may be discussed depending on contribution scope.
‑ Deliverables: scalar metrics + full de‑identified demonstrative PDF reports for your dataset.
‑ We may also discuss experimental design for meditation / altered‑state EEG paradigms.

### Tier 3 — Commercial / large‑batch processing (paid service)
For companies, hardware vendors or large‑scale proprietary projects without academic publication goals.
‑ Contact for pricing, volume‑based terms.

## Citation
If you use SLC‑C metrics in your work, please cite the preprint:

**APA‑7 format**
> Ou, Q. (2026). Spatiotemporal Limit‑Cycle Crystallinity (SLC‑C): A complex‑systems scalar for whole‑brain dynamical integration during meditative and flow states (v1.1) [Preprint]. Zenodo. https://doi.org/10.5281/zenodo.24377579

**BibTeX**
```bibtex
@misc{ou2026slcc,
  title={Spatiotemporal Limit‑Cycle Crystallinity (SLC‑C): A complex‑systems scalar for whole‑brain dynamical integration during meditative and flow states},
  author={Ou, Qiao},
  year={2026},
  version={1.1},
  publisher={Zenodo},
  doi={10.5281/zenodo.24377579},
  url={https://doi.org/10.5281/zenodo.24377579}
}
## Contact

Qiao Ou (ORCID: 0009‑0008‑4540‑1381)
Email: qiao.ou@outlook.com

When writing, briefly describe:
‑ your research topic / paradigm
‑ number of BDF files you plan to submit
‑ which usage‑tier you are requesting

## Repository note

This repository contains documentation only. No source code, no algorithm implementation.
All signal computation runs on closed‑backend API service.
