# Black Hole Ringdown Simulation

## Overview

This project aims to numerically simulate **black hole ringdown**, the damped oscillations that occur when a black hole is disturbed.

We will study how small perturbations evolve around a Schwarzschild (non-rotating) black hole and how their characteristic oscillations, known as **quasinormal modes**, can be extracted from the resulting waveforms.

The project is part of the *Introduction to Numerical Algorithms* course.

## Mathematical Model

We consider a wave equation of the form

$$
\frac{\partial^2 \Psi}{\partial r\_\*^2}\
+\
V(r)\Psi=0,\
$$

where:

- $\Psi$ represents the perturbation.
- $r\_\*$ is the tortoise coordinate.
- $V(r)$ is the effective potential associated with the black hole.

## Objectives

- Implement a numerical solver using finite differences.
- Simulate the evolution of an initial perturbation.
- Visualize the resulting ringdown waveform.
- Extract the oscillation frequencies and damping rates.
- Compare the numerical results with theoretical predictions.
- Investigate numerical stability, accuracy, and convergence.

## Methods and Tools

We plan to use **Python**, along with NumPy, SciPy, and Matplotlib.

The project will focus on numerical integration, finite-difference approximations, convergence testing, and numerical analysis of oscillatory signals.

## Project Status

**In development.**

The numerical implementation, results, and documentation will be added as the project progresses.

## Authors
M.O
