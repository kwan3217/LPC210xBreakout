# LPC210xBreakout
Breakout board for NXP LPC2101/2/3 microcontroller. The pinout for the crystals and power is similar enough to that of an LPC2104/5/6 that it will
probably work for that chip as well.

# How to use
All 48 pins on the chip are broken out to their respective pins on the board. Digital grounds (3 pins) are connected together. Several pins are connected to each other through default-shorted jumpers. If you wish, you can cut the jumpers with a razor blade.

 * Analog ground (pin 31) to digital ground
 * Analog power (pin 42) to digital I/O (3.3V) power
 * RTC power (pin 4) to digital I/O (3.3V) power

The chip uses a 1.8V core voltage, and needs both 3.3V and 1.8V to operate. I have included a 3.3->1.8V regulator on the board. Since the 1.8V supply pin is broken out, you don't have to use this regulator if you don't want -- just don't populate the regulator.

# Interesting things and oddities
The board file has the footprint for a TSSOP-16 and a TSSOP-20 chip. These footprints are outside of the board outline, and are there so that the stencil
I make also has those footprints, for another project I am working on.

# Getting this board
I recommend getting the board from oshpark.com. There isn't an explicit bill of materials. Instead, each component has either a Digikey or Mouser part number -- use those for generating your own bill of materials.

# How to modify
This board is Open Hardware, licensed under the GPL 3.0 license. That's the legal part. My intent is that:
 * You can make as many exact copies of the board as you wish. The link at oshpark.com is a good place to do that.
 * You may modify the board as you wish, but if you do so, please remove my StKwan logo from the board. If you are modifying it, you should take pride in your work and put your name on it anyway.
 * Follow the rest of the GPL as concerning share-alike, etc.
