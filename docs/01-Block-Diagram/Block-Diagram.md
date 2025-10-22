---
title: Individual Block Diagram
tags:
- tag1
- tag2
---
<!-- not yet DONE -->
## Overview

This block diagram is part of the larger machine but is still able to add fertilizer into a revoir on its own. Due to the motor actuation points this requires two motors. However, they have different purposes as one is to mix in the fertilizer and one is to drop fertilizer into the internal tank this is at a fixed angle from the loading platform. This makes it so we could have two different types of motors or one singular motor. Since one motor is just rotating in a circular fashion in order to mix the fertilizer then we could drive it using a motor driver. Also in order to keep power levels safe for the Curiosity Nano we will need to drop it from the 9v that motors use down to a maximum of 5v.

<!--
This block diagram is part of a larger machine but still is able to work on its own to measure moisture. Two power levels are required which can be derived from the same 9v 3a power supply. This can supply power to both the motor at 12v levels (combined at the H-Bridge #FAN8100N) and the second power level is a 5v 1a which is obtained through the Voltage regulator (#L7805CV). This allows the Curiosity Nano to function at its desired power levels. This also enables sensing from the two limit switches (463093691402) and the capacitive sensor due to their operating ranges. Finally the h-Bridge, part number aforementioned, controls the motor (711) which will help keep the capacitive sensor safe when not actively reading values. Otherwise Pins that are being utilized help the curiosity nano communicate with the central hub nano for this team project.

<!--
This needs to be updated with a brief purpose for having the block diagram.
Things to mention are:
* power levels
* sensor
* Actuator
* team connections
* Power source
* ...

To get some initial formatting help, one can view ["here"](https://embedded-systems-design.github.io/EGR304DataSheetTemplate/Appendix/basic-markdown-examples/) some basic techniques.
-->

**Parts List for sensors and actuators that are involved in the diagram.**
Are available as a list here and with all the other options in [*Component Selection.*]()

## Individual Block Diagram

![Uh oh we lost the Block Diagram](images/AustinBlockDiagram.png)

This block diagram is available on [*Draw.io here!*](https://drive.google.com/file/d/1KY_l_oFdGwqlsgwlLvn5x_c0yW5vuY1z/view?usp=sharing)
It can also be found [*in pdf form here.*](images/EGR304IndividualBlockDiagram.pdf)

<!--
## Example Block Diagram

Showing an example of how to import a screenshot of the block diagram created outside of git and brought into a page.

![Example of Individual Block diagram ](individual-block-diagram.png)
-->