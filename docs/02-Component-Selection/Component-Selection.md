---
title: Component Selection
---
<!-- not yet DONE -->

<!--
## Examples

### Style 1

> This is the example found in the assignment, uses more html

*Table 1: Example component selection*

**External Clock Module**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| ![](image1.png)<br>Option 1.<br> XC1259TR-ND surface mount crystal<br>$1/each<br>[link to product](http://www.digikey.com/product-detail/en/ECS-40.3-S-5PX-TR/XC1259TR-ND/827366)                 | \* Inexpensive[^1]<br>\* Compatible with PSoC<br>\* Meets surface mount constraint of project                                               | \* Requires external components and support circuitry for interface<br>\* Needs special PCB layout. |
| ![](image3.png)<br>\* Option 2. <br>\* CTX936TR-ND surface mount oscillator <br>\* $1/each <br>\* [Link to product](http://www.digikey.com/product-detail/en/636L3I001M84320/CTX936TR-ND/2292940) | \* Outputs a square wave <br>\* Stable over operating temperature <br> \* Direct interface with PSoC (no external circuitry required) range | * More expensive <br>\* Slow shipping speed                                                         |

**Choice:** Option 2: CTX936TR-ND surface mount oscillator

**Rationale:** A clock oscillator is easier to work with because it requires no external circuitry in order to interface with the PSoC. This is particularly important because we are not sure of the electrical characteristics of the PCB, which could affect the oscillation of a crystal. While the shipping speed is slow, according to the website if we order this week it will arrive within 3 weeks.

### Style 2

> Also acceptable, more markdown friendly

**External Clock Module**

1. XC1259TR-ND surface mount crystal

    ![](image1.png)

    * $1/each
    * [link to product](http://www.digikey.com/product-detail/en/ECS-40.3-S-5PX-TR/XC1259TR-ND/827366)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Inexpensive                               | Requires external components and support circuitry for interface |
    | Compatible with PSoC                      | Needs special PCB layout.                                        |
    | Meets surface mount constraint of project |

1. CTX936TR-ND surface mount oscillator

    ![](image3.png)

    * $1/each
    * [Link to product](http://www.digikey.com/product-detail/en/636L3I001M84320/CTX936TR-ND/2292940)

    | Pros                                                              | Cons                |
    | ----------------------------------------------------------------- | ------------------- |
    | Outputs a square wave                                             | More expensive      |
    | Stable over operating temperature                                 | Slow shipping speed |
    | Direct interface with PSoC (no external circuitry required) range |

**Choice:** Option 2: CTX936TR-ND surface mount oscillator

**Rationale:** A clock oscillator is easier to work with because it requires no external circuitry in order to interface with the PSoC. This is particularly important because we are not sure of the electrical characteristics of the PCB, which could affect the oscillation of a crystal. While the shipping speed is slow, according to the website if we order this week it will arrive within 3 weeks.
<!-- 

## <component Name>

1. <ItemName>

    ![](<fileLocation>){style="max-height:200px;"}

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                |
    | ----------------------------------------------------------------- | ------------------- |
    |                                                                   |                     |
    |                                                                   |                     |
    |                                                                   |                     |
    |                                                                   |                     |
    |                                                                   |                     |

1. <ItemName>

    ![](<fileLocation>){style="max-height:200px;"}

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                |
    | ----------------------------------------------------------------- | ------------------- |
    |                                                                   |                     |
    |                                                                   |                     |
    |                                                                   |                     |
    |                                                                   |                     |
    |                                                                   |                     |

1. <ItemName>

    ![](<fileLocation>){style="max-height:200px;"}

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                |
    | ----------------------------------------------------------------- | ------------------- |
    |                                                                   |                     |
    |                                                                   |                     |
    |                                                                   |                     |
    |                                                                   |                     |
    |                                                                   |                     |

**Choice:** Option #:

**Rationale:** 

-->

The purpose of this section is to highlight various solutions for the components used in the subsystem and identify the choices that will best suit this project.

## Components

### External Power Supply

**Choice:** Option 2:

**Rationale:** 

### Limit Switch

**Choice:** Option 3:

**Rationale:** 

### Motor Driver

**Choice:** Option 1:

**Rationale:** 

### Voltage Regulator

**Choice:** Option 2:

**Rationale:** 

### Barrel Jack

**Choice:** 

**Rationale:** 

### Motor

**Choice:** 

**Rationale:** 

### Moisture Sensor


**Choice:** Option 1:

**Rationale:** 

## Power Budget

After all of our components have been selected we need to ensure that we have enough power to actually complete the subsection as we have designed it. Otherwise, we'll need to find a new or a secondary power source or we'll need to choose different components.

This information can be found at the [*power budget tab*]()
