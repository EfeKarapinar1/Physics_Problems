# Physics Problem: Force Field and Power

## 1. Problem Statement
In a certain force field, the equations of motion of a particle with mass $m=0.5$ kg are as follows:

$$
x = 5t^2 - t, \quad y = 2t^3, \quad z = -3t + 2
$$

Find the time dependence of: the particle's velocity, the particle's momentum, the particle's acceleration, the force acting on the particle, and the power transferred by the field to the particle.

---

## 2. Fundamental Definitions and Formulas

Before solving, we define the physical quantities used:

* **Velocity ($\vec{v}$)**: The time derivative of the position vector.
    
    $$
    \vec{v} = \frac{d\vec{r}}{dt} = \left[ \frac{dx}{dt}, \frac{dy}{dt}, \frac{dz}{dt} \right]
    $$

* **Momentum ($\vec{p}$)**: The product of mass and velocity.
    
    $$
    \vec{p} = m \cdot \vec{v}
    $$

* **Acceleration ($\vec{a}$)**: The time derivative of the velocity vector.
    
    $$
    \vec{a} = \frac{d\vec{v}}{dt} = \left[ \frac{dv_x}{dt}, \frac{dv_y}{dt}, \frac{dv_z}{dt} \right]
    $$

* **Force ($\vec{F}$)**: Defined by Newton's Second Law.
    
    $$
    \vec{F} = m \cdot \vec{a}
    $$

* **Power ($P$)**: The scalar product of force and velocity.
    
    $$
    P = \vec{F} \cdot \vec{v} = F_x v_x + F_y v_y + F_z v_z
    $$

---

## 3. Step-by-Step Solution

**Given:**
* $m = 0.5$ kg
* $x(t) = 5t^2 - t$
* $y(t) = 2t^3$
* $z(t) = -3t + 2$

### Step 1: Particle's Velocity $\vec{v}(t)$
We differentiate each coordinate with respect to time $t$:

$$
v_x = \frac{d}{dt}(5t^2 - t) = 10t - 1
$$

$$
v_y = \frac{d}{dt}(2t^3) = 6t^2
$$

$$
v_z = \frac{d}{dt}(-3t + 2) = -3
$$

**Vector form:**

$$
\vec{v}(t) = [10t - 1, 6t^2, -3] \text{ m/s}
$$

---

### Step 2: Particle's Momentum $\vec{p}(t)$
Using $\vec{p} = m\vec{v}$ where $m = 0.5$:

$$
\vec{p}(t) = 0.5 \cdot [10t - 1, 6t^2, -3]
$$

**Vector form:**

$$
\vec{p}(t) = [5t - 0.5, 3t^2, -1.5] \text{ kg}\cdot\text{m/s}
$$

---

### Step 3: Particle's Acceleration $\vec{a}(t)$
We differentiate the velocity components with respect to time $t$:

$$
a_x = \frac{d}{dt}(10t - 1) = 10
$$

$$
a_y = \frac{d}{dt}(6t^2) = 12t
$$

$$
a_z = \frac{d}{dt}(-3) = 0
$$

**Vector form:**

$$
\vec{a}(t) = [10, 12t, 0] \text{ m/s}^2
$$

---

### Step 4: Force Acting on the Particle $\vec{F}(t)$
Using $\vec{F} = m\vec{a}$ where $m = 0.5$:

$$
\vec{F}(t) = 0.5 \cdot [10, 12t, 0]
$$

**Vector form:**

$$
\vec{F}(t) = [5, 6t, 0] \text{ N}
$$

---

### Step 5: Power Transferred by the Field $P(t)$
We calculate the dot product $P = \vec{F} \cdot \vec{v}$:

$$
P(t) = (5)(10t - 1) + (6t)(6t^2) + (0)(-3)
$$

$$
P(t) = 50t - 5 + 36t^3
$$

**Final Result:**

$$
P(t) = 36t^3 + 50t - 5 \text{ W}
$$
