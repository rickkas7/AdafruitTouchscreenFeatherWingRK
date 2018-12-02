# AdafruitTouchscreenFeatherWingRK

*Port of Adafruit TFT FeatherWing - 2.4" 320x240 Touchscreen for Particle Argon/Boron/Xenon*

The [Adafruit TFT FeatherWing](https://www.adafruit.com/product/3315) has a touch screen display on the front and a socket for any Feather on the back, including the Particle Argon, Boron, and Xenon. You can find [technical information](https://learn.adafruit.com/adafruit-2-4-tft-touch-screen-featherwing) at Adafruit.

There aren't any wires necessary, but it does use the following pins:

- SPI (SCK, MISO, MOSI)
- SD (SD card CS) = D2
- RT (Touch screen CS) = D3
- TFT_CS (display) = D4
- D/C (display) = D5

This library is just a wrapper around several other libraries:

- [Adafruit\_STMPE610\_RK](https://github.com/rickkas7/Adafruit_STMPE610_RK)
- [Adafruit\_ILI9341\_RK](https://github.com/rickkas7/Adafruit_ILI9341_RK)
- [Adafruit\_GFX\_RK](https://github.com/rickkas7/Adafruit_GFX_RK)

Once the SdFat library is modified to support the mesh devices it will be added as well. 

You don't need to use this library - if you only need the display and not the touchscreen, for example, you can use the Adafruit\_ILI9341\_RK directly directly.

There are two Adafruit examples:

- examples/graphicstest\_featherwing
- examples/touchpaint\_featherwing

Some more examples will be provided in the future.



