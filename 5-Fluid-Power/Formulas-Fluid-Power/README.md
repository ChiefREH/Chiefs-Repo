# BASIC FORMULAS - FLUID POWER

# Fluid Power Primer

A Foundation for Understanding Hydraulic Systems

---

## 1. Pressure: The Push Behind Fluid Power

### What Is Pressure?

Pressure is the amount of force applied over a given area. In fluid power systems, pressure represents the system's ability to exert a push against a load.

A useful way to think about pressure is that it measures how concentrated a force is. The same amount of force applied over a smaller area produces higher pressure.

### Formula

`P = F ÷ A`

Where:

- `P` = Pressure (psi)
- `F` = Force (lb)
- `A` = Area (in²)

### Why Does It Matter?

Pressure is what allows hydraulic systems to perform work. Every hydraulic cylinder, motor, press, and brake system depends on pressure to generate usable force.

A pump produces fluid flow, but pressure develops only when that flow encounters resistance. If there is no resistance, pressure remains low.

Think of pressure as the system's **pushing capability**.

### Real-World Applications

- Hydraulic presses
- Vehicle brake systems
- Forklifts
- Excavators
- Agricultural equipment
- Hydraulic jacks

Typical hydraulic operating pressures:

| Application | Typical Pressure |
|------------|----------------:|
| Power Steering | 800-1,500 psi |
| Industrial Hydraulics | 2,000-3,000 psi |
| Construction Equipment | 3,000-5,000 psi |

### Example

A hydraulic cylinder produces 2,000 lb of force over an area of 4 in².

`P = 2000 ÷ 4`

`P = 500 psi`

**Answer:** The system pressure is **500 psi**.

### Key Concept

> Pressure tells us how much force-producing potential exists within the hydraulic system.

---

## 2. Pascal's Law: How Hydraulics Multiply Force

### What Is Pascal's Law?

Pascal's Law states:

> Pressure applied to a confined fluid is transmitted equally and undiminished in all directions.

This principle is the foundation of hydraulic power.

### Why Does It Matter?

Pascal's Law allows a relatively small input force to produce a much larger output force.

Pressure remains the same throughout the hydraulic fluid. Force changes when pressure acts on different piston areas.

### Formula

`F = P × A`

Where:

- `F` = Force (lb)
- `P` = Pressure (psi)
- `A` = Area (in²)

### Real-World Application

A hydraulic floor jack uses Pascal's Law every time a vehicle is lifted.

1. A small piston creates pressure.
2. Pressure travels through the hydraulic oil.
3. The pressure reaches a larger piston.
4. The larger piston develops enough force to lift the vehicle.

The operator is not directly lifting the load. Instead, pressure is created and transmitted throughout the hydraulic system.

### Example

Small piston:

- Force = 50 lb
- Area = 2 in²

Pressure:

`P = 50 ÷ 2`

`P = 25 psi`

Large piston:

- Area = 20 in²

Output force:

`F = 25 × 20`

`F = 500 lb`

**Answer:** A 50-pound input force produces a 500-pound output force.

### Key Concept

> Pascal's Law explains why hydraulic systems can multiply force and lift loads far greater than an operator could lift directly.

---

## 3. Cylinder Area and Force: Where Hydraulic Power Becomes Mechanical Force

### What Is Cylinder Area?

A hydraulic cylinder produces force when pressure acts against the face of a piston.

The piston face is a circle, so determining cylinder force begins by calculating the area of that circle.

Without area, pressure has nothing to act upon.

Pressure alone does not create force.

### Why Does It Matter?

Cylinder size is one of the most important choices in hydraulic system design.

A cylinder that is too small may not produce enough force.

A cylinder that is too large may increase system cost, weight, and fluid requirements.

Engineers use cylinder area calculations to determine whether a machine can:

- Lift
- Push
- Pull
- Clamp
- Press
- Hold a load

---

### Step 1: Area of a Circle

Since the piston face is circular, start with the geometry formula:

`A = πr²`

Where:

- `A` = Area
- `r` = Radius
- `π` ≈ 3.1416

### Example

A circle with a radius of 2 inches:

`A = 3.1416 × (2)²`

`A = 12.57 in²`

---

### Step 2: Cylinder Area Formula

Hydraulic cylinders are normally specified by bore diameter rather than radius.

Since:

`r = D ÷ 2`

The circle area formula becomes:

`A = π(D ÷ 2)²`

Which simplifies to:

`A = πD² ÷ 4`

Where:

- `A` = Cylinder area (in²)
- `D` = Bore diameter (in)

This is the standard cylinder area formula used throughout fluid power.

---

### Step 3: Determine Cylinder Force

Once area is known, use pressure to calculate force:

`F = P × A`

Where:

- `F` = Force (lb)
- `P` = Pressure (psi)
- `A` = Area (in²)

This is one of the most common calculations in fluid power.

---

### Real-World Application

#### Excavator Boom Cylinder

When an excavator lifts a bucket of soil:

- Hydraulic pressure acts on the piston area.
- Cylinder area converts pressure into force.
- The cylinder raises the boom and bucket.

The available lifting force depends on:

- System pressure
- Cylinder area

Increasing either increases force.

---

### Example 1: Calculate Cylinder Area

Given:

- Bore Diameter = 3 in

Area:

