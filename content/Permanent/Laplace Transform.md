---
publish: true
aliases: laplace transform transform
created: 2026-01-22
modified: 2026-01-30T21:55:35.064+05:45
tags:
  - math/calc/de
cssclasses: ""
---

==[[2026-01-22]]==
# Laplace Transform
The Laplace transform of a function $f(t)$ is:
$$
\mathcal{L}\left\{ f(t) \right\} = F(s) = \int_{0}^{\infty}f(t)e^{-st}dt
$$
where, $t\geq{0}$, $s \in \mathbb{C}$.
## Laplace Inverse Theorem
$$
\mathcal{L}\left\{ f(t) \right\} = F(s) \iff \mathcal{L}^{-1}\left\{ F(s) \right\} =f(t)
$$
## Some Laplace Transformations
| $$f(t)$$     | $$F(s) = \mathcal{L}\{f(t)\}$$ | $$f(t)$$                    | $$F(s) = \mathcal{L}\{f(t)\}$$ | $$f(t)$$         | $$F(s) = \mathcal{L}\{f(t)\}$$ |
| ------------ | ------------------------------ | --------------------------- | ------------------------------ | ---------------- | ------------------------------ |
| $$1$$        | $$\dfrac{1}{s}$$               | $$t^n,\; n \in \mathbb{N}$$ | $$\dfrac{n!}{s^{n+1}}$$        | $$\sin(at)$$     | $$\frac{a}{s^{2}+a^{2}}$$      |
| $$t$$        | $$\dfrac{1}{s^2}$$             | $$e^{at}$$                  | $$\dfrac{1}{s-a}$$             | $$\cos(at)$$<br> | $$\frac{s}{s^{2}+a^{2}}$$      |
| $$\sin(at)$$ | $$\dfrac{a}{s^2 + a^2}$$       | $\sinh(at)$                 | $$\frac{a}{s^{2}-a^{2}}$$<br>  | $\cosh(at)$      | $$\frac{s}{s^{2}-a^{2}}$$      |
|              |                                |                             |                                |                  |                                |

## s-shifting theorem
$$
\mathcal{L}\left\{ e^{at}f(t) \right\} = F(s-a)
$$
## Powers in t theorem
$$
\mathcal{L}\left\{ t^{n}f(t) \right\} = (-1)^{n} \frac{d^{n}}{dt^{n}}F(s)
$$
## t-shifting theorem

### Unit Step Function
1. $$
u_{c}(t) =
\begin{cases}
0, & t < c \\
1, & t \geq c
\end{cases}
$$

2. $$
\mathcal{L}\left\{ u_{c}(t) \right\} = \frac{e^{-cs}}{s}
$$

### Theorem (t-shifting or second shifting theorem)
**If** $\mathcal{L}\{f(t)\} = F(s)$, **then** for $c > 0$,
$$
\mathcal{L}\left\{ f(t - c)u_{c}(t) \right\} = e^{-cs}F(s)
$$
**provided that** $f(t)$ is piece-wise continuous on every finite interval $[0, \infty)$.

### Laplace Transform of Derivatives
Let $\mathcal{L}\left\{ y(t) \right\}=Y(s)$
$$
\mathcal{L}\left\{ y' \right\} = sY(s)-y(0)
$$
$$
\mathcal{L}\left\{ y'' \right\} = s^{2}Y(s)-sy(0)-y'(0)
$$
