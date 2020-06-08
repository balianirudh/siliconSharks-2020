# Electrical System

The electrical system consists of the electronics that are used to make the ROV operational. The electrical system is designed to provide 
power and communication for all the sensors and cameras with minimal power consumption and simple circuitry. The ROV is surface powered by a 12-volt external power supply which is then converted to 5V onboard the ROV. The vehicle is controlled by a Logitech gamepad controller through a laptop and the video captured by cameras is displayed on the computer.

<p align="center"><img src="https://github.com/balianirudh/siliconSharks-2020/blob/master/images/prototypeElectronics.jpg" width="312" height="300"/></p>
<p align="center"> Prototype Electronics System </p>

## Power Distribution System

The 12V external power supply is connected directly to the onboard electronics through the ROV's tether. On the tether, there is a 25A fuse to ensure that the electronics are protected if the electronics system tries to draw too much current from the power supply. The 12V is supplied directly to a power distribution module. The power distribution module supplies 12V to each of the thrusters and the 12V-7.4V buck converter. Along with this, the power distribution module has an integrated 12V-5V converter which supplies a regulated voltage to the microcontroller.

"show picture of power distribution module and servo voltage converter here"

## Microcontroller

In the prototype electronics system, an Arduino Uno was used because of its affordabiity as well as its open source AVR microcontroller-based development which can be programmed easily. The Arduino had enough PWM ports to connect all of our thrusters and servos. (add something novel about why else we used arduino).
(add documentation about switch to SAM15x15)

<p align="center"><img src="https://github.com/balianirudh/siliconSharks-2020/blob/master/images/arduino-SAM15x15.jpg" width="400" height="300"/></p>
<p align="center"> Side by side comparison of Arduino Uno and SAM15x15 </p>

## Tether

The goal with the tether was to design the most lightweight and thin tether as possible while still satisfying the ROV's electronic demand. The tether encloses just two cables, a power cable and an ethernet cable. The two cables are enclosed in a mesh sheath to keep them together and prevent the cables from tangiling.

"change to better picture of tether"

<p align="center"><img src="https://github.com/balianirudh/siliconSharks-2020/blob/master/images/rovTether.png" width="304" height="300"/></p>
<p align="center"> ROV Tether </p>

To meet the safety requirements of the MATE competition, the tether has an inline 25A fuse. This protects the electronics onboard the ROV if a thruster or servo draws more current than allocated.

### Communication

Control signals are transmitted from a laptop to the ROV through one Category6 Ethernet cable which has 8 cores. Of the 8 cores, 4 cores are used for serial communication and 4 cores are used for the camera video feed. CAT6 was used as it can provide serial communication at a rate of 250 Kbps.

"add picture of USB to ethernet converters"

### Power

Two 12-gauge wires were used to meet the current rating needed for the ROV. A thicker gauge minimizes the voltage drop from the power supply to the electroncis enclosure. A 12 gauge wire is thick enough to carry a 25A current while keeping the overall tether fairly low profile. To connect to a power supply, the tether has Anderson Powerpole connectors while Wago Lever Nuts connect open leads of the tether to the power distribution board inside the electronics housing. Wago Lever Nuts are using within the enclosure due to their compact size compared to Anderson Powerpole connects or XT60 connectors.

"picture of tether connects" "on pic of wago, highlight open leads of tether and power distribution board"


