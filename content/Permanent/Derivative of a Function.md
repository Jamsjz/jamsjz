---
publish: true
aliases: derivative derivatives
title: Derivative of a Function
description: The slope of the tangent line to a curve measures the instantaneous rate of change of a curve. We can calculate it by finding the limit of the difference quotient or the difference quotient with …
created: "[[2026-01-30]]"
modified: 2026-02-01T03:20:14.329+05:45
tags:
  - "#math/calc/derivative"
cssclasses: ""
---

![alt](https://math.libretexts.org/@api/deki/files/2128/CNX_Calc_Figure_03_01_002.jpeg?revision=1)

Figure: We can calculate the slope of a secant line in either of two ways.
In Figure we see that, as the values of approach , the slopes of the secant lines provide better estimates of the rate of change of the function. Furthermore, the secant lines themselves approach the tangent line to the function at , which represents the [[Limit of a Function\|limit]] of the secant lines.

![This figure consists of three graphs labeled a, b, and c. Figure a shows the Cartesian coordinate plane with 0, a, x2, and x1 marked in order on the x-axis. There is a curve labeled y = f(x) with points marked (a, f(a)), (x2, f(x2)), and (x1, f(x1)). There are three straight lines: the first crosses (a, f(a)) and (x1, f(x1)); the second crosses (a, f(a)) and (x2, f(x2)); and the third only touches (a, f(a)), making it the tangent. At the bottom of the graph, the equation mtan = limx → a (f(x) - f(a))/(x - a) is given. Figure b shows a similar graph, but this time a + h2 and a + h1 are marked on the x-axis instead of x2 and x1. Consequently, the curve labeled y = f(x) passes through (a, f(a)), (a + h2, f(a + h2)), and (a + h1, f(a + h1)) and the straight lines similarly cross the graph as in Figure a. At the bottom of the graph, the equation mtan = limh → 0 (f(a + h) - f(a))/h is given. Figure c shows only the curve labeled y = f(x) and its tangent at point (a, f(a)).](https://math.libretexts.org/@api/deki/files/2129/CNX_Calc_Figure_03_01_003.jpeg?revision=1)

Figure: The secant lines approach the tangent line (shown in green) as the second point approaches the first. In Figure we show the graph of and its tangent line at in a series of tighter intervals about . As the intervals become narrower, the graph of the
function and its tangent line appear to coincide, making the values on the tangent line a good approximation to the values of the function for choices of close to . In fact, the graph of itself appears to be **locally linear**.

![This figure consists of four graphs labeled a, b, c, and d. Figure a shows the graphs of the square root of x and the equation y = (x + 1)/2 with the x-axis going from 0 to 4 and the y-axis going from 0 to 2.5. The graphs of these two functions look very close near 1; there is a box around where these graphs look close. Figure b shows a close up of these same two functions in the area of the box from Figure a, specifically x going from 0 to 2 and y going from 0 to 1.4. Figure c is the same graph as Figure b, but this one has a box from 0 to 1.1 in the x coordinate and 0.8 and 1 on the y coordinate. There is an arrow indicating that this is blown up in Figure d. Figure d shows a very close picture of the box from Figure c, and the two functions appear to be touching for almost the entire length of the graph.](https://math.libretexts.org/@api/deki/files/2130/CNX_Calc_Figure_03_01_008.jpeg?revision=1)

Figure: For values of close to, the graph of and its tangent line appear to coincide.

## The Derivative of a Function at a Point
Let $f$ be a function defined in an open interval $I$ containing the point $x=a$. The **derivative** of the function $f$ at $P_{o}$, denoted by $f'|_{P_{o}}$, is defined by:
$$
f'(a) = \lim_{ h \to 0 } \frac{f(a+h)-f(a)}{h}
$$
where $h>0$ is a small change in the input of the function.