# Physics Problem: Vector Lorentz Force Calculation

## 1. Necessary Definitions and Formulas

To solve this problem, we need to understand the interaction between a moving charge and a magnetic field.

### Magnetic Lorentz Force
The magnetic force $\vec{F}_m$ exerted on a particle with charge $q$ moving with velocity $\vec{v}$ in a magnetic field $\vec{B}$ is given by the vector cross product:

$$
\vec{F}_m = q(\vec{v} \times \vec{B})
$$

### Vector Cross Product (Determinant Form)
The cross product of two vectors $\vec{A}$ and $\vec{B}$ is calculated using the following determinant:

$$
\vec{A} \times \vec{B} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ A_x & A_y & A_z \\ B_x & B_y & B_z \end{vmatrix}
$$

### Magnitude of a Vector
The magnitude of a vector $\vec{A} = (A_x, A_y, A_z)$ is found using:

$$
|\vec{A}| = \sqrt{A_x^2 + A_y^2 + A_z^2}
$$

### Constants
* **Charge of a proton ($q$):** $\approx 1.602 \times 10^{-19} \text{ C}$

---

## 2. Step-by-Step Solution

### Step 1: List Given Values
* Velocity: $\vec{v} = (2\hat{i} - 4\hat{j} + \hat{k}) \text{ m/s}$
* Magnetic Field: $\vec{B} = (\hat{i} + 2\hat{j} - \hat{k}) \text{ T}$
* Charge: $q = 1.602 \times 10^{-19} \text{ C}$

### Step 2: Calculate the Cross Product $(\vec{v} \times \vec{B})$
We set up the determinant to find the direction and relative magnitude of the interaction:

$$
\vec{v} \times \vec{B} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ 2 & -4 & 1 \\ 1 & 2 & -1 \end{vmatrix}
$$

Expanding the determinant by the first row:

* **$\hat{i}$ component:** $(-4 \cdot -1) - (1 \cdot 2) = 4 - 2 = 2$
* **$\hat{j}$ component:** $-[(2 \cdot -1) - (1 \cdot 1)] = -[-2 - 1] = 3$
* **$\hat{k}$ component:** $(2 \cdot 2) - (-4 \cdot 1) = 4 + 4 = 8$

The resulting vector is:

$$
\vec{v} \times \vec{B} = (2\hat{i} + 3\hat{j} + 8\hat{k})
$$

### Step 3: Find the Magnitude of the Cross Product
We calculate the length of the vector derived in the previous step:

$$
|\vec{v} \times \vec{B}| = \sqrt{2^2 + 3^2 + 8^2}
$$

$$
|\vec{v} \times \vec{B}| = \sqrt{4 + 9 + 64} = \sqrt{77}
$$

$$
|\vec{v} \times \vec{B}| \approx 8.775 \text{ T}\cdot\text{m/s}
$$

### Step 4: Calculate the Total Force Magnitude
Finally, we multiply the magnitude of the cross product by the charge of the proton to get the force in Newtons (N):

$$
F_m = q \cdot |\vec{v} \times \vec{B}|
$$

$$
F_m = (1.602 \times 10^{-19} \text{ C}) \cdot \sqrt{77}
$$

$$
F_m \approx 1.602 \times 10^{-19} \cdot 8.775
$$

$$
F_m \approx 1.406 \times 10^{-18} \text{ N}
$$

---

## 3. Final Answer
The magnitude of the magnetic force experienced by the proton is:

**$|\vec{F}_m| \approx 1.41 \times 10^{-18} \text{ N}$**