`A = πD² ÷ 4`

`A = 3.1416 × 3² ÷ 4`

`A = 7.07 in²`

**Answer:** The piston area is approximately **7.07 in²**.

---

### Example 2: Calculate Cylinder Force

Given:

- Pressure = 2,000 psi
- Area = 7.07 in²

Force:

`F = 2000 × 7.07`

`F = 14,140 lb`

**Answer:** The cylinder can theoretically produce approximately **14,140 lb of force**.

---

### How Bore Size Affects Force

| Bore Diameter | Area (in²) | Force @ 2,000 psi |
|--------------|-----------:|------------------:|
| 2 in | 3.14 | 6,280 lb |
| 3 in | 7.07 | 14,140 lb |
| 4 in | 12.57 | 25,140 lb |

Notice how force increases rapidly as bore diameter increases.

Because area is based on diameter squared, doubling cylinder diameter nearly quadruples available force.

---

### Extension and Retraction Force

Most industrial cylinders are double-acting cylinders.

#### Extension Force (Cap End)

Pressure acts on the full piston area.

`Ac = πD² ÷ 4`

Maximum force is available.

#### Retraction Force (Rod End)

The piston rod occupies part of the piston area.

`Ar = π(D² - d²) ÷ 4`

Where:

- `D` = Bore diameter
- `d` = Rod diameter

Since the effective area is smaller:

- Retraction force is lower.
- Retraction speed is often higher.

### Key Concept

> Cylinder area is the direct link between hydraulic pressure and mechanical force.

---

## 4. Flow Rate and Speed: What Makes Things Move

### What Is Flow?

Flow is the volume of fluid moving through a system during a given amount of time.

While pressure creates force, flow creates motion.

A hydraulic system can have pressure without movement, but movement cannot occur without flow.

### Formula

`Q = V ÷ t`

Where:

- `Q` = Flow rate
- `V` = Volume
- `t` = Time

Common hydraulic flow units:

- Gallons per Minute (GPM)
- Liters per Minute (L/min)

### Why Does It Matter?

Flow determines how quickly cylinders and motors move.

Increasing flow increases speed.

Increasing pressure increases force.

Many beginning students incorrectly assume pressure and flow are the same thing.

They are not.

### Real-World Application

#### Log Splitter

A log splitter provides a simple illustration of the difference between pressure and flow.

- Pressure determines splitting force.
- Flow determines how quickly the wedge moves.

A larger pump increases cycle speed without necessarily increasing splitting force.

### Example

Two identical cylinders operate at:

`2,000 psi`

Cylinder A receives:

`5 GPM`

Cylinder B receives:

`10 GPM`

Both cylinders produce the same force because system pressure is identical.

Cylinder B moves approximately twice as fast because it receives twice as much flow.

### Key Concept

> Pressure determines force. Flow determines speed.

---

## 5. Hydraulic Power: Combining Force and Speed

### What Is Power?

Power is the rate at which work is performed.

Hydraulic power combines:

- Pressure (force potential)
- Flow (speed potential)

Neither pressure nor flow alone fully describes machine performance.

Power combines both.

### Formula

`HP = (PSI × GPM) ÷ 1714`

Where:

- `HP` = Hydraulic horsepower
- `PSI` = Pressure
- `GPM` = Flow rate

### Why Does It Matter?

A hydraulic system may have:

- High pressure but low flow
- High flow but low pressure

Neither tells the complete story.

Power tells us how much useful work a hydraulic system can perform over time.

### Real-World Application

#### Excavator Hydraulic System

An excavator must:

- Lift heavy loads
- Swing the machine
- Extend cylinders
- Move quickly under load

To accomplish all of these tasks, the hydraulic system requires both pressure and flow.

Hydraulic horsepower helps engineers properly size:

- Pumps
- Electric motors
- Diesel engines
- Hydraulic power units

### Example

Given:

- Pressure = 2,500 psi
- Flow = 15 GPM

`HP = (2500 × 15) ÷ 1714`

`HP = 21.9`

**Answer:** The system requires approximately **22 hydraulic horsepower**.

### Key Concept

> Power is the combination of force-producing pressure and motion-producing flow.

---

# The Five Big Ideas of Fluid Power

| Concept | Fundamental Question |
|----------|---------------------|
| Pressure | How much pushing capability exists? |
| Pascal's Law | How is pressure transmitted through a fluid? |
| Cylinder Area & Force | How much force can be produced? |
| Flow Rate & Speed | How fast will the actuator move? |
| Hydraulic Power | How much work can the system perform? |

---

# The Cause-and-Effect Chain

Fluid power can be summarized as a simple chain:

**Pressure creates force.**

`P = F ÷ A`

↓

**Pascal's Law transmits pressure.**

`F = P × A`

↓

**Cylinder area determines force output.**

`A = πD² ÷ 4`

↓

**Flow determines actuator speed.**

`Q = V ÷ t`

↓

**Power combines pressure and flow.**

`HP = (PSI × GPM) ÷ 1714`

---

## Final Takeaway

If you understand these five concepts, you understand the fundamental physics behind:

- Hydraulic jacks
- Forklifts
- Excavators
- Hydraulic presses
- Agricultural equipment
- Industrial machinery
- Most introductory fluid power systems

Everything else in fluid power builds upon these five foundational ideas.