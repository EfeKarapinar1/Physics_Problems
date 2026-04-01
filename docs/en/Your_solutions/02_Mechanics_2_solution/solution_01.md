## Question - 1. Gravitational Dependence

A simple pendulum has a period of 4 seconds on Earth. What would its period be on the Moon, where the gravitational acceleration is about 1/6th of Earth's?

What is the required length of a simple pendulum to have a period of exactly 1 second on Earth?

---

## 1. Key Definitions and Formulas

* **Simple Pendulum:** An idealized system consisting of a mass ($m$) suspended by a string of length ($L$) with negligible mass.
* **Period ($T$):** The time required for one complete cycle of motion.
* **Gravitational Acceleration ($g$):** The acceleration of an object in free fall.
    * Earth: $g_e \approx 9.81 \, \text{m/s}^2$
    * Moon: $g_m \approx \frac{1}{6}g_e$

### The Period Formula
For small amplitudes, the period is calculated using:

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

### The Length Formula
By rearranging the period formula to solve for $L$, we get:

$$
L = \frac{g T^2}{4\pi^2}
$$

---

## 2. Problem 1: Period on the Moon

**Scenario:** A pendulum has a period of $4$ seconds on Earth. What is its period on the Moon?

### Step 1: Establish the Relationship
Since the length ($L$) of the pendulum remains constant, we can see from the formula that $T$ is inversely proportional to the square root of gravity:

$$
T \propto \frac{1}{\sqrt{g}}
$$

### Step 2: Ratio Comparison
We set up a ratio between the Moon ($T_m$) and Earth ($T_e$):

$$
\frac{T_m}{T_e} = \sqrt{\frac{g_e}{g_m}}
$$

### Step 3: Substitute and Solve
Given $g_m = \frac{1}{6}g_e$, the ratio $\frac{g_e}{g_m}$ is $6$.

$$
T_m = T_e \times \sqrt{6}
$$

$$
T_m = 4 \times 2.449 \approx 9.80 \, \text{s}
$$

**Conclusion:** The period on the Moon is approximately **9.80 seconds**.

---

## 3. Problem 2: Required Length on Earth

**Scenario:** What length ($L$) is required for a pendulum to have a period of exactly $1$ second on Earth?

### Step 1: Use the Length Formula
We use the derivation where $L$ is the subject:

$$
L = \frac{g T^2}{4\pi^2}
$$

### Step 2: Plug in the Constants
* $T = 1 \, \text{s}$
* $g = 9.81 \, \text{m/s}^2$
* $\pi \approx 3.14159$

$$
L = \frac{9.81 \times (1)^2}{4 \times (3.14159)^2}
$$

### Step 3: Calculation
$$
L = \frac{9.81}{39.478} \approx 0.248 \, \text{m}
$$

**Conclusion:** To achieve a 1-second period on Earth, the pendulum must be **0.248 meters** (or **24.8 cm**) long.

---

## Summary Comparison

| Parameter | Earth Value | Moon Value |
| :--- | :--- | :--- |
| **Gravity ($g$)** | $9.81 \, \text{m/s}^2$ | $\approx 1.63 \, \text{m/s}^2$ |
| **Period ($T$) for $L \approx 4\text{m}$** | $4.0 \, \text{s}$ | $9.8 \, \text{s}$ |
| **Length ($L$) for $T = 1\text{s}$** | $0.248 \, \text{m}$ | $0.041 \, \text{m}$ |
