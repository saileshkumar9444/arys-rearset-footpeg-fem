# Rearset Footpeg – Static & Fatigue FEA  
### Arys Garage Assignment – Mechanical (Option A)

---

## Candidate Details

**Name:** Sailesh Kumar  
**Program:** B.E. – Industrial Engineering  
**Assignment Track:** Mechanical Design & Analysis  
**Project Title:** Structural Bracket (Rearset Footpeg) – Static Stress & Fatigue Evaluation

---

## Project Overview

This project involves the CAD design and structural verification of a motorcycle rearset footpeg bracket.  
Finite Element Analysis (FEA) was performed to evaluate the component’s ability to withstand real-world rider loads without plastic deformation or fatigue failure.

The work includes:

- CAD modeling of the rearset footpeg bracket
- Static structural FEA
- Displacement and stress evaluation
- Safety factor calculation
- Fatigue life prediction for long-term cyclic loading
- Design improvement recommendations

---

## Objectives

- Design a functional rearset footpeg bracket in CAD  
- Validate structural safety under service loads  
- Ensure stress levels remain below the material yield limit  
- Estimate fatigue life for **500,000 cycles**  
- Identify and recommend design improvements

---

## Software & Tools Used

- **Onshape**
  - CAD modeling
  - Static FEA simulation
  - Fatigue analysis

- **ChatGPT**
  - FEA setup guidance
  - Safety factor and result calculations
  - Report writing assistance
  - Workflow and submission preparation

- **GitHub**
  - Version control and project documentation

---

## AI Usage Documentation

### AI Tools Used
- ChatGPT

### How AI Was Used

AI was used as a learning and technical reference tool to:

- Understand CAD modelling workflow for mechanical components
- Learn correct boundary condition and loading setup for FEA
- Calculate safety factor using von Mises stress values
- Set up fatigue analysis simulation parameters
- Structure technical documentation and reporting format

All guidance provided by AI was manually reviewed and implemented step-by-step during the simulations.

---

### Sample Prompts Used

- "How to model a motorcycle rearset footpeg in CAD?"
- "How to run static structural FEA in Onshape?"
- "How to calculate safety factor from von Mises stress?"
- "How to perform fatigue life analysis for 500,000 cycles?"
- "How to write a professional FEA assignment report?"

---

---

## CAD Model

A detailed 3D CAD model of the rearset footpeg was created consisting of:

- Base mounting plate  
- Bolt holes for chassis mounting  
- Cylindrical footpeg shaft  
- Edge fillets for reduced stress concentration

### CAD File Included

- `Rearset_Footpeg.step`

---

---

## Material Properties

**Material Used:** Aluminium 6061-T6

| Property              | Value |
|------------------------|--------|
| Density                | 2700 kg/m³ |
| Young’s Modulus        | 69 GPa |
| Poisson’s Ratio        | 0.33 |
| Yield Strength         | **275 MPa** |

---

---

## Static FEA Methodology

### Boundary Conditions

- **Bolt mounting holes:** Fully fixed
- **Vertical Load:** 1.8 kN downward at peg end
- **Lateral Load:** 0.5 kN side load

### Meshing

- Automatic tetrahedral mesh
- Higher refinement near bolt holes and peg-base junction

### Outputs

- Von-Mises stress distribution
- Displacement magnitude field

---

---

## Static Analysis Results

| Parameter | Result |
|----------|----------|
| **Maximum Von Mises Stress** | **192 MPa** |
| **Maximum Displacement** | **1.61 mm** |
| **Material Yield Strength** | **275 MPa** |
| **Calculated Safety Factor** | **1.43 (Marginally Safe)** |

### Safety Factor Calculation

\[
Safety\ Factor = \frac{275\ \text{MPa}}{192\ \text{MPa}} = \mathbf{1.43}
\]

---

### Assessment

The maximum stress remains well below the aluminium yield strength.  
The safety factor of **1.43** indicates the design is structurally adequate and suitable for operating conditions, though it lies within the marginal safety range.

The deformation observed (**1.61 mm**) remains within acceptable limits for rider comfort and component function.

---

---

## Fatigue Analysis

### Simulation Parameters

- Loading Type: Cyclic
- Stress Ratio: R = 0
- Load Range: 0 – 1.8 kN
- Target Design Life: **500,000 cycles**

### Results

| Parameter | Value |
|-----------|--------|
| Minimum Predicted Life | **≥ 500,000 cycles** |
| Critical Region | Peg-to-base junction |
| Fatigue Status | ✅ PASS |

The optimized design meets the fatigue durability requirement for extended operating conditions.

---

---

## Design Improvements

The following enhancements were implemented or proposed:

1. Addition of fillets at high stress regions to reduce concentration effects  
2. Slight increase in base plate thickness to improve bending stiffness

These improvements provided stress reduction and increased fatigue reliability.

---

---

## Repository Structure

