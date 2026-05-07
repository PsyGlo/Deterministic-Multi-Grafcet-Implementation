# 🚀 Deterministic Multi-Grafcet Implementation
### Master/Slave Coordination | Schneider Unity Pro (Control Expert)

Study and implementation of concurrent SFC (Grafcet) structures. This project demonstrates high-reliability coordination using `INITCHART` and `FREEZECHART` functions to manage complex industrial sequences with deterministic precision.

![System Preview](./Visuals/GMaitre_Active.png)
*Figure 1: Master/Slave architecture executing in the Control Expert Simulator.*

---

### 🛠 Tech Stack & Tools
* **Software**: Schneider Control Expert v15 (Unity Pro)
* **Languages**: SFC (Grafcet), Ladder Logic (LD), Structured Text (ST)
* **Hardware Target**: Modicon M580 / Simulator
* **Data Standards**: EBOOL (Extended Booleans) for diagnostic traceability

---

### 📂 Logic Architecture (The Map)
The system is modularized to ensure separation of concerns between supervision and execution:

| Component | Language | Description | Documentation |
| :--- | :--- | :--- | :--- |
| **GMAITRE** | SFC | **Master**: Overall mission state & slave sync. | [View PDF](./Documentation/Logic_GMAITRE.pdf) |
| **G1 & G2** | SFC | **Slaves**: Task-specific sub-sequences. | [G1](./Documentation/Logic_G1_Slave.pdf) / [G2](./Documentation/Logic_G2_Slave.pdf) |
| **Initialization** | LD | High-priority reset logic (`INITCHART`). | [View PDF](./Documentation/Logic_Init_LD.pdf) |
| **Freeze Control** | ST | Emergency/Anomaly state management (`FREEZECHART`). | [View PDF](./Documentation/Logic_FREEZE_ST.pdf) |

---

### 📹 Mission Validation (Live)
Watch the logic in motion via the Control Expert Simulator:
* 📺 **[Watch G1/G2 Slave Coordination](./Visuals/Video_G1_Operation.mp4)**
* 📈 **[Watch Real-time Variable Monitoring](./Visuals/Video_Animation_Table.mp4)**

---

### 🚀 Usage / How to Restore
1. 🖥️ **Open** Schneider Unity Pro / Control Expert.
2. 📂 Go to **File > Restore Archive...** and select the `.sta` file from `Logic_Source/`.
3. 🏗️ Go to **Build > Rebuild All Project**.
4. 🔌 Connect to the **PLC Simulator**, transfer, and set to **Run** ▶️.
5. 👁️ Use the **Animation Table** to monitor synchronization and forcing.

---

### 🎓 Academic Context
This implementation is part of the **TSAII** (Technicien Supérieur en Automatique et Informatique Industrielle) curriculum. 
*For detailed credits regarding the AFPA source material, please refer to the [CREDITS.md](./CREDITS.md) file.*
