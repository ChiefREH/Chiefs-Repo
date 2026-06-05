# ROBOGUIDE WORLD PARAMETERS

Basic data for simulated components I use in class.

## ROBOGUIDE GRIPPER PARAMETERS

**36005F-200**
- Box dimensions when closed: 125/125/125mm
- Doesn’t animate. Already fully open.

**36005F-200-2**
- Box dimensions when closed: 110/110/110mm

**36005F-200-3**
- Box dimensions when closed: 87/87/87mm

**36005F-200-4**
- Box dimensions when closed: 30/30/30mm


## SINGLE TABLETOP FIXTURE

Fixture > Tables > “Table21”

|  LOC  |     | SCALE  |     |
| :---: | :-: | :----: | :-: |
| **X** | 400 | **X**  | 0.5 |
| **Y** |  0  | **Y**  | 0.5 |
| **Z** | 300 | **Z**  | 1.0 |
| **W** |  0  |        |     |
| **P** |  0  | **WT** |     |
| **R** |  0  |        | n/a |

## CONE FOR TCP EXERCISE

Parts > Workpieces > “ConeAtZero”

|  LOC  |     | SCALE  |        |
| :---: | :-: | :----: | :----: |
| **X** |  0  | **X**  |  1.0   |
| **Y** |  0  | **Y**  |  1.0   |
| **Z** |  0  | **Z**  |  1.0   |
| **W** |  0  |        |        |
| **P** |  0  | **WT** |        |
| **R** |  0  |        | 1.0 kg |

**ADDITIONAL PARAMETERS**
- Add to Table21 > Parts tab > Edit Part Offset > Z = +100

## POINTER TOOL EOAT

Tooling > EOAT1 > Properties > CAD Drawing > “Pointer”

|  LOC  |     | **UTOOL** |     | SCALE  |        |
| :---: | :-: | :-------: | :-: | :----: | :----: |
| **X** |  0  |   **X**   |  0  | **X**  |  0.5   |
| **Y** |  0  |   **Y**   |  0  | **Y**  |  0.5   |
| **Z** |  0  |   **Z**   | 90  | **Z**  |  0.5   |
| **W** |  0  |   **W**   | 180 |        |        |
| **P** |  0  |   **P**   |  0  | **WT** |        |
| **R** |  0  |   **R**   |  0  |        | 1.0 kg |

## BASIC BLUE BOX

Parts > Add Parts > Box

|  LOC  |     | SCALE  |        |
| :---: | :-: | :----: | :----: |
| **X** | n/a | **X**  | 30 mm  |
| **Y** | n/a | **Y**  | 30 mm  |
| **Z** | n/a | **Z**  | 30 mm  |
| **W** | n/a |        |        |
| **P** | n/a | **WT** |        |
| **R** | n/a |        | 1.0 kg |

_*Most simulation works best with 2 different fixtures_

## GRIPPER TOOL

Tooling > EOAT1 > Properties > CAD Drawing > “Grippers” > 3600f5-200

|  LOC  |     | **UTOOL** |     | SCALE  |        |
| :---: | :-: | :-------: | :-: | :----: | :----: |
| **X** |  0  |   **X**   |  0  | **X**  |  0.2   |
| **Y** |  0  |   **Y**   |  0  | **Y**  |  0.2   |
| **Z** |  0  |   **Z**   | 180 | **Z**  |  0.2   |
| **W** | -90 |   **W**   | 180 |        |        |
| **P** |  0  |   **P**   |  0  | **WT** |        |
| **R** | 90  |   **R**   |  0  |        | 1.0 kg |

**ADDITIONAL PARAMETERS**

- Parts tab > Edit Parts Offset > Y= -180, W= -90, P= 90 (to show the box when gripper closed)
- Simulation tab > Material Handling Clamp // Articulated CAD > 3600f5-200-4

## SINGLE TABLE SIMULATION

Fixture > Tables > “Table21” (_see previous table for data_)

**RED BOX**
- Parts > Add Parts > Box (color: red)

|  LOC  |      | SCALE  |        |
| :---: | :--: | :----: | :----: |
| **X** | -120 | **X**  | 30 mm  |
| **Y** | -150 | **Y**  | 30 mm  |
| **Z** | +30  | **Z**  | 30 mm  |
| **W** | n/a  |        |        |
| **P** | n/a  | **WT** |        |
| **R** | n/a  |        | 1.0 kg |

**BLUE BOX**
- Parts > Add Parts > Box (color: blue)

