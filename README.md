This repository contains the full simulation and analysis code for the study on temporal grain as a physical limit of recurrent computation.

The code implements a delayed recurrent neural-mass model and evaluates how the ratio between the update interval (ΔT) and the intrinsic integration timescale (T_int) governs dynamical stability, representational capacity, and metabolic cost.

Two numerical schemes are supported: forward Euler (dt = ΔT) and second-order Runge–Kutta (dt = ΔT/2). All results reported in the manuscript can be reproduced by running the main script.

Requirements: Python 3.11+, NumPy (no GPU required).

To reproduce the main results, run the script directly:
python temporal_grain_analysis.py

The script prints summary statistics (I_T, D, ⟨P_tot⟩) for fine, intermediate, and coarse temporal-grain conditions and saves figures if plotting is enabled.

All parameters match those described in the Methods section of the manuscript.
