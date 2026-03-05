# Probability of First-Grade Product from Two Machines

## Useful Definitions and Formulas

### 1. Total Probability Formula

If events \(M_1, M_2, \dots, M_n\) form a partition of the sample space (e.g., which machine produced a product), the probability of an event \(A\) (e.g., product is first-grade) is:

$$
P(A) = \sum_{i=1}^{n} P(A \mid M_i) \, P(M_i)
$$

---

### 2. Bayes' Theorem

The probability that event \(M_i\) occurred given that \(A\) occurred:

$$
P(M_i \mid A) = \frac{P(A \mid M_i) \, P(M_i)}{P(A)}
$$

---

## Given Data

- Ratio of production: \(3:2\) → probabilities:  
  $$
  P(M_1) = \frac{3}{5}, \quad P(M_2) = \frac{2}{5}
  $$
- Probability of first-grade product from each machine:  
  $$
  P(A \mid M_1) = \frac{65}{100} = 0.65, \quad P(A \mid M_2) = \frac{85}{100} = 0.85
  $$

---

## Step 1: Probability of First-Grade Product (Total Probability)

Using the total probability formula:

$$
P(A) = P(A \mid M_1) P(M_1) + P(A \mid M_2) P(M_2)
$$

Substitute the values:

$$
P(A) = 0.65 \cdot \frac{3}{5} + 0.85 \cdot \frac{2}{5}
$$

Calculate step by step:

$$
0.65 \cdot \frac{3}{5} = 0.65 \cdot 0.6 = 0.39
$$

$$
0.85 \cdot \frac{2}{5} = 0.85 \cdot 0.4 = 0.34
$$

$$
P(A) = 0.39 + 0.34 = 0.73
$$

So the probability that a randomly selected product is first-grade is:

$$
P(A) = 0.73
$$

---

## Step 2: Probability that Product Came from the First Machine (Bayes' Theorem)

We need \(P(M_1 \mid A)\):

$$
P(M_1 \mid A) = \frac{P(A \mid M_1) P(M_1)}{P(A)}
$$

Substitute the values:

$$
P(M_1 \mid A) = \frac{0.65 \cdot \frac{3}{5}}{0.73} = \frac{0.39}{0.73} \approx 0.5342
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
