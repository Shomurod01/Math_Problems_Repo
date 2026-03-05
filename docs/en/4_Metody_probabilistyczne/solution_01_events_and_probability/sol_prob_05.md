# Task 5 – Probability of Water Volume in a Concrete Culvert

## Useful Definitions and Formulas

### 1. Complementary Event

The **complement** of an event \(A\), denoted \(A'\), is the event that \(A\) does **not** occur.

$$
P(A') = 1 - P(A)
$$

---

### 2. Union of Two Events

For any two events \(A\) and \(B\):

$$
P(A \cup B) = P(A) + P(B) - P(A \cap B)
$$

---

### 3. Complement of Union (Neither Event Occurs)

The probability that **neither \(A\) nor \(B\) occurs** is the complement of their union:

$$
P(A' \cap B') = 1 - P(A \cup B)
$$

---

## Given Data

- \(P(A) = 0.6\), where \(A = [125, 250]\)  
- \(P(B) = 0.7\), where \(B = (200, 300]\)  
- \(P(A \cup B) = 0.8\)  

We are asked to find:

1. \(P(A')\)  
2. \(P(A \cap B)\)  
3. \(P(A' \cap B')\)

---

## Step 1: Probability of Complementary Event \(A'\)

By the complement rule:

$$
P(A') = 1 - P(A)
$$

Substitute \(P(A) = 0.6\):

$$
P(A') = 1 - 0.6 = 0.4
$$

---

## Step 2: Probability of Intersection \(A \cap B\)

From the union formula:

$$
P(A \cup B) = P(A) + P(B) - P(A \cap B)
$$

Solve for \(P(A \cap B)\):

$$
P(A \cap B) = P(A) + P(B) - P(A \cup B)
$$

Substitute the given values:

$$
P(A \cap B) = 0.6 + 0.7 - 0.8 = 0.5
$$

---

## Step 3: Probability of \(A' \cap B'\) (Neither Event Occurs)

Use the complement of the union:

$$
P(A' \cap B') = 1 - P(A \cup B)
$$

Substitute \(P(A \cup B) = 0.8\):

$$
P(A' \cap B') = 1 - 0.8 = 0.2
$$

---

## Final Answers

$$
P(A') = 0.4
$$

$$
P(A \cap B) = 0.5
$$

$$
P(A' \cap B') = 0.2
$$
