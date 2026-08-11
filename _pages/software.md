---
title: "Software"
permalink: /software/
author_profile: true
---

Research software and numerical tools developed as part of my research.

<!--
If more software packages are added in the future, duplicate the entire
software block below, starting from "## Software Name".
-->

## Analytic Dust-to-Gas Ratio Model

A standalone Python implementation of the analytic dust-transport models developed in Kuwahara & Lambrechts (2026, Papers I and II).  
Python 3.9 or newer is supported. The scientific package requires only NumPy and SciPy.

![Example output](/images/analytic-dust-to-gas.png)
{: .align-center}

[GitHub](https://github.com/AyumuKuwahara/analytic-dust-to-gas){: .btn .btn--small}
[Documentation](https://github.com/AyumuKuwahara/analytic-dust-to-gas/blob/main/docs/user_guide.md){: .btn .btn--inverse .btn--small}
[Paper I](https://arxiv.org/abs/2608.05661){: .btn .btn--inverse .btn--small}
[Paper II](https://arxiv.org/abs/2608.05672){: .btn .btn--inverse .btn--small}

### Overview

This package computes radial dust-to-gas ratio profiles in the envelopes of disk-embedded planets using the analytic models developed in Papers I and II.

It supports both convectively stable and fully convective envelopes in 2D and 3D, without requiring hydrodynamical simulation data.

### Features

- Compute dust-to-gas ratio profiles for fixed-Stokes-number or fixed-particle-size dust.
- Explore the 2D/3D envelope models presented in Papers I and II.
- Visualize model profiles with ready-to-use Jupyter notebooks.
- Export calculated profiles and model parameters to CSV and JSON files.

### Example

A dust profile for a 1-cm particle at 10 au can be computed with:

```python
from analytic_dust_to_gas import (
    EnvelopePreset,
    FixedParticleSize,
    ProfileSetup,
)

setup = ProfileSetup(
    envelope=EnvelopePreset.ISOLATED_CONVECTIVE_3D,
    particle=FixedParticleSize(1.0),
    orbital_radius_au=10.0,
)

result = setup.compute()
print(result.dust_to_gas)
```

Interactive and publication-oriented Jupyter notebooks are also available for visualization and parameter exploration.