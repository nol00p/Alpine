# The Alpine Project

this the final result:

![Ptero-Dactyl](/media/Ptero-Dactyl.JPEG)


# Acknoledgement
**Special thanks to [u/j_oshreve](https://www.reddit.com/user/j_oshreve/) on Reddit** for all his work on https://github.com/joshreve/dactyl-keyboard. Without all his is doing this project would not have been possible. 

I would note this repo would gave me a great guide to get to a working product. https://github.com/OutstandingOof/ducktyl-manuform

if you have questions on the build or any of the tools I used hit me up reddit [u/loss_of_signal](https://www.reddit.com/user/loss_of_signal)

# Though Process
the aim of the build is to try to get as clean a result as possible with all the features fully integrated in the case design. both the LCD are fully integrated in the case. the trays on both sides are mirrored to avoid crossing the trrs and the usb. 

# requirements 
* 3 Printer for : 
  * case: both sides top and bottom
  * tray holder: both sides 
  * ec11 adapters
  * LCD tray
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
![print](/media/Print.JPEG)

After the printing goes the painfully long process of picking out all of the support material, beeing carefull not to break anything. 

![print](/media/support.JPEG)

once the case is cleaned up, get the rest od teh component printed and install the sockets. 

![print](/media/kit.JPEG)

for this build I forked the loligagger tray to have a mirror version so that the usb and trrs wouldn't get crossed 

![tray](/media/tray.JPEG)
![tray2](/media/tray2.JPEG)


## Wiring 

the wiring is pretty straigh forward, juste take your time and use the right type of wires. I recommand signle core wire. for the wiring i follow this: 
![right](/media/dactyl_manuform_right_wire_diagram.png)
![left](/media/dactyl_manuform_left_wire_diagram.png)

this key here is to get the diode orientation right! the black line on the diodes should all be connected together to from the row. the idea is that the current would not go back in the switch when activated. 

### The oled screens
connect GND to GND, VCC to VCC, SDA to pin 2 and SCL to pin 3.

### Rotary Encoders
To add the rotary encoder, wire the two pins on one side into the matrix, just like any other switch (press the encoder acts like any other switch). f
From the other side of the encoder (the one with 3 pins) connect the middle one to GND. The two outer pins of the other side have to be wired to the pins A2 and A3. more details bellow.
![encoder](/media/encoder.jpeg)

### the controller

the final part is to connect all those wire to the controller. 

![wiring](/media/wiring.jpg)

the wiring for a Pro Micro controler is the exact same.

the end result is something like this

![wired](/media/wired.jpeg)

# The Code
for simplicity I have opted to go with 2 elite-c controlers. it makes flashing both half of the keybaord much more straight forward.  
note that to date the code for the oled screens is from the lily58. I need to spend some time to tweak that part to get to something I actually like. 
