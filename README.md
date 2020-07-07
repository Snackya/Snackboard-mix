# Snackboard µX - A DIY audio mixer for deej
![Snackboard photo](/docs/top_view_photo.jpg)

## Description
The Snackboard µX (mix/myx) is a PCB to control application volumes on Linux/Windows using [deej](https://github.com/omriharel/deej).
It is powered by an Arduino Micro over USB and utilises 6 sliders to control the audio volume of the software configured in deej. The microcontroller reads the current state via a 10bit ADC and sends a value of 0-1023 to the PC and deej via serial.

The goal of this build was to create a mixer without any need for a 3D-printer, mill or any kind of casing. It takes advantage of the fact, that most PCB manufacturers only ship 5 prototype board minimum and uses one of them for part assembly and another for a faceplate. All the tracks for connecting parts are routed on the bottom copper layer, so the front paste and silk layers stay clean.

## Specifications
- 222 x 156 x 25 mm
- 6 sliders
- powered via Micro-USB
- [deej](https://github.com/omriharel/deej)

## Parts
- 1x Arduino Micro
- 6x Alps sliding potentiometers, linear, RSA0N12-LIN10K (most alps sliders should work. make sure they are linear and have the same footprint)
- 5x M4 bolts
- 20x M4 nuts

## Usage
Just submit the files in /gerber/ to your preferred PCB manufacturer. (Most manufacturers prefer a .zip archive of these files.)
