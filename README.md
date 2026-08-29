# Sequential-Counter


## Overview

This project implements a **custom sequential counter** using digital logic in **Logisim Evolution**.

Unlike a conventional binary counter, this circuit follows a specific sequence of states:

```text
0 → 4 → 7 → 1 → 6 → 3 → 0 → ...
```

The counter advances to the next state on every clock pulse and continuously repeats the sequence.

## Sequence

|   Step | Decimal | Binary |
| -----: | ------: | ------ |
|      1 |       0 | `000`  |
|      2 |       4 | `100`  |
|      3 |       7 | `111`  |
|      4 |       1 | `001`  |
|      5 |       6 | `110`  |
|      6 |       3 | `011`  |
| Repeat |       0 | `000`  |

## How It Works

The counter is a **3-bit synchronous sequential circuit**.

Each clock pulse causes the circuit to transition from its current state to the next state in the predefined sequence.

The state transitions are:

```text
000 → 100 → 111 → 001 → 110 → 011 → 000
```

The circuit uses memory elements to store the current state and combinational logic to determine the next state.

## Main Components

* D flip-flops
* Logic gates
* Clock
* Combinational logic
* Seven-segment display / output indicators

## State Transition

```text
       ┌──────────────────────────────┐
       ↓                              │
     000 → 100 → 111 → 001 → 110 → 011
       └──────────────────────────────┘
```

Where:

* `000` = 0
* `100` = 4
* `111` = 7
* `001` = 1
* `110` = 6
* `011` = 3

## Tools

* **Logisim Evolution**
* Digital Logic Design

## Project Structure

```text
Sequential-Counter/
├── README.md
├── sequential_counter.circ
├── circuit.png
└── documentation.pdf
```

## Learning Outcomes

This project helped me practice:

* Sequential circuit design
* State machines
* State transition tables
* D flip-flops
* Clocked circuits
* Next-state logic
* Designing custom counting sequences
* Digital circuit simulation and debugging

## Circuit

[view actual circuit](https://1drv.ms/v/c/210e17635efde1f9/IQBdC2k9pN6iQ6YNUvHosUQZAfOHFwO1k0zHWvn71VleBRE?e=YF7oKS)
## Author

**Lujain Ayman**

Computer Engineering Student
