# 🎬 Visual Validation (Videos & Screenshots)

This folder contains the live demonstrations of the **Multi-Grafcet Coordination** in action. By viewing these files, you can see the project architecture (Browser), the logic flow, and the diagnostic tools all working together.

---

### 📹 Live Execution Videos

#### 1. Slave Sequences (G1 & G2)
* **Files**: `Video_G1_Operation.mp4` & `Video_G2_Operation.mp4`
* **What to observe**: These videos show the slave charts pulsing through their steps. You can see the browser on the left, confirming the modular structure of the project while the logic executes.

#### 2. Diagnostic Monitoring (Animation Table)
* **File**: `Video_Animation_Table.mp4`
* **What to observe**: A live look at the **EBOOL** variables. This video demonstrates the real-time state changes and the "Forcing" capabilities used to simulate sensor inputs or bypass hardware during testing.

---

### 🖼️ Static Capture

#### Master Supervision (GMaitre)
* **File**: **[Gmaitre Active](./Visuals/GMaitre_Active.jpg)**
* **What it shows**: A high-level snapshot of the supervisor chart. While the slaves are shown in motion in the videos, this capture provides a clear, still view of the Master’s transitions and state management.

---

### 💡 Note on Architecture
As seen in all video captures, the **Project Browser** (Navigateur du projet) remains visible on the left side of the screen. This confirms that all sections (**GMaitre, G1, G2, Init, and FREEZE**) are properly organized within the `MAST` task for deterministic execution.
