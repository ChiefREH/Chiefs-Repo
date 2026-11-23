# 5. Pneumatic Formulas – Gas Laws

Pneumatic systems use compressed air or other gases to transmit energy and produce mechanical motion. Unlike hydraulic systems, which use relatively incompressible liquids, pneumatic systems use compressible gases.

The behavior of compressed gases is described by several gas laws. These laws explain how pressure, volume, and temperature affect one another.

Understanding these relationships is important when working with air compressors, receivers, pneumatic actuators, and other compressed-air equipment.

## 5.1 Boyle's Law (Pressure and Volume)

Boyle's Law describes the relationship between the pressure and volume of a gas when temperature and the amount of gas remain constant.

Pressure and volume have an inverse relationship:

- When gas volume decreases, pressure increases.
- When gas volume increases, pressure decreases.

**Formula:**

$P_1 V_1 = P_2 V_2$

Where:

- $P_1$ = Initial absolute pressure
- $V_1$ = Initial volume
- $P_2$ = Final absolute pressure
- $V_2$ = Final volume

Pressure must be expressed as absolute pressure (PSIA), not gauge pressure (PSIG). Volume units must be consistent between the two states.

### Example: Calculating Final Pressure

A sealed container holds air at 30 PSIA with a volume of 10 gallons. The volume is reduced to 5 gallons while temperature remains constant. Calculate the final pressure.

$P_1 V_1 = P_2 V_2$

Solve for final pressure:

$P_2 = \frac{P_1 V_1}{V_2}$

$P_2 = \frac{30 \times 10}{5}$

**Answer: 60 PSIA**

The pressure doubles when the gas volume is reduced by half.

## 5.2 Charles' Law (Volume and Temperature)

Charles' Law describes the relationship between the volume and temperature of a gas when pressure and the amount of gas remain constant.

Volume and absolute temperature have a direct relationship:

- When gas temperature increases, volume increases.
- When gas temperature decreases, volume decreases.

**Formula:**

$\frac{V_1}{T_1} = \frac{V_2}{T_2}$

Where:

- $V_1$ = Initial volume
- $T_1$ = Initial absolute temperature
- $V_2$ = Final volume
- $T_2$ = Final absolute temperature

Temperature must be expressed using an absolute temperature scale:

- Kelvin (K)
- Rankine (°R)

Do not use Fahrenheit or Celsius directly in gas law calculations.

### Temperature Conversions

**Fahrenheit to Rankine:**

$°R = °F + 459.67$

**Celsius to Kelvin:**

$K = °C + 273.15$

### Example: Calculating Final Volume

A gas occupies 10 liters at 300 K. Its temperature increases to 450 K while pressure remains constant. Calculate the new volume.

$\frac{V_1}{T_1} = \frac{V_2}{T_2}$

Solve for final volume:

$V_2 = \frac{V_1 \times T_2}{T_1}$

$V_2 = \frac{10 \times 450}{300}$

**Answer: 15 liters**

The gas volume increases from 10 liters to 15 liters as its absolute temperature increases.

## 5.3 Gay-Lussac's Law (Pressure and Temperature)

Gay-Lussac's Law describes the relationship between the pressure and temperature of a gas when volume and the amount of gas remain constant.

Pressure and absolute temperature have a direct relationship:

- When gas temperature increases, pressure increases.
- When gas temperature decreases, pressure decreases.

**Formula:**

$\frac{P_1}{T_1} = \frac{P_2}{T_2}$

Where:

- $P_1$ = Initial absolute pressure
- $T_1$ = Initial absolute temperature
- $P_2$ = Final absolute pressure
- $T_2$ = Final absolute temperature

Pressure must be expressed as absolute pressure (PSIA), and temperature must be expressed as Kelvin (K) or Rankine (°R).

### Example: Calculating Final Pressure

A sealed air tank contains air at 100 PSIA and 300 K. The temperature increases to 360 K while the tank volume remains constant. Calculate the final pressure.

$\frac{P_1}{T_1} = \frac{P_2}{T_2}$

Solve for final pressure:

$P_2 = \frac{P_1 \times T_2}{T_1}$

$P_2 = \frac{100 \times 360}{300}$

**Answer: 120 PSIA**

The pressure increases from 100 PSIA to 120 PSIA as the absolute temperature increases.

*Note: A sealed, rigid air tank is a practical example of Gay-Lussac's Law. Heating the air increases its pressure because the volume cannot expand.*

## 5.4 Pneumatic Cylinder Force

Pneumatic cylinder force is the pushing or pulling force produced when compressed air acts against the piston inside a cylinder.

The force produced depends on the air pressure and the effective piston area.

**Formula:**

$F = P \times A$

Where:

- $F$ = Force (pounds, lb)
- $P$ = Pressure difference across the piston (PSI)
- $A$ = Effective piston area (in²)

For a typical pneumatic cylinder, the pressure gauge reading (PSIG) can be used when the opposite side of the piston is exhausted to atmospheric pressure.

As with hydraulic cylinders, a single-rod pneumatic cylinder has different effective areas for extension and retraction:

- **Extension force:** Uses the full piston area.
- **Retraction force:** Uses the annular area (piston area minus rod area).

### Example: Calculating Pneumatic Cylinder Extension Force

A pneumatic cylinder has a piston area of 2 in² and operates at 80 PSIG. Calculate its theoretical extension force.

$F = P \times A$

$F = 80 \times 2$

**Answer: 160 lb**

The pneumatic cylinder produces a theoretical extension force of 160 pounds.

*Note: Actual cylinder force is lower because of seal friction, mechanical losses, pressure losses, and any opposing pressure acting on the other side of the piston.*

## 5.5 Understanding the Gas Laws

The three gas laws describe how two properties of a gas change while a third property remains constant.

| Gas Law | Relationship | Constant Property |
|---|---|---|
| Boyle's Law | Pressure and volume | Temperature |
| Charles' Law | Volume and temperature | Pressure |
| Gay-Lussac's Law | Pressure and temperature | Volume |

The important relationships are:

- **Boyle's Law:** Pressure and volume move in opposite directions.
- **Charles' Law:** Volume and temperature move in the same direction.
- **Gay-Lussac's Law:** Pressure and temperature move in the same direction.

## 5.6 Important Concepts

- Gases are compressible, unlike the relatively incompressible liquids used in hydraulic systems.
- Boyle's Law assumes constant temperature and a fixed amount of gas.
- Charles' Law assumes constant pressure and a fixed amount of gas.
- Gay-Lussac's Law assumes constant volume and a fixed amount of gas.
- All three gas laws require absolute pressure when pressure is part of the calculation.
- Use PSIA rather than PSIG for gas law calculations.
- Gas law temperature must be expressed in Kelvin (K) or Rankine (°R).
- Fahrenheit and Celsius must be converted to absolute temperature before performing gas law calculations.
- Pneumatic cylinder force depends on pressure difference across the piston and effective piston area.
- Use full piston area for extension force and annular area for retraction force.
- Actual pneumatic cylinder force is affected by friction, pressure losses, and opposing pressure.

