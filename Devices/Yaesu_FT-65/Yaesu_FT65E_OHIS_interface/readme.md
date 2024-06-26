# Headphones
* 0dBV to -10dBV into a 16ohm to 64ohm load, a series resistor will be needed to drop the voltage to the correct level.
* No audio transformers because the radio only has 1 ground connection
* The radio has a H-bridge output stage.  The output is at 1.85V when no audio is present.  A capacitor is used to block the DC voltage.
* A small capacitor, parallel to the headphones, is used to filter out the high frequency noise.
* Only one channel is used to feed both headphones.  The radio has a mono output.  This reduces the number of components needed.

# Connection to the radio
* TRS-plugs (3.5mm and 2.5mm) and can be soldered directly to the interface:
  * Solder sleeve to the PCB.
  * Solder tip and ring using a loops of wire through two holes on either side of the plug.
* No filtering on TRS-plugs.
* GND of radio is directly connected to GND of interface.  The UTP-cable might be used as "radial" for the antenna.

# Connection to a sound card
Might also be connected to [Ai-thinker esp32-audio-kit](https://docs.ai-thinker.com/en/esp32-audio-kit), which uses an [ESP32-A1S module](https://docs.ai-thinker.com/_media/esp32-a1s_v2.3_specification.pdf)
Requires two 3.5mm TRS-jacks.  One for (line) input and one for (headphone) output.

# Isolation
If isolation is really needed, then an OHIS-OHIS interface could be created that contains two audio transformers.

# Connection to UART interface
* 6 pin JST XH connector (2.5mm pitch) to avoid wrong connection
* USB-UART bridge:
  * [Adafruit CP2102N Friend - USB to Serial Converter](https://www.adafruit.com/product/5335)
  * [Adafruit 70](https://www.adafruit.com/product/70)
  * [FTDI  TTL-232R-3V3](https://ftdichip.com/products/ttl-232r-3v3/)