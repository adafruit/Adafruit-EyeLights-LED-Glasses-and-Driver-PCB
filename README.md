## Adafruit EyeLights LED Glasses and Driver PCB

<a href="http://www.adafruit.com/products/5217"><img src="assets/5217.jpg?raw=true" width="500px"><br/>
Click here to purchase the EyeLights Glasses Driver from the Adafruit shop</a>
<a href="http://www.adafruit.com/products/5210"><img src="assets/5210.jpg?raw=true" width="500px"><br/>
Click here to purchase the EyeLights Glasses from the Adafruit shop</a>

PCB files for the Adafruit EyeLights LED Glasses and Driver. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/5217
* https://www.adafruit.com/product/5210

### Description

This board is designed to be a thin, bluetooth-enabled driver board for our Adafruit LED Glasses RGB LED matrix. That said, it's a perfectly good stand-alone development board for the Nordic nRF52840 chipset, with a very slim design, optional LiPo battery support, a few sensors, and a Stemma QT port for adding other devices or sensors with I2C plug-and-play.

The driver looks a little like a Feather but it does not have any breakout pins to keep it very compact. If you need access to GPIO pins, we recommend an nRF52840 ItsyBitsy, nRF52840 Feather or Feather Sense.

In exchange for GPIO outputs, we added some sensors on instead: each board comes with a LIS3DH triple-axis accelerometer that can be used for motion and orientation sensing, and a PDM digital microphone for audio sensing. To add more sensors or connect to the LED Glasses front panel, there's a  STEMMA QT connector for plug-and-play I2C support.

Unlike our Itsy/Feather boards, this driver also comes with a proper on/off switch which will cut power to the microcontroller and external sensors. There's optional LiPo charge support because we think that many folks will want to power this board with AAA or coin cell batteries. If you'd like to enable LiPo charging, short the jumper on the back and then make sure to only use 4.2V/3.7V rechargeable batteries in the battery port.

The nRF52840 is a lovely Bluetooth LE microcontroller, with good support in both Arduino and CircuitPython. It feathers a Cortex M4 processor with 1 MB of FLASH and 256KB of SRAM. Best of all, it's got that native USB! Finally, no need for a separate USB serial chip like CP2104 or FT232. Serial is handled as a USB CDC descriptor, and the chip can act like a keyboard, mouse, MIDI device or even disk drive. This chip has TinyUSB support - that means you can use it with Arduino as a native USB device and act as UART (CDC), HID, Mass Storage, MIDI and more!

Board Features:

* ARM Cortex M4F (with HW floating point acceleration) running at 64MHz
* 1MB flash and 256KB SRAM
* Bluetooth Low Energy compatible 2.4GHz radio (Details available in the nRF52840 product specification)
* FCC / IC / TELEC certified module with up to +8dBm output power
* 2MB external QSPI flash for CircuitPython file storage
* Built in LIS3DH accelerometer and PDM microphone
* Red LED for general purpose blinking, plus a tiny NeoPixel for colorful feedback
* STEMMA QT connector for plug-and-play I2C support.
* JST PH 2-pin battery port with optional LiPoly charger
* 4 mounting holes/slots
* Reset button and User button
* Native USB supported by every OS - can be used in Arduino or CircuitPython as USB serial console, Keyboard/Mouse HID, even a little disk drive for storing Python scripts.
* Can be used with Arduino IDE or CircuitPython
* Comes pre-loaded with the UF2 bootloader, which looks like a USB storage key. Simply drag firmware on to program, no special tools or drivers needed! It can be used to load up CircuitPython or Arduino IDE

For developers, we pre-programed the chip with our UF2 bootloader, which can use either command line UART programming with nrfutil (we use this for Arduino) or drag-n-drop mass storage, for CircuitPython installation and also because mass-storage-drive bootloaders make updating firmware so easy. Want to program the chip directly? You can use our command line tools with your favorite editor and toolchain. If you want to use an SWD programmer/debugger (for even more advanced usage), we have broken out the SWD pads for easy soldering.

Have you always wanted to upgrade your ensemble with a creepy-cool creature PCB silkscreen and an eye-blistering arrangement of LEDs? We love to put NeoPixels on our face, as evidenced by our many glowy LED glasses projects. Each of these requires quite a bit of soldering, and the cost of each NeoPixel adds up quickly. So we wanted to make a PCB assembly that can be used by any microcontroller to make glamorous face-tronics.

The Adafruit LED Glasses Front Panel has 116 artfully arranged 2x2mm RGB LEDs, all controlled with an IS31FL3741 I2C Driver that handles all the PWMing, so it's plug-and-play with almost any microcontroller.

On each side are STEMMA QT / JST-SH plugs - use these with one of our cables to attach it to your driver board of choice. Of course, you can pick left or right, then if you want to add on more hardware, like an accelerometer or light sensor, you can chain onto the other side. There's also six mounting holes for attaching to a glasses frame of your choosing - we recommend getting some 'fashion frames' from the mall or a street vendor, they're all the style and will provide a great mechanical support.

We have four different silkscreen designs: Bug, Wolf, Cat, and Dragon (peep those fearsome fangs!) Each design is exactly the same mechanically and electrically, the only difference is what is silkscreened on top of the PCB.

Gaze upon these features:

* IS31Fl3741 LED driver chip uses I2C to control the LEDs with 8-bit PWM per color (24-bit per RGB LED), write pixel data and it will handle the matrix driving automatically.
* Power and communicate over STEMMA QT for easy wiring
* The LEDs are arranged as 2 x 24-LED rings around each eye and an overlapping 16x5 matrix. The matrix has two bottom pixels 'missing' over the nose. Some LEDs are shared between both matrix and rings!
* Arduino and CircuitPython/Python library support

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
