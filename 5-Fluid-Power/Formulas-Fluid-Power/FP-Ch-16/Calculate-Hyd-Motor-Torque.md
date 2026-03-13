# Calculating Hydraulic Motor Torque

We are given:

- Pressure = 722 psig  
- Motor displacement = 22.7 cubic inches per revolution (in³/rev)  
- Goal: Find torque in inch-pounds (in·lb)

---

## Step 1: Understand the formula

Torque for a hydraulic motor can be calculated using:

    Torque (in·lb) = (Pressure × Displacement) / (2 × π)

Where:  
- Pressure in psia or psig (can use psig for relative torque)  
- Displacement in cubic inches per revolution (in³/rev)  
- 2 × π converts volume/pressure to torque per revolution  

**Note:** This gives torque in **inch-pounds**.

---

## Step 2: Identify the values

- Pressure = 722 psig  
- Displacement = 22.7 in³/rev

---

## Step 3: Apply the formula

    Torque = (722 × 22.7) / (2 × 3.1416)

---

## Step 4: Multiply numerator

    722 × 22.7 ≈ 16,379.4

---

## Step 5: Divide by 2π

    16,379.4 ÷ 6.2832 ≈ 2,608 in·lb

---

## Step 6: Include units

    Torque ≈ 2,608 inch-pounds

---

## Answer

Hydraulic Motor Torque:

    Torque ≈ 2,608 in·lb

---

# Note

- Should we convert PSIG to PSIA for torque?
  - PSIG = gauge pressure (above atmospheric pressure)
  - PSIA = absolute pressure (above vacuum)
  - Hydraulic torque is calculated based on the pressure acting on the motor piston.
  - The piston “feels” the pressure above atmospheric, which is exactly what PSIG measures.
  - The atmospheric pressure is already balanced on the other side of the piston (open reservoir).
- Conclusion: For hydraulic motor torque, you do NOT convert to absolute pressure — PSIG is correct.

