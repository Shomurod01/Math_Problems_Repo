# Reliability of a Series–Parallel Circuit

## Definitions

### 1. Intersection of events

The intersection of events \( A \) and \( B \) means that both events occur.

$$
A \cap B
$$

---

### 2. Union of events

The union of events \( A \) and \( B \) means that at least one of the events occurs.

$$
A \cup B
$$

---

### 3. Series connection rule

If elements are connected in series, the circuit works only if all elements work.

$$
\text{Series works} \Longleftrightarrow A \cap B
$$

---

### 4. Parallel connection rule

If elements are connected in parallel, the circuit works if at least one element works.

$$
\text{Parallel works} \Longleftrightarrow A \cup B
$$

---

## Problem

Element \( a_1 \) is connected in series with a block consisting of two elements \( a_2 \) and \( a_3 \) connected in parallel.

Let

$$
A_i = \{\text{element } a_i \text{ is functional at time } t\}, \quad i = 1,2,3.
$$

Describe the event

$$
A = \{\text{current flow is not interrupted at time } t\}.
$$

---

## Solution

### Step 1 — Parallel block

Since \( a_2 \) and \( a_3 \) are connected in parallel, the block works if at least one of them works:

$$
A_2 \cup A_3
$$

---

### Step 2 — Entire circuit

Element \( a_1 \) is in series with the parallel block.  
Thus, the circuit works if:

- \( a_1 \) works, and  
- the parallel block works.

Therefore,

$$
A = A_1 \cap (A_2 \cup A_3)
$$

---

## Final Answer

$$
A = A_1 \cap (A_2 \cup A_3)
$$