# Calculating Output Pressure of a Hydraulic Intensifier

We are given:

- Piston bore diameter = 2.5 inches  
- Rod diameter = 1 inch  
- Input air pressure = 600 psig  
- Goal: Find output hydraulic pressure (psig)

---

## Step 1: Understand the formula

For a **single-rod hydraulic intensifier**, the output pressure is determined by the **ratio of piston area to rod area**:

    P_out = P_in × (Piston Area / Rod Area)

Where:  
- P_out = output pressure (psig)  
- P_in = input pressure (psig)  
- Piston Area = π × (D_bore / 2)²  
- Rod Area = π × (D_rod / 2)²  

> This formula assumes a **single-stage intensifier**.  

---

## Step 2: Calculate piston area

    D_bore = 2.5 in → radius = 2.5 / 2 = 1.25 in

    A_piston = π × (1.25)² ≈ 3.1416 × 1.5625 ≈ 4.9087 in²

---

## Step 3: Calculate rod area

    D_rod = 1 in → radius = 1 / 2 = 0.5 in

    A_rod = π × (0.5)² ≈ 3.1416 × 0.25 ≈ 0.7854 in²

---

## Step 4: Calculate area ratio

    Area Ratio = A_piston / A_rod
    Area Ratio = 4.9087 / 0.7854 ≈ 6.25

---

## Step 5: Calculate output pressure

    P_out = P_in × Area Ratio
    P_out = 600 × 6.25 ≈ 3,750 psig

---

## Step 6: Include units

    Output Pressure ≈ 3,750 psig

---

## Answer

Final Pressure Output of Intensifier:

    P_out ≈ 3,750 psig

---

# Note

- Simple analogy
  - Imagine a garden hose with a narrow nozzle:
  - Water flows in at normal pressure.
  - The narrow nozzle “intensifies” the pressure, so it shoots out faster.
  - A hydraulic intensifier does the same thing for fluid pressure, but it’s precise and controlled.

- Key takeaway
  - “Intensifier” = device that increases pressure
  - It doesn’t change flow in proportion — it trades flow for higher pressure.
  - Essential in hydraulic systems where high pressure is needed from a lower-pressure source.

