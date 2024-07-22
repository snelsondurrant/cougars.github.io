---
layout: default
title: Electrical Instructions
nav_order: 2
parent: Assembly
---

# Electrical Instructions

---
## Main COUG-UV PCB

Open the .brd and .sch files (found below) in a PCB design software. For our purposes we will use Eagle.

For our PCB production we used JLCPCB. In order to process the file correctly for JlCPCB you must first download their custom CAM processor. [Custom Eagle JLCPCB CAM](https://jlcpcb.com/help/article/9-How-to-Generate-Gerber-and-Drill-Files-in-Autodesk-Eagle)

Now return to Eagle under the the .brd tab. Within the toolbar line across the top you will see the cam processor. Open ie and load in the custom processor you downloaded earlier. When it is run you will end up with a .zip file which you will upload to the JLCPCB website.


### Links to Main PCB board (.brd and .sch)

**.brd:**
[COUG_powerboard.brd link](https://byu.box.com/s/raniskul3jnl1tf10c4lscgmdiiq0gin)

**.sch:**
[COUG_powerboard.sch link](https://byu.box.com/s/jcqulffcyls4dua039p1142ic2lz8b0v)

{: .note }
> Put these files in the same folder. This is essential for PCB design software like Eagle to recognize they go together.


## Strobe Light PCB

Utilizing the same method as above, you can send the strobe light PCB out for production. (Links found below)

### Links to Strobe PCB board (.brd and .sch)

**.brd:**
[.brd link](https://byu.box.com/s/raniskul3jnl1tf10c4lscgmdiiq0gin)

**.sch:**
[.sch link](https://byu.box.com/s/jcqulffcyls4dua039p1142ic2lz8b0v)

---

## PCB Assembly
\
![](../../assets/images/COUG_PCB.jpg)

This is the milled board from JLCPCB. To begin soldering the components onto the board I would recommend doing it in the following order.

### LittleFuse and TVS Diode
\
![](../../assets/images/TVS_Littlefuse.jpg)

{: .note }
> Ensure you solder the TVS diode in the correct orientation.

### Headers
\
![](../../assets/images/PCB_Connectors.jpg)

#### Solder the headers in this order.
1. Yellow (1.25 mm headers)
2. Red (2.0 mm headers)
3. Green (2.54 mm headers)

{: .note }
> I used the 1.25mm headers unconventially by soldering surface mount headers into through hole connections. I find it to be easier and sturdier this way.

### Final Components
\
![](../../assets/images/last_PCB_components.jpg)

#### Solder the components in this order.
1. Red (Molex headers and Fuse)
2. Yellow (Header pins)
3. Green (Resistors and Capacitors)
4. DC-DC converter

### Completed Board
\
![](../../assets/images/Completed_PCB.jpg)

The finished board should look something like this.

---

## Thruster and Servos

To complete this step you will need the tailcone and rear extension parts printed.


Make sure the wires for the servo and thruster is threaded from the outside of the tailcone through their holes and then through the penetrators. As shown below.

\
![](../../assets/images/thruster_outside.jpg)

\
![](../../assets/images/thruster_servo_inside.jpg)

POV inside the tailcone

{: .note }
> You may need to cut off the connectors on the servos to fit them through the penetrators.

\
![](../../assets/images/servo_wires.jpg)

After you have the wires threaded through the penetrators you can fit them to the Molex micro connectors. You will need to crimp the ends so that they fit into the connector as shown. 

\
![](../../assets/images/thruster_terminal.jpg)

The three wires from the thruster should be secured in a screw terminal as shown.

