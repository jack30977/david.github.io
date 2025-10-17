---
title: Component Selection Example
---
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

    ![](<fileLocation>)

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

    ![](<fileLocation>)

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

    ![](<fileLocation>)

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

## External Power Supply

1. USB Power Bank Battery Charger 2A

    ![AdaFruit Industries USB Power Bank](images/PowerSupply/1566USB.png)

    * $39.95/each
    * [1566](https://www.digikey.com/en/products/detail/adafruit-industries-llc/1566/6612468?gclsrc=aw.ds&gad_source=1&gad_campaignid=20243136172&gbraid=0AAAAADrbLlhjMd1SI_TeFQt_5_XtjL5xo&gclid=CjwKCAjwr8LHBhBKEiwAy47uUk3q97qpKOk9OI4bVaExirH9Z_ZgJgqjou72gkbAOUQFlqWR2LLEgBoCRz8QAvD_BwE)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Outputs 5v which is what most of the components require  | Doesn’t connect to the easily to a barrel jack without an adapter |
    | Square footprint that doesn’t need to be on the pcb just connected | Doesn’t follow the project specifications                 |
    | Could be repurposed or replaced if it breaks easier than other integrated elements | Outputs 1-2A but isn’t clear on how to control the output |

1. BestCH 9V 3.0A AC Adapter

    ![EGR 304's power port](images/PowerSupply/Bestch_EGR304Jack.jpg)

    * $4.52/each
    * [B09ZTKTLGW](https://a.co/d/hFQdNi4)

    | Pros                                                              | Cons                |
    | ----------------------------------------------------------------- | ------------------- |
    | Outputs the 9V 3A needed for the motor and can be limited down   | Limited to a wall plug |
    | Over charge protection                               | Cord isn’t necessarily long enough |
    | Short circuit protection                             | Barrel jacks have a lot of variability so if it's lost it would be harder to replace |
    | Over current protection                              |Barrel jacks are prone to loosening over time |
    | Consistent voltage output                            |                                  |
    | 100V - 240V Alternating current input                |                                  |
    | Barrel jack can’t be inserted upside down and cause damage to the components |          |
    | Has been tested with other components provided in the class |                           |

1. 6V DC Power Supply 1A Universal AC Adapter

    ![EGR 455's power port](images/PowerSupply/6v1AEGR455Jack.png)

    * $5.96/each
    * [B0B2DWMYYH](https://a.co/d/5TMpGsm)

    | Pros                                                              | Cons                |
    | ----------------------------------------------------------------- | ------------------- |
    | In between the two required voltages                             | Only 1A output     |
    | 100-240V AC input                                                | Limited to a wall outlet |
    | Consistent output voltage                                        | Small cable which restricts movement |
    |                                                                   | Barrel jacks have a lot of variability so replacement is difficult on the user’s side |
    |                                                                   | Ports are prone to loosening over time with several movements |

**Choice:** Option 2: BestCH 9V 3A AC Adapter

**Rationale:** A barrel jack port works with project specifications and also helps prevent user error while inputting the power supply. The BestCH 9V 3A AC Adapter works the best of the two devices following this form factor. A bonus fact is that the team knows the process to connect it safely to the Micro-controller and various components. This provides ample power for everything within the circuit and doesn't require us to ramp voltage up through another means to power the most voltage intensive elements. The cost being lower than the other two options is a positive but not a critically deciding factor as there are other power supply options that are around the same price point.

## Limit Switch

1. TS02-66-60-BK-160-LCR-D (Push button)

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | Small outline                                                     | Not easily mounted                                                   |
    | Doesn’t require a lot of power                                    | Could require a secondary breadboard area to mount                   |
    | Signals can be in parallel                                        | Small sensing area                                                   |
    |                                                                   | More force than a traditional limit switch                           |
    |                                                                   | Hard to see limit is found                                           |
    |                                                                   | Target surface may move without mechanical support                   |

2. MS0850502F030P1A (limit switch)

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | Through hole mounting                                             | Relatively large                                                     |
    | Doesn’t need PCB connection directly (can wire connect)           | Needs support if at the end of actuator range                        |
    | Three states, but only two pins required                          | Acts parallel to placement                                           |
    | 50k+ operation lifespan                                           |                                                                      |
    |                                                                   |                                                                      |

3. 463093691402 (limit switch)

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | Thinner than other options                                        | Bent pin mounts                                                      |
    | Circle likely catches movement better than straight bar           | Pin connection extends past part width                               |
    | Can be mounted away from PCB                                      |                                                                      |
    | Three states, but only two pins required                          |                                                                      |
    | Through hole mounting                                             |                                                                      |

**Choice:** Option 3: 

**Rationale:** 

## Motor Driver

1. FAN8100N (H-Bridge)

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | Known specs for size, power, and pins                             | Cannot modify pin positions.                                         |
    | Easy-to-replicate footprint                                       | Backup difficult if internal circuit fails.                          |
    | Stands out on PCB canvas                                          | Depends on motor type for it to be effective.                        |
    | Allows for forward and reverse signals                            |                                                                      |
    | Doesn’t need PWM signal                                           |                                                                      |

1. Use a motor that doesn’t need a motor driver

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | Eliminates one component                                          | Forces PWM signals or encoder for control                            |
    | May remove need for a limit switch                                | Requires motor constant tuning                                       |
    | Reduces PCB failure points                                        | May need voltage amplification circuit                               |

1. 4035 (Motor Driver daughter board)

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | Built-in electrical protection =                                  | Breaks project rule: no daughter boards                              |
    | Plug-and-play on breadboard                                       | Needs extra male pin connectors to attach                            |
    | Supports PWM and H-Bridge control                                 |                                                                      |

**Choice:** Option 1: 

**Rationale:** 

## Voltage Regulator

1. Resistors in series

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | Can limit voltage                                                 | Voltage output varies with current draw                              |
    | Parallel configuration can alter current                          | Cannot change current and voltage simultaneously                     |
    | Compact placement near PCB face                                   | Requires more space than regulators                                  |
    | Fault-tolerant due to redundancy                                  | Troubleshooting is difficult                                         |

1. L7805CV (linear voltage regulator)

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | Already provided                                                  | Limited to 1.5A current (some needs are 3A)                          |
    | Well-understood by team                                           | Requires planning for voltage output                                 |
    | Supports additional heat-sinks                                    | Can't automatically adjust input to 5V output                        |
    | Example circuit available                                         |                                                                      |
    | Tested across various circuits                                    |                                                                      |

1. MC34063ADR (switching regulator)

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | Adjustable output voltage                                         | Max current output is 1.5A                                           |
    | Wide input range (3V–40V)                                         | Currently unfamiliar to team                                         |
    | Design equations provided                                         | Larger footprint than L7805CV                                       |
    | Can be surface or through-hole mounted                            |                                                                      |

**Choice:** Option #: 2

**Rationale:** Already available, familiar to the team, meets most current requirements, and aligns with the learning goals of the project.

## Barrel Jack

1. 10-02248 - lines

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | Matches power supply output port                                  | Amorphous shape makes secure mounting difficult                      |
    | Could be sealed for water resistance                              | Hard to diagnose wire issues                                         |
    | Variable footprint flexibility                                    | Only one ground contact                                              |

1. PJ-102AH - normal 

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | Stable footprint                                                  | Difficult to waterproof                                              |
    | 3 contacts from 2 conductors                                      | No built-in protection                                               |
    | Through-hole mounted                                              | Pins fragile until PCB-mounted                                       |
    | Matches supply ports                                              |                                                                      |
    | Rated for 24V/5A                                                  |                                                                      |

1. PJ-044BH - butt pins

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | Pins positioned at rear                                           | Internal exposure if seal is broken                                  |
    | Matches supply output port                                        | No electrical protection                                             |
    | 3 contacts from 2 conductors                                      | Needs firm PCB mounting                                              |
    | Through-hole attachment                                           |                                                                      |
    | Rated for 24V/5A                                                  |                                                                      |

**Choice:** Option #: 2

**Rationale:** Best balance of mechanical stability, rating, and footprint compatibility, with minor concessions on waterproofing.

## Motor

1. FIT0186 (Encoder Based motor)

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | High stall current & Max Operating voltage                        | Requires several control pins                                        |
    | Includes encoder                                                  | Software control needed, not easy to simulate                        |
    | No external software for encoder needed                           | Hard to secure due to cylindrical shape                              |

1. 711 (DC motor)

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | Works with predefined track                                       | No position feedback                                                 |
    | Flat side helps control torque output                             | Requires external bound control                                      |
    | Compact, easy to secure                                           | Rated 4.5–9V, slightly over 5V limit                                 |
    | Lightweight                                                       | Lower torque                                                         |
    | Mechanically simulative                                           |                                                                      |
    | Flexible mounting options                                         |                                                                      |

1. SER0006 - servo 

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | Rectangular shape for better torque transfer                      | Requires homing and configuration                                    |
    | Has incremental encoder                                           | Needs PWM (extra wire)                                               |
    | Rated at 4.8V DC                                                  | Cannot be simulated mechanically                                     |
    | High torque                                                       |                                                                      |
    | No motor controller needed                                        |                                                                      |

**Choice:** Option #: 3

**Rationale:** High torque, compact shape, encoder, and voltage alignment make it ideal even with setup complexity.

## Moisture Sensor

1. Handmade Resistive check using nails

    ![](<fileLocation>)

    * $5.96/each
    * [text](<link>)

    | Pros                                                              | Cons                                                                 |
    | ----------------------------------------------------------------- | -------------------------------------------------------------------- |
    | No daughter board needed                                          | Materials degrade over time                                          |
    | Easy soil removal                                                 | Readings may be biased by soil chemistry                             |
    | Reading handled in software                                       | Very dry soil might not register                                     |
    | Modular parts for easy repair                                     | Theoretical op-amp dependence unclear                                |

1. 13637

   ![](fileLocation)

   * $5.96/each
   * [text](link)

   | Pros                               | Cons                                                   |
   | ---------------------------------- | ------------------------------------------------------ |
   | Easy to extend to probe            | Is a daughter board – violates requirements            |
   | Prebuilt, screw terminals          | Large probes can harm plants                           |
   | Consumer-friendly design potential | Logic integration reduces student learning opportunity |
   | Reaches deeper into soil           |                                                        |

2. VH400 Soil Moisture Sensor Probe

   ![](fileLocation)

   * $5.96/each
   * [text](link)

   | Pros                                    | Cons                                       |
   | --------------------------------------- | ------------------------------------------ |
   | Wide input voltage range                | Likely includes daughter board (violation) |
   | Low current use (<13mA)                 | Probe may not fit pots or harm roots       |
   | Quick sampling (can be toggled on/off)  | Not available from reputable sellers       |
   | Unaffected by salt/fertilizer           |                                            |
   | Usable in hydroponics                   |                                            |
   | Long-lasting corrosion-resistant design |                                            |

**Choice:** Option 1:

**Rationale:** 