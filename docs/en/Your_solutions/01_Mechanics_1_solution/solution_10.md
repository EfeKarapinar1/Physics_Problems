# Kinematics: Analysis of 3D Particle Motion

This document provides a detailed solution to the motion of a point $M$ defined by a time-dependent position vector.

## 1. Necessary Definitions and Formulas

Before solving the problem, we define the fundamental kinematic quantities for motion in three-dimensional space.

### Position Vector
The position of a point in space is given by:

$$
\vec{r}(t) = x(t)\hat{i} + y(t)\hat{j} + z(t)\hat{k}
$$

### Velocity Vector
Velocity is the derivative of the position vector with respect to time $t$:

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = \left( \frac{dx}{dt}, \frac{dy}{dt}, \frac{dz}{dt} \right)
$$

### Speed (Scalar Velocity)
The magnitude of the velocity vector represents the instantaneous speed:

$$
v = |\vec{v}(t)| = \sqrt{\dot{x}^2 + \dot{y}^2 + \dot{z}^2}
$$

### Path Length
The total distance $s$ traveled along the curve from $t=0$ to $t=t_0$ is the integral of speed:

$$
s = \int_{0}^{t_0} |\vec{v}(t)| dt
$$

---

## 2. Problem Statement

Point $M$ moves according to the equation:

$$
\vec{r}(t) = (a \cos(\omega t), b \sin(\omega t), bt)
$$

where $a, b, \omega$ are positive constants.

---

## 3. Step-by-Step Solution

### a) Equation of the Trajectory

To find the trajectory, we eliminate the time parameter $t$ from the coordinate equations:
1. $x = a \cos(\omega t) \implies \frac{x}{a} = \cos(\omega t)$
2. $y = b \sin(\omega t) \implies \frac{y}{b} = \sin(\omega t)$
3. $z = bt \implies t = \frac{z}{b}$

Using the trigonometric identity $\cos^2(\theta) + \sin^2(\theta) = 1$, we combine the $x$ and $y$ equations:

$$
\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = 1
$$

This equation describes an **elliptical cylinder**. Since $z$ increases linearly with $t$ ($z = bt$), the point moves upward while orbiting the $z$-axis. The resulting trajectory is an **elliptical helix**.

### b) Path Length from $t=0$ to $t=t_0$

First, we find the velocity components by differentiating the position vector:

$$
\dot{x} = -a \omega \sin(\omega t)
$$

$$
\dot{y} = b \omega \cos(\omega t)
$$

$$
\dot{z} = b
$$

Next, we calculate the magnitude of the velocity (speed):

$$
v = \sqrt{(-a \omega \sin(\omega t))^2 + (b \omega \cos(\omega t))^2 + b^2}
$$

$$
v = \sqrt{a^2 \omega^2 \sin^2(\omega t) + b^2 \omega^2 \cos^2(\omega t) + b^2}
$$

The path length $s$ is:

$$
s = \int_{0}^{t_0} \sqrt{a^2 \omega^2 \sin^2(\omega t) + b^2 \omega^2 \cos^2(\omega t) + b^2} dt
$$

> **Note on the General Case:** If $a \neq b$, this integral is an **Elliptic Integral of the second kind**, which does not have a solution in elementary functions.
>
> **Special Case ($a = b$):** If the base is a circle, the speed simplifies to:
>
> $$
> v = \sqrt{a^2 \omega^2 (1) + a^2} = a\sqrt{\omega^2 + 1}
> $$
>
> The path length is then:
>
> $$
> s = a t_0 \sqrt{\omega^2 + 1}
> $$

---

## 4. Visualization (Python Implementation)

You can use the following Python script to visualize the elliptical helix trajectory.

```python
import numpy as np
import matplotlib.pyplot as plt

# Parameters
a, b, omega = 5, 3, 0.5
t0 = 20
t = np.linspace(0, t0, 1000)

# Coordinates
x = a * np.cos(omega * t)
y = b * np.sin(omega * t)
z = b * t

# Create 3D Plot
fig = plt.figure(figsize=(10, 8))
ax = fig.add_subplot(111, projection='3d')
ax.plot(x, y, z, 'b-', label='Elliptical Helix')

ax.set_xlabel('X axis')
ax.set_ylabel('Y axis')
ax.set_zlabel('Z axis')
ax.set_title(f'Trajectory of Point M (a={a}, b={b}, ω={omega})')
ax.legend()

plt.show()
```

# https://colab.research.google.com/drive/1HiVjOui6GNPSjcEUc-p5C0uotx17hwaA
