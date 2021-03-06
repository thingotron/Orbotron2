# Arduino Core for SAMD21 (E variant) CPU

This repository containts the source code and configuration files of the Arduino Core
for Atmel's SAMD21 (E variant) processor (used on the FemtoUSB board).

## Installation on Arduino IDE

Add the following package URL to the Additional Boards Manager URLs field in your Arduino IDE via **File > Preferences** (Settings tab).
```
http://downloads.femtoduino.com/ArduinoCore-atsamd21e18a/package_atsamd21e18a-hourly-build_index.json
```

or, for our stable release, try:

```
http://downloads.femtoduino.com/ArduinoCore-atsamd21e18a/package_atsamd21e18a-release-build_index.json
```

This core is now available as a package in the Arduino IDE cores manager.
Just open the **Boards Manager** and install the package called:

"Atmel ATSAMD21E18A core" by FemtoIO



For SAM R21 LwMesh support, you will need our fork of the `Pinnoccio/library-atmel-lwmesh` library, "at86rf233" branch.

See https://github.com/femtoio/library-atmel-lwm/tree/at86rf233



## Support

This package is derrived from the Arduino Zero bootloader and core. It has been modified to work with the E variant of the SAM D21 chips.

There is a dedicated section of the Arduino Forum for general discussion and project assistance:

http://forum.arduino.cc/index.php?board=98.0

## Bugs or Issues

If you find a bug you can submit an issue here on github:

https://github.com/femtoio/ArduinoCore-atsamd21e18a/issues

Before posting a new issue, please check if the same problem has been already reported by someone else
to avoid duplicates.

## Contributions

Contributions are always welcome. The preferred way to receive code cotribution is by submitting a 
Pull Request on github.

## Hourly builds

This repository is under a Continuos Integration system that every hour checks if there are updates and
builds a release for testing (the so called "Hourly builds").

The hourly builds are available through Boards Manager. If you want to install them:
  1. Open the **Preferences** of the Arduino IDE.
  2. Add this URL `http://downloads.femtoduino.com/ArduinoCore-atsamd21e18a/package_atsamd21e18a-hourly-build_index.json` in the **Additional Boards Manager URLs** field, and click OK.
  3. Open the **Boards Manager** (menu Tools->Board->Board Manager...)
  4. Install **Atmel ATSAMD21E18A core - Hourly build**
  5. Select one of the boards under **Atmel ATSAMD21E18A Hourly build XX** in Tools->Board menu
  6. Compile/Upload as usual

If you already installed an hourly build and you want to update it with the latest:
  1. Open the **Boards Manager** (menu Tools->Board->Board Manager...)
  2. Remove **Atmel ATSAMD21E18A core - Hourly build**
  3. Install again **Atmel ATSAMD21E18A core - Hourly build**, the Board Manager will download the latest build replacing the old one.

## License and credits

This core has been developed by Arduino LLC in collaboration with Atmel.

```
  Copyright (c) 2015 Arduino LLC.  All right reserved.

  This library is free software; you can redistribute it and/or
  modify it under the terms of the GNU Lesser General Public
  License as published by the Free Software Foundation; either
  version 2.1 of the License, or (at your option) any later version.

  This library is distributed in the hope that it will be useful,
  but WITHOUT ANY WARRANTY; without even the implied warranty of
  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
  See the GNU Lesser General Public License for more details.

  You should have received a copy of the GNU Lesser General Public
  License along with this library; if not, write to the Free Software
  Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA
```
