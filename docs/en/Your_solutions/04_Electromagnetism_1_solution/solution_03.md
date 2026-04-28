# Electrostatic Equilibrium Problem

## 1. Key Definitions and Formulas

### Definitions
* **Coulomb's Law:** Describes the electrostatic force of attraction or repulsion between two point charges. The force is directly proportional to the product of the magnitudes of charges and inversely proportional to the square of the distance between them.
* **Electrostatic Equilibrium:** A state where the net electrostatic force acting on a particle is zero ($\sum \vec{F} = 0$).
* **Principle of Superposition:** The total force on a charge is the vector sum of the individual forces exerted by all other charges in the system.

### Formulas

**Coulomb's Law Force:**

$$
F = k \frac{|q_1 q_2|}{r^2}
$$

Where:
* $k$ is Coulomb's constant ($\approx 8.99 \times 10^9 \text{ N}\cdot\text{m}^2/\text{C}^2$)
* $q_1, q_2$ are the magnitudes of the charges
* $r$ is the distance between the centers of the charges

---

## 2. Problem Statement
Find the equilibrium position for a charge $q_3 = +1\text{C}$ placed on the line between a charge $q_1 = +4\text{C}$ and a charge $q_2 = +9\text{C}$, which are separated by a distance of 2 m.



---

## 3. Step-by-Step Solution

### Step 1: Set up the Coordinate System
Let the charge $q_1$ be at the origin $(x = 0)$.
The charge $q_2$ is then at $x = 2\text{ m}$.
Let the third charge $q_3$ be placed at a distance $x$ from $q_1$. This means the distance between $q_3$ and $q_2$ is $(2 - x)$.

### Step 2: Identify the Forces
Since all charges are positive, $q_1$ will push $q_3$ to the right ($F_{13}$), and $q_2$ will push $q_3$ to the left ($F_{23}$). For equilibrium, these two forces must be equal in magnitude:

$$
|F_{13}| = |F_{23}|
$$

### Step 3: Apply Coulomb's Law
Substitute the formula for both forces:

$$
k \frac{q_1 q_3}{x^2} = k \frac{q_2 q_3}{(2 - x)^2}
$$

### Step 4: Simplify the Equation
Notice that $k$ and $q_3$ appear on both sides, so they cancel out:

$$
\frac{q_1}{x^2} = \frac{q_2}{(2 - x)^2}
$$

### Step 5: Plug in the Given Values
Substitute $q_1 = 4\text{C}$ and $q_2 = 9\text{C}$:

$$
\frac{4}{x^2} = \frac{9}{(2 - x)^2}
$$

### Step 6: Solve for $x$
Instead of expanding the quadratic, we can take the square root of both sides to simplify the math:

$$
\sqrt{\frac{4}{x^2}} = \sqrt{\frac{9}{(2 - x)^2}}
$$

$$
\frac{2}{x} = \frac{3}{2 - x}
$$

Now, cross-multiply:

$$
2(2 - x) = 3x
$$

$$
4 - 2x = 3x
$$

$$
4 = 5x
$$

$$
x = 0.8 \text{ m}
$$

### Final Result
The equilibrium position for $q_3$ is **0.8 meters** from charge $q_1$ (or 1.2 meters from charge $q_2$).
