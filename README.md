# Viscous Burgers' Equation Solver

This MATLAB package solves the viscous Burgers' equation with smooth solutions generated from Gaussian Random Fields.

## Equation
The viscous Burgers' equation:
```
u_t = u*u_x + u_xx
```

## Domain
- Time: [0, 0.15]
- Space: [0, 2)
- Grid: 501 × 201 points

## Features
- 10 smooth initial conditions using Gaussian Random Fields
- Crank-Nicolson + upwind numerical scheme
- Smooth solutions avoiding sharp corners
- Comprehensive visualization and verification

## Files
- `burgers_solver.m` - Main solver
- `run_simulations.m` - Driver script with visualization
- `verify_smoothness.m` - Smoothness verification
- `README.md` - This file

## Usage

1. Run the main simulation:
```matlab
run_simulations
```

2. Verify smoothness:
```matlab
verify_smoothness
```

## Output
- `solution_*.mat` - Individual solutions (10 files)
- `all_solutions.mat` - All solutions combined
- `figures/` - Visualization plots
- `smoothness_report.mat` - Smoothness metrics

## Key Parameters
- Viscosity coefficient: ν = 1.0
- Smoothness ensured through spectral filtering
- Maximum wavenumber: k_max = 5
- Gaussian filtering applied for additional smoothness