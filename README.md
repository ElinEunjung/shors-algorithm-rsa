![Python Version](https://img.shields.io/badge/python-3.13.3%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Built with Qiskit](https://img.shields.io/badge/Built%20with-Qiskit-purple)
![Status](https://img.shields.io/badge/status-draft-blue)
![Course](https://img.shields.io/badge/PGR213-Final_Project-blueviolet)
![Oral Exam Ready](https://img.shields.io/badge/Oral_Exam-Ready-success)
[![School](https://img.shields.io/badge/School-Kristiania%20University%20of%20Applied%20Sciences-red)](https://www.kristiania.no/)

# Breaking RSA encryption with Shor's Algorithm - RSA Factorization Demo

simulates Shor’s algorithm using Qiskit to demonstrate how RSA encryption could, in theory, be broken by quantum computer. 

Since **order finding(period estimation)** is the key quantum step in breaking RSA, this project focuses on how a quantum computer can estimate the period `r` (order `r`) of a number `a mod n`  The implementation includes:

- Modular exponentiation as a unitary gate
- Quantum Phase Estimation (QPE)"
- Visualization of circuit behavior for small composite numbers (e.g, `n = 15`)"
- [Optional] "Comparison: Classical vs. Quantum order finding"
- [Optional] "Classical post-processing to factor `n` using the found order `r`"
 
The goal is to illustrate the **quantum speedup** enabled by QPE in Shor's algorithm. 
An optional section shows how full RSA factorization could proceed once the period is known.

⚠️ Due to current hardware limitations, this simulation only works with very small values (e.g., n = 15).

<br>

![Quantum Circuit](images/shor_circuit.png)

**Figure 1:** *QPE-based circuit for estimating the order r of a mod n. (here `2 mod 15`)*

<br><br>

![QPE outcome bar chart](images/shor_circuit_outcome.png)

**Figure 2:** *Bar-chart of measurement outcomes after 100 shots of the QPE circuit*

<br>

---
📢 **Extra**: I shared this project on LinkedIn to reflect on the learning process and connect with others interested in quantum computing.

🔗 [View the post on LinkedIn](https://www.linkedin.com/posts/MY_POST_ID)

