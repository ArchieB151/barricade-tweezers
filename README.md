Barricade Tweezers

Python code developed during my PhD for calculating three-dimensional optical tweezer potentials and simulating particle trajectories.

The simulations were used to investigate how a repulsive optical barrier surrounding an attractive tweezer affects particle transport and loading efficiency.

Numerical Methods

Optical potentials

The optical fields are calculated using the Richards–Wolf diffraction integral, accounting for the vector nature of tightly focused light.

The resulting intensity distributions are used to construct three-dimensional optical dipole potentials for the attractive and repulsive beams.

Monte Carlo simulations

Particle trajectories are calculated by numerically integrating the classical equations of motion,

[
m\frac{d^2\mathbf r}{dt^2}=-\nabla U(\mathbf r).
]

Initial positions and velocities are sampled from specified distributions. The trajectories are propagated through the potential to determine the rate at which particles cross a defined boundary.

Repeating this for different barrier configurations allows us to investigate how the barrier height affects particle flux.

Computational performance

Numba is used to accelerate the numerical calculations. Larger parameter studies were run in parallel on Durham University’s Hamilton HPC cluster.

Research

This code was developed for:

A. C. Baldock et al., Near-deterministic loading of optical tweezer arrays via repulsive barricade potentials.

Submitted to Physical Review Letters (2026), under review.

The simulations were used to design a loading protocol that increased predicted loading efficiency from approximately 35% to 82%.

Dependencies

Python, NumPy, SciPy, pandas and Numba.

Author

Archie Baldock
Department of Physics, Durham University
