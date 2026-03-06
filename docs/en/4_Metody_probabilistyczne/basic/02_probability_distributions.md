# Probability Theory Exercises – Selected Distributions

## Introduction

In many real-world random situations we are interested in the number of occurrences of certain events: defective products in a batch, the number of errors in a text, the waiting time until the first event occurs, or the number of requests in a system. To describe such phenomena mathematically, probability theory uses probabilistic models, also called probability distributions.

Each distribution describes a different type of random experiment and corresponds to different assumptions about how events occur.

In this set of exercises we use five important models:

- **Bernoulli scheme** – describes situations in which an experiment consists of many independent trials and each trial has only two possible outcomes (for example success or failure).
- **Hypergeometric distribution** – used when we draw elements **without replacement** from a finite population containing elements of different types.
- **Geometric distribution** – describes the number of trials needed to obtain the **first success** in a sequence of independent trials.
- **Poisson distribution** – models the number of events occurring within a given time or space interval.
- **Multinomial distribution** – a generalization of the Bernoulli scheme when each trial can result in **more than two possible outcomes**.

The analysis of these models allows us to formally describe random experiments and compute probabilities of events in many practical situations.

---

## Exercises – Probability Theory

### Part I – Modeling and Sample Spaces

#### Exercise 1 – Bernoulli Scheme (Quality Control)

In a factory, screws are produced. Each screw can be either **good** or **defective**.  
The probability that a randomly selected screw is defective equals \(p\).

We consider an experiment consisting of checking **3 consecutive screws**.

**Tasks**

1. Describe the random experiment.  
2. Determine the sample space \( \Omega \).  
3. Specify the probabilities of the elements of the sample space.  
4. Define what is considered a **success** in this model.

---

#### Exercise 2 – Hypergeometric Scheme (Sampling from a Batch)

A warehouse contains **20 components**, of which **5 are defective** and **15 are functional**.

We randomly select **4 components without replacement** for inspection.

**Tasks**

1. Describe the random experiment.  
2. Define the sample space \( \Omega \) as the number of defective elements in the sample.  
3. Determine the possible values of the random variable.  
4. Provide the probability distribution.  
5. Explain what a **success** means in this model.

---

#### Exercise 3 – Geometric Scheme (Waiting for the First Event)

In a printing house, each printed page may contain a **printing error** with probability \(p\).

The experiment consists of observing consecutive pages until the **first error** appears.

**Tasks**

1. Describe the random experiment.  
2. Determine the sample space \( \Omega \).  
3. Provide the probability distribution.  
4. Specify what is considered a success.

---

#### Exercise 4 – Poisson Distribution (Arrival of Events)

A web service receives on average **3 error reports per hour**.

We assume that the number of reports in a given time interval follows a **Poisson distribution**.

**Tasks**

1. Describe the random experiment.  
2. Determine the sample space \( \Omega \).  
3. Provide the formula of the probability distribution.  
4. Interpret the parameter \( \lambda \).

---

#### Exercise 5 – Multinomial Scheme (Categories of Outcomes)

A player rolls a **die 5 times**.

The outcomes are grouped into three categories:

- small numbers (1–2)  
- medium numbers (3–4)  
- large numbers (5–6)

**Tasks**

1. Describe the random experiment.  
2. Define the sample space.  
3. Specify the multinomial distribution.  
4. Explain the interpretation of the parameters.

---

### Part II – Exploration and Calculations

#### Exercise 6 – Bernoulli Scheme

The probability of producing a defective part is **0.04**.

An inspector checks **10 parts**.

Calculate the probability that:

- exactly **2 parts are defective**,  
- **at least one part** is defective.

---

#### Exercise 7 – Hypergeometric Scheme

A box contains:

- 12 working light bulbs  
- 3 defective ones

We draw **5 bulbs without replacement**.

Calculate the probability that the sample contains **exactly 2 defective bulbs**.

---

#### Exercise 8 – Geometric Scheme

The probability of an error in program compilation is **0.1** for each compilation.

A programmer performs consecutive compilations until the **first error** occurs.

Calculate the probability that:

- the first error appears on the **4th compilation**,  
- it appears **no later than the 3rd compilation**.

---

#### Exercise 9 – Poisson Distribution

A customer service center receives on average **5 requests per hour**.

Calculate the probability that during one hour there will be:

- exactly **3 requests**,  
- **at least one request**.

---

#### Exercise 10 – Multinomial Scheme

A box contains candies of three flavors:

- strawberry – 40%  
- lemon – 35%  
- mint – 25%

We randomly select **6 candies independently**.

Calculate the probability that we obtain:

- 3 strawberry  
- 2 lemon  
- 1 mint
