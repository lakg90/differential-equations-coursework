# Numerical Methods for Dynamical Systems and PDEs

This repository contains numerical experiments investigating **ordinary differential equations (ODEs)** and **partial differential equations (PDEs)**, with an emphasis on **accuracy, stability, and sensitivity to initial conditions**.  
The project combines analytical reasoning, numerical implementation, and visualisation.

---

## Contents

- `task1_wave_equation.ipynb` – Damped wave equation using spectral methods  
- `task2_lorenz_system.ipynb` – Lorenz system, numerical accuracy, and chaos  
- `README.md` – Project overview  

---

## Part 1: Damped Wave Equation

### Overview
A **damped wave equation** is solved on a one-dimensional spatial domain using a **Fourier sine series expansion**. The infinite series is truncated to a finite number of modes and reconstructed in physical space.

### Methods
- Modal decomposition and series truncation
- Reconstruction of the solution \( u(x,t) \)
- Comparison of solutions for different numbers of modes
- Time-dependent visualisation and animation

### Key Results
- Increasing the number of modes improves spatial accuracy
- Low truncation leads to loss of fine-scale structure
- The numerical solution exhibits physically consistent damping

---

## Part 2: Lorenz System

### Overview
The Lorenz system is a nonlinear system of ODEs that exhibits **chaotic behaviour** for certain parameter values. Despite being deterministic, the system shows strong **sensitivity to initial conditions**, limiting long-term predictability.

### What Was Done
- Analytical computation of equilibrium (critical) points
- Implementation of **Forward Euler** and **4th-order Runge–Kutta (RK4)** schemes
- Comparison of global error vs timestep
- Simulation and visualisation of the Lorenz strange attractor
- Sensitivity analysis using perturbed initial conditions

### Key Findings
- Euler’s method converges with first-order accuracy, while RK4 converges with fourth-order accuracy
- Small perturbations in initial conditions grow rapidly over time
- Trajectories diverge but remain confined to the same strange attractor
- Illustrates the distinction between short-term predictability (“weather”) and long-term statistical structure (“climate”)

---

## Author

**Leon Godtfredsen**  
University of Edinburgh  

---

## Acknowledgements

This project was completed as part of the Image Processing component of the course at the University of Edinburgh.


