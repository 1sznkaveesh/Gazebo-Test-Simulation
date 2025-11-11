# Gazebo-Test-Simulation

# Mobile Differential Drive Robot-
- This package provides a simulated mobile differential drive robot, modeled and tested using Gazebo, URDF, and Xacro in the ROS2 framework.​

# Features-
- Modular robot description using URDF and Xacro for flexible configuration and parameterization.​​
- Gazebo simulation support for dynamic testing and visualization of robot behavior.​​
- Launch files provided for spawning the robot in Gazebo with all relevant plugins and state publishers.​

---
### Modeling Approach

- URDF defines robot structure: links, joints, physical properties.
- Xacro adds macros and parameters for easier editing.
- Gazebo simulates physics and environment for robot testing.

---

## Getting Started


### 1. Clone this repository
```bash
cd ~/ws_ddmobile
```

### 2. Build the package
```bash
colcon build
```

### 3. Source the workspace

```bash
source install/setup.bash
```

```bash
source /opt/ros/humble/setup.bash
```

### 4. Launch the robot in Gazebo

```bash
ros2 launch mobile_dd_robot gazebo_model.launch.py
```

### 5. Teleoperate the robot using keyboard

- Open a new terminal: (Keep this terminal window open along with gazebo)

```bash
ros2 run teleop_twist_keyboard teleop_twist_keyboard
```

- Open an another terminal to monitor output:

```bash
ros2 topic echo /cmd_vel
```

---

### Youtube 
https://youtu.be/EN-gyx4WqCU


