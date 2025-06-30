# Computational Fluid Dynamics Simulation in a 2D Heat Exchanger

This project simulates fluid flow within a two-dimensional heat exchanger using different numerical schemes (Adams–Bashforth, Runge–Kutta, and fourth‑order centered differences) to validate their impact on the results.

## Project Structure

- **[Report.pdf](./Report.pdf)**  
  Full analytical report, divided into seven parts.  
- Each section’s folder contains the relevant data and source code.

## Sections

1. [Baseline Simulation with Second‑Order Adams–Bashforth](./1%20Baseline%20Simulation%20with%20Second-Order%20Adams-Bashforth/)  
2. [Stability Analysis with Increased CFL](./2%20Stability%20Analysis%20with%20Increased%20CFL/)  
3. [Implementing a Third‑Order Runge–Kutta Scheme](./3%20Implementing%20a%20Third-Order%20Runge-Kutta%20Scheme/)  
4. [Implementing Fourth‑Order Centered Differences](./4%20Implementing%20Fourth-Order%20Centered%20Differences/)  
5. [Long‑Term Flow Behavior Analysis](./5%20Long-Term%20Flow%20Behavior%20Analysis/)  
6. [Reverse Flow Direction Simulation](./6%20Reverse%20Flow%20Direction%20Simulation/)  
7. [Simulation of a Single Cylinder with Inflow/Outflow Boundary Conditions](./7%20Simulation%20of%20a%20Single%20Cylinder%20with%20Inflow-Outflow%20Boundary%20Conditions/)  

## Compilation and Execution

To compile the main solver:

```bash
gfortran -O3 2D_compressible.f90
```
(Replace gfortran with your Fortran compiler of choice.)

This produces an executable called **[a.out](./a.out)** .

If you are using gnuplot to generate the pgn files for the figures : 

```bash
gnuplot plot_gnu
```

If you are using python to generate the pgn files for the figures : 

```bush
python3 plot_py
```
