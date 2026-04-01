# Physics Problem: Work and Energy with a Constant Force

## Problem Description
A constant force acts on a body of mass $m = 2\ \mathrm{kg}$:

$$
\vec F = [6, 2]\ \mathrm{N}
$$

The body starts with an initial velocity $\vec v(0) = (1, -1)\ \mathrm{m/s}$ from the point $\vec r(0) = (0, 0)\ \mathrm{m}$.

**Tasks:**
1. Determine $\vec a(t)$.
2. Determine $\vec v(t)$.
3. Determine $\vec r(t)$.
4. Draw the trajectory of the motion.
5. Calculate the work done by the force at time $t = 3\ \mathrm{s}$.
6. Check the consistency with the work-energy theorem.

---

## 1. Necessary Definitions and Formulas

* **Newton's Second Law**: Relates force, mass, and acceleration.
    
$$
\vec{F} = m \vec{a} \implies \vec{a} = \frac{\vec{F}}{m}
$$

* **Kinematic Equations**: Used for objects moving with constant acceleration.
    
$$
\vec{v}(t) = \vec{v}_0 + \vec{a}t
$$

$$
\vec{r}(t) = \vec{r}_0 + \vec{v}_0 t + \frac{1}{2} \vec{a} t^2
$$

* **Work Done by a Constant Force**: The dot product of force and displacement.
    
$$
W = \vec{F} \cdot \Delta \vec{r}
$$

* **Work-Energy Theorem**: Work equals the change in kinetic energy ($K = \frac{1}{2}mv^2$).
    
$$
W = \Delta K = K_f - K_i
$$

---

## 2. Step-by-Step Solution

### Step 1: Determine Acceleration $\vec{a}(t)$
Since the force and mass are constant, the acceleration is constant over time:

$$
\vec{a} = \frac{[6, 2]\ \mathrm{N}}{2\ \mathrm{kg}} = [3, 1]\ \mathrm{m/s^2}
$$

### Step 2: Determine Velocity $\vec{v}(t)$
We use the initial velocity $\vec{v}_0 = [1, -1]$ and add the change due to acceleration:

$$
\vec{v}(t) = [1, -1] + [3, 1]t = [1 + 3t, -1 + t]\ \mathrm{m/s}
$$

### Step 3: Determine Position $\vec{r}(t)$
Starting from the origin $\vec{r}_0 = [0, 0]$:

$$
\vec{r}(t) = [0, 0] + [1, -1]t + \frac{1}{2}[3, 1]t^2 = [t + 1.5t^2, -t + 0.5t^2]\ \mathrm{m}
$$

### Step 4: Trajectory
The trajectory follows a parabolic path. At $t=0$, the body moves toward $(1, -1)$, but the constant force eventually pulls it in the positive $x$ and $y$ directions.

### Step 5: Calculate Work at $t = 3\ \mathrm{s}$
First, find the displacement vector $\Delta \vec{r}$ at $t=3$:

$$
\Delta \vec{r} = \vec{r}(3) = [3 + 1.5(3^2), -3 + 0.5(3^2)] = [16.5, 1.5]\ \mathrm{m}
$$

Now, calculate the work $W$:

$$
W = \vec{F} \cdot \Delta \vec{r} = [6, 2] \cdot [16.5, 1.5] = (6 \times 16.5) + (2 \times 1.5) = 102\ \mathrm{J}
$$

### Step 6: Consistency with Work-Energy Theorem
We check if $W = \Delta K$.

* **Initial Kinetic Energy ($t=0$):**
    $v_0^2 = 1^2 + (-1)^2 = 2$
    
$$
K_i = \frac{1}{2}(2)(2) = 2\ \mathrm{J}
$$

* **Final Kinetic Energy ($t=3$):**
    $\vec{v}(3) = [1 + 3(3), -1 + 3] = [10, 2]$
    $v(3)^2 = 10^2 + 2^2 = 104$
    
$$
K_f = \frac{1}{2}(2)(104) = 104\ \mathrm{J}
$$

* **Change in Kinetic Energy:**
    
$$
\Delta K = 104\ \mathrm{J} - 2\ \mathrm{J} = 102\ \mathrm{J}
$$

**Conclusion:** Since $W = \Delta K = 102\ \mathrm{J}$, the solution is consistent.
