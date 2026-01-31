---
publish: true
created: 2026-01-10
modified: 2026-01-30T22:06:45.594+05:45
tags:
  - math/stats/inference
cssclasses: ""
---

==[[2026-01-10]]==
# Sampling Distribution
1. Take every possible sample of size $n$
2. Take [[Sample Statistics]] of each sample.
3. The distribution of the sample statistics is sampling distribution

## Finite Population Correction
[[Finite Population Correction\|FPC]] is a factor you multiply to remove the bias.
$$
FPC = \sqrt{ \frac{N-n}{N-1} }
$$
> [!note] FPC is used when the population is finite i.e $N$ is given.
## [[Sampling Distribution of Sample Mean]]
* [[Standard Error]]
$$
S.E = \frac{\sigma}{\sqrt{ n }}
$$
* Z-value
$$
Z = \frac{\bar{X}-\mu}{SE}
$$
## [[Sampling Distribution of Sample Proportion]]
* Standard Error
$$
S.E = \sqrt{ \frac{PQ}{n} }
$$
* Z-value
$$
Z = \frac{p-P}{SE}
$$
## [[Confidence Interval]], [[Confidence Level]] and [[Significance Level]]
$$
1-\alpha = P[\bar{X}-a<\mu<\bar{X}+b], \quad a,b >0
$$
$$
\text{Confidence Interval} = (\bar{X}-a,\bar{X}+b)
$$
$$
\text{Confidence Level} = 1-\alpha
$$
$$
\text{Significance Level} = \alpha
$$
## [[Maximum Error]]
$$
1-\alpha = P[\bar{X}-E<\mu<\bar{X}+E]
$$
$$
E = |Z_{\alpha / 2}|*S.E
$$

## [[Population Standard Deviation]] Unknown
Use [[Sample Standard Deviation]] as an estimator for $\sigma$
i.e $\sigma = s$

> [!important] For Difference $\mu_{1}-\mu_{2}$ when $\sigma$ is known,
> $$
> SE = \sqrt{ \frac{\sigma_{1}^{2}}{n_{1}}+\frac{\sigma_{2}^{2}}{n_{2}} }
> $$

> [!important] For difference $\mu_{1}-\mu_{2}$
> $$
> SE = s_{p} \sqrt{ \frac{1}{n_{1}}+\frac{1}{n_{2}} }
> $$
where,
>
> $$
> s_{p}^{2} = \frac{(n_{1}-1)s_{1}^{2}+(n_{2}-1)s_{2}^{2}}{n_{1}+n_{2}-2}
> $$

> [!important] For difference $P_{1}-P_{2}$
> $$
> S.E. = \sqrt{ \frac{p_{1}q_{1}}{n_{1}}+\frac{p_{2}q_{2}}{n_{2}} }
> $$
## Condition for Using [[t-Test]]
To use the t-table, Both the condition should be fullfilled.
1. $n<30$
2. $\sigma$ is unknown

## [[Degrees of Freedom]]
$\nu = n-1$
$\nu = n_{1}+n_{2}-2$

## [[F-Test]]
Two samples:

$$
F_{\text{obs}} = \frac{s_{1}^{2}}{s_{2}^{2}}
$$
## [[Chi-Square Test]]
Test Statistics
$$
\chi^{2} = \frac{(n-1)s^{2}}{\sigma_{o}^{2}}
$$
### [[Goodness of Fit]]
Test Statistics
$$
\chi^{2} = \sum_{j=1}^{k} \frac{(O_{j}-E_{j})^{2}}{E_{j}}
$$
where,
$E_{j} = np_{j}$

For degrees of freedom,
$\nu=k-1-m$ where m are parameters estimated from the data.
### [[Independence Test]]
Test Statistics
For a table $R\times C$
$$
\chi^{2} = \sum_{i=1}^{R} \sum_{j=1}^{C} \frac{(O_{ij}-E_{ij})^{2}}{E_{ij}}
$$
where,
$$
E_{ij} = \frac{\text{Row i total} \times \text{Column j total}}{\text{Grand Total}}
$$
For [[Degrees of Freedom]],
$\nu = (R-1)(C-1)$
## Tables
### Z-table
![[Assets/Z-table.png]]
### t-table
![[Assets/t-table.png]]
### F-table
![[Assets/F-test.png]]
### $\chi^{2}$-table
![[Assets/Chi-square-Table.png]]