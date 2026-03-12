# Optimization Problem: Maximum Area of a Rectangle

## 1. Necessary Definitions and Formulas

Before solving, we need to establish the mathematical tools required for optimization:

* **The Area of a Rectangle**: For a rectangle with width $w$ and height $h$, the area $A$ is:

$$
A = w \cdot h
$$

* **The First Derivative Test**: To find the local maximum or minimum of a function $f(x)$, we find the critical points where $f'(x) = 0$.
* **The Power Rule**: A fundamental derivative rule used here:

$$
\frac{d}{dx}[x^n] = n x^{n-1}
$$

---

## 2. Problem Setup

We are looking for a rectangle in the **first quadrant** bounded by the curve:

$$
y = 3 - x^2
$$

### Geometry of the Problem
1.  One vertex of the rectangle is at the origin $(0,0)$.
2.  One side lies on the x-axis, and another on the y-axis.
3.  The "upper-right" vertex lies on the curve at some point $(x, y)$.



Since the point $(x, y)$ is on the curve, the height of our rectangle is $y = 3 - x^2$ and the width is simply $x$.

---

## 3. Step-by-Step Solution

### Step 1: Define the Objective Function
We want to maximize the Area ($A$). Substituting the curve equation into the area formula:

$$
A(x) = x \cdot (3 - x^2)
$$

Distributing the $x$:

$$
A(x) = 3x - x^3
$$

### Step 2: Determine the Domain
Since the rectangle is in the first quadrant:
* $x$ must be greater than $0$.
* $y$ must be greater than $0$, which means $3 - x^2 > 0 \implies x < \sqrt{3}$.
* **Domain**: $0 < x < \sqrt{3}$

### Step 3: Find the Critical Points
To find the maximum, we take the derivative of $A(x)$ and set it to zero:

$$
A'(x) = 3 - 3x^2
$$

Setting the derivative to zero:

$$
3 - 3x^2 = 0
$$

$$
3 = 3x^2
$$

$$
1 = x^2
$$

$$
x = 1
$$

*(We ignore $x = -1$ because it is outside our first-quadrant domain).*

### Step 4: Verify the Maximum
Using the second derivative test:

$$
A''(x) = -6x
$$

At $x = 1$, $A''(1) = -6$. Since the second derivative is negative, the function is concave down, confirming that $x = 1$ is a **maximum**.

### Step 5: Calculate Final Dimensions
Now we find the corresponding height ($y$):

$$
y = 3 - (1)^2 = 2
$$

---

## 4. Final Result

The dimensions of the rectangle that yield the maximum area are:
* **Width ($x$):** 1 unit
* **Height ($y$):** 2 units
* **Maximum Area:** $1 \times 2 = 2$ square units.
