# Physics Problem: Conservation of Energy in a Pendulum

## 1. Key Definitions and Formulas

Before solving, let's review the fundamental concepts required for this problem:

### Law of Conservation of Energy
In an isolated system where only conservative forces (like gravity) are acting, the total mechanical energy ($E_{total}$) remains constant.
$$
E_{initial} = E_{final}
$$

### Kinetic Energy ($K$)
The energy an object possesses due to its motion.
$$
K = \frac{1}{2} m v^2
$$
*Where $m$ is mass and $v$ is velocity.*

### Gravitational Potential Energy ($U$)
The energy stored in an object due to its vertical position (height) relative to a reference point.
$$
U = mgh
$$
*Where $g$ is the acceleration due to gravity ($\approx 9.81 \text{ m/s}^2$) and $h$ is the height.*

### Pendulum Geometry
When a pendulum of length $L$ is displaced by an angle $\theta$, its height $h$ above the lowest point (the equilibrium position) is given by:
$$
h = L - L\cos(\theta) = L(1 - \cos(\theta))
$$



---

## 2. Problem Solving Steps

### Given Data:
* Length of the pendulum ($L$) = $1.0 \text{ m}$
* Initial angle ($\theta$) = $15^\circ$
* Acceleration due to gravity ($g$) = $9.81 \text{ m/s}^2$
* Initial velocity ($v_i$) = $0 \text{ m/s}$ (released from rest)

### Step 1: Determine the initial height ($h$)
We need to find how high the bob is relative to the bottom of the swing.

$$
h = 1.0 \cdot (1 - \cos(15^\circ))
$$

Using $\cos(15^\circ) \approx 0.9659$:

$$
h = 1.0 \cdot (1 - 0.9659) = 0.0341 \text{ m}
$$

### Step 2: Set up the Energy Conservation equation
At the release point (top), the energy is purely potential. At the bottom of the swing, all that potential energy has converted into kinetic energy.

$$
U_{top} = K_{bottom}
$$

$$
mgh = \frac{1}{2}mv^2
$$

### Step 3: Simplify and Solve for $v$
Notice that the mass ($m$) appears on both sides, so it cancels out. This means the speed of the pendulum does not depend on the weight of the bob!

$$
gh = \frac{1}{2}v^2
$$

Rearranging to solve for $v$:

$$
v^2 = 2gh
$$

$$
v = \sqrt{2gh}
$$

### Step 4: Final Calculation
Plug in the values for $g$ and $h$:

$$
v = \sqrt{2 \cdot 9.81 \cdot 0.0341}
$$

$$
v = \sqrt{0.6690}
$$

$$
v \approx 0.818 \text{ m/s}
$$

---

## 3. Final Answer
The speed of the pendulum bob at the bottom of its swing is approximately **0.82 m/s**.
