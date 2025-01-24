# Quantum Cloning Attack and Intercept-Resend Attack Analysis

![GitHub](https://img.shields.io/badge/license-MIT-blue) 
![Python](https://img.shields.io/badge/Python-3.7%2B-blue)

This repository contains Python-based analyses of mutual information in the context of **quantum cloning attacks** and **intercept-resend attacks**. The projects explore the relationship between Alice, Bob, and Eve in quantum communication scenarios, focusing on mutual information measures and their dependence on the probability of error.

## Table of Contents
- [Overview](#overview)
- [Key Concepts](#key-concepts)
- [Repository Structure](#repository-structure)
- [Requirements](#requirements)
- [Usage](#usage)
- [Results](#results)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

## Overview

### Quantum Cloning Attack
The `Cloning_Attack.ipynb` notebook analyzes the mutual information between Alice, Bob, and Eve in a quantum cloning attack scenario. It calculates and plots \(I_{AB}\), \(I_{AE}\), and \(I_{BSE}\) as functions of \(P_{error}\).

### Intercept-Resend Attack
The `intrecept_resend.py` script analyzes the mutual information in the context of a quantum intercept-resend attack. It calculates and plots \(I_{AB}\), \(I_{AE}\), and \(I_{BSE}\) as functions of \(P_{error}\).

---

## Key Concepts

### Mutual Information

#### \(I_{AB}\): Mutual Information between Alice and Bob
\[
I_{AB} = \log_2(2 - 0.5 \cdot w) - \left(0.25 \cdot w\right) \cdot \log_2\left(\frac{4}{w} - 1\right)
\]
This measures the correlation between Alice and Bob's shared quantum states.

#### \(I_{AE}\): Mutual Information between Alice and Eve
\[
I_{AE} = 0.5 \cdot \log_2\left(1 - 0.25 \cdot w^2\right) + \left(0.25 \cdot w\right) \cdot \log_2\left(\frac{1 + 0.5 \cdot w}{1 - 0.5 \cdot w}\right)
\]
This measures the correlation between Alice and Eve's cloned quantum states.

#### \(I_{BSE}\): Mutual Information of Bob Superior to Eve
\[
I_{BSE} = I_{AB} - I_{AE}
\]
This represents the advantage Bob has over Eve in terms of mutual information.

### Probability of Error (\(P_{error}\))
The probability that Bob's measurement result differs from Alice's sent state. It is calculated as:
\[]
P_{error} = 0.25 \cdot w
\]
where \(w\) is a parameter related to the quantum state or attack strategy.

---


---

## Requirements

To run the code in this repository, you need the following Python packages:
- **NumPy**: For numerical calculations.
- **Matplotlib**: For plotting the results.

You can install the required packages using the following command:
```bash

---

### Key Changes:
1. Added mathematical expressions for \(I_{AB}\), \(I_{AE}\), and \(I_{BSE}\) in the **Key Concepts** section.
2. Explained the meaning of each formula and its role in the analysis.

---

### How to Use:
1. Copy the updated `README.md` content above.
2. Replace the existing `README.md` file in your repository with this updated version.
3. Commit and push the changes:
   ```bash
   git add README.md
   git commit -m "Added mathematical expressions for I_AB, I_AE, and I_BSE"
   git push origin main
pip install numpy matplotlib
