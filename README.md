# The Privacy Light

A controller for an LED light strip on a five minute timer that you can turn on and off with one button.

## Table of contents

- [Functions] (#functions)
- [What you'll need] (#what you'll need)
- [Setup] (#setup)
- [Background] (#Background)

## Functions

Push the button once and the LED strip will light up red and the light on the button will turn on. After five minutes, these will turn off. If the button is pressed a second time before the five minutes is up, the strip and the button will flash blue three times and they will both turn off. A two second delay has been set at the end to prevent any errors from overzealous button mashing.

## What you'll need

- **Arduino Uno.** The Uno is best for this project, but just about any Arduino board will work.  
- **Adafruit NeoPixel Digital RGB LED strip.** Adafruit has [a wide variety of strips and other devices](https://www.adafruit.com/category/183) that will work. If you would prefer to use a single three pin RGB LED, Arduino has good documentation [here](https://create.arduino.cc/projecthub/muhammad-aqib/arduino-rgb-led-tutorial-fc003e).
- **Adafruit NeoPixel library.** This can be downloaded from [the Adafruit website](https://learn.adafruit.com/adafruit-neopixel-uberguide/arduino-library-use).
- **Momentary switch push button.** I used a Ulincos [U19C3SG Momentary Push Button Switch](http://www.ulincos.com/product.php?id=97), but any momentary switch will work. Be careful not to puchase a latch switch, or you will have to hit the button two times (once to push it down and another time to bring it back up).
- **A few spools of wire.** Three colors are best, since you will need to differentiate between power, ground, and data. If you are a daredevil, one color will do.
- **Jumper wires.** These will allow you to easily connect your components to the Arduino Uno.
- **Wire stripper.** This will make it easier for you to connect your spool wire to your jumper wires.
- **Power supply.** 5V is all you need, but the Arduino Uno is rated up to 12V.
- **Housing.** You need something to mount the button into and something to hold the Arduino Uno. I used a [metal outlet box](https://www.homedepot.com/p/4-in-x-2-in-Drawn-Handy-Electrical-Box-Raised-Ground-8660/100560024) for the housing and an [outlet box faceplate](https://www.homedepot.com/p/RACO-1-Gang-Handy-Box-Blank-Cover-860/202056194?MERCH=REC-_-pipsem-_-202077375-_-202056194-_-N) for the button mount. This will require drilling a hole for your button. To ensure there was no short circuiting, I placed a piece of paper between the back of the Arduino Uno and the metal box.

## Setup

1. Install the code on your Arduino Uno.
2. Disconnect the Arduino Uno from your computer before connecting the wires.
3. Connect the button's switch terminals to pin 4 and GND.
4. Connect the button's LED power terminals to pin 8 and GND.
5. Connect the NeoPixel's data wire to pin 6.
6. Connect the NeoPixel's power wires to 5V and GND.
7. Mount the button on the faceplate and place the Arduino in the outlet box, placing a piece of paper between the back of the Arduino Uno and the outlet box.
8. Using hot glue, affix the LED strip to the wall outside the door.
9. Using screws, mount the housing to the wall inside the room.
10. Enjoy your five minutes of privacy.


## Background

This program was originally developed as a way for my five year old daughter to
indicate she wants privacy in her bedroom without having to lock her door. It is a useful visual timer and can be modified to gradually change color over time.

**Why did you do it like this?** Before the pandemic, I owned an escape room company, so my garage was full of escape room supplies. The button had been a component of a puzzle in on of my games. I also had the LED strip on hand, which is why this project calls for a strip with individually addressable LEDs but makes zero use of that functionality.


## License

[MIT © Punsultant.](../LICENSE)
