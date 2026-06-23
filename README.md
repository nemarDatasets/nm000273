[![DOI](https://img.shields.io/badge/DOI-10.82901%2Fnemar.nm000273-blue)](https://doi.org/10.82901/nemar.nm000273)

# OpenBMI SSVEP EEG dataset (Lee et al. 2019)

## Overview

A derivative dataset of SSVEP (steady-state visually evoked potential) recordings processed and organized using the Mother of All BCI Benchmarks (MOABB) framework. This dataset represents EEG data formatted according to BIDS standards, enabling standardized analysis and benchmarking of brain-computer interface paradigms based on steady-state visual stimulation. The dataset is derived from the Lee2019 source dataset (DOI: 10.5524/100542) and has been converted to BIDS format using MNE-BIDS tools. The dataset contains EEG recordings from multiple subjects across multiple sessions with SSVEP stimulation paradigms.

## Dataset Summary

| Property | Value |
|---|---|
| Subjects | 54 |
| Channels | 62 |
| Classes | 4 |
| Trial length | 4 s |
| Sampling frequency | 1000 Hz |
| Sessions | 2 |
| Total trials | 21600 |
| Paradigm | SSVEP |

## Data Collection Methods

See the primary publication for details on data collection and experimental protocol.

## How to Access via MOABB

Install MOABB and load this dataset directly:

```python
from moabb.datasets import Lee2019_SSVEP
from moabb.paradigms import SSVEP
paradigm = SSVEP()

dataset = Lee2019_SSVEP()
X, y, metadata = paradigm.get_data(dataset)
```

For more details see the [MOABB documentation](https://moabb.neurotechx.com/) and the
[MOABB dataset page](https://moabb.neurotechx.com/docs/generated/moabb.datasets.Lee2019_SSVEP.html).

## Citation

If you use this dataset please cite the primary publication:

> DOI: [10.1093/gigascience/giz002](https://doi.org/10.1093/gigascience/giz002)

## NEMAR / MOABB Benchmark Collection

This BIDS-formatted dataset was converted from the original data using the
[MOABB](https://moabb.neurotechx.com/) pipeline and re-hosted on
[NEMAR](https://nemar.org/) as part of the MOABB benchmark collection.
The original data and license terms apply — see `dataset_description.json` for details.
