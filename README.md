# Simbha Robot - A differential Drive two wheeled robot 
## Installation Procedure to install Simbha Robot in ROS2-FOXY.


Gazebo Installation in ROS2-Foxy:

``` 
sudo apt install ros-foxy-gazebo-ros-pkgs
```

Cloning the package:

```
cd ~/{workspace-dir}/src
```

``` 
git clone git@github.com:anugrah1112/simbha_robot.git -b ros2-foxy
```

Building the package using colcon build

```
cd ~/{workspace-dir}
```

```
colcon build --symlink-install --packages-select simbha_structure
```

```
source ~/{workspace-dir}/install/setup.bash
```
Running the code for bug algorithm 

```
ros2 launch simbha_structure gazebo.launch.py
```

```
ros2 run simbha_structure bug_algorithms.py
```
