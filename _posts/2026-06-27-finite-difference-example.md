---
layout: post
title: "A Simple Finite-Difference Example"
date: 2026-06-27 12:00:00 +0800
categories:
  - Physics
  - Numerical Methods
tags:
  - finite-difference
  - python
  - schrodinger-equation
---

The finite-difference method replaces derivatives with differences between nearby grid points. For example, the second derivative of a function can be approximated by

$$
\frac{d^2\psi}{dx^2}\bigg|_{x_i}
\approx
\frac{\psi_{i+1}-2\psi_i+\psi_{i-1}}{(\Delta x)^2}.
$$

This approximation lets us represent the one-dimensional kinetic-energy operator as a matrix:

```python
import numpy as np

n = 100
x = np.linspace(-5.0, 5.0, n)
dx = x[1] - x[0]

diagonal = -2.0 * np.ones(n)
off_diagonal = np.ones(n - 1)

laplacian = (
    np.diag(diagonal)
    + np.diag(off_diagonal, 1)
    + np.diag(off_diagonal, -1)
) / dx**2
```

From here, we can add a potential-energy matrix and diagonalize the resulting Hamiltonian. This basic construction is the starting point for many numerical quantum-mechanics calculations.
