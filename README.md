# Lid-Driven Cavity Flow Simulation using ANSYS Fluent

## Overview

This project demonstrates a classic CFD problem: the **lid-driven cavity flow**. The flow is generated inside a square cavity where the top lid moves at a constant velocity, driving the fluid motion within the cavity. The objective is to simulate the velocity field and understand vortex formation due to shear forces at the moving lid.

---

## Problem Description

- **Geometry:** 1 m × 1 m square cavity.
- **Boundary Conditions:**
  - **Top lid:** Moves horizontally with a constant velocity (e.g., 0.001 m/s).
  - **Other walls:** Stationary with no-slip condition (velocity = 0).
- **Fluid:** Incompressible, Newtonian fluid - water, with standard properties.
- **Flow Regime:** Laminar flow simulated at low Reynolds number.

---

## Software & Tools Used

- **ANSYS Fluent 2025 R2 Student Edition** for simulation and post-processing.
- **Git & GitHub** for version control and project hosting.

---

## Running the Simulation

1. Open the Fluent case file (`.cas`) in ANSYS Fluent.
2. Set solver parameters (pressure-based, steady-state, laminar).
3. Initialize the solution and run the simulation until convergence.
4. Use Fluent post-processing tools to generate velocity contours and streamline plots.
5. Export relevant images and data for analysis.

---

## Key Results

- The velocity contours show the formation of a **primary vortex** in the center of the cavity.
- Smaller **secondary vortices** appear near the bottom corners.
- Velocity magnitude decreases from the moving lid toward stationary walls, consistent with expected physical behavior.
- The simulation results can be compared with benchmark solutions from literature for validation.

---

## Files Description

| File / Folder | Description |
|---------------|-------------|
| `mesh.msh` | Mesh used for simulation |
| `case.cas`, `data.dat` | Main Fluent case and solution files |
| `results.csv` | Exported field data (e.g., velocities, pressure) |
| `*.png` | Visuals of contours, residuals, plots |
| `report.html` | Full simulation report exported from Fluent |
| `journal.wbjn` | Workbench journal file (setup automation, optional) |
| `README.md` | Project overview and structure |

---

## How to Reproduce

1. Open Fluent via ANSYS Workbench or standalone.
2. Load the mesh or `.cas` file.
3. Set up boundary conditions as per report.
4. Initialize and iterate until convergence.
5. Post-process using the included plots or generate your own.

---

## Future Work / Improvements

- Study the effect of varying Reynolds number on vortex structure.
- Implement turbulence models for higher Reynolds number simulations.
- Perform mesh independence studies.
- Automate post-processing using scripting tools.
