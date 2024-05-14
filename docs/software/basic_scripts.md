---
layout: default
title: Basic Scripts
nav_order: 2
parent: Software
---

# Basic Scripts

---

## Accessing the Coug-UV
\
**(1) Connect to the 'inhand' WiFi network**

(password: 'frostlab')

**(2) SSH into the Raspberry Pi**
```bash
ssh frostlab@coug<number>.local 
```
(password: 'frostlab')

**(3) Start the latest Docker container**
```bash
cd ~/CougarsStarter
bash docker.sh
```
(password: 'frostlab')

---

## Starting the Coug-UV
```bash
# from the Docker container
cd ~/ros2_ws
bash start.sh
```
(type Ctrl-C into the terminal to stop if needed)

---

## Testing the Coug-UV
```bash
# from the Docker container
cd ~/ros2_ws
bash agent.sh
```
```bash
# from a new terminal on the Raspberry Pi
cd ~/CougarsStarter
bash extra.sh
 
# from the Docker container (new terminal)
cd ~/ros2_ws
bash test.sh
```

---

## Accessing Bag Files
```bash
# from your local computer
scp -r frostlab@coug<number>.local:~/bag/<bag_wanted> <path_to_destination>
```

---

## Setting Up a New Coug-UV
```bash
# from the newly-flashed Raspberry Pi
git clone https://github.com/snelsondurrant/CougarsSetup.git
cd ~/CougarsSetup
bash setup.sh
 
# download and run the latest Docker image
bash docker.sh
```