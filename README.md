# Diffusion-Limited Aggregation and Reaction-Diffusion Simulation

Group project exploring computational methods for modelling aggregation and pattern-formation phenomena. The project implements three numerical simulations: a Diffusion-Limited Aggregation (DLA) model solved with Successive Over-Relaxation (SOR), a Monte Carlo DLA model using random walkers on a discrete grid, and the Gray-Scott reaction-diffusion system. Each simulation demonstrates how simple local rules give rise to complex emergent spatial structures, and the results are analysed through concentration-field visualisations and animations.

## Methods and Tools

- **DLA with SOR** -- Solves the Laplace equation on a grid to compute diffusion probabilities, iteratively growing fractal aggregates.
- **Monte Carlo DLA** -- Simulates individual random walkers that attach on contact with a seed cluster, building aggregates stochastically.
- **Gray-Scott Model** -- Integrates a two-species reaction-diffusion PDE system to produce Turing-type patterns (spots, stripes, waves) under varying feed and kill rates.
- **Libraries**: NumPy, Matplotlib, Numba (JIT acceleration), SciPy

## Project Structure

```
├── src/
│   ├── simulation.py        # DLA simulation with SOR
│   ├── dla.py               # DLA helper functions
│   ├── gs_class.py          # Gray-Scott model class
│   ├── gs_visual.py         # Gray-Scott visualisation utilities
│   └── 2c.py                # Supplementary analysis
├── grid.py                  # Grid class for Monte Carlo DLA
├── random_walker.py         # Random walker class for Monte Carlo DLA
├── dla_notebook.ipynb       # DLA with SOR -- run and analysis
├── montecarlo_dla.ipynb     # Monte Carlo DLA -- run and analysis
├── gray_scott.ipynb         # Gray-Scott model -- run and analysis
└── new.py                   # Additional experiments
```

## Requirements

- Python 3.12+
- NumPy, Matplotlib, Numba, SciPy

## Usage

Open and run the Jupyter notebooks to reproduce the simulations:

```bash
jupyter notebook dla_notebook.ipynb        # DLA with SOR
jupyter notebook montecarlo_dla.ipynb      # Monte Carlo DLA
jupyter notebook gray_scott.ipynb          # Gray-Scott reaction-diffusion
```

Note: some cells in the Gray-Scott notebook may take over a minute to execute due to the PDE integration.

## Authors

Liesbet Ooghe, Frederieke Loth, Kushnava Singha

## Course

Scientific Computing, University of Amsterdam, 2024
