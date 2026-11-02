# Numerical simulation of two coupled oscillators

**Introduction to Numerical Algorithms — final project proposal**  
**Student:** Mohamed OUKLILENE (T2; individual project subject to instructor approval)

## Aim

Compare two numerical methods for solving the motion of two masses joined by
springs. The normal-mode solution provides a reference, so we can measure the
error of each method rather than judging the plots by eye.

## Model

For displacements \(x_1,x_2\), masses \(m_1,m_2\), and spring constants
\(k_1,k_2,k_3\),

\[
m_1\ddot x_1=-(k_1+k_2)x_1+k_2x_2,\qquad
m_2\ddot x_2=k_2x_1-(k_2+k_3)x_2.
\]

We will use \(m_1=m_2=1\), \(k_1=k_3=1\), \(k_2=2\), with initial
displacements \((0,0.4)\) and velocities \((1,0)\). Other parameters can be
explored after the basic comparison works.

## Numerical methods

1. Convert the equations to a first-order system for
   \((x_1,x_2,v_1,v_2)\).
2. Implement the explicit Euler method and the fourth-order Runge–Kutta
   method (RK4) in Python.
3. Find the normal frequencies and modes from the matrix eigenvalue problem
   \(K\eta=\omega^2 M\eta\). Use their analytic time dependence as a reference.

## Comparison and expected results

- Plot both masses' displacement against time for the numerical and
  normal-mode solutions.
- Repeat with several time steps. Plot the maximum displacement error against
  step size on logarithmic axes and check the expected first- and fourth-order
  trends.
- Plot the total energy
  \(E=\tfrac12m_1v_1^2+\tfrac12m_2v_2^2+
  \tfrac12k_1x_1^2+\tfrac12k_2(x_2-x_1)^2+\tfrac12k_3x_2^2\)
  to compare numerical energy drift.
- Explain when a method is sufficiently accurate and how its step size affects
  the result.

## Planned deliverables

The finished repository will contain the Python implementation, reproducible
plots, and a short discussion of numerical error and limitations. This README
records the topic and plan for the initial project selection.
