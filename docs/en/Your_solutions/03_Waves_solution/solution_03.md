# Physics Problem: Superposition and Standing Waves

## Problem

Two waves are described by the equations $y_1(x, t) = A \sin(kx - \omega t)$ and $y_2(x, t) = A \sin(kx + \omega t)$. What is the equation of the resulting standing wave? Identify the positions of the nodes.

## 1. Key Definitions and Formulas

Before solving the problem, it is essential to understand the underlying physical principles and the mathematical tools required.

### Definitions
* **Superposition Principle:** When two or more waves overlap in space, the resulting displacement at any point is the algebraic sum of the displacements of the individual waves.
* **Standing Wave:** A wave pattern that remains in a constant position. It is formed by the interference of two waves of the same frequency and amplitude traveling in opposite directions.
* **Nodes:** Specific points along a standing wave where the displacement is always zero due to destructive interference.
* **Antinodes:** Points where the displacement reaches its maximum value due to constructive interference.

### Necessary Formulas
1.  **Wave Equation:** $y(x, t) = A \sin(kx \pm \omega t)$
2.  **Trigonometric Sum Identity:** 

$$
\sin(\alpha) + \sin(\beta) = 2 \sin\left(\frac{\alpha + \beta}{2}\right) \cos\left(\frac{\alpha - \beta}{2}\right)
$$
    
3.  **Wave Number ($k$):**

$$
k = \frac{2\pi}{\lambda}
$$

---

## 2. Step-by-Step Solution

### Problem Statement
Given two waves:
1. $y_1(x, t) = A \sin(kx - \omega t)$ (Traveling in the $+x$ direction)
2. $y_2(x, t) = A \sin(kx + \omega t)$ (Traveling in the $-x$ direction)

Find the resulting standing wave equation and identify the positions of the nodes.

### Step 1: Apply the Superposition Principle
The resulting displacement $y(x, t)$ is the sum of the two individual wave functions:

$$
y(x, t) = y_1(x, t) + y_2(x, t)
$$

Substituting the given equations:

$$
y(x, t) = A \sin(kx - \omega t) + A \sin(kx + \omega t)
$$

### Step 2: Use Trigonometric Identities
To simplify the expression, we factor out the amplitude $A$ and apply the sum-to-product identity:
Let $\alpha = kx - \omega t$ and $\beta = kx + \omega t$.

$$
y(x, t) = A \left[ 2 \sin\left(\frac{(kx - \omega t) + (kx + \omega t)}{2}\right) \cos\left(\frac{(kx - \omega t) - (kx + \omega t)}{2}\right) \right]
$$

### Step 3: Simplify the Terms
* **Sine argument:** $\frac{kx - \omega t + kx + \omega t}{2} = \frac{2kx}{2} = kx$
* **Cosine argument:** $\frac{kx - \omega t - kx - \omega t}{2} = \frac{-2\omega t}{2} = -\omega t$

Now we have:

$$
y(x, t) = 2A \sin(kx) \cos(-\omega t)
$$

Since the cosine function is even, $\cos(-u) = \cos(u)$, the final **standing wave equation** is:

$$
y(x, t) = [2A \sin(kx)] \cos(\omega t)
$$

> **Note:** The term in the brackets, $2A \sin(kx)$, represents the position-dependent amplitude of the standing wave.

### Step 4: Identify the Positions of the Nodes
Nodes occur where the displacement is zero at all times. This happens when the spatial part of the equation equals zero:

$$
\sin(kx) = 0
$$

The sine function is zero when its argument is an integer multiple of $\pi$:

$$
kx = n\pi \quad \text{where } n = 0, \pm 1, \pm 2, \dots
$$

Substitute $k = \frac{2\pi}{\lambda}$ to find the positions in terms of wavelength:

$$
\left(\frac{2\pi}{\lambda}\right)x = n\pi
$$

Solving for $x$:

$$
x = \frac{n\lambda}{2}
$$

### Final Result
* **Standing Wave Equation:** $y(x, t) = 2A \sin(kx) \cos(\omega t)$
* **Positions of Nodes:** $x = 0, \frac{\lambda}{2}, \lambda, \frac{3\lambda}{2}, \dots$ (every half-wavelength).
