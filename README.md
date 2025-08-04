
# 📦 Numerical Analysis of FOWLP Chamber

This repository summarizes the CFD simulation results of internal flow behavior in a soft bake chamber used in Fan-Out Wafer-Level Packaging (FOWLP).

---

## 🔬 Abstract

This study explores the flow characteristics within a soft bake chamber for the Fan-Out Wafer-Level Packaging (FOWLP) process. Using steady-state CFD simulations in ANSYS Fluent, we examined how different inlet shapes (hole/slit) and the inclusion of baffles influence the velocity and pressure distribution across the wafer. The results demonstrate that baffle structures significantly improve flow uniformity and pressure stability, contributing to more reliable thermal processing.

---

## 📐 Mathematical Model

- **Turbulence Model**: Realizable *k–ε* model
-<p align="left"><img width="633" height="166" alt="image" src="https://github.com/user-attachments/assets/9d1e4a75-1fc1-45b3-9253-ed5f16536330" />

- **Boundary Conditions**:
  - Inlet pressure: 100 kPa
  - Outlet pressure: 0.05 or 0.15 kPa
  - Periodic boundary conditions (30°, 45°, 90° sectors)
  - <p align="left"><img width="339" height="282" alt="image" src="https://github.com/user-attachments/assets/b78886ba-3757-4de4-9835-498b0d66b361" />

---

## 📊 Results Overview

| Chamber Type | Baffle | Velocity Avg (m/s) | Pressure Avg (kPa) | Notes |
|--------------|--------|--------------------|---------------------|-------|
| Hole         | ❌     | ~4.4               | ~24                 | High velocity, unstable |
| Hole         | ✅     | ~2.1               | ~80                 | Uniform, stabilized |
| Slit         | ❌     | ~9.1               | ~78.1               | High speed, nonuniform |
| Slit         | ✅     | ~2.4               | ~97.5               | Most stable & uniform |

---

## 🖼️ Representative Figures

<p align="left">
  <img width="604" height="506" alt="image" src="https://github.com/user-attachments/assets/89500a91-83de-4ab3-a72e-067d7cbf63dd" />
  <img width="604" height="506" alt="image" src="https://github.com/user-attachments/assets/3cee4401-174d-43b8-aaa0-fc017c82f17a" />
  <img width="604" height="506" alt="image" src="https://github.com/user-attachments/assets/fca3b40b-6abd-4c67-b389-e31b66078602" />
  <img width="604" height="506" alt="image" src="https://github.com/user-attachments/assets/142be1f9-a73b-4cb9-9636-37b2c2db0b6b" />
</p>

- Velocity and pressure contours
- Graphs of velocity/pressure by radial range
- Comparison between hole and slit inlet designs with/without baffles

---
