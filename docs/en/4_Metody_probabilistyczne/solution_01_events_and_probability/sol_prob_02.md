# Task List No. 1 – Random Events and Probability
## 📘 Useful Definitions and Formulas
### 1. Sample Space
The **sample space** is the set of all possible elementary outcomes of a random experiment.
$$
\Omega = \{ \omega_1, \omega_2, \dots, \omega_n \}
$$
---
### 2. Event
An **event** is any subset of the sample space.
$$
A \subseteq \Omega
$$
---
### 3. Union of Events
The union of two events contains all outcomes that belong to **at least one** of the events.
$$
A \cup B = \{ \omega : \omega \in A \text{ or } \omega \in B \}
$$
---
### 4. Intersection of Events
The intersection contains outcomes that belong to **both** events.
$$
A \cap B = \{ \omega : \omega \in A \text{ and } \omega \in B \}
$$
---
### 5. Difference of Events
The difference of events contains outcomes that belong to one event but **not** the other.
$$
A \setminus B = \{ \omega : \omega \in A \text{ and } \omega \notin B \}
$$
---
# ✅ Problem Solution
## Given:
The sample space:
$$
\Omega = \{ \omega_1, \omega_2, \omega_3, \omega_4, \omega_5 \}
$$
Event A:
$$
A = \{ \omega_1, \omega_3, \omega_5 \}
$$
Event B:
$$
B = \{ \omega_2, \omega_3, \omega_4 \}
$$
---
## 1️⃣ Union of Events
We collect all elements that are in **A or B (or both)**.
From A:  
$\omega_1, \omega_3, \omega_5$
From B:  
$\omega_2, \omega_3, \omega_4$
Combine without repetition:
$$
A \cup B = \{ \omega_1, \omega_2, \omega_3, \omega_4, \omega_5 \}
$$
Notice that:
$$
A \cup B = \Omega
$$
---
## 2️⃣ Intersection of Events
=
We find elements common to both A and B.
Common element:
$\omega_3$
Therefore:
$$
A \cap B = \{ \omega_3 \}
$$
---
## 3️⃣ Difference of Events \( B \setminus A \)
We take elements that belong to B but not to A.
Elements of B:
$\omega_2, \omega_3, \omega_4$
Since $\omega_3 \in A$, we remove it.
$$
B \setminus A = \{ \omega_2, \omega_4 \}
$$
---
## 4️⃣ Difference of Events \( A \setminus B \)
We take elements that belong to A but not to B.
Elements of A:
$\omega_1, \omega_3, \omega_5$
Since $\omega_3 \in B$, we remove it.
$$
A \setminus B = \{ \omega_1, \omega_5 \}
$$
---
# 📌 Final Answers
$$
A \cup B = \{ \omega_1, \omega_2, \omega_3, \omega_4, \omega_5 \}
$$
$$
A \cap B = \{ \omega_3 \}
$$
$$
B \setminus A = \{ \omega_2, \omega_4 \}
$$
$$
A \setminus B = \{ \omega_1, \omega_5 \}
$$