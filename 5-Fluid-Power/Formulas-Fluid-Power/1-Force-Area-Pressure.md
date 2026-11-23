# 1. Pressure, Force, and Area

Pressure, force, and area are fundamental concepts in fluid power systems. These three quantities are directly related and determine how hydraulic and pneumatic systems generate and transmit force.

Understanding the relationship between them is essential when calculating cylinder force, selecting components, and troubleshooting fluid power systems.

## 1.1 Pressure

Pressure is the amount of force applied over a given area.

**Formula:**

$P = \frac{F}{A}$

Where:

- $P$ = Pressure (PSI)
- $F$ = Force (pounds, lb)
- $A$ = Area (square inches, in²)

In a hydraulic or pneumatic system, pressure is created when resistance acts against the movement of a fluid. A pump or compressor supplies the energy needed to move the fluid, while resistance to that movement allows pressure to develop.

### Gauge Pressure vs. Absolute Pressure

Pressure can be measured using two different reference points.

**Gauge Pressure (PSIG)**

Gauge pressure measures pressure relative to the surrounding atmospheric pressure. It is the measurement commonly displayed on hydraulic and pneumatic pressure gauges.

- A reading of 0 PSIG means the pressure is equal to atmospheric pressure.
- A reading of 100 PSIG means the pressure is 100 PSI above atmospheric pressure.
- Gauge pressure is generally used for hydraulic and pneumatic cylinder force calculations when the opposite side of the piston is exposed to atmospheric pressure.

**Absolute Pressure (PSIA)**

Absolute pressure measures pressure relative to a perfect vacuum.

- A perfect vacuum is 0 PSIA.
- At sea level, atmospheric pressure is approximately 14.7 PSIA.
- Absolute pressure is required for gas law calculations because those calculations must use pressure measured from a true zero reference.

**Pressure Conversions:**

- Gauge to Absolute: $PSIA = PSIG + 14.7$
- Absolute to Gauge: $PSIG = PSIA - 14.7$

*Note: 14.7 PSI is the approximate atmospheric pressure at sea level. Actual atmospheric pressure changes with altitude and weather conditions.*

### Example: Converting Gauge Pressure to Absolute Pressure

A pneumatic system pressure gauge reads 100 PSIG. What is the equivalent absolute pressure?

$PSIA = PSIG + 14.7$

$PSIA = 100 + 14.7$

**Answer: 114.7 PSIA**

## 1.2 Force

Force is the push or pull produced by pressure acting on a surface.

In a hydraulic cylinder, fluid pressure acts against the piston area to produce linear force. Increasing pressure or increasing piston area increases the theoretical force produced by the cylinder.

**Formula:**

$F = P \times A$

Where:

- $F$ = Force (pounds, lb)
- $P$ = Pressure (PSI)
- $A$ = Area (square inches, in²)

For typical cylinder force calculations, use gauge pressure when the opposite side of the piston is vented to atmosphere. More generally, the force is determined by the pressure difference across the piston.

### Example: Calculating Cylinder Force

A hydraulic cylinder has a piston area of 4 square inches. The system pressure is 1,000 PSIG. Calculate the theoretical extension force.

$F = P \times A$

$F = 1,000 \times 4$

**Answer: 4,000 lb**

The cylinder produces a theoretical extension force of 4,000 pounds.

*Note: Actual cylinder force may be lower due to friction, mechanical losses, and pressure acting on the opposite side of the piston.*

## 1.3 Area

Area is the surface over which fluid pressure acts. In fluid power systems, piston area is especially important because it determines how much force a cylinder can produce at a given pressure.

**Formula:**

$A = \frac{F}{P}$

Where:

- $A$ = Area (square inches, in²)
- $F$ = Force (pounds, lb)
- $P$ = Pressure (PSI)

### Example: Calculating Required Piston Area

A hydraulic cylinder must produce 6,000 pounds of theoretical force at 1,500 PSIG. Calculate the required piston area.

$A = \frac{F}{P}$

$A = \frac{6,000}{1,500}$

**Answer: 4 in²**

The cylinder requires a piston area of 4 square inches.

## 1.4 Understanding the Relationship

Pressure, force, and area are directly related:

- Increasing pressure increases force when area remains constant.
- Increasing area increases force when pressure remains constant.
- Increasing the required force requires increasing pressure, area, or both.

The three formulas are different arrangements of the same relationship:

| Quantity | Formula           |
| -------- | ----------------- |
| Pressure | $P = \frac{F}{A}$ |
| Force    | $F = P \times A$  |
| Area     | $A = \frac{F}{P}$ |

## 1.5 Important Concepts

- **PSIG** is commonly used for hydraulic and pneumatic operating pressure and typical cylinder force calculations.
- **PSIA** is required for gas law calculations.
- Gas law calculations must also use absolute temperature: Rankine (°R) or Kelvin (K).
- The pressure used in a cylinder force calculation represents the pressure difference across the piston. If pressure exists on both sides, account for both sides when determining net force.
- The formulas calculate theoretical force. Actual output force can be reduced by friction, mechanical losses, and other system conditions.
- Maintain consistent units throughout calculations.
