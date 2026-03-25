# Relative Velocity Problem: Boat Crossing a River

This document provides a step-by-step solution for calculating the heading and time required for a boat to cross a flowing river directly.

## 1. Key Definitions and Formulas

Before solving, let's establish the physical framework:

* **Relative Velocity:** The velocity of an object $A$ as observed from the reference frame of object $B$.
* **Vector Addition:** The resultant velocity of the boat relative to the earth ( $\vec{v} _ {b/e}$ ) is the vector sum of the boat's velocity relative to the water ($\vec{v} _ {b/w}$) and the water's velocity relative to the earth ($\vec{v} _ {w/e}$).

### The Fundamental Formula

$$
\vec{v}_{b/e} = \vec{v}_{b/w} + \vec{v}_{w/e}
$$

In this scenario:
* $v_{w/e} = 2 \text{ m/s}$ (East)
* $v_{b/w} = 5 \text{ m/s}$ (Speed of the boat in still water)
* $v_{b/e}$ must be directed **directly North**.

---

## 2. Problem Solution



### Step 1: Determine the Heading Angle ($\theta$)

To move directly North, the boat must aim **upstream** (West of North) to cancel out the river's eastward push. This forms a right-angled triangle where:
* The hypotenuse is the boat's speed in still water ($v_{b/w} = 5 \text{ m/s}$).
* The opposite side (horizontal) must equal the river's speed to cancel it ($v_{w/e} = 2 \text{ m/s}$).

Using trigonometry ($\sin \theta = \frac{\text{Opposite}}{\text{Hypotenuse}}$):

$$
\sin(\theta) = \frac{v_{w/e}}{v_{b/w}} = \frac{2}{5}
$$

$$
\theta = \arcsin(0.4) \approx 23.58^\circ
$$

**Direction:** The boat should head **$23.58^\circ$ West of North**.

---

### Step 2: Calculate the Resultant Velocity ($v_{b/e}$)

The actual speed at which the boat moves North is the adjacent side of our velocity triangle. We can use the Pythagorean theorem:

$$
v_{b/e}^2 + v_{w/e}^2 = v_{b/w}^2
$$

$$
v_{b/e} = \sqrt{5^2 - 2^2} = \sqrt{25 - 4} = \sqrt{21}
$$

$$
v_{b/e} \approx 4.58 \text{ m/s}
$$

---

### Step 3: Calculate the Time to Cross

Since the boat is moving directly North at $v_{b/e}$, and the width of the river ($d$) is 200 meters, we use the basic motion formula:

$$
t = \frac{d}{v_{b/e}}
$$

$$
t = \frac{200}{\sqrt{21}} \approx \frac{200}{4.5826}
$$

$$
t \approx 43.64 \text{ seconds}
$$

---

## 3. Final Results Summary

| Parameter | Value |
| :--- | :--- |
| **Heading Direction** | $23.58^\circ$ West of North |
| **Resultant Speed** | $\approx 4.58 \text{ m/s}$ |
| **Time to Cross** | $\approx 43.64 \text{ s}$ |
