---
layout: default
title: Testing
nav_order: 3
parent: Software Setup
---

# Testing

---

## Testing Connected Sensors
```bash
# from the Docker container
cd ~/ros2_ws
bash agent.sh
```
```bash
# from a new terminal on the Raspberry Pi
cd ~/CougarsSetup
bash extra.sh
 
# from the Docker container (new terminal)
cd ~/ros2_ws
bash test.sh
```

{: .note }
> The micro-ROS publishers on both Teensy's are configured to publish empty messages unless the corresponding sensors are enabled. You can enable/disable sensors using the #define statements in "teensy_ws/controls/src/main.cpp" and "teensy_ws/sensors/src/main.cpp."