---
publish: true
created: 2026-01-25
modified: 2026-01-30T22:52:38.287+05:45
tags:
  - math/calc/de
cssclasses: ""
---

==[[2026-01-25]]==
# System of [[Linear Differential Equations]]
A system of 2 **linear homogeneous differential equations** can be written as:
$$
\begin{align}
x_{1}'&=a_{11}x_{1}+a_{12}x_{2} \quad \text{(i)}\\
x_{2}'&=a_{21}x_{1}+a_{22}x_{2} \quad \text{(ii)}
\end{align}
$$
which is called **component-wise** notation. The same system can be represented by [[Matrix]] notation:
$$
\vec{x}'=A\vec{x}
$$
Solving this system of [[Permanent/Differential Equation\|D.E]] can be done using two methods.
1. [[Permanent/System of Linear Differential Equations and Solutions#Elimination Method]]
2. [[Permanent/System of Linear Differential Equations and Solutions#Eigenvalue and Eigenvector Method]]

---
## Elimination Method
---
$$
\begin{align}
x_{1}'&=a_{11}x_{1}+a_{12}x_{2} \quad \text{(i)}\\
x_{2}'&=a_{21}x_{1}+a_{22}x_{2} \quad \text{(ii)}
\end{align}
$$
Steps:
1. From Equation (ii), find $x_{1}$ and $x_{1}'$
2. Substitute $x_{1}$ and $x_{1}'$ from Equation (ii) in Equation (i)
3. Solve the 2<sup>nd</sup> order D.E to get solution for $x_{2}$
4. Find $x_{2}'$ from the solution found
5. Substitute $x_{2}$ and $x_{2}'$ in the value of $x_{1}$ derived from Equation (ii) to find $x_{1}$

---
## Eigenvalue and Eigenvector Method
---
$$
\begin{bmatrix}
x_{1}' \\
x_{2}'
\end{bmatrix}=\vec{x}'=A\vec{x} = \begin{bmatrix}
a_{11} & a_{12} \\
a_{21}  & a_{22}
\end{bmatrix} \begin{bmatrix}
x_{1} \\
x_{2}
\end{bmatrix}
$$
Steps: [^1]
1. Find **eigenvalues** of $A$ solving the equation $\det(A-\lambda I)=0$
2. Find **eigenvector** for each $\lambda$ solving the equation $(A-\lambda I)\vec{v}=0$. Here, $\vec{v}$ is **non-trivial** i.e $\vec{v}\neq \vec{0}$
> [!note] 
3. We have, $\vec{x}=\vec{v}e^{\lambda t}$
### Three cases of Eigenvalues
1. Real and Distinct
$$
\vec{x} = c_{1}\vec{v}_{1}e^{\lambda_{1}t}+c_{2}\vec{v}_{2}e^{\lambda_{2}t}
$$
2. Complex and Conjugate
	The corresponding eigenvector for $\lambda=a\pm \iota b$ is $\vec{v}=\vec{u}\pm \iota \vec{w}$
	Then, $e^{\lambda t}\vec{v}=e^{at}(\cos bt+\iota \sin bt)(u+\iota w)$
	And general solution is:
	$$
	\begin{align}
	\vec{x}&=c_{1}\vec{x_{1}}+c_{2}\vec{x_{2}}\\&=c_{1}\mathrm{Re}(e^{\lambda t}\vec{v})+c_{2}\mathrm{Im}(e^{\lambda t}\vec{v})\\&=e^{at}(\vec{u}(c_{1}\cos bt+c_{2}\sin bt)-\vec{w}(c_{1}\sin bt-c_{2}\cos bt))
	\end{align}
	$$
3. Real and Same
- The corresponding eigenvector for $\lambda_{1}=\lambda_{2}=\lambda$ is $\vec{v}_{1}$
- Find **Generalized Eigenvector** by solving $(A-\lambda I)\vec{v}_{2}=\vec{v}_{1}$
Then the **General Solution** is:
$$
\vec{x} = c_{1}\vec{v}_{1}e^{\lambda t}+c_{2}(\vec{v}_{1}t+\vec{v}_{2})e^{\lambda t}
$$
---

# Footnotes
[^1]: https://math.libretexts.org/Bookshelves/Differential_Equations/Differential_Equations_for_Engineers_(Lebl)/3%3A_Systems_of_ODEs/3.4%3A_Eigenvalue_Method

