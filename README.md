# MicroFTDI
My take on a tiny modern USB to UART converter.

<img src="/images/V2Front.jpg" width="40%" alt="V2 Board Front"/>    <img src="/images/V2Back.jpg" width="40%" alt="V2 Board Back"/>

This one works like any other, but here are the specs anyways:

Board Size: 23.8x13.7x1.6mm\
Soldered module size: 31.7x13.7x6.4mm\
Connectors: USB-C to male 2.54mm dupont headers\
Max current supply: 1A at 3.3V with voltage regulator (often limited by USB supply)\

Bugs to squash: 
- Not sure, however TX ad RX labels might be switched around. According the the datasheet it should be correct.
- No easy way to disconnect internal regulator from external one without scratching out a copper trace which is difficult to do.

Improvements:
- Add zero ohm resistor to switch between using the built in regulator or the external one.
- Perhaps add power indicator LED?
- Different color RX and TX?
- Find part number of correctly angled dupont connectors.
- Design and print a case (Not something I have a use for, so I won't do this)
- Might want to add USB ESD protection?

The chip selection of FT230XQ-R is not the cheapest option, but it is a nice reliable chip, and has a very small footprint.
I am open to and looking for cheaper alternatives to reduce cost of this device.