# Computational Chemistry: Hückel Theory vs Density Functional Theory (DFT)

This repository presents a **computational chemistry project** that integrates **Python programming**, **quantum theory**, and **molecular orbital analysis**.  
The goal is to compare the effectiveness of **Hückel Molecular Orbital (HMO) theory** and **Density Functional Theory (DFT)** in modeling π-electron systems and UV-Vis absorption spectra of conjugated organic molecules.

---

## 🧠 Overview

This project combines **computer science** and **chemistry** to explore how computational models can predict molecular electronic structures.  
Through both simplified (Hückel) and advanced (DFT) quantum mechanical methods, we analyze molecules such as:

- Ethene  
- Propene  
- Butadiene  
- Cyclobutadiene  
- Cyclopentadienyl radical, cation, and anion  
- Benzene  

---

## ⚙️ Computational Methods

### **1. Hückel Theory (Python Implementation)**  
- Constructed and diagonalized the **Hückel Hamiltonian matrix** using Python.  
- The Hamiltonian represents π orbital interactions between carbon atoms via two parameters:  
  - **α (on-site energy)**  
  - **β (interaction energy)**  
- Solved the **eigenvalue problem** `|H - EI| = 0` to obtain:  
  - **Eigenvalues →** π orbital energies  
  - **Eigenvectors →** molecular orbital coefficients  
- Visualization of π molecular orbitals (Ψ₁, Ψ₂, …) for each compound.

### **2. Density Functional Theory (DFT, WebMO)**  
- Performed DFT calculations using **B3LYP/6-31G** level of theory.  
- Considered **electron–electron interactions** and **exchange–correlation effects**, absent in Hückel theory.  
- Predicted **total molecular energies**, **HOMO–LUMO gaps**, and **UV-Vis absorption transitions**.

---

## 📊 Results Summary

| Molecule | Method | HOMO–LUMO Gap (Ha) | Notes |
|-----------|---------|--------------------|-------|
| **Benzene** | Hückel | 0.286 | Simplified π-only model |
| **Benzene** | DFT | 0.250 | Matches experiment (0.256 Ha) |
| **Butadiene** | Hückel | Stable conjugation | Demonstrates delocalized π bonding |
| **Cyclobutadiene** | Hückel | Degenerate orbitals | Explains antiaromatic instability |
| **Cyclopentadienyl anion** | DFT | Most stable species | Consistent with aromaticity rule |

- **UV-Vis absorption energy:**  
  \( E = \dfrac{hc}{\lambda} = 0.256 \text{ Ha} \)  
  (calculated from 177.8 nm experimental wavelength)
- **Percentage error:**  
  - Hückel: 11.7 %  
  - DFT: 2.3 % → much more accurate  

---

## 🧩 Interpretation

- The **Hückel method** offers fast, approximate insight into conjugated π systems and electronic delocalization.  
- The **DFT method** provides a more realistic representation of molecular electronic structure by including all electron interactions and density effects.  
- The **HOMO–LUMO energy gap** determines the wavelength of light absorbed (UV-Vis spectrum), linking quantum results to observable spectroscopy.  
- Comparing DFT and Hückel predictions illustrates how computational complexity improves chemical accuracy.

---

## 💻 Integration of Computer Science and Chemistry

| Aspect | Computer Science | Chemistry |
|--------|------------------|-----------|
| Model setup | Python matrix construction | Atomic orbital framework |
| Algorithm | Eigenvalue problem solving | Molecular orbital energies |
| Output | Numerical eigenvalues/vectors | Orbital diagrams and spectra |
| Analysis | Data comparison, visualization | Stability and transition prediction |

This project demonstrates how **linear algebra algorithms** in Python directly translate to understanding **chemical bonding, stability, and reactivity** — a true intersection of computing and molecular science.

---

## 🧾 Conclusion

Hückel theory provides a simple and intuitive understanding of conjugated π systems, useful for quick and conceptual calculations.  
In contrast, DFT offers higher accuracy by incorporating electron density and correlation effects.  
By comparing the two, this study highlights how computational chemistry bridges **quantum mechanics, programming, and molecular spectroscopy**, enabling us to simulate and explain experimental results with scientific precision.

---

**Author:** Yixue Zhao
**Course:** CHEM0019 – Computational Chemistry Lab
**Institution:** University College London  
**Keywords:** Computational Chemistry, Hückel Theory, DFT, Python, Molecular Orbitals, UV-Vis, Quantum Simulation
