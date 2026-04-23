## Problem

For the given equation describing a damped harmonic oscillator:

$$
m \frac{d^2 x}{dt^2} + b \frac{dx}{dt} + k x = 0
$$

make interactive HTML animation with a slider for the parameter $b$ to show the behavior of the system in the underdamped, critically damped, and overdamped cases. Include graphs of $x(t)$ and the phase portrait for each case.

1. Write down the general solution.
2. Present the classification of cases: underdamped, critically damped, overdamped.
3. Solve the equation numerically (RK4).
4. Investigate the effect of parameter $b$.
5. Generate the graph of $x(t)$.
6. Generate the phase portrait.

## 1. Fundamental Definitions and Formulas

Before solving the equation, let's establish the physical parameters and the mathematical framework.

### The Equation of Motion
The motion of a damped harmonic oscillator is governed by Newton's Second Law ($F = ma$), considering a restoring force (Hooke's Law) and a resistive force (damping) proportional to velocity:

$$
m \frac{d^2 x}{dt^2} + b \frac{dx}{dt} + k x = 0
$$

Where:
* **$m$**: Mass of the object $[kg]$.
* **$b$**: Damping coefficient $[N \cdot s/m]$.
* **$k$**: Spring constant $[N/m]$.

### Standard Form
To simplify analysis, we divide by $m$:

$$
\frac{d^2 x}{dt^2} + 2\gamma \frac{dx}{dt} + \omega_0^2 x = 0
$$

Where:
* **$\gamma = \frac{b}{2m}$**: Damping attenuation parameter.
* **$\omega_0 = \sqrt{\frac{k}{m}}$**: Undamped natural angular frequency.

### The Characteristic Equation
Assuming a solution of the form $x(t) = e^{rt}$, we get the characteristic quadratic equation:

$$
r^2 + 2\gamma r + \omega_0^2 = 0
$$

The roots are:

$$
r_{1,2} = -\gamma \pm \sqrt{\gamma^2 - \omega_0^2}
$$



---

## 2. General Solution and Case Classification

The behavior of the system depends entirely on the term under the square root: the discriminant $\Delta = \gamma^2 - \omega_0^2$ (or $b^2 - 4mk$).

### Case I: Underdamped ($\gamma < \omega_0$ or $b^2 < 4mk$)
The roots are complex. The system oscillates with an exponentially decaying amplitude.
* **Solution:** $x(t) = A e^{-\gamma t} \cos(\omega_d t + \phi)$
* **Damped Frequency:** $\omega_d = \sqrt{\omega_0^2 - \gamma^2}$

### Case II: Critically Damped ($\gamma = \omega_0$ or $b^2 = 4mk$)
The roots are real and identical ($r = -\gamma$). The system returns to equilibrium as quickly as possible without oscillating.
* **Solution:** $x(t) = (C_1 + C_2 t) e^{-\gamma t}$

### Case III: Overdamped ($\gamma > \omega_0$ or $b^2 > 4mk$)
The roots are real and distinct. The system returns slowly to equilibrium without ever crossing it (assuming no initial velocity toward equilibrium).
* **Solution:** $x(t) = C_1 e^{r_1 t} + C_2 e^{r_2 t}$

---

## 3. Numerical Solution: Runge-Kutta (RK4)

To solve the second-order ODE numerically, we break it into a system of two first-order ODEs:

1.  $\frac{dx}{dt} = v$
2.  $\frac{dv}{dt} = -\frac{b}{m}v - \frac{k}{m}x$

The RK4 algorithm updates the state $y = [x, v]$ using a weighted average of four increments:

$$
k_1 = f(t_n, y_n)
$$

$$
k_2 = f(t_n + \frac{h}{2}, y_n + \frac{h}{2}k_1)
$$

$$
k_3 = f(t_n + \frac{h}{2}, y_n + \frac{h}{2}k_2)
$$

$$
k_4 = f(t_n + h, y_n + h k_3)
$$

$$
y_{n+1} = y_n + \frac{h}{6}(k_1 + 2k_2 + 2k_3 + k_4)
$$
