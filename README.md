hvac-eda
========

This is the hardware design component of an embedded HVAC controller. The source
code component is [hvac-app](https://github.com/rrendec/hvac-app). Refer to that
repository for a detailed description of the project.

The hardware design is done in [KiCad](https://www.kicad.org/). The custom parts
(symbols/footprints) are bundled into a library that is hosted in a separate Git
repository, available [here](https://github.com/rrendec/kicad-lib).

This repository includes two KiCad projects:
* **hvac-ctrl**: This is the main control board. It includes both on-board parts
  and physically distinct daughter boards, which are modelled as connectors.
  Examples of daughter boards are the Raspberry Pi, which is the "brains" of the
  system, and relay boards.
* **hvac-sys**: This is the entire HVAC system, which includes the control board
  and the major appliances, such as the furnace. The system components are
  modelled as connectors.
