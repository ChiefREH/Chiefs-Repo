# 3. Flow and Speed

Flow and speed are important factors in hydraulic systems because they determine how quickly fluid moves through the system and how fast a hydraulic cylinder operates.

Pressure determines the amount of force a hydraulic cylinder can produce, while flow rate determines how quickly the cylinder moves.

Understanding the relationship between flow, area, velocity, and time is essential when calculating cylinder speed and cycle time.

## 3.1 Flow Rate

Flow rate is the volume of fluid that moves through a hydraulic system over a specific period of time.

In hydraulic systems, flow rate is commonly measured in gallons per minute (GPM). Flow rate determines how quickly a cylinder can extend or retract when its effective area is known.

**Formula:**

$Q = \frac{V}{t}$

Where:

- $Q$ = Flow rate
- $V$ = Volume of fluid
- $t$ = Time

Common units include:

- Flow rate: gallons per minute (GPM)
- Volume: gallons (gal)
- Time: minutes (min)

### Example: Calculating Flow Rate

A hydraulic pump delivers 5 gallons of fluid in 1 minute. Calculate the flow rate.

$Q = \frac{V}{t}$

$Q = \frac{5}{1}$

**Answer: 5 GPM**

The pump delivers 5 gallons of hydraulic fluid per minute.

## 3.2 Fluid Velocity

Fluid velocity is the speed at which fluid travels through a pipe, hose, or passage. It depends on the flow rate and the cross-sectional area available for the fluid to move through.

**Formula:**

$v = \frac{Q}{A}$

Where:

- $v$ = Fluid velocity
- $Q$ = Flow rate
- $A$ = Cross-sectional area

The flow rate and area must use compatible units. For example, if flow is measured in cubic inches per second and area is measured in square inches, velocity will be in inches per second.

A smaller passage produces a higher fluid velocity at the same flow rate. A larger passage produces a lower fluid velocity at the same flow rate.

### Example: Calculating Fluid Velocity

Fluid flows through a pipe with an internal cross-sectional area of 2 in². The flow rate is 20 in³/s. Calculate the fluid velocity.

$v = \frac{Q}{A}$

$v = \frac{20}{2}$

**Answer: 10 in/s**

The fluid travels through the pipe at 10 inches per second.

*Note: In practical hydraulic calculations, flow rate may need to be converted from GPM to cubic inches per second before using this formula.*

## 3.3 Cylinder Extension Speed

Cylinder extension speed is the rate at which the piston and rod move outward from the cylinder.

Extension speed depends on the flow rate entering the cylinder and the full piston area. For a given flow rate, a cylinder with a smaller piston area extends faster than one with a larger piston area.

**Formula:**

$v = \frac{Q}{A_p}$

Where:

- $v$ = Cylinder extension speed
- $Q$ = Flow rate entering the cylinder
- $A_p$ = Piston area

When using GPM and square inches, use the following conversion to calculate speed in inches per minute:

$v = \frac{231 \times Q}{A_p}$

Where:

- $Q$ = Flow rate (GPM)
- $A_p$ = Piston area (in²)
- $231$ = Cubic inches per US gallon

To convert inches per minute to inches per second, divide by 60.

### Example: Calculating Cylinder Extension Speed

A hydraulic cylinder has a piston area of 4 in². The pump supplies 5 GPM to the cylinder. Calculate the extension speed.

$v = \frac{231 \times Q}{A_p}$

$v = \frac{231 \times 5}{4}$

$v = \frac{1,155}{4}$

**Answer: 288.75 in/min**

Convert to inches per second:

$v = \frac{288.75}{60}$

**Answer: 4.81 in/s**

The cylinder extends at approximately 4.81 inches per second.

## 3.4 Cylinder Retraction Speed

Cylinder retraction speed is the rate at which the piston and rod move back into the cylinder.

During retraction, hydraulic pressure acts on the annular area rather than the full piston area. Because the annular area is smaller, the cylinder generally retracts faster than it extends when the same flow rate is supplied in both directions.

**Formula:**

$v = \frac{Q}{A_a}$

Where:

