# Mechanical Subsystems

The ROV is made up of several mechanical subsystems. The primary mechanical systems of the ROV are the frame, the main electronics
enclosure, the camera enclosures, and the gripper. Our goal was to make a neutrally buoyant, compact, and easily-assembled ROV. To do this, there was a constant emphasis on original design and exploiting custom fabrication.

<p align="center"><img src="https://github.com/balianirudh/siliconSharks-2020/blob/master/images/rovIsoView.png" width="391" height="300"/></p>
<p align="center"> Isometric View of ROV </p>
<p align="center"><img src="https://github.com/balianirudh/siliconSharks-2020/blob/master/images/rovFrontView.png" width="326" height="186"/><img src="https://github.com/balianirudh/siliconSharks-2020/blob/master/images/rovSideView.png" width="300" height="186"/></p>
<p align="center"> Front View of ROV (left), Side View of ROV (right) </p>

## Frame

When designing the frame of the ROV, the focus was put on creating a high strenth, lightweight, customizable structure with room for adaptability and expasion. The frame was produced thorugh addititive manufacturing (3D printing) due to its rapid prototyping capabilities and ease of customizable. PLA plastic was the primary plastic used for manufacturing because it was a plastic that was not only strong enough, but it is safe to use in underwater applications.

The parts that make up the frame are connected in several ways. The main way is through brackets that are soley meant to bring a general structure to the frame. From here, specific parts such as the main electronics housing or thruster guards reinforce the frame while serving different purposes altogether.

<p align="center"><img src="https://github.com/balianirudh/siliconSharks-2020/blob/master/images/frameAssembly.png" width="400" height="239"/><img src="https://github.com/balianirudh/siliconSharks-2020/blob/master/images/transparentFrameAssembly.png" width="400" height="241"/></p>
<p align="center">Frame Assembly</p>

In the process of desiging the frame, considerations had to made for the propulsion of the ROV. The team was constrainted to four thrusters. With these four thrusters, the team had to maximize the ROV's degrees of freedom. The way this was done is discussed in the next section.

## Propulsion

As stated before, the team was constrained to four thrusters. This constraint stems from the regulations of the MATE competition and the thrusters chosen for this ROV. For safety reasons, teams participating in the Ranger class are limited to a 25 amp power supply. The thrusters chosen for this ROV were the Blue Robotics T200 thruster. This thruster was chosen because of its force to current ratio and relative affordability.

"screenshot of force vs current graph of thruster"

Knowing that the power supply can only supply 25 amps, in the electrical design, 20 amps was allocated to the propulsion system. This maximizes the current dedicated to thrusters while leaving enough current for other electrical components and a safety buffer to avoid blowing a fuse. Maximizing the total thrust force is advantageous for obvious reasons. It would provide the maximum agility and make the ROV practical for real-world applications.

The final design was between a three thruster configuration or a four thruster configuration. The team opted for the four thrsuter configuration because of its higher total thrust, but more importantly its symmetry resulting in better controllability. The thruster configuration consists of two thrusters dedicated for vertical movement (z-axis) and two thrusters dedicated for lateral movement (xy plane). This thruster configuration with the thrusters ability to produce a thrust in either direction gives the ROV control over its pitch and yaw. However, the ROV doesn't have explicit control of its roll. Buoyancy foam placed on the top of the ROV keeps it upright and prevents it from rolling. 

<p align="center"><img src="https://github.com/balianirudh/siliconSharks-2020/blob/master/images/rovTopView.png" width="338" height="300"/></p>
<p align="center"> Top View of ROV that highlights thruster configuration</p>

In a future iteration of this ROV, the team plans to gimbal the two thrusters dedicated for lateral movement. This will allow the ROV to move on more complicated paths giving the ROV greater freedom in the water.

## Electronic Enclosures & Sealing

### Main Enclosure

The main electronics enclosure is a diecast aluminum enclosure produced by Polycase. The enclosure is a 6.5in box that houses all the main electronics for communication and thruster control. The diecast aluminum is non-porus and high strength to ensure that the material won't allow water to move into the box over long periods of time submerged in water and won't deform under the water pressures we expect to face.

The electronics within the box are accessed by opening the lid of the enclosure that is held down by four screws. The screws ensure that the lid does not move and keeps the face seal O-ring compressed.

<p align="center"><img src="https://github.com/balianirudh/siliconSharks-2020/blob/master/images/electronicsEnclosure.png" width="329" height="299"/><img src="https://github.com/balianirudh/siliconSharks-2020/blob/master/images/internalElectronicsEnclosure.png" width="350" height="299"/></p>
<p align="center"> AN-10F enclosure from Polycase (left), Interior ellectronics enclosure assembly (right) </p>

### Camera Enclosure

The camera enclosure is made up of a clear acrylic tube, two aluminum flanges, and two endcaps. The aluminum flanges allow for the endcaps to mount to the acrylic tube in a way that creates a water-tight seal. Each aluminum flange has two bore O-rings and one face seal O-ring. The acrylic tube compresses the bore O-rings when the flange is inserted and the endcap compresses the face seal O-ring. Clear acrylic tubes were used for the camera enclosures because they make it easy to adjust the camera angle while leaving a wide, unobstructed view for the camera.

"add pictures of camera enclosure"

### Cable Routing

To move cables in and out of the electronics enclosures (with exception to the cameras), aluminum cable penetrators were used. A face seal O-ring on the outside made a water-tight seal with the face of the electronics enclosure while washers inside along with a nut hold the penetrator in place. The cables are secured inside the penetrator with a rubber marine epoxy. This epoxy allows the cable to flex within the penetrator minimizing strain in the cable. The rubber epoxy also ensures no gaps are created by a moving wire.

"add picture of side view of cable penetrator"

For the camera USB cables, submersible grip cords were used to route the cable from the main electronics enclosure to the camera enclosure. Grip cords were used for these specific connections to eliminate the splicing and soldering process that comes with using a regular cable penetrator. Having several solder points in the USB cable was corrupting the camera data so we made a shift to grip cords which solved the problem.

"add picture of grip cord maybe"
