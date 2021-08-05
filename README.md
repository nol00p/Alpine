# The Ptero-Dactyl

this the final result:

![Ptero-Dactyl](/media/Ptero-Dactyl.JPEG)


# Acknoledgement
**Special thanks to [u/j_oshreve](https://www.reddit.com/user/j_oshreve/) on Reddit** for all his work on https://github.com/joshreve/dactyl-keyboard. Without all his is doing this project would not have been possible. 

I would note this repo would gave me a great guide to get to a working product. https://github.com/OutstandingOof/ducktyl-manuform

# Though Process
the aim of the build is to try to get as clean a result as possible with all the features fully integrated in the case design. both the LCD are fully integrated in the case. the trays on both sides are mirrored to avoid crossing the trrs and the usb. 

# requirements 
* 3 Printer for : 
  ** case
* tray holder
* ec11 adapter
* Screws: whatert M3 screws
* Screw inserts
* diodes: 1N4148
* wires: I recommend single core wire, it is much easier to work with
* controllers: Elite C or Pro Micro x2
* oled screens: SSD1306 128x32 0,91" OLED Display x2
* ec11 rotary encoders x2 
* Kailh hot swap sockets
* switches
* keycaps

# The Build
## The case
all the 3D design and case generation was done thanks to the awesome work from u/j_oshrev at https://github.com/joshreve/dactyl-keyboard


## Wiring 
![wiring](/media/wiring.jpg)

the wiring for a Pro Micro controler is the exact same.

## The oled screens
connect GND to GND, VCC to VCC, SDA to pin 2 and SCL to pin 3.
## Rotary Encoders
To add the rotary encoder, wire the two pins on one side into the matrix, just like any other switch (press the encoder acts like any other switch). f
From the other side of the encoder (the one with 3 pins) connect the middle one to GND. The two outer pins of the other side have to be wired to the pins A2 and A3. 
![encoder](/media/encoder.jpeg)

# The Code
