Flashing the bootloader

Downloading the bootloader
Download the USBaspLoader source code from https://github.com/rtitmuss/USBaspLoader/tree/torn. This can be done directly from Git Hub Desktop.

Arduino Uno as ISP
Program the Arduino Uno as an ISP, as described in Load the Sketch at https://www.arduino.cc/en/Tutorial/ArduinoISP#toc5. See hand written instructions.

Wiring the programmer
Use an Arduino Uno to program the AtMega328P on a breadboard. You need to connect the following pins. See pinout diagrams for the ISP header on the Arduino Uno and the ATMega328P pinout diagram.

Arduino Uno 				Target ATMega328P
ISP Pin 1 - MISO 		Pin 18 - MISO
ISP Pin 2 - +Vcc 		Pin 7 and 20 - +5V
ISP Pin 3 - SCK 		Pin 19 - SCK
ISP Pin 4 - MOSI 		Pin 17 - MOSI
ISP Pin 6 - Gnd 		Pin 8 and 22 - GND
Digital Pin 10 			Pin 1 - Reset

The Arduino Uno board needs a 10µF electrolytic capacitor connected to RESET and GND with the positive (long leg) connected to RESET. The capacitor has to be placed after the programmer board has been loaded with the ISP sketch.

Flashing

You may need to change the port to your Arduino in the Makefile.inc. Replace the path in line 41 /dev/cu.usbmodem* with your own. I used com6 under windows 10.

41:     PROGRAMMER = -c avrisp -P com6 -b19200

Make sure to save your changes before continuing.

Open a QMK MSYS terminal and navigate to your USBaspLoader (bluejay branch) folder and  at that location. Flash the bootloader using:

    make
    make flash
    make fuse

Once the bootloader has been flashed to the board, disconnect the Arduino Uno.