---
layout: project
title: Thermo Assignment
description: Rigid-bar design, then beam deflection and redesign
technologies: [Goodnotes, Statics, Solid Mechanics]
---

This project involved designing a 2D lifting mechanism within a prescribed design window and then analyzing the same mechanism as a flexible beam. The assignment proceeded in two steps:

1. Rigid-bar lifting mechanism (HW5)  
2. Beam bending and redesign (HW12)

---

## 1. Problem Definition

The mechanism must fit inside a 150 cm × 50 cm envelope and use:

- One bar of fixed length  
- Three pin joints (two grounded)  
- One linear actuator  
- Exactly one degree of freedom  

Goals:

- Maximize lifted mass  
- Maximize vertical lift height  

Modeling assumptions:

- Homework 5: bar is rigid  
- Homework 12: bar is a flexible beam

---

## 2. Design Constraints and Geometry

Actuator:

- Maximum force F_act,max = 36,000 N (36 kN)  
- Stroke s_act = 500 mm  

Bar layout (hockey-stick shaped bar):

- Point A at (–1000, 200) mm  
- Point B at (0, 0) mm  
- Point C at (100, 30) mm  

Segment lengths from this geometry:

- AB length ≈ 1019.8 mm → about 1020 mm  
- BC length ≈ 104.4 mm → about 104 mm  

Total bar length used in the beam model:

- L_total ≈ 1124 mm  

Actuator and load:

- Actuator attached near A  
- Bar pinned at B  
- Payload hangs at C  

These positions match the annotated free-body diagram shown in the project image.

---

## 3. Mechanism Layout and Degree of Freedom

Layout:

- Ground pin at B  
- Bar from A → B → C (two straight segments)  
- Actuator attached at A  
- Payload attached at C  

The actuator length determines the bar angle and the payload height, so the mechanism has **1 degree of freedom**.

---

## 4. Rigid-Bar Static Analysis (HW5)

Goal: determine the **maximum mass** the mechanism can lift if the bar is rigid.

Forces on the bar:

- Downward payload weight: W = m g at C  
- Actuator force: F_act (up to 36 kN) at an angle  
- Reaction at the ground pin at B  

From my free-body diagram:

- Horizontal offset between B and C: 1000 mm  
- Vertical offset used for the actuator moment arm: 200 mm  
- Actuator angle relative to the bar: about 20°  
- Bar orientation around this load case: about 30°  

### 4.1 Moment About B

Using kN·mm units, the scalar moment equilibrium about B that I wrote in my notes is:

- ΣM_B = 1000 (36) sin(20°)  
  + 200 (36) cos(30°)  
  – 1000 m = 0

Here:

- 36 is the actuator force in kN  
- The last term is the payload moment in kN·mm with m in kg (consistent with how I set up the FBD)

Compute each term:

- 1000 × 36 × sin(20°) ≈ 12,312  
- 200 × 36 × cos(30°) ≈ 6,235  

Total actuator moment about B:

- 12,312 + 6,235 ≈ 18,547  

Set equal to the payload moment:

- 1000 m = 18,547  
- m ≈ 18.55 kg  

**Rigid-bar lifting capacity with my actual geometry:**

- **m_max ≈ 18.6 kg**

---

## 5. Rigid-Bar Kinematics (Lift Height)

From my kinematic sketch:

- Start bar angle ≈ 14°  
- End bar angle ≈ 30°  

For the main lifting segment, the vertical position of the payload is approximated as:

- y(θ) = L_bar · sin(θ)  

Using the longer segment as the effective lifting arm (about 1000 mm):

- Δh = L_bar · (sin θ₂ – sin θ₁)  
- L_bar ≈ 1000 mm  
- θ₁ ≈ 14°, θ₂ ≈ 30°  

Result from my calculation:

- Δh ≈ 50.64 mm  

**Rigid-bar lift height: 50.64 mm**

This matches the “50.64 mm high” written on my original solution page.

---

## 6. Observations from the Rigid-Bar Model

