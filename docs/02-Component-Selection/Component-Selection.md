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

**Choice:** Option 2: BestCH 9V 3A AC Adapter

**Rationale:** A barrel jack port works with project specifications and also helps prevent user error while inputting the power supply. The BestCH 9V 3A AC Adapter works the best of the two devices following this form factor. A bonus fact is that the team knows the process to connect it safely to the Micro-controller and various components. This provides ample power for everything within the circuit and doesn't require us to ramp voltage up through another means to power the most voltage intensive elements. The cost being lower than the other two options is a positive but not a critically deciding factor as there are other power supply options that are around the same price point.

### Limit Switch

**Choice:** Option 3: Limit Switch SPDT 3A 125V

**Rationale:** This limit switch is rated for the maximum power supply current and for a higher voltage than the project will be using. It's useful in ensuring the motor doesn't go too far and making it so the moisture sensor won't corrode by being in the soil for long periods of time. This particular option is better than the rest due to the smaller size and mounting options. Since it is smaller we won't need as powerful a motor to move the prismatic joint and other components at the end toward the plant. Secondarily, the cylindrical element at the end can create a depression in the soil which will have even more resistance to being moved and will help the actuation of the switch part of the component.

### Motor Driver

**Choice:** Option 1: Brush DC Motor Controller

**Rationale:** Even though it adds a component, it follows project specifications and helps ensure the mechanical testing of the motor part. It doesn't hurt that there is a secondary integrated circuit for potential mishaps. Also the unique footprint of the through-hole option helps create an easier design assembly. As an added benefit the team knows how to use this particular component in order to drive a similar motor which will help in testing the overall system. It also removes a limit on the potential motor options and if the motor chosen later doesn't require one then we can change to Option 2. (Spoiler the motor chosen uses this.)

### Voltage Regulator

**Choice:** Option 2: Linear Voltage Regulator IC Positive Fixed 1 Output

**Rationale:** A linear voltage regulator is a clean solution to help get the power down from a higher voltage and amperage to the voltage we need for parts of this sub-system. In turn this one allows for an additional heat sink attachment if required to help prevent dangerous conditions and enable long-term use. While the price point isn't that much different from a switching regulator the ease of integration into the circuit elevates this option over the others. Also the consistency of this option promotes it over using a line of resistors.

### Barrel Jack

**Choice:** Option 2: Power Barrel Connector Jack 2.00mm ID (0.079"), 5.50mm OD (0.217") Through Hole, Right Angle

**Rationale:** A barrel jack is a good input due to the form factor of the power supply. However, the right angle of the pins allows us to at least create some form of security for the board as well as offer mechanical stability. Otherwise the footprint is distinct which will help in identifying its location on the board. Since it is a hard mechanical component we don't have to worry about it being taken out of the housing or tearing lose from the soldered ends as easily as the amorphous solution. Also due to the pins being perpendicular to the force of the plug being inserted or extracted we know that the solder won't get pulled on its thinnest surface area.

### Motor

**Choice:** Option 2: DC Motor Standard 9100 RPM 6VDC

**Rationale:** While it does have a lowered torque this acts as a safety feature for both the user and the plant in case the moisture sensor is misaligned. Also the flat sides on the housing of the motor allow for a brace to be installed in order to ensure the motor doesn't just spin. An added benefit of not having an encoder is a reduction in the wires that need to be connected directly to the motor. Reducing the amount of wires that would be exposed to the user's environment and needed to be searched to debug errors with the motor. Its size also helps the keep the housing smaller and doesn't force the team to come up with a clever way to hide it or to prevent damage over a larger surface.

### Moisture Sensor


**Choice:** Option 1: Handmade resistive check using nails

**Rationale:** This option forces the student team to delve into how electricity is transferred through space. This also follows the project specifications of not having a daughter board component. Unfortunately, for the accuracy due to soil chemistry that is the best option due to majority of moisture sensors needing a daughter board of some kind in order to function.

## Power Budget

After all of our components have been selected we need to ensure that we have enough power to actually complete the subsection as we have designed it. Otherwise, we'll need to find a new or a secondary power source or we'll need to choose different components.

This information can be found at the [*power budget tab*]()
