---
layout: default
title: Quick Start
nav_order: 1
parent: Operation
---

# Quick Start

---

## Connecting to the Coug-UV
\
**(1) Connect to the "inhand" WiFi network**

(password: "frostlab")

**(2) SSH into the Raspberry Pi**
```bash
ssh frostlab@coug<number>.local 
```
(password: "frostlab")

**(3) Start the latest Docker container**
```bash
cd ~/CougarsSetup
bash docker.sh
```
(password: "frostlab")

---

## Starting the Coug-UV
```bash
# from the Docker container
cd ~/ros2_ws
bash start.sh
```
(type Ctrl-C into the terminal to stop if needed)

{: .note }
> Different ROS 2 nodes can be enabled/disabled from running on start by editing the "cougars_launch.py" file in "ros2_ws/src/cougars/launch/."

---

## Copying Bag Files
```bash
# from your local computer
scp -r frostlab@coug<number>.local:~/bag/<bag_wanted> <path_to_destination>
```
