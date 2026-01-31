---
publish: true
title: First-Order Numerical Technique
created: 2026-01-30
modified: 2026-02-01T03:25:32.619+05:45
cssclasses: ""
---

==On [[Private/Daily/2026-01-30]] at 22:53==

---
[[Permanent/First-Order Numerical Technique]] are the [[Numerical Methods\|numerical techniques]] that only use information from the [[Gradient of a Function]] or the first [[Permanent/Derivative of a Function]] to solve the problem i.e [[Optimization Problem]] or [[Permanent/Euler's Method\|approximating solutions for an ODE]].

# General Process
The general process involves iteratively using $\text{New Value} = \text{Old Value} + \text{Step}*\text{(Gradient at Old Value Point)}$

# Examples
- Solving [[Permanent/Ordinary Differential Equation\|ODE]]
	- [[Permanent/Euler's Method]]
- [[Optimization Problem]]
	- [[Backpropagation Algorithm]]

# Global Error
The global error of the estimate is proportional to $h$ the step.

---
# Footnotes
---