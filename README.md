# Template

## Documentation
It is mandatory that every project is documented. The documentation must be written in English and with the following goals in mind:
1. A novice reader must be able to understand the main functionalities of the system (high level introduction)
2. The interaction with external systems must be discussed to an appropriate level of detail (e.g. input *x* does not need pull-up because *this* is the output configuration on board *a*)
3. All taken decisions must be discussed so that future colleagues will understand the reasons behind the design choices and will not repeat solved mistakes that to them were unknown before reading the documentation

The documentation must be written in Markdown and must be saved in the repository of the project of interest. In particular is must be saved in the `documentation/` folder.
The README.md file in the root of the repository must include a high level introduction to the system (can be the same as in point 1).

## Datasheets
It is mandatory that for every component in the project there must be a link to the relative datasheet.
The link must be referring to a local document which is saved in the `docs/datasheets/` folder of the project.
The most important parameters of the datasheets must be highlighted and for datasheets referring to a series of components, the relevant one(s) must be highlighted.

## Schematic fields
Every component must have the fields shown in the table below (assigned on a project level with custom field names) in addition to the default ones. These are needed for BOM compilation and Cost Report.

| Field name | URL | Use |
|---|---|---|
| Secondary datasheet | :heavy_check_mark: | Use this if a secondary datasheet is needed. On connectors use this to add the datasheet of the connected device |
| PN | :x: | Part number of the device |
| Store | :heavy_check_mark: | Link to the device's store page |
| Price [€] | :x: | Price of the device at time of design |
| BOM Name | :x: | Simple name of the device, according to the guidelines shown below |

The *BOM Name* field must contain a very simple and short name of the device that must be understandable by everyone.
For simple, generic components use a generic name:
- Resistor
- Capacitor
- Inductor
- LED
- RGB LED
- Connector
- Microcontroller
- Diode
- Zener diode
- CAN transceiver
- Relay
- Voltage regulator
- Crystal
- Optocoupler
- Mosfet
- BJT
- ...

If instead the component has a notable function, write something more specific, but not too much:
- Maintenance connector
- TS connector
- Precharge relay
- HV Resistor
- Isolated CAN transceiver
- ...

## Naming scheme

use the following naming scheme for all projects: `teamname-carname-projectname` (all lowercase)
example: `hw-fenice-steering-wheel`
