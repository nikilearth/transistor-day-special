# transistor-day-special
# Discrete BJT Logic Gates

A hardware-level exploration of digital logic using **NPN Bipolar Junction Transistors (BJTs)**. This project implements fundamental Boolean gates (AND, OR, NOT) using physical switches to demonstrate the bridge between electrical engineering and computer science.

##  Overview
By treating transistors as electronic switches rather than amplifiers, this project verifies truth tables in real-time. Tactile push buttons represent inputs **A** and **B**, while LEDs provide visual output.

---

##  Logic Implementations

### 1. AND Gate (Series)
* **Configuration:** Transistors are wired in series.
* **Logic:** Output is HIGH only if $A$ **and** $B$ are closed.
* **Boolean:** $Y = A \cdot B$

### 2. OR Gate (Parallel)
* **Configuration:** Transistors are wired in parallel.
* **Logic:** Output is HIGH if $A$ **or** $B$ is closed.
* **Boolean:** $Y = A + B$

### 3. NOT Gate (Inverter)
* **Configuration:** The transistor acts as a shunt to ground.
* **Logic:** Output is HIGH only when input $A$ is LOW.
* **Boolean:** $Y = \overline{A}$

---

##  Truth Tables

| Input A | Input B | AND | OR | NOT (A) |
| :---: | :---: | :---: | :---: | :---: |
| 0 | 0 | 0 | 0 | 1 |
| 0 | 1 | 0 | 1 | 1 |
| 1 | 0 | 0 | 1 | 0 |
| 1 | 1 | 1 | 1 | 0 |

---

##  Components
* **Transistors:** 2N2222 (NPN)
* **Resistors:** $10\text{k}\Omega$ (Base), $220\Omega$ (LED)
* **Inputs:** Tactile Push Buttons
* **Power:** 5V DC

##  Key Takeaways
* **Transistor Switching:** Mastering the Saturation and Cutoff regions.
* **Pull-down Resistors:** Preventing floating inputs to ensure stable logic levels.
* **Voltage Drops:** Accounting for the $\approx 0.7\text{V}$ $V_{BE}$ drop in series configurations.

---
*Created for the love of low-level hardware.*