- With the current geometry and actuator, the mechanism can lift about **18.6 kg**.  
- The vertical travel of the payload is about **50.64 mm**.  
- Geometry and positions were hand-tuned, not optimized.  
- This model assumes the bar is perfectly rigid; Homework 12 relaxes that assumption.

---

## 7. Beam Model (HW12 – Bar Is Flexible)

For the beam analysis, I treat the bar as a single equivalent beam of length:

- L_total ≈ 1124 mm (sum of AB and BC)

Supports and loads for the beam model:

- Effective supports: near the ground connection at B and at the actuator/payload locations  
- Loads: transverse components of  
  - the actuator force  
  - the payload weight  

Only the **perpendicular components** of these forces contribute to bending.

---

## 8. Beam Properties

For the redesign, I chose a solid round steel bar:

- Diameter d = 40 mm  
- Cross-sectional area:  
  - A = (π d²) / 4 ≈ 1,256.6 mm²  
- Second moment of area:  
  - I = (π d⁴) / 64 ≈ 125,664 mm⁴  
- Young’s modulus:  
  - E = 200,000 N/mm²  
- Beam length for deflection check:  
  - L ≈ 1124 mm  

---

## 9. Equivalent Transverse Loads

Using the limiting rigid-bar case (m ≈ 18.6 kg):

Actuator vertical component:

- P₁ = F_act · sin(20°)  
- F_act = 36,000 N  
- P₁ ≈ 36,000 · sin(20°) ≈ 12,313 N  

Payload vertical component (assuming bar around 30°):

- Payload weight magnitude: m g ≈ 18.6 · 9.81 ≈ 183 N  
- Vertical component using cos(30°):  
- P₂ ≈ 183 · cos(30°) ≈ 158 N  

Total effective transverse load (approximate equivalent at midspan):

- P_eq ≈ P₁ + P₂ ≈ 12,313 + 158 ≈ 12,471 N  

---

## 10. Beam Deflection with Corrected Span

For a simply supported beam with a point load at midspan, maximum vertical deflection is:

- δ_max = (P_eq · L³) / (48 · E · I)

Substitute the values:

- P_eq ≈ 12,471 N  
- L ≈ 1124 mm  
- E = 200,000 N/mm²  
- I ≈ 125,664 mm⁴  

Numerically:

- δ_max ≈ (12,471 · 1124³) / (48 · 200,000 · 125,664)  
- δ_max ≈ 14.7 mm  

Deflection limit (2% of beam length):

- δ_allow = 0.02 · L ≈ 0.02 · 1124 ≈ 22.5 mm  

Comparison:

- δ_max ≈ 14.7 mm  
- δ_allow ≈ 22.5 mm  

So:

- 14.7 mm < 22.5 mm → **deflection is acceptable** for this beam geometry.

---

## 11. Optional Redesign for Mass Reduction

If I wanted to reduce mass further, I could:

1. Compute the required second moment of area I_req by setting δ_max = δ_allow = 0.02 L in the same formula.  
2. Choose a more efficient cross-section (e.g., a thin-walled rectangular tube) such that:  
   - I ≥ I_req  
   - Cross-sectional area A is smaller than 1,256.6 mm²  

That would decrease weight while still keeping deflection within the 2% requirement.

---

## 12. Ways I Could Improve

- Use a more detailed beam model that separates the two segments AB and BC instead of treating them as one equivalent span.  
- Apply beam formulas with the actual load positions (actuator at A, payload at C) rather than a single equivalent midspan load.  
- Perform a full bending stress check using  
  - σ_max = (M_max · c) / I.  
- Optimize actuator and pin locations to increase lifting capacity and reduce deflection.  
- Validate the design using finite element analysis (FEA).

---

## Results

| Feature             | Result                             |
|---------------------|------------------------------------|
| Maximum lifted mass | 18.6 kg                            |
| Lift height         | 50.64 mm                           |
| Beam deflection     | 14.7 mm                            |
| Allowable limit     | ≈ 22.5 mm (2% of 1124 mm span)     |
| Beam used           | 40 mm solid round steel bar        |
