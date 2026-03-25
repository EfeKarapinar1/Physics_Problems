# Projectile Motion: Range Optimization

This document provides an analytical proof to determine the optimal launch angle for maximum horizontal range in a vacuum (neglecting air resistance).

## 1. Key Definitions and Formulas

To solve this problem, we must understand the components of motion and the governing equation for range.

* **Initial Velocity ($v_0$):** The starting speed of the projectile at $t = 0$.
* **Launch Angle ($\theta$):** The angle at which the projectile is launched relative to the horizontal plane.
* **Gravitational Acceleration ($g$):** The constant downward acceleration (approx. $9.81 \, \text{m/s}^2$ on Earth).
* **Range ($R$):** The total horizontal distance traveled by the projectile before returning to its initial vertical height.

### The Range Equation
The horizontal range of a projectile, assuming it starts and ends at the same height, is given by:

$$
R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}
$$

### Trigonometric Identity
The derivation relies on the double-angle identity:

$$
\sin(2\theta) = 2 \sin(\theta) \cos(\theta)
$$

---

## 2. Step-by-Step Analytical Proof

To find the maximum value of a function $R(\theta)$, we find the derivative with respect to $\theta$, set it to zero (to find critical points), and verify the nature of the point.

### Step 1: Differentiate the Range Equation
We treat $v_0$ and $g$ as constants. We differentiate $R$ with respect to $\theta$ using the chain rule on the $\sin(2\theta)$ term.

$$
\frac{dR}{d\theta} = \frac{d}{d\theta} \left[ \frac{v_0^2 \sin(2\theta)}{g} \right]
$$

$$
\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \cos(2\theta) \cdot 2
$$

$$
\frac{dR}{d\theta} = \frac{2v_0^2 \cos(2\theta)}{g}
$$

### Step 2: Set the Derivative to Zero
To find the extremum (maximum or minimum), we set the first derivative to zero. Since $v_0$ and $g$ are non-zero, the trigonometric term must be the one that equals zero.

$$
\frac{2v_0^2 \cos(2\theta)}{g} = 0
$$

$$
\cos(2\theta) = 0
$$

### Step 3: Solve for $\theta$
We know that the cosine function equals zero when its argument is $90^\circ$ (or $\pi/2$ radians).

$$
2\theta = 90^\circ
$$

$$
\theta = 45^\circ
$$

### Step 4: Verification (Second Derivative Test)
To ensure this is a maximum, we look at the second derivative:

$$
\frac{d^2R}{d\theta^2} = -\frac{4v_0^2 \sin(2\theta)}{g}
$$

At $\theta = 45^\circ$:

$$
\frac{d^2R}{d\theta^2} = -\frac{4v_0^2 \sin(90^\circ)}{g} = -\frac{4v_0^2}{g}
$$

Since the second derivative is **negative**, the function is concave down at this point, confirming that $\theta = 45^\circ$ is indeed a **maximum**.

## 3. Conclusion
Analytically, the maximum horizontal range for any given initial velocity $v_0$ is achieved when the projectile is launched at an angle of **$45^\circ$**. At this angle, the term $\sin(2\theta)$ reaches its maximum value of $1$.
