# My Awesome Projects

Welcome to my project portfolio, this site is built using Docsify and showcases some of my work.

## Featured Projects

Here are a few highlights:

* **Senior Project:**  Senior Project at Cal Poly Pomona 2016.  Bi-directional transmission of torque through software.
* **Dual Battery E Bike:** LiFePo and SuperCapacitor dual chemistry EV bike.  Supercapacitors have 10x the power output but <1/10th the capacity of LiFePo.  Using both chemistries does introduce design challendges which are addressed in this project.
* **Real Time Super Resolution:**  Thermal cameras have low resolution which makes it difficult for real time applications.  Photo stacking can be used to increase the resolution but typically is not used in real time.  This project explores how to photo stack in real time using some techniques in FIR filters.
* **Eye Mouse:** This was before VR/AR/XR is a thing.  Nothing beats the arc pixel density of a computer screen.  The intent is that a computer screen will simulate the AR screen depending on the eye movements.  First step to do this is to track the eye movements which is explored in this project. 


## More to Explore Work in Progress

Currently I am working on what I call a phaseless brushless DC axial flux motor.  3-phase motors are typical because they were born from the 3-phase power generation and distribution.  4-5-6-phase designs were previously explored but the tradeoffs were not worth the increase in complexity.  Time to revisit this "too complex notion".  Many design aspects are changed, but allows for the follow optimizations below.

### Electrical Optimizations

*** Unconventioal coil excitation ***
Instead of a recommended minimum of 7 pwm cycles for a smooth sine wave, you can go down to 1 cycle and just control when to turn on the driver circuit and let the coil impedance control the sine wave. The 1 cycle can be timed to start earler for higher power.
*** More Cooling surface Area ***
Instead of 1 IGBT or FET driver module that needs lots of cooling. Power can be distributed over multiple driver units which have greater surface area for higher heat extraction. Less chances for critical/cascading failures where one gate failure means whole module is destroyed.
*** Greater Efficiency potential ***
Non-sinusiodal generation means you can apply coil power only at max torque positions.

### Software Optimizations
*** No need for complicated control algorithms ***
Each coil driver only has to know the position and speed of the incoming/outgoing magnet, and the input power demands.  This allows use for "dumb" but blazingly fast Look Up Table control.
*** High pole count without decreasing top speed ***
Poles can be overlapped and "joined" via software control.

### Physical Optmizations 

*** What cogging? ***
Allows use for nonconventional stator rotor pole counts like 5:7 or more, with high stator/rotor poles like 10:15 cogging is reduced to be negligible.
*** Higher total flux densities: ***  
Many smaller magnets and poles allow for more airgap surface area.
Increasing flux density by creating bigger magnets have diminishing returns simply because you are adding more magnet mass further away from the airgap. Smaller magnets are cheaper and have greater flux density to volume.
*** Better Flux Paths *** 
Instead of trying to push the flux out from the magnets by adding reluctance paths, you can pull the flux out with the other magnets.
*** Decrease in total loads in rotor ***
You only have to strengthen the outside stacks of the magnets since they experience axial loads.  The middle stacks are pull relatively equally which means rotor only needs to deal with radial and tangential loads. Outer stacks can be thick since they are at the ends.
*** Dual coil optimization ***
Allows use of multiple different wire gauges so you can have half the motor optimized for efficiency and the other half optimized for power. These can be split with seperate coil drivers in the same unit.
*** Dual Cell Chemistries ***
Similar to the previous dual coil optimization which allows you to use multipl cell chemistries to power one motor. You can even run one coil in drive and the other in regen to transfer power to and from each cell chemistries. So now cells can be optmized solely for power or range, instead of balancing both in one.
*** Optimized Cooling ***
High stator surface area means high heat extraction.  Why have water cooling just to have an water to air intercooler.  The spinning of the rotor introduces turbulence to help the air extract heat from the stator.

I'm constantly adding new projects, so be sure to check back often!
