---
publish: true
title: First-Order Numerical Technique
created: 2026-01-30
modified: 2026-01-30T23:44:44.262+05:45
cssclasses: ""
---

==On [[Private/Daily/2026-01-30]] at 22:53==

---
[[Fleeting/First-Order Numerical Technique]] are the [[Numerical Methods\|numerical techniques]] that only use information from the [[Gradient of a Function]] or the first [[Fleeting/Derivative of a Function]] to solve the problem i.e [[Optimization Problem]] or [[Permanent/Euler's Method\|approximating solutions for an ODE]].

# General Process
The general process involves iteratively using $\text{New Value} = \text{Old Value} + \text{Step}*\text{(Gradient at Old Value Point)}$
until difference between New Value and Old Value is not significant.

# Examples
- Solving [[Fleeting/Ordinary Differential Equation\|ODE]]
	- [[Permanent/Euler's Method]]
- [[Optimization Problem]]
	- [[Backpropagation Algorithm]]

# Global Error
The global error of the estimate is proportional to $h$ the step.

---
# Footnotes
---