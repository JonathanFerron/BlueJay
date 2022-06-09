# BlueJay54 design principles

- no oled
- exclude 6 pin for programming chip since chip is socketed (can be progammed on a breadboard or connect with test hooks)
- no rotary encoder
- reduce leds from 3 to 0
- no led on board per se (opt)
- no per key rgb
- no underglow
- no speaker

- kailh mx hotswap sockets only, chery mx mount
- move step up resistors for trrs connection to right hand
- row2col scanning
- usb mini b
- reduce A of fuse to 100mA (hold current) (200mA trip current max)
- add a second 4.7uF decoup cap to right hand

- blue pcb
- gazzew boba u4 65g or 68g keys
- black dcs keycaps

- crystal and small decoupling caps closest to mcu
- fuse and large decoupling cap close to usb jack
- keep usb data lines short and same length, no vias
- regular trace .25mm and power trace .4mm
- minimize number of vias
- keep traces short in general

- split, can be tented (very moderate, 3 to 4 degrees, use rubber bumpers)

- through hole

- 6 columns, 5 rows in total (of which one is thumb cluster): 5 top row + 3x6 middle + 4 thumb cluster per hand: total of 54 keys

