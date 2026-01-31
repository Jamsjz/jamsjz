---
publish: true
title: Euler's Method
created: 2026-01-30
modified: 2026-01-31T09:54:29.761+05:45
tags:
  - math/calc/de
  - cs/NM
cssclasses: ""
---

==On [[Private/Daily/2026-01-30]] at 22:36==
[Euler's Method Visualizer](https://www.geogebra.org/m/NUeFjm9J)

---
**Euler's Method** is a [[Fleeting/First-Order Numerical Technique\|first-order]] [[Numerical Methods\|numerical method]] used to approximate solutions to a [[Fleeting/Ordinary Differential Equation\|ODE]] with a given set of [[Initial Conditions to a Differential Equations\|initial conditions]].

---
# The Method
For an [[Initial Value Problem\|IVP]] $x' = f(x,t), x(t_{o})=x_{o}$, the method gives the approximate solution values at discrete points such that:
$$
\begin{align}
x_{n+1} &= x_{n} + h*f(x_{n},t_{n}) \\
t_{n+1} &= t_{n} + h
\end{align}
$$
where, 
- $n$ iteratively goes from $0 \to \infty$ as whole numbers
- $h$ is the step which is a [[Hyperparameter Tuning\|hyperparameter]]

---
Initially,
$$
x_{1} = x_{o}+h*f(x_{o}, t_{o})
$$
and process is repeated with increasing $n$ until our desired number of data points are observed.

---
Plotting all the data points gives us our approximation for the solution of the differential equation for the given [[Initial Conditions to a Differential Equations\|initial conditions]].

---
> [!example] Example: ${} x' = x + t, x(0)=1$
> The solution of the [[Fleeting/Ordinary Differential Equation\|ODE]] is:
> $$
> x(t) = 2e^{t}-t-1
> $$
> Visualizing the process of Euler's Method,
> ![[Assets/Euler's Method.mp4]]

---
# Footnotes
---
