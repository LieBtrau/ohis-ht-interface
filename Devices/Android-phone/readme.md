# Measurements
## Maximum mic level
### Hardware setup
1. Connect TRS-cable to sound card (Tip=audio out, Sleeve=GND). 
2. Connect a TRRS-cable to the smartphone (Sleeve=MIC, R2=GND).
3. Connect audio out of TRS with a capacitor to MIC of TRRS.
4. Connect an oscilloscope parallel to the TRRS-cable connections.
5. Connect a 1K resistor from MIC to GND.  The internal microphone of a smartphone headset has the same value.

### Software setup
1. Smartphone runs [Phyphox](https://phyphox.org/) : Audio Scope
2. Laptop runs [REW](https://www.roomeqwizard.com/) : Generator
3. Generator set to 0dB.
4. Increase output volume setting of the laptop just before clipping occurs on the Audio Scope.

### Result
Maximum mic level is 30mVrms before clipping occurs.

## Maximum headphone level
### Hardware setup
1. Connect TRRS-cable to the smart phone
2. Connect oscilloscope between TIP and R2.

### Software setup
1. Smartphone runs [Phyphox](https://phyphox.org/) : Tone Generator
2. Set frequency to 1kHz
3. Set audio level of smartphone to maximum

### Result
AC-level = 457mVrms, DC-offset = 0V
