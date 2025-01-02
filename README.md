# Nixie
All you need to know to build a cold cathode tube display clock

## Concept
There are many different layouts with different features possible.

**Best for me is the following:**
![NTC](https://github.com/user-attachments/assets/dcb12e0a-b194-440a-8b89-950e80abbbd8)
* Controlled by a Raspberry Pi Pico
* Designed for Gazotron IN-14 tubes, may be adapted for others easily
* Prepared for IN-3 tubes as colon dots
* Tube voltage Step-up boost converter not inclued on this PCB,  
instead the layout has free space and connectors for it
* Unlike most others, this doesn't use a RTC (real-time clock) with battery to keep the exact time,  
instead a DCF77 (77,5 kHz) radio clock receiver to get the time once powered on.
* Supplied by external 12V DC
* Provides connectors for 5V LEDs (e.g. for WS2812B)

## Datasheets
Soon to be found on the wiki page.

## Dimensioning
Resistor and voltage calculations to be added soon.
