# Projectile Motion: Range Optimization

## Objective
Analytically prove that the maximum horizontal range $R$ of a projectile, for a fixed initial velocity $v_0$, is achieved when the launch angle $\theta$ is $45^\circ$.

## 1. The Range Function
The range of a projectile (ignoring air resistance) is defined by the following function:

$$
R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}
$$

Where:
* $v_0$ is the initial velocity (constant).
* $g$ is the acceleration due to gravity (constant).
* $\theta$ is the launch angle.

## 2. Analytical Proof (Calculus Method)
To find the maximum of a function, we take its first derivative with respect to the variable ($\theta$) and set it to zero to find the critical points.

### Step 1: Differentiate $R(\theta)$
We apply the chain rule to the sine function:

$$
\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \frac{d}{d\theta}[\sin(2\theta)]
$$

$$
\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \cos(2\theta) \cdot 2
$$

$$
\frac{dR}{d\theta} = \frac{2v_0^2 \cos(2\theta)}{g}
$$

### Step 2: Set the derivative to zero
To find the extremum, we set $\frac{dR}{d\theta} = 0$:

$$
\frac{2v_0^2 \cos(2\theta)}{g} = 0
$$

Since $v_0$ and $g$ are non-zero constants, we must have:

$$
\cos(2\theta) = 0
$$

### Step 3: Solve for $\theta$
In the context of projectile motion, the angle $2\theta$ must fall within a physically meaningful range (typically $0^\circ < 2\theta < 180^\circ$). The cosine function is zero at $90^\circ$:

$$
2\theta = 90^\circ
$$

$$
\theta = 45^\circ
$$

## 3. Alternative Proof (Trigonometric Logic)
We can also solve this without calculus by looking at the properties of the sine function.

1.  The formula for range is $R(\theta) = \frac{v_0^2}{g} \sin(2\theta)$.
2.  The maximum value any sine function can achieve is **1**.
3.  Therefore, $R$ is maximized when $\sin(2\theta) = 1$.
4.  The sine of an angle is 1 when the angle is $90^\circ$.
5.  Setting $2\theta = 90^\circ$, we find $\theta = 45^\circ$.

## Conclusion
Both analytical methods confirm that for a given initial velocity, the **maximum range is achieved at a launch angle of 45°**. At this angle, the range becomes:

$$
R_{max} = \frac{v_0^2}{g}
$$
