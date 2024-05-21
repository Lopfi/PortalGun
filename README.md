# PortalGun
Code to control a Portal Gun (From Rick and Morty)
[Link to 3D model](https://www.thingiverse.com/thing:1100601)
##Libraries
Download and install the following libraries:

- [ClickEncoder](https://github.com/0xPIT/encoder)
- [Adafruit_GFX](https://github.com/adafruit/Adafruit-GFX-Library)
- [Adafruit_LEDBackpack](https://github.com/adafruit/Adafruit-LED-Backpack-Library)


## Pin Definitions
If you deviate from the following definitions, you will have to change the firmware to account for that.

| LED Display | Arduino Nano |
|--------|--------|
|   SCL  |   A5   |
|	SDA  | 	 A4   |
|	GND  | 	 GND  |
|	Vcc  |   5V   |
|   Vi2c |   5V	  |


| Rotary Encoder | Arduino Nano |
|--------|--------|
|    A    |   4  |
|    B    |   5  |
|   GND   |  GND  |
| Button  |   2  |


| Neopixel | Arduino Nano |
|-------------|---------|
|Data         |    11   |


## Installing Firmware
Connect the arduino select the correct model and port, then hit upload.

## Button Behavior
The rotary encoder has a click button, and we can detect a single click, a double click, and a hold.
- Single Click : Wakes the Trinket Pro from low power mode
- Double Click : Reset to dimension C137
- Hold : Turn off LEDs and put the Trinket Pro into a low power mode.

##Installing SFX
The main branch doesn't have SFX support. Use the SFX branch to test this out (I found that the speaker inside the case was too quiet to hear.)
