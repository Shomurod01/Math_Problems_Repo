# Reliability of a Series–Parallel Electrical Circuit

## 📌 Useful Definitions and Formulas

## 1. Event
An **event** is a set of outcomes of a random experiment.  
In our case:

- \( A_i \) — event that element \( a_i \) is functional at time \( t \).

---

### 2. Intersection of Events ( ∩ )

The intersection of events \( A \) and \( B \) means **both events occur**.

$$
A \cap B
$$

This represents:  
> Event \( A \) occurs **and** event \( B \) occurs.

---

### 3. Union of Events ( ∪ )

The union of events \( A \) and \( B \) means **at least one of them occurs**.

$$
A \cup B
$$

This represents:  
> Event \( A \) occurs **or** event \( B \) occurs (or both).

---

## 📌 Circuit Structure Analysis

We are given:

- Element \( a_1 \) is connected **in series**
- Elements \( a_2 \) and \( a_3 \) are connected **in parallel**
- \( A_i \) = event that element \( a_i \) is functional at time \( t \)

We must describe event:

> \( A \): "At time \( t \), the current flow through the circuit is not interrupted."

---

## 📌 Step 1 — Series Connection Rule

For elements connected **in series**,  
the current flows only if **all elements work**.

So for series:

$$
\text{Series works} \Longleftrightarrow \text{all components work}
$$

Mathematically (for two elements):

$$
A \cap B
$$

---

## 📌 Step 2 — Parallel Connection Rule

For elements connected **in parallel**,  
the current flows if **at least one element works**.

So for parallel:

$$
\text{Parallel works} \Longleftrightarrow \text{at least one component works}
$$

Mathematically (for two elements):

$$
A \cup B
$$

---

## 📌 Step 3 — Apply to Our Circuit

### 🔹 Parallel Block (a₂ and a₃)

Since \( a_2 \) and \( a_3 \) are in parallel, the block works if:

$$
A_2 \cup A_3
$$

---

### 🔹 Entire Circuit

Element \( a_1 \) is in **series** with the parallel block.

So the whole circuit works if:

- \( a_1 \) works  
AND  
- the parallel block works

Therefore:

$$
A = A_1 \cap (A_2 \cup A_3)
$$

---

## ✅ Final Answer

The event that the current is not interrupted at time \( t \) is:

$$
A = A_1 \cap (A_2 \cup A_3)
$$
