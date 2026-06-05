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

Add to Table21 > Parts tab > Edit Part Offset > Z = +100

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

ADDITIONAL PARAMETERS

- Parts tab > Edit Parts Offset > Y= -180, W= -90, P= 90 (to show the box when gripper closed)
- Simulation tab > Material Handling Clamp // Articulated CAD > 3600f5-200-4

## SINGLE TABLE SIMULATION

