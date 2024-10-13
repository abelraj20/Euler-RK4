This repository contains Python implementations and visualisations of numerical solutions to ordinary differential equations (ODEs) using the Euler and fourth order of
Runge-Kutta (RK4) method. The solutions include time-dependent graphs and phase-space plots for various physical models. The repository also demonstrates the accuracy and 
convergence of these methods for different initial conditions, step sizes, and equation parameters.

Euler Method: A first-order numerical method used to approximate solutions by updating the solution incrementally based on the slope at the current point.

RK4: A higher-order numerical method that provides more accurate solutions by taking weighted averages of slopes at intermediate steps.


Euler Method Visualisations:

Program E1 - Radioactive decay was simulated using the Euler method with a time step of 0.1, a maximum time of 10, and a decay constant of 2. The initial quantity was set to 
10 at t = 0, and the Euler formula was applied to update the values of N and time. A plot of N(t) against time was produced to observe the decay process. 

Program E2 - Solved the nonlinear differential equation dx/dt = t - x² using the Euler method, with an initial condition of x₀ = 1, a time step h = 0.05, and a maximum time 
of 9. Different initial values of x₀ were tested, and the behaviour of the system was observed over time, with graphs of x(t) plotted to examine the solutions. 

Program E3 - Focused on solving a system of coupled first-order differential equations, dx/dt = y and dy/dt = -x, to model the motion of a harmonic oscillator using the Euler 
method. Initial conditions of x₀ = 0 and v₀ = 1 were set, and the time step h was varied to explore the accuracy of the solution. Numerical solutions were compared to the 
exact solution x = sin(t), with graphs illustrating the solution behaviour for different step sizes.

Program E4 - The improved Euler method was applied to the harmonic oscillator problem with the same initial conditions as in Program E3. Solutions obtained from both the 
simple and improved Euler methods were compared, with the exact solution plotted alongside the numerical results to assess accuracy improvements.

RK4 Method Visualisations:

Program R1 - Solved the nonlinear differential equation dy/dt = −ay³ + sin(bt) using the SciPy function solve_ivp based on the RK45 method. The function was defined to 
calculate dy/dt, and the main function set up initial conditions (y₀ = 0) and solved the equation over time (t₀ = 0 to tf = 20) with various parameter pairs (a=1, b=1; 
a=2, b=1; a=2, b=2; a=3, b=3). The time evolution of the solution for each parameter set was plotted, with labeled axes and a legend.

Subsequent programs (R2 to R8) built upon this by expanding and modifying the R1 template to explore different setups such as ODEs, circuits, simple harmonic oscillators,
damped harmonic oscillators, driven oscillators and resonance patterns.
