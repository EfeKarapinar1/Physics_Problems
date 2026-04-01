# Question - 11. Dynamics with a time-dependent force

A particle of mass $m=3$ kg moves in a force field $F$ dependent on time in the following way:

$$
F = (15t, 3t-12, -6t^2) \, \text{N}
$$

Assuming initial conditions $r_0=(5,2,-3)$ m, $v_0=(2,0,1)$ m/s, find the dependence of the particle's position and velocity on time.

---

## Step-by-Step Solution

### 1. Calculate the Acceleration
According to Newton's Second Law $\vec{F} = m\vec{a}$, we find the acceleration vector by dividing the force by the mass ($m = 3$ kg):

$$
\vec{a}(t) = \frac{\vec{F}(t)}{m} = \frac{1}{3} (15t, 3t-12, -6t^2)
$$

$$
\vec{a}(t) = (5t, t-4, -2t^2) \, \text{m/s}^2
$$

### 2. Find the Velocity Function
We integrate the acceleration components with respect to time $t$:

$$
\vec{v}(t) = \int \vec{a}(t) dt = \left( \int 5t \, dt, \int (t-4) \, dt, \int -2t^2 \, dt \right)
$$

$$
\vec{v}(t) = \left( \frac{5}{2}t^2 + C_1, \frac{1}{2}t^2 - 4t + C_2, -\frac{2}{3}t^3 + C_3 \right)
$$

Now, apply the initial condition $\vec{v}(0) = (2, 0, 1)$:
- $x$-comp: $\frac{5}{2}(0)^2 + C_1 = 2 \implies C_1 = 2$
- $y$-comp: $\frac{1}{2}(0)^2 - 4(0) + C_2 = 0 \implies C_2 = 0$
- $z$-comp: $-\frac{2}{3}(0)^3 + C_3 = 1 \implies C_3 = 1$

Thus, the velocity as a function of time is:

$$
\vec{v}(t) = \left( \frac{5}{2}t^2 + 2, \frac{1}{2}t^2 - 4t, -\frac{2}{3}t^3 + 1 \right) \, \text{m/s}
$$

### 3. Find the Position Function
We integrate the velocity components with respect to time $t$:

$$
\vec{r}(t) = \int \vec{v}(t) dt = \left( \int \left(\frac{5}{2}t^2 + 2\right) dt, \int \left(\frac{1}{2}t^2 - 4t\right) dt, \int \left(-\frac{2}{3}t^3 + 1\right) dt \right)
$$

$$
\vec{r}(t) = \left( \frac{5}{6}t^3 + 2t + D_1, \frac{1}{6}t^3 - 2t^2 + D_2, -\frac{2}{12}t^4 + t + D_3 \right)
$$

Now, apply the initial condition $\vec{r}(0) = (5, 2, -3)$:
- $x$-comp: $0 + 0 + D_1 = 5 \implies D_1 = 5$
- $y$-comp: $0 - 0 + D_2 = 2 \implies D_2 = 2$
- $z$-comp: $0 + 0 + D_3 = -3 \implies D_3 = -3$

Simplifying $-\frac{2}{12}$ to $-\frac{1}{6}$, the position as a function of time is:

$$
\vec{r}(t) = \left( \frac{5}{6}t^3 + 2t + 5, \frac{1}{6}t^3 - 2t^2 + 2, -\frac{1}{6}t^4 + t - 3 \right) \, \text{m}
$$

---

## Final Results

**Velocity Dependence:**

$$
\vec{v}(t) = \left( \frac{5}{2}t^2 + 2, \frac{1}{2}t^2 - 4t, -\frac{2}{3}t^3 + 1 \right)
$$

**Position Dependence:**

$$
\vec{r}(t) = \left( \frac{5}{6}t^3 + 2t + 5, \frac{1}{6}t^3 - 2t^2 + 2, -\frac{1}{6}t^4 + t - 3 \right)
$$
