---
title: Individual Block Diagram
tags:
- tag1
- tag2
---

## Overview

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

* [463093691402](https://www.digikey.com/en/products/detail/w-rth-elektronik/463093691402/14113680?gclsrc=aw.ds&gad_source=1&gad_campaignid=20243136172&gbraid=0AAAAADrbLlhjMd1SI_TeFQt_5_XtjL5xo&gclid=CjwKCAjwr8LHBhBKEiwAy47uUmrm-bK4boEMAm9Mk_cnw0iZMQBKQOZvTpEZI7Jhn9Q0tGQiBCwf3BoC28MQAvD_BwE)
* ["FAN8100N"](https://www.digikey.com/en/products/detail/fairchild-semiconductor/FAN8100N/11558200)
* [L7805CV](https://www.digikey.com/en/products/detail/stmicroelectronics/L7805CV/585964)
* [PJ-102AH](https://www.digikey.com/en/products/detail/cui-devices/PJ-102AH/408448)
* [711](https://www.digikey.com/en/products/detail/adafruit-industries-llc/711/5353610)

## Individual Block Diagram

![Uh oh we lost the Block Diagram](images/DirksBlockDiagramT102.png)

This block diagram is available on [Draw.io here!](https://drive.google.com/file/d/1KY_l_oFdGwqlsgwlLvn5x_c0yW5vuY1z/view?usp=sharing)
It can also be found [in pdf form here.](images/EGR304IndividualBlockDiagram.pdf)
<!--
## Example Block Diagram

Showing an example of how to import a screenshot of the block diagram created outside of git and brought into a page.

![Example of Individual Block diagram ](individual-block-diagram.png)
-->