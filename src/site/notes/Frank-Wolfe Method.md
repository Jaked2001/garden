---
{"dg-publish":true,"permalink":"/frank-wolfe-method/"}
---

# [[Frank-Wolfe Method\|Frank-Wolfe Method]]

The following problem is given:
$$
\min_{\mathbf{x}} f(\mathbf{x})
$$
subjet to
$$
\mathbf{A} \mathbf{x} = \mathbf{b}, \quad \mathbf{x} \ge 0
$$
from which we get the solution $\mathbf{\hat{x}}$.

where:
- $f(\mathbf{x}): \mathbb{R}^{n}\to \mathbb{R}$
- $\mathbf{A}\in \mathbb{R}^{n}\times \mathbb{R}^{n}$
- $\mathbf{x}\in \mathbb{R}^{n}$
- $\mathbf{b}\in \mathbb{R}^{n}$

The Frank-Wolfe is an iterative method to solve the problem with the following steps

## 0. Find a feasible solution

The first step is to find any feasible solution $\mathbf{x}^{(k)}$. In the first iteration, $k=0$.

This solution has to meet the condition $\mathbf{A} \mathbf{x} = \mathbf{b}, \quad \mathbf{x} \ge 0$

## 1. Define the subproblem

The Frank-Wolfe method works generating a new problem, called a subproblem. This is still an optimization problem but is allegedly easier to solve.

In order to define the new problem, we first need to find the [[Gradient\|Gradient]] of $f(\mathbf{x})$. Then, the subproblem is:
$$
\min_{\mathbf{y}} \boldsymbol{\nabla f}(\mathbf{x}^{(k)})^T \cdot \mathbf{y}
$$
subj to:
$$
\mathbf{A} \mathbf{y} = \mathbf{b}, \quad \mathbf{y} \ge 0
$$
from which we get the value $\mathbf{\hat{y}}$.

### Calculate the descent direction

The, we need to calculate a new vector, called the direction, that will allow us to get the solution for the next step of the algorithm.

$$
\mathbf{d}^{(k)} = \mathbf{\hat{y}} - \mathbf{x}^{(k)}
$$
## 2. Stopping criteria

We need some sort of stopping criteria to know if the solution $\mathbf{x}^{(k)}$ is close enough to the actual solution $\mathbf{\hat{x}}$ of the original problem.

We calculate a relative gap, $r$ as
$$
r = - \frac{\mathbf{\nabla f}(\mathbf{x}^{(k)})^{T} \cdot \mathbf{d}^{(k)} }{\mathbf{\nabla f}(\mathbf{x}^{(k)})^{T} \cdot \mathbf{x}^{(k)}}
$$

We define a relative gap that we find suitable. This is going to be a very small value, $\varepsilon$ ($= 10^{-2}, 10^{-4},...$)

If $r < \varepsilon$ than we stop and accept $\mathbf{x}^{(k)}$ as a solution ($\mathbf{x}^{(k)} \approx \mathbf{\hat{x}}$). Otherwise, we go the next step

## 3. Line search

The new solution will be given by
$$
\mathbf{x}^{(k+1)} = \mathbf{x}^{(k)} + \alpha^* \mathbf{d}^{(k)}
$$
where $\alpha^{*}$ is the solution to the problem:
$$
\min_{0\le\alpha\le 1} h(\alpha ) = \min_{0\le\alpha\le 1} f\left( \mathbf{x}^{(k)} + \alpha \mathbf{d}^{(k)} \right)
$$
This can be solved finding the first derivative of $h(\alpha)$, imposing it equal to 0 and then solving for $\alpha$. This last step is often impossible to do analitically, so we rely on numeric methods to find $\alpha^{*}$ (like: [[Università/Triennale/2° anno/2° Semestre/Analisi Numerica/Appunti/03.2 Il metodo delle Tangenti\|Metodo di Newton]] o [[Università/Triennale/2° anno/2° Semestre/Analisi Numerica/Appunti/03.2 Il metodo delle Tangenti\|Il metodo delle Tangenti]], [[Università/Triennale/2° anno/2° Semestre/Analisi Numerica/Appunti/03.1 Metodo di Bisezione\|Metodo di Bisezione]], [[Università/Triennale/2° anno/2° Semestre/Analisi Numerica/Appunti/03.3 Il metodo delle Secanti\|Il metodo delle Secanti]]).

```ad-note

In the particular case that all elements of $\boldsymbol{\nabla} \mathbf{f} \left( \mathbf{x}^{(k)} \right) \stackrel{\triangle}{=} \mathbf{s}(\mathbf{x}^{(k)})$ are in the form $a+bx$, then $\alpha^{*}$ can be taken equal to
$
\min\{1, \tilde{\alpha } \}
$
where:
$
\tilde{\alpha} = \frac{\sum\limits_{i} s_{i}(x_{i}) \cdot d_{i}^{(k)}}{\sum\limits_{i} b_{i}\cdot \left(d_{i}^{(k)}\right)^{2}}
$


```


## 4. Update

After having found $\alpha^{*}$ is time to update the solution to the next step: $\mathbf{x}^{(k)}$ and repeat the method from step [[Frank-Wolfe Method#0. Find a feasible solution\|#0. Find a feasible solution]]
