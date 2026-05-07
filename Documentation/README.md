# 📄 Logic Documentation (PDF Reports)

This folder contains the official project reports exported from **Schneider Control Expert v15**. These documents provide a static, high-resolution view of the Grafcet structures, variables, and code sections without needing the software installed.

---

### 📑 Detailed Logic Breakdown

#### 1. Supervisor Control (Master)
* **[Logic_GMAITRE.pdf](./Logic_GMAITRE.pdf)**: This is the "brain" of the system. It contains the master SFC (Grafcet) that monitors the overall system state and sends synchronization commands to the slave sequences.

#### 2. Sub-Sequences (Slaves)
* **[Logic_G1_Slave.pdf](./Logic_G1_Slave.pdf)**: Detailed logic for the first slave sequence (G1).
* **[Logic_G2_Slave.pdf](./Logic_G2_Slave.pdf)**: Detailed logic for the second slave sequence (G2).

#### 3. Support & Coordination Logic
* **[Logic_Init_LD.pdf](./Logic_Init_LD.pdf)**: The **Ladder Logic (LD)** section. It shows how the `INITCHART` function is triggered to ensure all sequences start from a safe, known state.
* **[Logic_FREEZE_ST.pdf](./Logic_FREEZE_ST.pdf)**: The **Structured Text (ST)** section. It contains the logic for the `FREEZECHART` function, demonstrating how the system can safely pause (freeze) its current state during an anomaly.

---

### 🔍 What to look for in these reports
* **Transitions**: Note the use of timed transitions (e.g., `5s/X..`) and cross-chart synchronization variables.
* **EBOOL Variables**: All variables are defined as **Extended Booleans**, allowing for the advanced diagnostic forcing seen in the `Visuals` folder.
* **Deterministic Flow**: These reports confirm that only one master is directing the flow, preventing conflicting commands to the hardware.

---

> **Note**: These reports were generated using the *Documentation Projet* tool in Control Expert. For the live, editable source code, please refer to the [Logic_Source](../Logic_Source/) folder.
