# Reliability of a Parallel Electrical System

## 📘 Useful Definitions and Formulas

## 1. Parallel System Reliability

For two elements connected in **parallel**, the system functions if **at least one element works**.

If  
- $A_1$ — element $a_1$ works at least time $t$  
- $A_2$ — element $a_2$ works at least time $t$  

then the system works if:

$$
A = A_1 \cup A_2
$$

---

### 2. Probability of the Union of Two Events

For any two events:

$$
P(A_1 \cup A_2) = P(A_1) + P(A_2) - P(A_1 \cap A_2)
$$

---

### 3. Given Data

We are given:

$$
P(A_1) = P(A_2) = p
$$

$$
P(A_1 \cap A_2) = p^2
$$

---

# ✅ Step-by-Step Solution

## Step 1: Identify the Required Probability

The system provides continuous current flow for at least time $t$ if **at least one element works**.

Thus, we need:

$$
P(A_1 \cup A_2)
$$

---

## Step 2: Apply the Union Formula

Using the formula:

$$
P(A_1 \cup A_2) = P(A_1) + P(A_2) - P(A_1 \cap A_2)
$$

Substitute the given values:

$$
P(A_1 \cup A_2) = p + p - p^2
$$

---

## Step 3: Simplify

$$
P(A_1 \cup A_2) = 2p - p^2
$$

Factorizing:

$$
P(A_1 \cup A_2) = p(2 - p)
$$

---

# 📌 Final Answer

The probability of continuous current flow for at least time $t$ is:

$$
P(\text{system works}) = 2p - p^2
$$

or equivalently:

$$
P(\text{system works}) = p(2 - p)
$$
