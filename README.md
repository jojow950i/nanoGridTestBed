# nanoGridTestBed
This project is about a Smart Nanogrid Testbed for exploring the performance and behaviour of Smart Nanogrids. 
This model consists of a hardware and a software part. 

##Hardware
The main part of the hardware are four Raspberry Pis, these mini computer are located in small 3D printed houses. 
Each Raspberry has its own case.
Small 3D printed houses and Raspberry Pis represent the houses. 

###House model
The model was designed with the 3D-drawing programm SketchUp from Google. 
The house is about 17 cm long, 15 cm high and 10 cm wide. In the inside of it there is a perfect shaped retainer for the Raspberry Pi. 
For this project there are some ports and LC-Display necessary, because of this there is a big gap in the defined front side and some smaller gaps for USB ports, LAN and 3.5 mm jack.
Two solar panels are located on the roof.  

###Electronics
Each house implements two solar panels, a circuit to emulate consumers and a battery backup. All houses are connected directly without any voltage conversion involved.

##Software
###Accessing the Hardware
For accessing the GPIO on the Raspberry Pi, the pi4j project (http://pi4j.com) has been used. 

###Communication
Communication has been done using the JAVA Agent DEvelopment Framework (http://jade.tilab.com).




