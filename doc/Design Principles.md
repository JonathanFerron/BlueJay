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
- keep trace from decoupling caps to ground plane as short as possible
- fuse and large decoupling cap close to usb jack, large decouping cap close to jack on right hand
- keep usb data lines short and same length, no vias
- regular trace .25mm and power trace .4mm
- ideal spacing between PTH components: spread components on entire board as uniformly as possible, minimum distance between two components (body to body) of 4mm, minimum distance from lead to lead of 2.54mm (100 mils), or minimum distance equal to height of the neigbour components
- minimize number of vias
- keep traces short in general

- split, can be tented (very moderate, 3 to 4 degrees, use rubber bumpers)

- through hole

- 6 columns, 5 rows in total (of which one is thumb cluster): 5 top row + 3x6 middle + 4 thumb cluster per hand: total of 54 keys
	+ All 1U keys:
	+ 10 x R1 top (number) row
	+ 12 x R2 qwerty row
	+ 10 x R3 home row + 2 R3 homing keys
	+ 12 x R4 bottom row
	+ 8 x R2 thumb keys (get an extra set of 8 R1 keys as well)
	+ = Total 54 keycaps