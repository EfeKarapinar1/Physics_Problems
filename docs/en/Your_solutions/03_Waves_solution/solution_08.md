# Solution: Identifying Traveling Waves

## Problem

Which of the following functions can describe a traveling wave? Hint: check if it satisfies the wave equation 

$$\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}$$

a) $y(x,t) = A \cos(kx^2 - \omega t)$

b) $y(x,t) = A(x-vt)^2$

c) $y(x,t) = A \log(x+vt)$

## 1. Necessary Definitions and Formulas

### The Linear Wave Equation
A function $y(x,t)$ represents a traveling wave if it satisfies the one-dimensional linear wave equation:

$$
\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}
$$

Where:
- $y$ is the displacement.
- $x$ is the position.
- $t$ is the time.
- $v$ is the constant wave speed.

### General Form of a Traveling Wave
Any differentiable function of the form $y(x,t) = f(x \pm vt)$ is a solution to the wave equation. This represents a wave shape $f$ traveling in the negative ($+$) or positive ($-$) x-direction with a constant velocity $v$.



---

## 2. Step-by-Step Solution

We will test each function by calculating its second-order partial derivatives with respect to $x$ and $t$.

### Case a) $y(x,t) = A \cos(kx^2 - \omega t)$

**Step 1: Calculate the second derivative with respect to $x$.**
First derivative:

$$
\frac{\partial y}{\partial x} = -A \sin(kx^2 - \omega t) \cdot (2kx) = -2Akx \sin(kx^2 - \omega t)
$$

Second derivative (using the product rule):

$$
\frac{\partial^2 y}{\partial x^2} = -2Ak \sin(kx^2 - \omega t) - 4Ak^2x^2 \cos(kx^2 - \omega t)
$$

**Step 2: Calculate the second derivative with respect to $t$.**
First derivative:

$$
\frac{\partial y}{\partial t} = -A \sin(kx^2 - \omega t) \cdot (-\omega) = A\omega \sin(kx^2 - \omega t)
$$

Second derivative:

$$
\frac{\partial^2 y}{\partial t^2} = -A\omega^2 \cos(kx^2 - \omega t)
$$

**Step 3: Comparison.**
The ratio of $\frac{\partial^2 y}{\partial x^2}$ to $\frac{\partial^2 y}{\partial t^2}$ is not a constant ($1/v^2$); it depends on $x$ and $t$. 
**Conclusion:** Function (a) **cannot** describe a standard traveling wave.

---

### Case b) $y(x,t) = A(x-vt)^2$

This function is of the form $f(x-vt)$ where $f(u) = Au^2$. Let's verify it via the wave equation.

**Step 1: Calculate $\frac{\partial^2 y}{\partial x^2}$.**

$$
\frac{\partial y}{\partial x} = 2A(x-vt)
$$

$$
\frac{\partial^2 y}{\partial x^2} = 2A
$$

**Step 2: Calculate $\frac{\partial^2 y}{\partial t^2}$.**

$$
\frac{\partial y}{\partial t} = 2A(x-vt) \cdot (-v) = -2Av(x-vt)
$$

$$
\frac{\partial^2 y}{\partial t^2} = (-2Av) \cdot (-v) = 2Av^2
$$

**Step 3: Comparison.**
Substitute into the wave equation:

$$
\frac{1}{v^2} \frac{\partial^2 y}{\partial t^2} = \frac{1}{v^2} (2Av^2) = 2A
$$

Since $2A = 2A$, the equation is satisfied.
**Conclusion:** Function (b) **can** describe a traveling wave.

---

### Case c) $y(x,t) = A \log(x+vt)$

This is of the form $f(x+vt)$ where $f(u) = A \log(u)$.

**Step 1: Calculate $\frac{\partial^2 y}{\partial x^2}$.**

$$
\frac{\partial y}{\partial x} = \frac{A}{x+vt}
$$

$$
\frac{\partial^2 y}{\partial x^2} = -\frac{A}{(x+vt)^2}
$$

**Step 2: Calculate $\frac{\partial^2 y}{\partial t^2}$.**

$$
\frac{\partial y}{\partial t} = \frac{A \cdot v}{x+vt}
$$

$$
\frac{\partial^2 y}{\partial t^2} = -\frac{Av^2}{(x+vt)^2}
$$

**Step 3: Comparison.**

$$
\frac{1}{v^2} \left( -\frac{Av^2}{(x+vt)^2} \right) = -\frac{A}{(x+vt)^2}
$$

The wave equation is satisfied.
**Conclusion:** Function (c) **can** describe a traveling wave (mathematically), though physically it is only defined for $x+vt > 0$.

---

## Final Result Summary

| Function | Satisfies Wave Equation? | Traveling Wave? |
| :--- | :--- | :--- |
| $A \cos(kx^2 - \omega t)$ | No | No |
| $A(x-vt)^2$ | Yes | **Yes** |
| $A \log(x+vt)$ | Yes | **Yes** |
