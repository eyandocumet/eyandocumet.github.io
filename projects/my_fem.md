---
layout: project
type: project
image: img/my_fem/plot_k_32.png
title: "\"My FEM\" MATLAB Finite Element Solver"
date: 2025
published: true
labels:
  - FEA
  - MATLAB
  - Programming
  - Simulation
  - Structural Analysis
summary: "A custom-built FEM solver developed in MATLAB for structural mechanics and thermal simulations."
---
<div class="d-flex justify-content-center">
  <img class="img-fluid" src="../img/my_fem/plot_k_32.png" alt="My FEM Plot" style="width: 45%; margin-right: 5%;">
  <img class="img-fluid" src="../img/my_fem/adaptive_mesh.png" alt="Adaptive meshing!" style="width: 45%;">
</div>

My FEM is a repository that contains a home-made Finite Element Method (FEM) solver for structural mechanics simulations in 1D, 2D, and 3D. Developed as part of coursework for ME C180 at UC Berkeley, it tackles a variety of FEM problems.

The solver is designed for high efficiency and capable of running on standard laptops and even smartphones. The solver was systematically analyzed and compared against benchmark problems to validate its accuracy.

The implemented features so far include:
- 1D Stick Problems and Error Estimation of Benchmarks ODE's.
- Higher order nodes and p-refinement (up to 3rd order)
- Remeshing
- Adaptive h-refinement
- Principle of Minimum Potential Energy (PMPE) (Error approximation)

Up next, I'm tackling:
- Optimizing solution and storage efficiency. (Mainly eliminating all the extra zero's in my stiffness matrix.)

Over the course of eight distinct projects, it is being iteratively enhanced with various techniques like h-refinement, p-refinement, and even machine learning integration to improve its performance. The project successfully implemented 1D stick problem simulations, and 2D and 3D problem setups are currently in progress.

Most of this work is derived from _The Basics_, by Tarek Zhodi, a comprehensive primer on the mathematics of FEM, which is [available from Springer Nature](https://link.springer.com/book/10.1007/978-3-319-70428-9).
