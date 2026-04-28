## 1. Necessary Definitions and Formulas

### Electric Potential ($V$)
Electric potential is a **scalar** quantity representing the potential energy per unit charge at a point in space. Because it is a scalar, we do not need to use vector addition; we simply sum the values algebraically.

### Point Charge Potential Formula
The potential $V$ created by a point charge $q$ at a distance $r$ from the charge is:

$$
V = k \frac{q}{r}
$$

Where:
- $k$ is Coulomb's constant $\approx 8.99 \times 10^9 \text{ N}\cdot\text{m}^2/\text{C}^2$
- $q$ is the magnitude of the charge (with its sign)
- $r$ is the distance from the charge to the point of interest

### Principle of Superposition
For a system of multiple charges, the total potential is the sum of the individual potentials:

$$
V_{total} = \sum_{i=1}^{n} V_i = k \sum_{i=1}^{n} \frac{q_i}{r_i}
$$

---

## 2. Problem Statement

Point charges of **+1C, -2C, +3C, and -4C** are placed at the corners of a square with sides of **1.0 m** (in sequential order). Calculate the electric potential at the center of the square.

---

## 3. Step-by-Step Solution

### Step 1: Determine the distance $r$
The center of the square is equidistant from all four corners. This distance $r$ is half the length of the diagonal. Using the Pythagorean theorem for a square with side $a$:

$$
\text{Diagonal} = \sqrt{a^2 + a^2} = a\sqrt{2}
$$

$$
r = \frac{a\sqrt{2}}{2} = \frac{a}{\sqrt{2}}
$$

Given $a = 1.0 \text{ m}$:

$$
r = \frac{1.0}{\sqrt{2}} \approx 0.7071 \text{ m}
$$

### Step 2: Sum the charges
Since $r$ and $k$ are the same for all charges, we can factor them out of the summation:

$$
V_{center} = \frac{k}{r} (q_1 + q_2 + q_3 + q_4)
$$

Substitute the given charge values:

$$
\sum q = (+1\text{C}) + (-2\text{C}) + (+3\text{C}) + (-4\text{C}) = -2\text{ C}
$$

### Step 3: Final Calculation
Now, we plug the values into the factored formula:

$$
V_{center} = \frac{8.99 \times 10^9}{1 / \sqrt{2}} \times (-2)
$$

Which simplifies to:

$$
V_{center} = (8.99 \times 10^9) \times \sqrt{2} \times (-2)
$$

$$
V_{center} \approx (8.99 \times 10^9) \times (1.414) \times (-2)
$$

$$
V_{center} \approx -2.54 \times 10^{10} \text{ V}
$$

---

## Conclusion

The electric potential at the center of the square is approximately **$-2.54 \times 10^{10} \text{ Volts}$** (or $-25.4 \text{ GV}$). The negative sign indicates that the net work required to bring a positive test charge from infinity to this point is negative.
