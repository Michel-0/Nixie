# Nixie
All you need to know to build a cold cathode tube display clock

## Concept
There are many different layouts with different features possible.

**Best for me is the following:**
![NTC](https://github.com/user-attachments/assets/dcb12e0a-b194-440a-8b89-950e80abbbd8)
* Controlled by a Raspberry Pi Pico.
* Designed for Gazotron IN-14 tubes, may be adapted for others easily.  
E.g. IN-8 and IN-8-2 should be compatible without any change.
* Makes use of the right decimal point of the tube, but not the left one.
* Prepared for IN-3 tubes as colon dots.
* Tube voltage step-up boost converter not inclued on this PCB.  
Instead the layout has free space and connectors for it.
* Unlike most others, this doesn't use a RTC (real-time clock) with battery to keep the exact time.  
Instead a DCF77 (77,5 kHz) radio clock receiver to get the time once powered on.
* Tube driver based on MPSA42 transistors controlled by MCP23008 & MCP23017 connected by I²C to the pico.  
No historical sovjet ICs necessary
* Supplied by external 12V DC.
* Provides connectors for 5V RGB LEDs (e.g. WS2812B).

## Repository
### KiCAD project
Folder `NTC` contains 2 projects:
* **Main**:  
Clock schematic and PCB
* **Socket**:  
IN-14 schematic and PCB
* As well as a project footprint library and a project schematic symbols library.
* Also the CAD models which weren't included in the default library.

### C++ VSCode project
Pico software may or may not be added to this repository in near future.

## Datasheets
[IN-14 Manual](../../wiki/IN‐14-Manuals)

## Dimensioning
[IN-14 Calculations](../../wiki/IN‐14-Calculations)
