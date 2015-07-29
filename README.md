# nanoGridTestBed
This project is about a **Smart Nanogrid Testbed** for exploring the performance and behaviour of Smart Nanogrids.
This model consists of a hardware and a software part.

##Hardware
The main part of the hardware are four [Raspberry Pi](https://www.raspberrypi.org)s. These mini computers are located in small 3D printed houses.
Each Raspberry Pi has its own house which acts as a case at the same time. Each one of these represent a prosumer in the nanogrid as they consume energy as well as they feed in energy from their PVs.

###House model
The model was designed with the 3D-drawing programm [SketchUp](http://www.sketchup.com) from Google.
The house is about 17 cm long, 15 cm high and 10 cm wide. In the inside of it there is a perfect shaped retainer for the Raspberry Pi.
For this project there are some ports and a LC-Display necessary, because of this there is a big gap in the defined front side and some smaller gaps for USB ports, LAN and 3.5 mm jack.
Two solar panels are located on the roof.
Finally it was printed by a [MakerBot Replicator Fifth Gen](https://eu.makerbot.com/shop/de/3d-drucker/replicator/55/makerbot-replicator).

###Electronics
Each house implements two solar panels, a circuit to emulate consumers and a battery backup. All houses are connected directly without any voltage conversion involved. Within the house voltage conversion is done to and from the predefined voltage which is on the main bus by DC/DC converters.

####PV Panels
Two solar panels are in use. each of them theme is 10 cm long and hast a with of 8 cm. The highest power one that can be

To get the most power out of the PV panels, [MPPT (Maximum Power Point Tracking)](https://en.wikipedia.org/wiki/Maximum_power_point_tracking) is used to detect the sweet spot.

##Software
To keep things simple and straight forward, the software is pure [Java](https://java.com/).

###Accessing the Hardware
For accessing the GPIO on the Raspberry Pi, the [pi4j project](http://pi4j.com) has been used. This library is based on the [WiringPi](http://wiringpi.com) project and offers almost all the features as the native library.

###Communication
Communication has been done using the [JAVA Agent DEvelopment Framework](http://jade.tilab.com).
