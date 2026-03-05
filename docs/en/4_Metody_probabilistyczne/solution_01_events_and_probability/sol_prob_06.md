# Task 6 – Probability of First-Grade Product from Two Machines

## Useful Definitions and Formulas

### 1. Total Probability Formula

If an event \(A\) (product is first-grade) can occur from multiple sources \(M_1, M_2, \dots\), the total probability is:

$$
P(A) = \sum_{i} P(A \mid M_i) \, P(M_i)
$$

Where:

- \(P(M_i)\) is the probability that the product comes from machine \(i\)  
- \(P(A \mid M_i)\) is the probability that a product from machine \(i\) is first-grade

---

### 2. Bayes' Theorem

To find the probability that a product came from a specific machine given that it is first-grade:

$$
P(M_i \mid A) = \frac{P(A \mid M_i) \, P(M_i)}{P(A)}
$$

---

## Given Data

- Production ratio: \(3:2\) → probabilities:

$$
P(M_1) = \frac{3}{5}, \quad P(M_2) = \frac{2}{5}
$$

- Probability of first-grade product from each machine:

$$
P(A \mid M_1) = \frac{65}{100} = 0.65, \quad P(A \mid M_2) = \frac{85}{100} = 0.85
$$

---

## Step 1: Probability that a randomly selected product is first-grade

Using the total probability formula:

$$
P(A) = P(A \mid M_1) P(M_1) + P(A \mid M_2) P(M_2)
$$

Substitute the values:

$$
P(A) = 0.65 \cdot \frac{3}{5} + 0.85 \cdot \frac{2}{5}
$$

Step-by-step calculation:

$$
0.65 \cdot 0.6 = 0.39
$$

$$
0.85 \cdot 0.4 = 0.34
$$

$$
P(A) = 0.39 + 0.34 = 0.73
$$

---

## Step 2: Probability that the product came from the first machine (Bayes' theorem)

$$
P(M_1 \mid A) = \frac{P(A \mid M_1) P(M_1)}{P(A)}
$$

Substitute values:

$$
P(M_1 \mid A) = \frac{0.65 \cdot 0.6}{0.73} = \frac{0.39}{0.73} \approx 0.534
$$

---

## Final Answers

- Probability that a randomly selected product is first-grade:

$$
P(A) = 0.73
$$

- Probability that a first-grade product was produced by the first machine:

$$
P(M_1 \mid A) \approx 0.534
$$