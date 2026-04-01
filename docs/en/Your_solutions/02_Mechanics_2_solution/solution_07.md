# Question - 7. Dynamics with Friction

A 5 kg block is placed on a 10 kg block. A horizontal force of 45 N is applied to the 10 kg block, and the 5 kg block is tied to the wall. The coefficient of kinetic friction between all moving surfaces is 0.2. Find the acceleration of the 10 kg block.

---

## 1. Necessary Definitions and Formulas

To solve this problem, we use the principles of Newton's Second Law and the physics of friction.

**Newton’s Second Law**: The net force acting on an object is equal to the mass of that object multiplied by its acceleration.

$$
\sum F = m \cdot a
$$

**Normal Force ($N$)**: The support force exerted by a surface. For a horizontal surface, it is equal to the weight of the objects pressing down on it.
    
$$
N = m \cdot g
$$
    
**Kinetic Friction ($f_k$)**: The resistive force between moving surfaces.
    
$$
f_k = \mu_k \cdot N
$$
    
where $\mu_k$ is the coefficient of kinetic friction.

---

## 2. Problem Solution

### Given Data
* Mass of top block ($m_1$): $5\text{ kg}$
* Mass of bottom block ($m_2$): $10\text{ kg}$
* Applied force ($F$): $45\text{ N}$
* Coefficient of friction ($\mu_k$): $0.2$
* Gravity ($g$): $9.8\text{ m/s}^2$

### Step 1: Analyze the Top Block ($m_1$)
The top block is tied to the wall, so its acceleration is zero ($a_1 = 0$). However, it exerts a downward normal force on the bottom block and experiences friction.

**Normal force between $m_1$ and $m_2$:**

$$
N_1 = m_1 \cdot g = 5 \cdot 9.8 = 49\text{ N}
$$

**Frictional force between $m_1$ and $m_2$:**
Since the bottom block moves to the right, this friction force pulls the bottom block to the left.

$$
f_{k1} = \mu_k \cdot N_1 = 0.2 \cdot 49 = 9.8\text{ N}
$$

### Step 2: Analyze the Bottom Block ($m_2$)
The bottom block slides against both the top block and the floor. We need the total normal force on the floor to find the floor's friction.

**Total Normal force on the floor ($N_2$):**

$$
N_2 = (m_1 + m_2) \cdot g = (5 + 10) \cdot 9.8 = 147\text{ N}
$$

**Frictional force from the floor ($f_{k2}$):**

$$
f_{k2} = \mu_k \cdot N_2 = 0.2 \cdot 147 = 29.4\text{ N}
$$

### Step 3: Calculate the Acceleration of the 10 kg Block
We apply Newton's Second Law to the bottom block. The forces acting on it are the applied force ($F$) to the right, and two friction forces ($f_{k1}$ and $f_{k2}$) acting to the left.

**Net Force equation:**

$$
\sum F = F - f_{k1} - f_{k2}
$$

$$
\sum F = 45 - 9.8 - 29.4 = 5.8\text{ N}
$$

**Solving for Acceleration ($a_2$):**

$$
a_2 = \frac{\sum F}{m_2}
$$

$$
a_2 = \frac{5.8}{10} = 0.58\text{ m/s}^2
$$

---

### Final Result
The acceleration of the 10 kg block is **$0.58\text{ m/s}^2$**.
