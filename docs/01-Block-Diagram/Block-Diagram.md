---
title: Individal Block Diagram
tags:
- tag1
- tag2
---

## Overview

This block diagram is part of a larger machine but still is able to work on its own to measure moisture. Two power levels are required which can be derived from the same 9v 3a power supply. This can supply power to both the motor at 12v levels (combined at the H-Bridge #FAN8100N) and the second power level is a 5v 1a which is obtained through the Voltage regulator (#L7805CV). This allows the Curiosity Nano to function at its desired power levels. This also enables sensing from the two limit switches (MS0850502F030P1A) and the capacitive sensor (ATSAMD10) due to their operating ranges. Finally the h-Bridge, part number aforementioned, controls the motor (711) which will help keep the capacitive sensor safe when not actively reading values. Otherwise Pins that are being utilized help the curiosity nano communicate with the central hub nano for this team project.

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

* ["ATSAMD10](https://www.digikey.com/en/products/detail/adafruit-industries-llc/4026/9745252?gclsrc=aw.ds&gad_source=1&gad_campaignid=20243136172&gbraid=0AAAAADrbLlg9a_M-PIXbOAU_b01BOFJHH&gclid=CjwKCAjw6P3GBhBVEiwAJPjmLlOWuwDv2P4LYTNa84dpeTVmIGIF3-ip6gdPgq7dAOYefjMucUHwJxoCIpUQAvD_BwE)
* ["MS0850502F030P1A"](https://www.digikey.com/en/products/detail/e-switch/MS0850502F030P1A/1628122?gclsrc=aw.ds&gad_source=4&gad_campaignid=20243136172&gbraid=0AAAAADrbLlj9VOp3m0S33_Eo5bb054Aan&gclid=CjwKCAjw6P3GBhBVEiwAJPjmLlhCRaDt99omgLz1hzmr-Y8tHiwT0D3Go3Vv2fcdLCyhnChq4JJsNxoCfLgQAvD_BwE)
* ["FAN8100N"](https://www.digikey.com/en/products/detail/fairchild-semiconductor/FAN8100N/11558200)
* ["L7805CV"](https://www.digikey.com/en/products/detail/stmicroelectronics/L7805CV/585964)
* ["PJ-102AH"](https://www.digikey.com/en/products/detail/cui-devices/PJ-102AH/408448)
* ["711"](https://www.digikey.com/en/products/detail/adafruit-industries-llc/711/5353610)

## Individual Block Diagram

![Uhoh we lost the Block Diagram](images\DirksBlockDiagramT102.png)

<!--
## Example Block Diagram

Showing an example of how to import a screenshot of the block diagram created outside of git and brought into a page.

![Example of Indivial Block diagram ](individual-block-diagram.png)
-->