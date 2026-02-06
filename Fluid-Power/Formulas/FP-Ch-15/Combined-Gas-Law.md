# Calculating Resulting Air Pressure Using the Combined Gas Law

We are given:

- Initial Volume: V1 = 850 in³  
- Initial Pressure: P1 = 325 psig  
- Initial Temperature: T1 = 700 K  
- Final Volume: V2 = 1200 in³  
- Final Temperature: T2 = 400 K  
- Goal: Find final pressure P2 in PSIG

---

## Step 1: Convert initial pressure to absolute

For gas law calculations, we must use **absolute pressure**:

    P1_abs = P1 + Atmospheric Pressure
    P1_abs = 325 + 14.7 ≈ 339.7 psia

---

## Step 2: Use the Combined Gas Law

The combined gas law (for a fixed amount of gas) is:

    (P1 × V1) / T1 = (P2 × V2) / T2

Solve for P2:

    P2_abs = (P1_abs × V1 × T2) / (V2 × T1)

---

## Step 3: Identify the values

- P1_abs = 339.7 psia  
- V1 = 850 in³  
- V2 = 1200 in³  
- T1 = 700 K  
- T2 = 400 K

---

## Step 4: Apply the formula

    P2_abs = (339.7 × 850 × 400) / (1200 × 700)

Step by step:

1. Multiply numerator: 339.7 × 850 ≈ 288,745  
2. Multiply by T2: 288,745 × 400 ≈ 115,498,000  
3. Multiply denominator: 1200 × 700 = 840,000  
4. Divide: 115,498,000 ÷ 840,000 ≈ 137.5 psia

---

## Step 5: Convert back to PSIG

    P2_gauge = P2_abs - Atmospheric Pressure
    P2_gauge = 137.5 - 14.7 ≈ 122.8 psig

---

## Step 6: Include units

    P2 ≈ 122.8 psig

---

## Answer

Resulting Air Pressure:

    P2 ≈ 122.8 psig
---

# Note

- Always convert gauge pressure to absolute before using the gas laws.
- Temperatures must be in Kelvin.
- After solving, convert back to PSIG if required.