- $v$ = Cylinder retraction speed
- $Q$ = Flow rate entering the rod side of the cylinder
- $A_a$ = Annular area

When using GPM and square inches, use:

$v = \frac{231 \times Q}{A_a}$

### Example: Calculating Cylinder Retraction Speed

A hydraulic cylinder has an annular area of 3 in². The pump supplies 5 GPM to the rod side. Calculate the retraction speed.

$v = \frac{231 \times Q}{A_a}$

$v = \frac{231 \times 5}{3}$

$v = \frac{1,155}{3}$

**Answer: 385 in/min**

Convert to inches per second:

$v = \frac{385}{60}$

**Answer: 6.42 in/s**

The cylinder retracts at approximately 6.42 inches per second.

### Comparing Extension and Retraction Speed

Using the previous examples:

| Measurement | Extension | Retraction |
|---|---:|---:|
| Flow rate | 5 GPM | 5 GPM |
| Effective area | 4 in² | 3 in² |
| Speed | 288.75 in/min | 385 in/min |

The cylinder retracts faster because the annular area is smaller than the full piston area.

*Note: These calculations assume the same flow rate is supplied to each side of the cylinder. Actual speed can vary due to flow losses, load conditions, pump characteristics, and flow-control settings.*

## 3.5 Cylinder Cycle Time

Cylinder cycle time is the amount of time required for a cylinder to complete a movement over a specified stroke distance.

Cycle time can be calculated by dividing the volume of fluid required for the movement by the flow rate supplied to the cylinder.

**Formula:**

$t = \frac{V}{Q}$

Where:

- $t$ = Time
- $V$ = Fluid volume required for the movement
- $Q$ = Flow rate

The volume and flow rate must use compatible units. For example, gallons divided by gallons per minute produces time in minutes.

For cylinder calculations:

- Use piston area to calculate extension-side volume.
- Use annular area to calculate retraction-side volume.
- Use the appropriate flow rate for each direction.

### Example: Calculating Extension Time

A hydraulic cylinder has a piston area of 4 in² and a stroke length of 12 inches. The pump supplies 5 GPM. Calculate the extension time.

First, calculate the extension-side volume:

$V = A_p \times L$

$V = 4 \times 12$

$V = 48 \text{ in}^3$

Convert the volume to gallons:

$V = \frac{48}{231}$

$V = 0.208 \text{ gal}$

Now calculate the extension time:

$t = \frac{V}{Q}$

$t = \frac{0.208}{5}$

$t = 0.0416 \text{ min}$

Convert minutes to seconds:

$t = 0.0416 \times 60$

**Answer: 2.50 seconds**

The cylinder requires approximately 2.5 seconds to complete its 12-inch extension stroke.

### Calculating Total Cycle Time

A complete cylinder cycle includes both extension and retraction.

To calculate total cycle time:

1. Calculate extension-side volume using piston area.
2. Calculate retraction-side volume using annular area.
3. Calculate the time required for each movement using its respective flow rate.
4. Add the extension and retraction times.

**Formula:**

$t_{\text{cycle}} = t_{\text{extension}} + t_{\text{retraction}}$

*Note: This calculation represents movement time only. Actual machine cycle time may also include dwell periods, valve switching, acceleration, deceleration, and other process delays.*

## 3.6 Important Concepts

- Flow rate determines how much fluid moves through a system over time.
- Pressure determines the force a cylinder can produce; flow rate determines how quickly it moves.
- Fluid velocity depends on flow rate and the cross-sectional area of the passage.
- Cylinder extension speed is calculated using the full piston area.
- Cylinder retraction speed is calculated using the annular area.
- A typical single-rod cylinder retracts faster than it extends when the flow rate is the same in both directions.
- Cylinder cycle time depends on fluid volume and flow rate.
- Extension and retraction require different fluid volumes because the effective areas are different.
- One US gallon equals 231 cubic inches.
- Maintain consistent units throughout calculations.

## Clarification

The central relationship in this section is that flow rate controls cylinder speed. At a constant flow rate, a smaller effective area produces greater speed. This explains why a typical single-rod cylinder retracts faster than it extends when supplied with the same flow rate.
