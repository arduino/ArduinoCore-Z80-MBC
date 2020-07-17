# Arduino board platform for Z80-MBC

The [Z80-MBC](https://hackaday.io/project/19000-a-4-4ics-z80-homemade-computer-on-breadboard) is a mini Z80 system implemented by [Just4Fun](https://hackaday.io/Just4Fun) using an Atmega32A.

This repository contains an extension to [MightyCore](https://github.com/MCUdude/MightyCore) by [MCUDude](https://github.com/MCUdude) which adds a menu item in the Arduino IDE that allows users to select the serial buffer size limit.

The main purpose of this repository is to show a less known feature of the Arduino cores, i.e. the ability to extend an existing core without copying and pasting everything. The referencing syntax allows to inherit the definitions from an existing core, and just add or override the desired things. Read the [documentation](https://arduino.github.io/arduino-cli/latest/platform-specification/#referencing-another-core-variant-or-tool) to learn more about extending cores.

### Installation

This repo was created mainly for demonstration purposes so it's not part of the official Arduino core index. You'll need to install it manually:

- This platform has a dependency on MightyCore so you must also install that platform, following its [instructions](https://github.com/MCUdude/MightyCore#how-to-install)
- Download this platform from https://github.com/arduino/ArduinoCore-Z80-MBC/archive/master.zip
- Extract the folder into the **hardware** subfolder of your sketchbook folder. You can find the location of your sketchbook folder in the Arduino IDE at **File > Preferences > Sketchbook location:**.
- If the Arduino IDE is running then restart it.

### Usage
- Select the "Z80-MBC" board from the Arduino IDE's **Tools > Board** menu.
