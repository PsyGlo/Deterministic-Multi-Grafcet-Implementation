# Deterministic-Multi-Grafcet-Implementation

Study and implementation of concurrent SFC (Grafcet) structures using Schneider Unity Pro. This project focuses on Master/Slave coordination using `INITCHART` and `FREEZECHART` functions to manage complex industrial sequences.

---

### 📂 System Architecture (Logic Map)
Since the project is modular, the logic is divided into specialized sections. You can view the specific charts and code below:

*   **[GMaitre](./Documentation/Logic_GMAITRE.pdf)**: The supervisor sequence (Master) that manages the overall mission states.
*   **[G1](./Documentation/Logic_G1_Slave.pdf) & [G2](./Documentation/Logic_G2_Slave.pdf)**: Sub-sequences (Slaves) for handling specific repeated tasks.
*   **[Initialization](./Documentation/Logic_Init_LD.pdf)**: Implemented in **Ladder Logic (LD)** using the `INITCHART` function for safe system resets.
*   **[Freeze Control](./Documentation/Logic_Freeze_ST.pdf)**: Implemented in **Structured Text (ST)** using the `FREEZECHART` function for sequence pausing during anomalies.

---

### ⚙️ Technical Objectives
*   **Deterministic Control**: Ensuring predictable behavior between concurrent sequences.
*   **Multi-Language Integration**: Combining SFC, LD, and ST within a single Unity Pro project.
*   **Professional Diagnostics**: Utilization of `EBOOL` data types for advanced forcing and animation table monitoring.

---

### 🎓 Academic Context
This implementation is part of the **TSAII** (Technicien Supérieur en Automatique et Informatique Industrielle) curriculum. 
*For detailed credits regarding the AFPA source material, please refer to the [CREDITS.md](./CREDITS.md) file.*
