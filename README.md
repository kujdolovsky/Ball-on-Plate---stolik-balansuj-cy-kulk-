# Brake Pedal Design and FEA Simulation for BAJA SAE Vehicle

## Project Overview
This project presents the **design, optimization, and structural verification** of a lightweight brake pedal assembly for a BAJA SAE vehicle.  

A **Finite Element Analysis (FEA)** was conducted to validate structural integrity under realistic loading conditions while maintaining minimal mass and manufacturability.

![Brake pedal CAD model](https://github.com/user-attachments/assets/598a4884-95ae-4fd5-9efe-03baa3ac3c71)
*Figure 1: CAD model of the brake pedal assembly*

---

## Design Objectives
The brake pedal was designed to meet the following engineering requirements:

- Mechanical advantage ratio: **3:1**  
- Maximum applied load: **2 kN**  
- Minimum safety factor: **≥ 1.5**  
- Target mass: **< 300 g**  
- Manufacturable on a **3-axis CNC machine** with simple geometry  

---

## Tools & Technologies
- **CAD Modeling:** Autodesk Inventor / SolidWorks  
- **FEA Simulation:** ANSYS Workbench (Static Structural)  
- **Analysis Type:** Linear static structural analysis  

---

## My Contributions
- Developed **3D CAD model** of the brake pedal  
- Performed **FEA simulation** to verify stress, deformation, and safety factor  
- Optimized geometry for **weight reduction** and **stress distribution**  
- Verified **mass of the pedal assembly** (0.247 kg)  
- Prepared the design for **physical manufacturing**  

---

## Boundary Conditions & Loading
- **Symmetry** applied to reduce computational cost  

### Symmetry
- Only **half of the pedal was modeled** due to symmetry along the vertical plane  
- This approach **reduces computational complexity** and number of elements in the mesh  
- Applied **symmetry boundary condition** on the cut plane to represent the full pedal  

### Supports
- Cylindrical supports at pivot locations  
- Fixed supports at mounting interfaces  

![Boundary conditions](https://github.com/user-attachments/assets/3e04c71b-9af5-4fb3-bb5e-a54dafef58ce)
*Figure 2: Boundary conditions and support locations used in FEA*

### Applied Loads
- **1000 N applied to the half-model**, representing a total load of **2 kN**  
- Contact definitions:
  - Bonded contacts  
  - Frictional contacts (μ = 1.0) between pedal pad and arm  

![Load application](https://github.com/user-attachments/assets/676769ef-24e0-44c9-8a73-44615e678ae1)
*Figure 3: Load application on the brake pedal*

---

## Results

### CAD Model and Design Evolution
![Previous and final pedal versions](https://github.com/user-attachments/assets/83f2363b-c1a9-40f7-8c3f-358056254787)
*Figure 4: Previous and final versions of the pedal designed in Inventor*

### Mesh Convergence
![Final mesh](https://github.com/user-attachments/assets/bbd04676-5a56-4bf8-96f3-06dcb25e55f6)
*Figure 5: Final mesh with 120,295 nodes and 33,088 elements*

### Stress Analysis (von Mises)
![Von-Mises stress distribution](https://github.com/user-attachments/assets/91148a64-c91f-4e4a-884f-d6605f2bc7d1)
*Figure 6: Von-Mises stress distribution; max stress = 102.65 MPa*

### Deformation & Safety Factor
![Total deformation](https://github.com/user-attachments/assets/367ef497-e41c-4bc1-a2ad-05755f7be24d)
*Figure 7: Total deformation under maximum load (~1.07 mm)*

![Safety factor distribution](https://github.com/user-attachments/assets/bfb079a7-5fc2-4953-9d5f-e79bc54f4fc4)
*Figure 8: Minimum safety factor = 1.57*

### Mass Verification
- Total mass: **0.247 kg**  
- ✅ Below target 300 g, competitive with commercial pedals  

---

## Limitations & Sensitivity
- Fully fixed support at pivot leads to local stress up to **131.05 MPa**  
- Results depend on:
  - Contact assumptions  
  - Boundary condition simplifications  
  - Linear material model (no plasticity considered)  

---

## Conclusion
The brake pedal design satisfies all engineering requirements:

- Structural strength ✔️  
- Safety factor ✔️  
- Mass target ✔️  
- Manufacturability ✔️  

The component is **ready for prototyping and physical testing**.
