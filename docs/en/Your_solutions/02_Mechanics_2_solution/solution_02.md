# Question - 2. Harmonic Motion

A 10 kg mass is attached to a spring and oscillates according to the equation $x(t) = 0.2 \cos(10\pi t)$ (in meters). What is the spring constant $k$? What is the total mechanical energy of the system?

---

## 1. Necessary Definitions and Formulas

To solve problems involving **Simple Harmonic Motion (SHM)**, we use the following fundamental concepts:

### Displacement Equation
The position of an object in SHM as a function of time $t$ is generally expressed as:

$$
x(t) = A \cos(\omega t + \phi)
$$

Where:
* **$A$**: Amplitude (maximum displacement from equilibrium).
* **$\omega$**: Angular frequency (measured in rad/s).
* **$\phi$**: Phase constant.

### Angular Frequency and Spring Constant
For a mass-spring system, the angular frequency is related to the mass $m$ and the spring constant $k$ by:

$$
\omega = \sqrt{\frac{k}{m}} \implies k = m \omega^2
$$

### Total Mechanical Energy
In an ideal system without friction, the total mechanical energy $E$ is constant and depends on the spring constant and the amplitude:

$$
E = \frac{1}{2} k A^2
$$

---

## 2. Problem Data

From the problem statement, we have:
* **Mass ($m$):** $10 \text{ kg}$
* **Equation of motion:** $x(t) = 0.2 \cos(10\pi t)$

---

## 3. Step-by-Step Solution

### Step 1: Identify Parameters from the Equation
By comparing the given equation $x(t) = 0.2 \cos(10\pi t)$ to the standard form $x(t) = A \cos(\omega t)$, we can identify:
* $A = 0.2 \text{ m}$
* $\omega = 10\pi \text{ rad/s}$

### Step 2: Calculate the Spring Constant ($k$)
We use the formula derived from the angular frequency definition:

$$
k = m \omega^2
$$

Substituting the known values:

$$
k = 10 \cdot (10\pi)^2
$$

$$
k = 10 \cdot 100\pi^2
$$

$$
k = 1000\pi^2 \text{ N/m}
$$

*Numerical approximation (using $\pi^2 \approx 9.87$): $k \approx 9869.6 \text{ N/m}$.*

### Step 3: Calculate the Total Mechanical Energy ($E$)
Now we use the energy formula with the calculated $k$ and the identified $A$:

$$
E = \frac{1}{2} k A^2
$$

Substituting the values:

$$
E = \frac{1}{2} (1000\pi^2) (0.2)^2
$$

$$
E = 500\pi^2 \cdot 0.04
$$

$$
E = 20\pi^2 \text{ J}
$$

*Numerical approximation: $E \approx 197.39 \text{ J}$.*

---

## 4. Final Results

| Parameter | Exact Value | Numerical Approx. |
| :--- | :--- | :--- |
| **Spring Constant ($k$)** | $1000\pi^2 \text{ N/m}$ | $9869.6 \text{ N/m}$ |
| **Total Energy ($E$)** | $20\pi^2 \text{ J}$ | $197.39 \text{ J}$ |
