# Electrical System

The electrical system consists of the electronics that are used to make the ROV operational. The electrical system is designed to provide 
power and communication for all the sensors and cameras with minimal power consumption and simple circuitry. The ROV is surface powered by a 12-volt external power supply which is then converted to 5V onboard the ROV. The vehicle is controlled by a Logitech gamepad controller through a laptop and the video captured by cameras is displayed on the computer.

## Power Distribution System

The 12V external power supply is connected directly to the onboard electronics through the ROV's tether. On the tether, there is a 25A fuse to ensure that the electronics are protected if the electronics system tries to draw too much current from the power supply. The 12V is supplied directly to a power distribution module. The power distribution module supplies 12V to each of the thrusters and the 12V-7.4V buck converter. Along with this, the power distribution module has an integrated 12V-5V converter which supplies a regulated voltage to the microcontroller.

"show picture of power distribution module and servo voltage converter here"

## Microcontroller


