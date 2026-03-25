# Path Intersection and Proximity Analysis

## 1. Definitions and Formulas

**Parametric Position:**
For any time $t$, the position is given by:

$$
P(t) = (x(t), y(t))
$$

**Distance Formula:**
The distance between Alice ($A$) and Bob ($B$) at time $t$:

$$
d(t) = \sqrt{(x_A(t) - x_B(t))^2 + (y_A(t) - y_B(t))^2}
$$

## 2. Collision Check
To check for a collision, we set $A(t) = B(t)$:

1. $2 + t = 2t - 1 \implies t = 3$
2. Check $y$ at $t = 3$: 
   - $y_A(3) = 8 - 3(3) = -1$
   - $y_B(3) = 2(3) + 2 = 8$

Since $y_A(3) \neq y_B(3)$, they **do not collide**.

## 3. Minimum Distance Calculation
We minimize the squared distance $D(t) = (x_A - x_B)^2 + (y_A - y_B)^2$:

$$
D(t) = (3 - t)^2 + (6 - 5t)^2 = 26t^2 - 66t + 45
$$

Finding the derivative $D'(t)$:

$$
D'(t) = 52t - 66
$$

Setting $D'(t) = 0$:

$$
t = \frac{66}{52} = \frac{33}{26} \approx 1.27
$$

The minimum distance is:

$$
d = \sqrt{D\left(\frac{33}{26}\right)} = \sqrt{\frac{81}{26}} = \frac{9}{\sqrt{26}} \approx 1.765
$$

**Result:** The paths intersect geometrically, but no collision occurs. The minimum distance is **1.765** at $t \approx 1.27$.
