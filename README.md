# Tri-Band Cross-Shaped Slotted Patch Antenna

![Antenna Geometry](antenna_structure.png)

## 📌 Project Overview
This project presents a modified microstrip patch antenna capable of **tri-band operation**, designed and simulated in **Ansys HFSS**. While originally based on a dual-band 5G concept, modifications to the Defected Ground Structure (DGS) introduced a third resonance, allowing this single antenna to cover **LTE (4G)**, **5G (n79)**, and **V2X** standards simultaneously.

## 📊 Performance Summary
Unlike standard dual-band designs, this geometry achieves resonance at three distinct communication standards:

| Application | Frequency | S11 Magnitude | Bandwidth Note |
| :--- | :--- | :--- | :--- |
| **LTE / 4G** | **2.05 GHz** | -25 dB | Covers global LTE Mid-bands |
| **5G Sub-6** | **4.85 GHz** | -28 dB | Covers **n79** band (4.4–5.0 GHz) |
| **V2X / DSRC** | **5.90 GHz** | -40 dB | Automotive Safety & IoT |

![S-Parameter Plot](s11_graph.png)

## 🛠️ Design Specs
* **Substrate:** FR-4 ($\epsilon_r = 4.3$, $h = 1.6$ mm)
* **Top Layer:** Theta-shaped radiating patch.
* **Bottom Layer:** Modified Defected Ground Structure (DGS) with a vertical tuning stub.
* **Software:** Ansys HFSS 2025.

## 📂 File Structure
* `Theta_Antenna_Design.aedt`: The Ansys HFSS simulation source file.
* `simulation_data.csv`: Raw S-Parameter data exported from simulation.
* `antenna_structure.png`: 3D model view.
* `s11_graph.png`: Return loss plot from simulation.

## 📜 Attribution
This design is a modified implementation of research presented in:
> *N. A. Nafi et al., "A novel theta-shaped slotted patch antenna with a unique DGS for Sub-6 GHz 5G communication," Results in Engineering, vol. 24, 2024.*
