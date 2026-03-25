# Projectile Motion Analysis

This document provides a step-by-step derivation and solution for a projectile motion problem.

---

## 1. Key Definitions and Formulas

### Definitions
* **Projectile Motion:** The motion of an object thrown or projected into the air, subject only to the acceleration of gravity.
* **Initial Velocity ($v_0$):** The velocity at which the object is launched.
* **Launch Angle ($\theta$):** The angle relative to the horizontal plane.
* **Trajectory:** The parabolic path followed by the projectile.

### Fundamental Formulas
Given an initial velocity $v_0$ and angle $\theta$, we decompose the velocity into components:

**Velocity Components:**

$$
v_{0x} = v_0 \cos(\theta)
$$

$$
v_{0y} = v_0 \sin(\theta)
$$

**Position Equations (Kinematics):**

$$
x(t) = v_{0x} t
$$

$$
y(t) = v_{0y} t - \frac{1}{2} g t^2
$$

---

## 2. Problem Statement

A projectile is fired from the ground with:
* **Initial Velocity ($v_0$):** $100 \text{ m/s}$
* **Launch Angle ($\theta$):** $37^\circ$
* **Gravity ($g$):** $9.8 \text{ m/s}^2$ (assumed)

### Pre-calculations
Using $\sin(37^\circ) \approx 0.6$ and $\cos(37^\circ) \approx 0.8$:

$$
v_{0x} = 100 \cdot 0.8 = 80 \text{ m/s}
$$

$$
v_{0y} = 100 \cdot 0.6 = 60 \text{ m/s}
$$

---

## 3. Step-by-Step Solution

### Task 1: Derive the Differential Equations of Motion
Using Newton's Second Law ($F = ma$), and neglecting air resistance:

**Horizontal Direction ($x$):**
There is no horizontal force.

$$
m \frac{d^2x}{dt^2} = 0 \implies \frac{d^2x}{dt^2} = 0
$$

**Vertical Direction ($y$):**
The only force is gravity acting downwards.

$$
m \frac{d^2y}{dt^2} = -mg \implies \frac{d^2y}{dt^2} = -g
$$

---

### Task 2: Determine the Time of Flight ($T$)
The projectile returns to the ground when $y(t) = 0$.

$$
v_{0y} T - \frac{1}{2} g T^2 = 0
$$

Solving for $T$ (ignoring $T=0$):

$$
T = \frac{2 v_{0y}}{g}
$$

$$
T = \frac{2 \cdot 60}{9.8} \approx 12.24 \text{ s}
$$

---

### Task 3: Determine the Maximum Height ($H$)
Maximum height occurs when the vertical velocity is zero ($v_y = 0$).

$$
v_y = v_{0y} - gt = 0 \implies t_{peak} = \frac{v_{0y}}{g}
$$

Substituting $t_{peak}$ into the displacement equation:

$$
H = \frac{v_{0y}^2}{2g}
$$

$$
H = \frac{60^2}{2 \cdot 9.8} = \frac{3600}{19.6} \approx 183.67 \text{ m}
$$

---

### Task 4: Determine the Range ($R$)
The range is the horizontal distance traveled during the total time $T$.

$$
R = v_{0x} \cdot T
$$

$$
R = 80 \cdot 12.24 \approx 979.2 \text{ m}
$$

---

## Summary of Results

| Parameter | Symbol | Value |
| :--- | :--- | :--- |
| Time of Flight | $T$ | $12.24 \text{ s}$ |
| Maximum Height | $H$ | $183.67 \text{ m}$ |
| Horizontal Range | $R$ | $979.2 \text{ m}$ |
