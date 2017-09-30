# ONC_Autonomous_Robot

This repository showcases the code used for a school project in first year engineering at University of Victoria.

## Background
Ocean Networks Canada is a UVic research initiative that uses deep-sea sensors to monitor chemical and biological conditions on the ocean floor. Due to the depth of the sensors, it is necessary for them to be cabled for adequate power and data-retrieval. Unfortunately, cables deteriorate in deep-sea environments and need to be replaced.

Due to the high cost and danger of sending human divers down to recable the sensors, it would be preferable if there was a robot which could navigate the ocean floor to find the sensors and attach new cables. This is where we came in. Our class was divided into groups of 3-4 and tasked with creating prototypes for an autonomous cabling robots using VEX Cortex robotics kits. I was lucky enough to have a few mech students in my group that were more than happy to let me take care of all the coding.


## Conceptualization

The prototype was meant to be a proof of concept for beacon location and cable connection. It would be placed in an arena facing away from a target beacon. The robot would then - without any intervention - have to locate the beacon, move toward it, attach a cable (or similar mechanism), and proceed to the edge of the arena without disturbing the cable it had just attached.

We were strongly encouraged to use a switch-case implementation and develop a finite state machine to guide our robot's actions.

![Imgur](https://i.imgur.com/SWFNfqT.jpg)


The FSM itself is fairly self-explanatory; the robot has 8 active states that it switches between based on sensory input and the completion of motor functions. The robot used an accoustic rangefinder and dual infrared sensors for sensory input. The beacon had attached to it, infrared lights flashing at 10Hz. This was to be our means of locating the beacon in order to proceed.

Without going into too much detail about the physical structure, our robot used a two-train locomotive system for movement on a four-wheeled square base. The cable-attachment mechanism used an earth magnet on a heavy-duty string for the sake of simplicity. The magnet was held in a mobile claw which can pinch or retract on command.

!


## The Source Code


##
