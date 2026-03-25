# Kinematics: Variable Velocity Solution

## 1. Necessary Definitions and Formulas

To solve problems involving variable velocity, we use the following calculus-based relationships between position ($x$), velocity ($v$), and acceleration ($a$).

### Position ($x$)
The position of an object is found by integrating the velocity function with respect to time.

$$
x(t) = \int v(t) \, dt
$$

### Velocity ($v$)
Velocity is the first derivative of position with respect to time.

$$
v(t) = \frac{dx}{dt}
$$

### Acceleration ($a$)
Acceleration is the rate of change of velocity. It is found by taking the derivative of the velocity function.

$$
a(t) = \frac{dv}{dt}
$$

### Power Rule for Calculus

**Integration:**

$$
\int t^n \, dt = \frac{t^{n+1}}{n+1} + C
$$

**Differentiation:**

$$
\frac{d}{dt}(t^n) = n t^{n-1}
$$

---

## 2. Problem Solution

**Given:**
* Velocity function: $v(t) = t^2 + 2t - 5$
* Initial condition: $x(0) = 4$
* Target: Find position $x(3)$ and acceleration $a(3)$

### Step 1: Derive the Position Function $x(t)$
We integrate the velocity function:

$$
x(t) = \int (t^2 + 2t - 5) \, dt
$$

Applying the power rule for integration:

$$
x(t) = \frac{t^3}{3} + t^2 - 5t + C
$$

### Step 2: Solve for the Constant $C$
Using the initial condition $x(0) = 4$:

$$
4 = \frac{0^3}{3} + 0^2 - 5(0) + C
$$

$$
C = 4
$$

The full position function is:

$$
x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4
$$

### Step 3: Calculate Position at $t = 3$
Substitute $t = 3$ into the function:

$$
x(3) = \frac{1}{3}(3)^3 + (3)^2 - 5(3) + 4
$$

$$
x(3) = 9 + 9 - 15 + 4
$$

$$
x(3) = 7
$$

### Step 4: Derive the Acceleration Function $a(t)$
Differentiate the velocity function:

$$
a(t) = \frac{d}{dt}(t^2 + 2t - 5)
$$

$$
a(t) = 2t + 2
$$

### Step 5: Calculate Acceleration at $t = 3$
Substitute $t = 3$ into the acceleration function:

$$
a(3) = 2(3) + 2
$$

$$
a(3) = 8
$$

---

## Final Results Summary

| Metric | Result |
| :--- | :--- |
| **Position at $t=3$** | $x(3) = 7$ |
| **Acceleration at $t=3$** | $a(3) = 8$ |
