# Probability of Receiving a Letter Sequence via Noisy Channel

## Useful Definitions and Formulas

### 1. Probability of Independent Letters

If letters in a sequence are transmitted **independently**, the probability of receiving a specific sequence given the transmitted sequence is the **product of probabilities** for each letter:

$$
P(\text{received sequence} \mid \text{transmitted sequence}) = \prod_{i=1}^{n} P(\text{received letter}_i \mid \text{transmitted letter}_i)
$$

---

### 2. Total Probability Formula

If several sequences \(S_1, S_2, S_3\) are transmitted with a priori probabilities, the total probability of receiving a specific sequence \(R\) is:

$$
P(R) = \sum_{i=1}^{3} P(R \mid S_i) \, P(S_i)
$$

---

## Given Data

- Transmitted sequences and probabilities:

| Sequence | Probability |
|----------|------------|
| AAAA     | 0.4        |
| BBBB     | 0.3        |
| CCCC     | 0.3        |

- Error probability matrix (per letter):

| Transmitted \ Received | A   | B   | C   |
|-----------------------|-----|-----|-----|
| A                     | 0.8 | 0.1 | 0.1 |
| B                     | 0.1 | 0.8 | 0.1 |
| C                     | 0.1 | 0.1 | 0.8 |

- Received sequence:  

$$
R = AAAACA AA
$$

For clarity, assume the sequence is 8 letters: A, A, A, A, C, A, A, A.

---

## Step 1: Probability Given a Specific Transmitted Sequence

Because letters are independent:

$$
P(R \mid S_i) = \prod_{j=1}^{8} P(\text{received letter}_j \mid \text{transmitted letter}_j)
$$

---

### Step 2: Compute Probability for Each Transmitted Sequence

#### Case 1: Transmitted sequence \(S_1 = AAAA\) (all A’s)

- First 4 letters received as A: probability \(0.8^4\)  
- 5th letter received as C: probability \(0.1\) (A → C)  
- 6th–8th letters received as A: probability \(0.8^3\)  

Multiply:

$$
P(R \mid AAAA) = 0.8^7 \cdot 0.1
$$

---

#### Case 2: Transmitted sequence \(S_2 = BBBB\)

- Letters received as A or C according to table:  
- 1st letter A: \(0.1\) (B → A)  
- 2nd letter A: \(0.1\)  
- 3rd letter A: \(0.1\)  
- 4th letter A: \(0.1\)  
- 5th letter C: \(0.1\) (B → C)  
- 6th–8th letters A: \(0.1^3\)  

Multiply:

$$
P(R \mid BBBB) = 0.1^7 \cdot 0.1 = 0.1^8
$$

---

#### Case 3: Transmitted sequence \(S_3 = CCCC\)

- Letters received as A or C according to table:  
- First 4 letters A: \(0.1^4\) (C → A)  
- 5th letter C: \(0.8\) (C → C)  
- 6th–8th letters A: \(0.1^3\)  

Multiply:

$$
P(R \mid CCCC) = 0.1^7 \cdot 0.8
$$

---

## Step 3: Total Probability

Use total probability formula:

$$
P(R) = P(R \mid AAAA) \cdot 0.4 + P(R \mid BBBB) \cdot 0.3 + P(R \mid CCCC) \cdot 0.3
$$

Substitute values:

$$
P(R) = (0.8^7 \cdot 0.1) \cdot 0.4 + (0.1^8) \cdot 0.3 + (0.1^7 \cdot 0.8) \cdot 0.3
$$

---

### Step 4: Simplify

1. Compute first term: \(0.8^7 \approx 0.2097152\) → multiply by 0.1 → 0.02097152 → multiply by 0.4 → 0.008388608  
2. Second term: \(0.1^8 \cdot 0.3 = 10^{-8} \cdot 0.3 = 3 \cdot 10^{-9}\) (negligible)  
3. Third term: \(0.1^7 \cdot 0.8 = 10^{-7} \cdot 0.8 = 8 \cdot 10^{-8}\) → multiply by 0.3 → 2.4 × 10⁻⁸ (negligible)  

Add:

$$
P(R) \approx 0.008388608
$$

---

## Final Answer

The probability of receiving the sequence \(AAAACA AA\) is approximately:

$$
P(R) \approx 0.00839
$$
