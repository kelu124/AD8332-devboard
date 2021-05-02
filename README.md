![GitHub repo size](https://img.shields.io/github/repo-size/kelu124/AD8332-devboard?style=plastic)
![GitHub language count](https://img.shields.io/github/languages/count/kelu124/AD8332-devboard?style=plastic)
![GitHub top language](https://img.shields.io/github/languages/top/kelu124/AD8332-devboard?style=plastic)
![GitHub last commit](https://img.shields.io/github/last-commit/kelu124/AD8332-devboard?color=red&style=plastic)

[![Patreon](https://img.shields.io/badge/patreon-donate-orange.svg)](https://www.patreon.com/kelu124) 
[![Kofi](https://badgen.net/badge/icon/kofi?icon=kofi&label)](https://ko-fi.com/G2G81MT0G)

[![Slack](https://badgen.net/badge/icon/slack?icon=slack&label)](https://join.slack.com/t/usdevkit/shared_invite/zt-2g501obl-z53YHyGOOMZjeCXuXzjZow)
[![made-with-Markdown](https://img.shields.io/badge/Made%20with-Markdown-1f425f.svg)](http://commonmark.org)


# AD8332-devboard

![](tests/ad8332_test_board.jpg)



Changing filter components is more or less "easy". Two places contain footprints for filters, one on the input and another on the output to the ADC.
* The input filter has three 1206 footprints (one in serial and two in parallel to input signal). 
* The output filter is a bit more complex (20MHz LPF) and composed out of 0603 SMD parts. Those are also easy to replace with an air solder station and tweezers.

More on the output filter [in here](datasheets/aa_filter_report.pdf).

# Overview

![](schematics.png)

On this schematics, VOH/VOL1 and VIP2/VIN2 seem inverted, but the device appears to be working as well.

# Testing 

![](tests/batch.jpg)

### Setup

![](tests/setup.png)

### Results

![](tests/gain.png)



# License

See [LICENSE.txt](LICENSE.txt)

```
 ------------------------------------------------------------------------------
| SPDX-FileCopyrightText: 2020 Jorge Arija, Luc Jonveaux                       |
| SPDX-License-Identifier: CERN-OHL-S-2.0                                      |
|                                                                              |
| This source describes Open Hardware and is licensed under the CERN-OHL-S v2. |
|                                                                              |
| You may redistribute and modify this source and make products using it under |
| the terms of the CERN-OHL-S v2 (https://ohwr.org/cern_ohl_s_v2.txt).         |
|                                                                              |
| This source is distributed WITHOUT ANY EXPRESS OR IMPLIED WARRANTY,          |
| INCLUDING OF MERCHANTABILITY, SATISFACTORY QUALITY AND FITNESS FOR A         |
| PARTICULAR PURPOSE. Please see the CERN-OHL-S v2 for applicable conditions.  |
|                                                                              |
| Source location: https://github.com/kelu124/ft600/                           |
|                                                                              |
| As per CERN-OHL-S v2 section 4, should You produce hardware based on this    |
| source, You must where practicable maintain the Source Location visible      |
| on the external case of the Gizmo or other products you make using this      |
| source.                                                                      |
 ------------------------------------------------------------------------------
```

[More details in cern_ohl_s_v2](https://ohwr.org/project/cernohl/wikis/Documents/CERN-OHL-version-2)


