# Essential Fluid Power Formulas

## 1. Pressure, Force, and Area

- **Pressure:** $P = \frac{F}{A}$
- **Force:** $F = P \times A$
- **Area:** $A = \frac{F}{P}$

### Pressure Measurement

- **Gauge Pressure (PSIG):** Pressure measured relative to atmospheric pressure. Commonly used for hydraulic and pneumatic system operating pressure and cylinder force calculations.
- **Absolute Pressure (PSIA):** Pressure measured relative to a perfect vacuum. Used in gas law calculations involving pressure.

**Pressure Conversions:**

- **Gauge to Absolute:** $PSIA = PSIG + 14.7$
- **Absolute to Gauge:** $PSIG = PSIA - 14.7$

*Note: 14.7 PSI represents approximate atmospheric pressure at sea level.*

## 2. Hydraulic Cylinder Formulas

- **Piston Area:** $A_p = \frac{\pi D^2}{4}$
- **Rod Area:** $A_r = \frac{\pi d^2}{4}$
- **Annular Area (Rod-Side Area):** $A_a = A_p - A_r$
- **Extension Force:** $F = P \times A_p$
- **Retraction Force:** $F = P \times A_a$
- **Cylinder Volume:** $V = A \times L$

## 3. Flow and Speed

- **Flow Rate:** $Q = \frac{V}{t}$
- **Fluid Velocity:** $v = \frac{Q}{A}$
- **Cylinder Extension Speed:** $v = \frac{Q}{A_p}$
- **Cylinder Retraction Speed:** $v = \frac{Q}{A_a}$
- **Cylinder Cycle Time:** $t = \frac{V}{Q}$

## 4. Hydraulic Power

- **Hydraulic Horsepower:** $HP = \frac{PSI \times GPM}{1714}$
- **Mechanical Horsepower:** $HP = \frac{F \times v}{550}$
- **System Efficiency:** $\eta = \frac{Output}{Input} \times 100$

## 5. Pneumatic Formulas – Gas Laws

- **Boyle's Law (Pressure and Volume):** $P_1 V_1 = P_2 V_2$
- **Charles' Law (Volume and Temperature):** $\frac{V_1}{T_1} = \frac{V_2}{T_2}$
- **Gay-Lussac's Law (Pressure and Temperature):** $\frac{P_1}{T_1} = \frac{P_2}{T_2}$
- **Pneumatic Cylinder Force:** $F = P \times A$

## 6. Fluid Properties

- **Density:** $\rho = \frac{m}{V}$
- **Specific Gravity:** $SG = \frac{\text{Fluid Density}}{\text{Water Density}}$

## Basic Units of Measurement

| Measurement | Unit |
|---|---|
| Pressure | PSI (PSIG or PSIA) |
| Force | Pounds (lb) |
| Area | Square inches (in²) |
| Flow Rate | Gallons per minute (GPM) |
| Volume | Gallons (gal) or cubic inches (in³) |
| Distance | Inches (in) |
| Velocity | Inches per second (in/s) |
| Time | Seconds (s) |
| Power | Horsepower (HP) |
| Temperature | °F, °C, °R, or K |
| Density | lb/in³ or kg/m³ |

## Important Calculation Notes

- Hydraulic and pneumatic cylinder force calculations generally use gauge pressure (PSIG).
- Gas law calculations involving pressure require absolute pressure (PSIA), not gauge pressure (PSIG).
- Gas law temperature must be expressed in absolute temperature units: Rankine (°R) or Kelvin (K).
- **Fahrenheit to Rankine:** $°R = °F + 459.67$
- **Celsius to Kelvin:** $K = °C + 273.15$
- Cylinder retraction force uses annular area (piston area minus rod area).
- The hydraulic horsepower formula uses PSI and GPM.
- The mechanical horsepower formula uses force in pounds and velocity in feet per second.
- Maintain consistent units throughout calculations.

## Clarification

- Charles' Law assumes constant pressure, while Gay-Lussac's Law assumes constant volume.
- Boyle's Law assumes constant temperature.
