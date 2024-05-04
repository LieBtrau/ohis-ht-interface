# OHIS-interface
According to [the OHIS-reference document](https://open-headset-interconnect-standard.github.io/ohis/Open-Headset-Interconnect-Standard.pdf):
> With the Open Headset Interconnect Standard, or OHIS, the club/EOC can build/buy one adapter for every
radio which stays with that radio, and the user only needs to build/buy one adapter for their specific headset
which stays with their headset, and now they can achieve full interoperability with only O(N) adapters.

# Critics to OHIS
* Too many rigs are already using 8C/8p modular jack connectors, but with a different pinout.  There's a big chance of breaking the radio if you plug in the wrong headset.
* The hook on the modular jack easily breaks if you don't protect it.
* One ground wire for mic and a separate ground wire for everything else would be enough instead of all the ground wires in the OHIS standard.
* When compared to a 3.5mm TRRS jack and cable, the modular jack is quite a bulky connector.

# Alternative to OHIS
* [CAIRO](https://web.archive.org/web/20060618023257/http://www-users.aston.ac.uk/~bestpj/cairo/manual/engineering.html#ce1) : based on DIN-connectors

## SATA-interface
OHIS, but using SATA-connectors.  The SATA-interface is a 7-pin connector, which is more than enough for a headset.  The SATA-interface is also a very common connector, and it's easy to find cables and connectors for it.  The SATA-connector has a locking mechanism, which is a big advantage over the TRS-jack.

| Pin | Signal | Description |
| --- | ------ | ----------- |
| 1 | GND | Ground |
| 2 | SPK | Speaker |
| 3 | VCC | Power, max 5V, 200mA |
| 4 | GND | Ground |
| 5 | PTT | Push-To-Talk |
| 6 | MIC | Microphone |
| 7 | GND | Ground |

This repository will contain OHIS-interface boards to the following handheld radios:

## Yaesu FT-65E
* [Radio technical doc](https://github.com/LieBtrau/digital-walkie-talkie/blob/master/SoftwareModem/Yaesu_FT65-E.ipynb)
* [OHIS FT-65E interface, version 1.0.0 (Altium online viewer)](https://365.altium.com/files/52D7B6AC-E25B-4030-AC4F-B64CA4D52889)

## Midland G9 Pro
* [Radio technical doc](https://github.com/LieBtrau/digital-walkie-talkie/blob/master/SoftwareModem/MidlandG9pro.ipynb)

These interfaces might work on more radios, but they have only been tested on the radios listed above.