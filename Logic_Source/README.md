# 📂 Logic_Source

This folder contains the primary automation files for the **Multi-Grafcet Coordination** project. The logic is designed to demonstrate deterministic control through a Master/Slave architecture.  

---

### 📄 File Inventory

**TSAII_MultiGrafcet_Coordination_V1.sta**: The primary project archive. This is the most reliable file for opening the project in Schneider Unity Pro / Control Expert.  

**TSAII_MultiGrafcet_Coordination_V1.zef**: A full project export used for comprehensive backups, including application data.  

**TSAII_MultiGrafcet_Coordination_V1.xef**: An XML-based export. This version allows for text-based version tracking of the Grafcet logic and variable definitions.  

---

### ⚙️ Technical Highlights

**Architecture**: Uses a main supervisor chart (GMAITRE) to coordinate the execution of sub-sequences (G1 and G2).  

**Functions Implemented**:

**INITCHART**: High-priority initialization of sequences.  
**FREEZECHART**: State-freezing logic to pause evaluation during anomalies.  
**Data Types**: Implementation of **EBOOL** (Extended Booleans) across all variables to enable diagnostic forcing and history tracking in the animation table.  

---

### 🚀 Usage

To run this project:
1. Open **Schneider Unity Pro / Control Expert**.
2. Go to **File > Restore Archive...** and select the `.sta` file from this folder.
3. Once opened, go to **Build > Rebuild All Project**.
4. Connect to the **PLC Simulator**, transfer the project, and set to **Run**.
5. Use the **Animation Table** to observe the interaction between `GMAITRE` and the slave charts
