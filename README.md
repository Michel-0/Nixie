# Nixie
All you need to know to build a cold cathode tube display clock

## Concept
There are many different layouts with different features possible.

**Best for me is the following:**
![NTC](https://github.com/user-attachments/assets/dcb12e0a-b194-440a-8b89-950e80abbbd8)
* Controlled by a Raspberry Pi Pico
* Designed for Gazotron IN-14 tubes, may be adapted for others easily
* Prepared for IN-3 tubes as colon dots
* Tube voltage step-up boost converter not inclued on this PCB,  
instead the layout has free space and connectors for it
* Unlike most others, this doesn't use a RTC (real-time clock) with battery to keep the exact time,  
instead a DCF77 (77,5 kHz) radio clock receiver to get the time once powered on
* Tube driver based on MPSA42 transistors controlled by MCP23008 & MCP23017 connected by I²C to the pico  
No historical sovjet ICs necessary
* Supplied by external 12V DC
* Provides connectors for 5V RGB LEDs (e.g. WS2812B)

## Repository
### KiCAD project
Folder `NTC` contains 3 projects:
**NTC** (*contains all*), **Main** (*clock schematic and PCB*), **Socket** (*IN-14 PCB*), as well as a project footprint library (containing **all** used footprints) and a project schematic symbols library (contains only a single symbol, all others are out of default libraries).

### C++ VSCode project
Pico software may or may not be added to this repository in near future.

## Datasheets
Soon to be found on the wiki page.

## Dimensioning
Resistor and voltage calculations to be added soon.
