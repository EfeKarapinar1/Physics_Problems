# Kinematics: Elimination of Time and Acceleration Analysis

This document provides a step-by-step solution for finding the trajectory and kinematic properties of a particle defined by parametric equations.

---

## 1. Necessary Definitions and Formulas

Before solving, we define the fundamental kinematic relationships for a particle moving in a 2D plane:

* **Position Vector:** Represented as $\vec{r}(t) = [x(t), y(t)]$.
* **Velocity Vector ($\vec{v}$):** The first derivative of position with respect to time.

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = \left[ \frac{dx}{dt}, \frac{dy}{dt} \right]
$$

* **Acceleration Vector ($\vec{a}$):** The second derivative of position (or first derivative of velocity) with respect to time.

$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = \left[ \frac{dv_x}{dt}, \frac{dv_y}{dt} \right]
$$

* **Vector Magnitude:** The length of a vector is calculated using the Pythagorean theorem:

$$
|\vec{A}| = \sqrt{A_x^2 + A_y^2}
$$

---

## 2. Problem Solution

Given the parametric equations:

$$
x(t) = 2t^2, \quad y(t) = 3t^3
$$

### A. Eliminate the parameter $t$

To find the path equation $y(x)$, we express $t$ in terms of $x$ and substitute it into the $y$ equation.

1. From the $x$ equation, we solve for $t^2$:

$$
t^2 = \frac{x}{2}
$$

2. Taking the square root (assuming $t \ge 0$ for standard motion):

$$
t = \sqrt{\frac{x}{2}}
$$

3. Substitute these into the $y(t)$ equation, noting that $t^3 = (t^2)^{3/2}$:

$$
y = 3(t^2)^{3/2}
$$

**Final Path Equation:**

$$
y = 3 \left( \frac{x}{2} \right)^{3/2} = \frac{3}{2\sqrt{2}} x^{3/2}
$$

This curve is a **semi-cubical parabola**.

---

### B. Calculate Velocity $\vec{v}(t)$ and Magnitude $|\vec{v}(t)|$

Differentiating the position components with respect to time $t$:

* $v_x(t) = \frac{d}{dt}(2t^2) = 4t$
* $v_y(t) = \frac{d}{dt}(3t^3) = 9t^2$

**Velocity Vector:**

$$
\vec{v}(t) = \begin{bmatrix} 4t \\ 9t^2 \end{bmatrix}
$$

**Magnitude of Velocity (Speed):**

$$
|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2} = \sqrt{16t^2 + 81t^4} = t \sqrt{16 + 81t^2}
$$

---

### C. Calculate Acceleration $\vec{a}(t)$ and Magnitude $|\vec{a}(t)|$

Differentiating the velocity components with respect to time $t$:

* $a_x(t) = \frac{d}{dt}(4t) = 4$
* $a_y(t) = \frac{d}{dt}(9t^2) = 18t$

**Acceleration Vector:**

$$
\vec{a}(t) = \begin{bmatrix} 4 \\ 18t \end{bmatrix}
$$

**Magnitude of Acceleration:**

$$
|\vec{a}(t)| = \sqrt{4^2 + (18t)^2} = \sqrt{16 + 324t^2} = 2\sqrt{4 + 81t^2}
$$

---

### D. Is the acceleration constant?

**No, the acceleration is not constant.**

A vector is constant only if both its magnitude and direction do not change. 
* **Magnitude:** $|\vec{a}(t)|$ is a function of time; it increases as $t$ increases.
* **Direction:** The $x$-component is constant, but the $y$-component grows. This means the vector changes its angle over time.
