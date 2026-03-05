# Probability of Receiving Pulses in Random Order

## Useful Definitions and Formulas

### 1. Probability of an Event

If all outcomes are equally likely:

$$
P(E) = \frac{\text{Number of favorable outcomes}}{\text{Total number of outcomes}}
$$

---

### 2. Random Selection Without Replacement

For sequential events without replacement:

- Probability of first event \(E_1\): 

$$
P(E_1) = \frac{\text{number of favorable items}}{\text{total items}}
$$

- Probability of second event \(E_2\) given first: 

$$
P(E_2 \mid E_1) = \frac{\text{remaining favorable items}}{\text{remaining total items}}
$$

- Probability of sequence \(E_1, E_2\): 

$$
P(E_1 \text{ then } E_2) = P(E_1) \cdot P(E_2 \mid E_1)
$$

---

## Given Data

- Total pulses: 7  
  $$
  4 \text{ of type } A, \quad 2 \text{ of type } B, \quad 1 \text{ of type } C
  $$

- Random arrangement.

---

## Step 1: Probability that the first received pulse is \(A\)

There are 4 \(A\) pulses out of 7 total:

$$
P(\text{first pulse } A) = \frac{4}{7}
$$

---

## Step 2: Probability that the first received pulse is \(A\) or \(C\)

- Number of favorable pulses: 4 \(A\) + 1 \(C\) = 5  

$$
P(\text{first pulse } A \text{ or } C) = \frac{5}{7}
$$

---

## Step 3: Probability that the first two pulses are \(A\) and \(C\) in that order

- Step 1: First pulse is \(A\): \(4/7\)  
- Step 2: Second pulse is \(C\) given first was \(A\): \(1/6\) (since 1 \(C\) out of remaining 6 pulses)

Multiply:

$$
P(\text{first } A \text{ then } C) = \frac{4}{7} \cdot \frac{1}{6} = \frac{4}{42} = \frac{2}{21} \approx 0.0952
$$

---

## Final Answers

- Probability first pulse is \(A\):

$$
P(\text{first pulse } A) = \frac{4}{7} \approx 0.571
$$

- Probability first pulse is \(A\) or \(C\):

$$
P(\text{first pulse } A \text{ or } C) = \frac{5}{7} \approx 0.714
$$

- Probability first two pulses are \(A\) then \(C\):

$$
P(\text{first } A \text{ then } C) = \frac{2}{21} \approx 0.095
$$
