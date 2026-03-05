# Probability of Receiving Signals with Interference

## Useful Definitions and Formulas

## 1. Conditional Probability for Independent Symbols

If each symbol is independently transmitted and may flip due to interference:

$$
P(\text{received symbol} \mid \text{sent symbol}) =
\begin{cases}
1 - p_e & \text{if symbol is received correctly} \\
p_e & \text{if symbol is flipped}
\end{cases}
$$

where \(p_e\) is the error probability.

---

### 2. Probability of Receiving a Code

For a code of length 3 (symbols independent):

$$
P(\text{received code} \mid \text{sent code}) = \prod_{i=1}^{3} P(\text{received symbol}_i \mid \text{sent symbol}_i)
$$

---

### 3. Total Probability Formula

If \(S_1, S_2\) are the possible sent signals with a priori probabilities \(P(S_1)\) and \(P(S_2)\):

$$
P(\text{received code}) = P(\text{received code} \mid S_1) P(S_1) + P(\text{received code} \mid S_2) P(S_2)
$$

---

## Given Data

- Sent signals and probabilities:  
  $$
  S_1 = 111, \quad P(S_1) = 0.65
  $$  
  $$
  S_2 = 000, \quad P(S_2) = 0.35
  $$

- Symbol error probability: \(p_e = 0.2\)  

- Symbols are independent.

---

## Step 1: Probability of Receiving 111

### Case 1: Sent 111

- Probability all three 1s are received correctly:

$$
P(111 \mid 111) = (1 - 0.2)^3 = 0.8^3 = 0.512
$$

### Case 2: Sent 000

- Probability all three 0s are flipped to 1:

$$
P(111 \mid 000) = 0.2^3 = 0.008
$$

### Total Probability

$$
P(\text{received 111}) = 0.512 \cdot 0.65 + 0.008 \cdot 0.35
$$

$$
P(\text{received 111}) = 0.3328 + 0.0028 = 0.3356
$$

---

## Step 2: Probability of Receiving 000

### Case 1: Sent 111

- Probability all three 1s flip to 0:

$$
P(000 \mid 111) = 0.2^3 = 0.008
$$

### Case 2: Sent 000

- Probability all three 0s are received correctly:

$$
P(000 \mid 000) = 0.8^3 = 0.512
$$

### Total Probability

$$
P(\text{received 000}) = 0.008 \cdot 0.65 + 0.512 \cdot 0.35
$$

$$
P(\text{received 000}) = 0.0052 + 0.1792 = 0.1844
$$

---

## Step 3: Probability of Receiving 010

### Case 1: Sent 111

- Probability to receive 0,1,0 given 111:

$$
P(010 \mid 111) = 0.2 \cdot 0.8 \cdot 0.2 = 0.032
$$

### Case 2: Sent 000

- Probability to receive 0,1,0 given 000:

$$
P(010 \mid 000) = 0.8 \cdot 0.2 \cdot 0.8 = 0.128
$$

### Total Probability

$$
P(\text{received 010}) = 0.032 \cdot 0.65 + 0.128 \cdot 0.35
$$

$$
P(\text{received 010}) = 0.0208 + 0.0448 = 0.0656
$$

---

## Final Answers

- Probability of receiving 111:

$$
P(111) = 0.3356
$$

- Probability of receiving 000:

$$
P(000) = 0.1844
$$

- Probability of receiving 010:

$$
P(010) = 0.0656
$$