|  LOC  |      | SCALE  |        |
| :---: | :--: | :----: | :----: |
| **X** | +120 | **X**  | 30 mm  |
| **Y** | +150 | **Y**  | 30 mm  |
| **Z** | +30  | **Z**  | 30 mm  |
| **W** | n/a  |        |        |
| **P** | n/a  | **WT** |        |
| **R** | n/a  |        | 1.0 kg |

**ADDITIONAL PARAMETERS**

- Red: Create Delay = 2 sec
    - _we’ll change to 3 seconds after we see the timing issue_
- Blue: Destroy Delay = 2 sec
    - _we’ll change to 3 seconds after we see the timing issue_
- Change both to RED at the end, so it looks like a single box


## 2 TABLE SIMULATION

**GREEN PICK-UP TABLE**

Fixture > Tables > “Table21” > Color = GREEN

|  LOC  |      | SCALE  |     |
| :---: | :--: | :----: | :-: |
| **X** | +300 | **X**  | 0.5 |
| **Y** | -300 | **Y**  | 0.5 |
| **Z** | +300 | **Z**  | 1.0 |
| **W** |  0   |        |     |
| **P** |  0   | **WT** |     |
| **R** |  0   |        | n/a |

ADDITIONAL PARAMETERS

- Parts tab > “Blue Box” > Edit Parts Offset > Z = +30 mm // check Visible at Teach, Visible at Run
- Simulation tab > check “Allow part to be picked” > 2 sec // uncheck “Allow parts to be placed”

**RED DROP TABLE**

Fixture > Tables > “Table21” > Color = RED

|  LOC  |      | SCALE  |     |
| :---: | :--: | :----: | :-: |
| **X** | +300 | **X**  | 0.5 |
| **Y** | +300 | **Y**  | 0.5 |
| **Z** | +300 | **Z**  | 1.0 |
| **W** |  0   |        |     |
| **P** |  0   | **WT** |     |
| **R** |  0   |        | n/a |

ADDITIONAL PARAMETERS

- Parts tab > “BLUE BOX” > Edit Parts Offset > Z = 30 mm // check Visible at Teach // uncheck Visible at Run
- Simulation tab > uncheck “Allow part to be picked” // check “Allow parts to be placed” > 2 sec

## USERFRAMES

Fixture > Tables > **“Table-With-Legs”**

TABLE STARTING LOCATION

|  LOC  |      | SCALE  |     |
| :---: | :--: | :----: | :-: |
| **X** | +300 | **X**  | 0.5 |
| **Y** | -200 | **Y**  | 0.5 |
| **Z** | +290 | **Z**  | 0.5 |
| **W** |  90  |        |     |
| **P** |  0   | **WT** |     |
| **R** |  90  |        | n/a |

Parts > Add Parts > Blue BOX

BOX ON TABLE

|  LOC  |     | SCALE  |        |
| :---: | :-: | :----: | :----: |
| **X** |  0  | **X**  | 100 mm |
| **Y** |  0  | **Y**  | 100 mm |
| **Z** |  0  | **Z**  | 30 mm  |
| **W** | 90  |        |        |
| **P** | 90  | **WT** |        |
| **R** |  0  |        | 1.0 kg |

After USERFRAME has been entered, move the Table here and touch-up

|  LOC  |      | SCALE  |     |
| :---: | :--: | :----: | :-: |
| **X** | +300 | **X**  | 0.5 |
| **Y** | +200 | **Y**  | 0.5 |
| **Z** | +290 | **Z**  | 0.5 |
| **W** |  90  |        |     |
| **P** |  0   | **WT** |     |
| **R** |  90  |        | n/a |

**ADDITIONAL PARAMETERS**

- Don’t forget to SETIND for your new frame in the SETUP > FRAMES list


## BASIC CIRCLES

SINGLE TABLETOP FIXTURE

Fixture > Tables > “Table21”

|  LOC  |     | SCALE  |     |
| :---: | :-: | :----: | :-: |
| **X** | 400 | **X**  | 0.5 |
| **Y** |  0  | **Y**  | 0.5 |
| **Z** | 300 | **Z**  | 1.0 |
| **W** |  0  |        |     |
| **P** |  0  | **WT** |     |
| **R** |  0  |        | n/a |

BLUE CYLINDER

|  LOC  |     |   SCALE   |        |
| :---: | :-: | :-------: | :----: |
| **X** |  0  | **DIAM.** | 200 mm |
| **Y** |  0  | **LEN.**  | 50 mm  |
| **Z** |  0  |           |        |
| **W** |  0  |           |        |
| **P** |  0  |  **WT**   |        |
| **R** |  0  |           | 1.0 kg |

**ADDITIONAL PARAMETERS**

- Add to Table21 > Parts tab > Edit Part Offset > W + 90
