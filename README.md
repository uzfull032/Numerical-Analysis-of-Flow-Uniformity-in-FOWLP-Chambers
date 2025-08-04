
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

You can find the simulation results in the [`FOWLP_Simulation_Summary.pdf`](./FOWLP_Simulation_Summary.pdf) file which includes:

- Velocity and pressure contours
- Graphs of velocity/pressure by radial range
- Comparison between hole and slit inlet designs with/without baffles

---
