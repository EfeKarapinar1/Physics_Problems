# Question - 8. Work of a variable force

Given a one-dimensional force:

$$
F(x)=-kx
$$

* Write down the equation of motion and solve it.
* Calculate the work done during the displacement from $0$ to $x_0$.
* Interpret the result as potential energy.
* Verify the relationship $F = -\frac{dU}{dx}$.
* Draw the graph of $F(x)$ and $U(x)$.

---

## 1. Essential Definitions and Formulas

Before solving the problem, we define the physical principles governing a system with a linear restoring force:

* **Newton's Second Law:** The fundamental law relating force, mass, and acceleration.
    
$$
F = m \cdot a = m \frac{d^2x}{dt^2}
$$

* **Work Done by a Variable Force:** Since the force changes with position, we must use integration to find the total work $W$ over a path from $x_1$ to $x_2$.
    
$$
W = \int_{x_1}^{x_2} F(x) \, dx
$$

* **Potential Energy ($U$):** For a conservative force, the change in potential energy is defined as the negative of the work done by that force.
    
$$
\Delta U = -W
$$

* **Force-Potential Relationship:** The force can be recovered by taking the negative derivative of the potential energy function.
    
$$
F = -\frac{dU}{dx}
$$

---

## 2. Step-by-Step Solution

### Step 1: Equation of Motion and its Solution
We are given the force $F(x) = -kx$. By applying Newton's Second Law ($F = ma$), we write the differential equation:

$$
m \frac{d^2x}{dt^2} = -kx
$$

To solve this, we rearrange it into the standard form for a harmonic oscillator:

$$
\frac{d^2x}{dt^2} + \frac{k}{m}x = 0
$$

Let $\omega^2 = \frac{k}{m}$, where $\omega$ is the angular frequency. The equation becomes:

$$
\ddot{x} + \omega^2 x = 0
$$

**The Solution:**
This is a second-order linear homogeneous differential equation. Its general solution describes **Simple Harmonic Motion (SHM)**:

$$
x(t) = A \cos(\omega t + \phi)
$$

*Where $A$ is the amplitude and $\phi$ is the phase constant determined by initial conditions.*

---

### Step 2: Calculate Work Done from $0$ to $x_0$
To find the work done by the force $F(x) = -kx$ during a displacement from the origin ($x=0$) to a point $x_0$, we integrate the force function:

$$
W = \int_{0}^{x_0} (-kx) \, dx
$$

Calculating the definite integral:

$$
W = -k \left[ \frac{1}{2}x^2 \right]_{0}^{x_0}
$$

$$
W = -\frac{1}{2}kx_0^2
$$

---

### Step 3: Interpret Result as Potential Energy
Potential energy $U(x)$ is the energy stored in the system due to its configuration. By convention, the potential energy is the negative of the work done by the conservative force:

$$
U(x) = -W = -\left( -\frac{1}{2}kx^2 \right)
$$

Assuming the potential energy at the equilibrium point is zero ($U(0) = 0$):

$$
U(x) = \frac{1}{2}kx^2
$$

**Interpretation:** The work done by the restoring force is negative because the force opposes the displacement. This energy is not lost but is stored as **Elastic Potential Energy** in the system.

---

### Step 4: Verify the Relationship $F = -\frac{dU}{dx}$
We verify our results by differentiating the potential energy function $U(x) = \frac{1}{2}kx^2$ with respect to position:

$$
\frac{dU}{dx} = \frac{d}{dx} \left( \frac{1}{2}kx^2 \right) = kx
$$

Applying the negative sign:

$$
-\frac{dU}{dx} = -kx
$$

Since $-kx$ is exactly our original force $F(x)$, the relationship is confirmed.

---

### Step 5: Graphs of $F(x)$ and $U(x)$

* **Force $F(x)$:** A straight line with a negative slope ($-k$) passing through the origin. It shows that as displacement increases, the restoring force increases in the opposite direction.
* **Potential Energy $U(x)$:** A parabola opening upwards. It shows that energy increases quadratically as the object moves away from equilibrium ($x=0$) in either direction.
