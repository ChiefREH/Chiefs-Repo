# Calculating Air Receiver Volume (Standard Formula)

We are given:

- Airflow = 500 CFM  
- Drawdown time = 3.25 minutes  
- Pressure band = 12 psig  
- Atmospheric pressure ≈ 14.7 psia  
- Goal: Find air receiver volume in cubic feet (ft³)

---

## Step 1: Understand the formula

The standard formula for sizing an air receiver:

    V = (Airflow × Drawdown Time × Atmospheric Pressure) / Pressure Band

Where:  
- V = receiver volume in cubic feet (ft³)  
- Airflow in CFM (cubic feet per minute)  
- Drawdown time in minutes  
- Pressure Band = ΔP in psig  
- Atmospheric pressure in psia (≈ 14.7 psia)  

> This formula assumes **gauge pressure for the pressure band** and moderate compression.

---

## Step 2: Identify the values

- Airflow = 500 CFM  
- Drawdown = 3.25 minutes  
- Pressure Band = 12 psig  
- Atmospheric Pressure = 14.7 psia

---

## Step 3: Apply the formula

    V = (500 × 3.25 × 14.7) / 12

---

## Step 4: Multiply numerator

    500 × 3.25 = 1,625  
    1,625 × 14.7 ≈ 23,887.5

---

## Step 5: Divide by pressure band

    23,887.5 ÷ 12 ≈ 1,990.63 ft³

---

## Step 6: Include units

    Receiver Volume ≈ 1,990.63 cubic feet

---

## Answer

Air Receiver Volume:

    V ≈ 1,990.63 ft³

---

# Note: Understanding Drawdown Time and Pressure Band

---

## Drawdown Time

- **Definition:** The time it takes for the air receiver (tank) pressure to drop from the **cut-out pressure** (when the compressor stops) to the **cut-in pressure** (when the compressor starts).  
- **Importance:**  
  - Determines how long the system can supply air before the compressor runs again.  
  - Longer drawdown time means the compressor runs less frequently.

**Example:**  

- Compressor cut-out = 120 psig  
- Compressor cut-in = 108 psig  
- Drawdown time = 3 minutes  

> The tank can supply air for 3 minutes while the pressure drops from 120 psig to 108 psig.

---

## Pressure Band

- **Definition:** The difference between the maximum and minimum pressures in the tank — basically **cut-out pressure minus cut-in pressure**.  
- **Importance:**  
  - Determines how much usable air is available per compressor cycle.  
  - A wider pressure band means more air is drawn before the compressor starts again, reducing the number of cycles.

**Example:**  

- Cut-out pressure = 120 psig  
- Cut-in pressure = 108 psig  
- Pressure band = 120 − 108 = 12 psig  

> This is the ΔP used in air receiver sizing formulas.

---

## Putting It Together

- **Drawdown time** tells you **how long the tank can supply air**.  
- **Pressure band** tells you **how much air is available per cycle**.  
- Together, they let you **calculate the required tank volume** so the compressor runs efficiently and air supply is stable.


