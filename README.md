# Acknoledgement
**Special thanks to [u/j_oshreve](https://www.reddit.com/user/j_oshreve/) on Reddit** for all his work on https://github.com/joshreve/dactyl-keyboard. Without all his is doing this project would not have been possible. 

I would note this repo would gave me a great guide to get to a working product. https://github.com/OutstandingOof/ducktyl-manuform

# Though Process

# requirements 
* case
* tray holder
* ec11 adapter
* Screws 
* Screw inserts
* diodes
* wires
* Elite C / Pro Micro
* oled screens
* ec11 encoders
* switches
* keycaps

# The Build
## The case
all the 3D design and case generation was done thanks to the awesome work from u/j_oshrev at https://github.com/joshreve/dactyl-keyboard
## Wiring 
## The oled screens
connect GND to GND, VCC to VCC, SDA to pin 2 and SCL to pin 3.
## Rotary Encoders
To add the rotary encoder, wire the two pins on one side into the matrix, just like any other switch (press the encoder acts like any other switch). f
From the other side of the encoder (the one with 3 pins) connect the middle one to GND. The two outer pins of the other side have to be wired to the pins A2 and A3. 

# The Code
