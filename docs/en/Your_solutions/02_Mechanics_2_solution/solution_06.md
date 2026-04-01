# Problem: Energy Dissipation of a Bouncing Ball

## Necessary Definitions and Formulas

### 1. Gravitational Potential Energy ($E_p$)
The energy an object possesses due to its position in a gravitational field. At the maximum height of a bounce, the ball's kinetic energy is zero, so its total mechanical energy is equal to its potential energy:

$$
E_p = m \cdot g \cdot h
$$

Where:
* **$m$**: Mass of the object.
* **$g$**: Acceleration due to gravity ($\approx 9.81 \, \text{m/s}^2$).
* **$h$**: Height above the reference level.

### 2. Energy Retention Factor ($k$)
If an object loses a specific percentage of energy ($L$) during an impact, the energy remaining ($E_{after}$) is calculated using the retention factor $k$:

$$
k = 1 - L
$$

Because potential energy is directly proportional to height ($E \propto h$), the height after a bounce scales linearly with the energy:

$$
h_{new} = h_{old} \cdot k
$$

---

## Step-by-Step Solution

**Given Data:**
* Initial height ($h_0$): $2.0$ m
* Energy loss ($L$): $30\%$ (expressed as $0.30$)
* Retention factor ($k$): $1 - 0.30 = 0.70$

### Step 1: Calculate the height after the first bounce ($h_1$)
After the first impact, the ball retains $70\%$ of its mechanical energy, which corresponds to $70\%$ of its initial height.

$$
h_1 = h_0 \cdot 0.70
$$

$$
h_1 = 2.0 \, \text{m} \cdot 0.70 = 1.4 \, \text{m}
$$

### Step 2: Calculate the height after the second bounce ($h_2$)
The ball loses another $30\%$ of its remaining energy upon the second impact. We apply the retention factor to the height reached after the first bounce ($h_1$).

$$
h_2 = h_1 \cdot 0.70
$$

$$
h_2 = 1.4 \, \text{m} \cdot 0.70 = 0.98 \, \text{m}
$$

### Alternative Method: General Formula
For any number of bounces ($n$), the height can be found using the following formula:

$$
h_n = h_0 \cdot k^n
$$

Applying this for the second bounce ($n = 2$):

$$
h_2 = 2.0 \cdot (0.70)^2 = 2.0 \cdot 0.49 = 0.98 \, \text{m}
$$

**Final Result:**
The tennis ball rises to a height of **$0.98$ m** after the second bounce.
