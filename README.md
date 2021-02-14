# MicroFTDI

###### My take on a tiny modern USB to UART converter.

<img src="/images/V2Front.jpg" width="40%" alt="V2 Board Front"/>    <img src="/images/V2Back.jpg" width="40%" alt="V2 Board Back"/>

## Specs:

**Board Size:** 23.8x13.7x1.6mm\
**Soldered module size:** 31.7x13.7x6.4mm\
**Connectors:** USB-C to male 2.54mm dupont headers\
**Max current supply:** 
- without regulator: 50mA @ 3.3V
- with regulator: 1A @ 3.3V (often limited by USB supply)

## V3:

#### V3 Changelog:
- Added R7 resistor that can be removed if using external regulator.
- Switched RX and TX label on LEDs. Now the are labelled from the computer's (USB) perspective.

#### EasyEDA link:
https://oshwlab.com/Cinbarker/ftdi-c_copy

## V2:

#### Bugs to squash:
- Not sure, however TX ad RX labels might be switched around. According the the datasheet it should be correct. **(update: done)**
- No easy way to disconnect internal regulator from external one without scratching out a copper trace which is difficult to do. **(update: done)**

#### Improvements:
- Add zero ohm resistor to switch between using the built in regulator or the external one. **(update: done)**
- Perhaps add power indicator LED? 
- Different color RX and TX?
- Find part number of correctly angled dupont connectors.
- Design and print a case (Not something I have a use for, so I won't do this)
- Might want to add USB ESD protection?


## Notes:
The chip selection of FT230XQ-R is not the cheapest option, but it is a nice reliable chip, and has a very small footprint.
I am open to and looking for cheaper alternatives to reduce cost of this device.