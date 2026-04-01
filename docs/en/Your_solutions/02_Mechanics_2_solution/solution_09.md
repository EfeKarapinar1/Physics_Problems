# Question - 9. Vertical throw with drag

We have the equation of motion:

$$
m\frac{dv}{dt} = -mg - kv
$$

with initial conditions $v(0)=v_0$, $x(0)=10$.

* Solve the equation by analytical methods.
* Determine the maximum height.
* Compare with the case without drag.
* Perform a numerical simulation using HTML or Pythyon.

---

## 1. Definitions and Fundamental Formulas

To solve this problem, we must define the physical quantities and the governing laws of motion.

### Newton's Second Law
The net force acting on an object is equal to the rate of change of its momentum. For constant mass:

$$
F_{net} = m \cdot a = m \frac{dv}{dt}
$$

### Linear Drag Force
For objects moving at relatively low speeds through a fluid, the drag force $F_d$ is proportional to the velocity:

$$
F_d = -kv
$$

Where:
* $k$ is the drag coefficient (kg/s).
* The negative sign indicates the force opposes the direction of motion.

### Key Constants
* $g$: Acceleration due to gravity ($9.81 \, \text{m/s}^2$).
* $\gamma = \frac{k}{m}$: The damping coefficient per unit mass ($s^{-1}$).
* $v_t = \frac{mg}{k} = \frac{g}{\gamma}$: The terminal velocity (magnitude).

---

## 2. Analytical Solution

We are given the differential equation:

$$
m\frac{dv}{dt} = -mg - kv
$$

### Step A: Finding the Velocity $v(t)$
First, we rearrange the equation to isolate the derivative:

$$
\frac{dv}{dt} = -g - \frac{k}{m}v = -(g + \gamma v)
$$

This is a separable first-order differential equation. We group terms involving $v$ and $t$:

$$
\frac{dv}{g + \gamma v} = -dt
$$

Integrating both sides:

$$
\int \frac{1}{g + \gamma v} dv = \int -dt
$$

Using substitution $u = g + \gamma v$, we get:

$$
\frac{1}{\gamma} \ln(g + \gamma v) = -t + C
$$

Applying the initial condition $v(0) = v_0$:

$$
\frac{1}{\gamma} \ln(g + \gamma v_0) = C
$$

Substituting $C$ back and solving for $v(t)$:

$$
\ln\left(\frac{g + \gamma v}{g + \gamma v_0}\right) = -\gamma t
$$

$$
v(t) = \left(v_0 + \frac{g}{\gamma}\right)e^{-\gamma t} - \frac{g}{\gamma}
$$

### Step B: Finding the Position $x(t)$
Since $v(t) = \frac{dx}{dt}$, we integrate the velocity function:

$$
x(t) = \int \left[ \left(v_0 + \frac{g}{\gamma}\right)e^{-\gamma t} - \frac{g}{\gamma} \right] dt
$$

$$
x(t) = -\frac{1}{\gamma}\left(v_0 + \frac{g}{\gamma}\right)e^{-\gamma t} - \frac{g}{\gamma}t + C_2
$$

Using the initial condition $x(0) = 10$:

$$
10 = -\frac{1}{\gamma}\left(v_0 + \frac{g}{\gamma}\right) + C_2 \implies C_2 = 10 + \frac{v_0}{\gamma} + \frac{g}{\gamma^2}
$$

The final equation for position is:

$$
x(t) = 10 + \frac{1}{\gamma} \left( v_0 + \frac{g}{\gamma} \right) (1 - e^{-\gamma t}) - \frac{g}{\gamma} t
$$

---

## 3. Determining Maximum Height

The maximum height occurs when the velocity is zero ($v(t_{peak}) = 0$).

Using the velocity equation:

$$
0 = \left(v_0 + \frac{g}{\gamma}\right)e^{-\gamma t_{peak}} - \frac{g}{\gamma}
$$

Solving for $t_{peak}$:

$$
e^{-\gamma t_{peak}} = \frac{g}{g + \gamma v_0}
$$

$$
t_{peak} = \frac{1}{\gamma} \ln\left(1 + \frac{\gamma v_0}{g}\right)
$$

The maximum height $H_{max}$ is found by substituting $t_{peak}$ into the $x(t)$ equation:

$$
H_{max} = 10 + \frac{v_0}{\gamma} - \frac{g}{\gamma^2} \ln\left(1 + \frac{\gamma v_0}{g}\right)
$$

---

## 4. Comparison with the Vacuum Case

| Feature | No Drag ($k=0$) | With Drag ($k > 0$) |
| :--- | :--- | :--- |
| **Velocity** | $v(t) = v_0 - gt$ | Decays exponentially toward $-v_t$ |
| **Peak Time** | $t = \frac{v_0}{g}$ | $t = \frac{1}{\gamma} \ln(1 + \frac{\gamma v_0}{g})$ (Shorter) |
| **Max Height** | $10 + \frac{v_0^2}{2g}$ | Lower than vacuum case due to energy dissipation |
| **Acceleration** | Constant $-g$ | Magnitude $> g$ on the way up, $< g$ on the way down |

---

## 5. Numerical Simulation (Python)

```python
import numpy as np
import matplotlib.pyplot as plt
from scipy.integrate import odeint

# Constants
m = 1.0        # mass (kg)
g = 9.81       # gravity (m/s^2)
k = 0.5        # drag coefficient (kg/s)
v0 = 30.0      # initial velocity (m/s)
x0 = 10.0      # initial height (m)
gamma = k / m

# Time array
t = np.linspace(0, 5, 500)

# 1. Analytical Solution (With Drag)
v_analytical = (v0 + g/gamma) * np.exp(-gamma * t) - g/gamma
x_analytical = x0 + (1/gamma)*(v0 + g/gamma)*(1 - np.exp(-gamma * t)) - (g/gamma)*t

# 2. Vacuum Case (No Drag)
x_vacuum = x0 + v0*t - 0.5*g*t**2

# Filter out values where the object hits the ground (x < 0)
mask_drag = x_analytical >= 0
mask_vac = x_vacuum >= 0

# Plotting
plt.figure(figsize=(10, 6))
plt.plot(t[mask_drag], x_analytical[mask_drag], label='With Drag (Linear)', linewidth=2)
plt.plot(t[mask_vac], x_vacuum[mask_vac], '--', label='No Drag (Vacuum)', color='gray')
plt.axhline(0, color='black', lw=1)
plt.title('Vertical Throw: Drag vs. Vacuum')
plt.xlabel('Time (s)')
plt.ylabel('Height (m)')
plt.legend()
plt.grid(True, alpha=0.3)
plt.show()
