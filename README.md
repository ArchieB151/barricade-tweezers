# Barricade Tweezers

Scientific Python code developed during my PhD to model repulsive optical barriers for improving loading in molecular optical-tweezer arrays.

The simulations were used to design a repeated-loading protocol predicted to increase array loading from 35% to 81% at experimentally realistic laser powers.

## Methods

- Calculate three-dimensional vector optical fields using Richards-Wolf diffraction integrals.
- Convert optical intensities and molecular light shifts into state-dependent potentials.
- Propagate thermal particle ensembles using 3D Monte Carlo simulations to estimate particle flux through the barrier.
- Parallelise optical-potential calculations across CPU cores and accelerate trajectory and force-interpolation routines with Numba.

Large parameter studies were run on Durham University's Hamilton HPC cluster.

## Setup

Requires Python 3.13 and [`uv`](https://docs.astral.sh/uv/).

```bash
uv sync
```

The workflow scripts are contained in `scripts/`. Full `501^3` potential grids are generated locally and are not stored in the repository.

## Research

Code developed for:

**A. C. Baldock et al., *Near-deterministic loading of optical tweezer arrays via repulsive barricade potentials*.**

Accepted in *Physical Review Research* (2026).

## Author

Archie Baldock  
Department of Physics, Durham University
