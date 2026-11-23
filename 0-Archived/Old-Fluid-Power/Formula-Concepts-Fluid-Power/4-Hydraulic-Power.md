# 4. Hydraulic Power

Power is the rate at which work is performed or energy is transferred. In hydraulic systems, power describes how quickly hydraulic energy is delivered by the fluid and converted into mechanical work.

Hydraulic power depends on both pressure and flow rate. Pressure determines the amount of force the system can produce, while flow rate determines how quickly the fluid moves.

Understanding hydraulic power is important when selecting pumps, motors, cylinders, and other system components.

## 4.1 Hydraulic Horsepower

Hydraulic horsepower is the power transferred by pressurized hydraulic fluid. It is calculated using system pressure and flow rate.

**Formula:**

$HP = \frac{PSI \times GPM}{1714}$

Where:

- $HP$ = Hydraulic horsepower
- $PSI$ = Hydraulic pressure (PSI)
- $GPM$ = Flow rate (gallons per minute)
- $1714$ = Conversion constant

The formula calculates the theoretical hydraulic power available in the fluid. It does not account for losses in the pump, motor, or other system components.

Higher pressure or greater flow rate increases hydraulic horsepower.

### Example: Calculating Hydraulic Horsepower

A hydraulic system operates at 2,000 PSI and has a flow rate of 10 GPM. Calculate the hydraulic horsepower.

$HP = \frac{PSI \times GPM}{1714}$

$HP = \frac{2,000 \times 10}{1714}$

$HP = \frac{20,000}{1714}$

**Answer: 11.67 HP**

The hydraulic fluid delivers approximately 11.67 horsepower.

*Note: This is theoretical hydraulic output power. The pump requires more mechanical input horsepower because of efficiency losses.*

## 4.2 Mechanical Horsepower

Mechanical horsepower describes the rate at which mechanical work is performed.

In a hydraulic system, mechanical horsepower can be calculated when the force produced by a cylinder or other mechanical device and its velocity are known.

**Formula:**

$HP = \frac{F \times v}{550}$

Where:

- $HP$ = Mechanical horsepower
- $F$ = Force (pounds, lb)
- $v$ = Linear velocity (feet per second, ft/s)
- $550$ = Conversion constant (foot-pounds per second per horsepower)

This formula calculates the mechanical power being delivered by a moving load or actuator.

Force and velocity must be expressed in the correct units. If velocity is given in inches per second, convert it to feet per second before using the formula.

**Conversion:**

$v_{\text{ft/s}} = \frac{v_{\text{in/s}}}{12}$

### Example: Calculating Mechanical Horsepower

A hydraulic cylinder produces 4,000 pounds of force and moves a load at 2 feet per second. Calculate the mechanical horsepower.

$HP = \frac{F \times v}{550}$

$HP = \frac{4,000 \times 2}{550}$

$HP = \frac{8,000}{550}$

**Answer: 14.55 HP**

The cylinder delivers approximately 14.55 mechanical horsepower while moving the load.

*Note: Mechanical horsepower is the power delivered at the moving load. Actual power available at the load may be lower than the hydraulic power supplied because of system losses.*

## 4.3 System Efficiency

System efficiency describes how effectively a hydraulic system converts input power into useful output power.

No hydraulic system is 100% efficient. Some energy is lost through friction, fluid turbulence, leakage, heat generation, and mechanical losses.

**Formula:**

$\eta = \frac{Output}{Input} \times 100$

Where:

- $\eta$ = Efficiency (percent, %)
- $Output$ = Useful power delivered by the system
- $Input$ = Power supplied to the system

For a hydraulic system, input and output are commonly measured in horsepower. Both values must use the same units.

### Example: Calculating System Efficiency

A hydraulic pump receives 15 HP of mechanical input power and delivers 12 HP of hydraulic output power. Calculate the pump efficiency.

$\eta = \frac{Output}{Input} \times 100$

$\eta = \frac{12}{15} \times 100$

$\eta = 0.8 \times 100$

**Answer: 80%**

The pump is 80% efficient. This means 80% of the mechanical input power is converted into hydraulic power, while approximately 20% is lost.

### Understanding Power Losses

Using the previous example:

| Measurement | Horsepower |
|---|---:|
| Mechanical input power | 15 HP |
| Hydraulic output power | 12 HP |
| Power loss | 3 HP |
| Efficiency | 80% |

The 3 HP difference represents energy that is not delivered as useful hydraulic output. Much of this lost energy is converted into heat.

## 4.4 Understanding the Relationship Between Hydraulic and Mechanical Power

Hydraulic power and mechanical power describe two different stages of energy transfer in a hydraulic system.

1. A motor supplies mechanical power to drive the hydraulic pump.
2. The pump converts mechanical input power into hydraulic power by producing fluid flow and pressure.
3. The hydraulic fluid transfers energy through the system.
4. A cylinder or hydraulic motor converts hydraulic energy into mechanical output power.
5. Some energy is lost during each conversion and transfer.

A simplified power relationship is:

$Mechanical\ Input\ Power \rightarrow Hydraulic\ Power \rightarrow Mechanical\ Output\ Power$

The actual power available at the output is lower than the power supplied at the input because of system losses.

## 4.5 Important Concepts

- Hydraulic horsepower depends on both pressure and flow rate.
- Increasing pressure increases hydraulic horsepower when flow remains constant.
- Increasing flow rate increases hydraulic horsepower when pressure remains constant.
- The hydraulic horsepower formula calculates theoretical fluid power, not the mechanical horsepower required to drive the pump.
- Mechanical horsepower describes the rate at which mechanical work is performed.
- Mechanical horsepower calculations require force in pounds and velocity in feet per second.
- System efficiency compares useful output power to supplied input power.
- Efficiency is expressed as a percentage.
- Power losses commonly occur through friction, leakage, turbulence, and heat generation.
- Input and output power must use compatible units when calculating efficiency.

## Clarification

Emphasize the difference between hydraulic horsepower and mechanical horsepower. Hydraulic horsepower describes power carried by the fluid, while mechanical horsepower describes power delivered by a moving load or actuator. Efficiency accounts for the power lost during energy conversion.
