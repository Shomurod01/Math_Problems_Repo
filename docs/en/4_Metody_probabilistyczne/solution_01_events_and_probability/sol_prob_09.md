# Probability of First-Quality Item from Three Plants

## Useful Definitions and Formulas

## 1. Probability of Independent Events

If events are independent, the probability that **all occur** is the product of their probabilities:

$$
P(A_1 \cap A_2 \cap \dots \cap A_n) = P(A_1) \cdot P(A_2) \cdot \dots \cdot P(A_n)
$$

---

### 2. Complementary Event

The probability that **at least one occurs** can also be found using the complement:

$$
P(\text{at least one event fails}) = 1 - P(\text{all succeed})
$$

---

## Given Data

Three plants produce items independently:

| Plant | Probability of First-Quality Item |
|-------|----------------------------------|
| 1     | 0.97                             |
| 2     | 0.90                             |
| 3     | 0.86                             |

We randomly select **one item from each plant**, and we want the probability that **all three items are first-quality**.

---

## Step 1: Probability that all three items are first-quality

Using independence:

$$
P(\text{all first-quality}) = P_1 \cdot P_2 \cdot P_3
$$

Substitute the values:

$$
P(\text{all first-quality}) = 0.97 \cdot 0.90 \cdot 0.86
$$

Calculate step by step:

1. \(0.97 \cdot 0.90 = 0.873\)  
2. \(0.873 \cdot 0.86 \approx 0.75078\)

---

## Final Answer

$$
P(\text{all first-quality}) \approx 0.751
$$
