# Movo Simulation Scene

Kinova Movo scene for [CoppeliaSim](https://www.coppeliarobotics.com/). Uses Movo with 2 
7DOF Kinova Jaco arms and 2 Robotiq grippers.

### Setup & Run
1. Install [CoppeliaSim](https://www.coppeliarobotics.com/downloads)
2. Place `libsimExtROSInterface.so` in CoppeliaSim folder, replacing the original
3. Run `roscore`
4. Run CoppeliaSim
5. Click `File > Open Scene...` and select `movoScene.ttt`

### Simulated ROS Topics

#### Published
* `/movo/right_arm/joint_states`
* `/movo/left_arm/joint_states`
* `/movo_camera/vision`
* `/movo_camera/depth`

#### Subscribed
* `/movo/right_arm/angular_vel_cmd`
* `/movo/left_arm/angular_vel_cmd`
* `/movo/linear_actuator_cmd`
* `/movo/left_gripper/cmd`
* `/movo/head/cmd`
