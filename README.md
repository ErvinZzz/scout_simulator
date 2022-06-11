# scout_simulator
Scout_Simulator ROS package
```

├── sensors
│   ├── realsense_simulator
│   └── robosense_simulator
├── robots
│   └── scout_ros
├── environment
│   └── warehouse_simulation_toolkit
└── README.md
```

## Tested environment

* ### Ubuntu 18.04
* ### ROS Melodic

## Install

```
mkdir src
cd src
git clone https://github.com/ErvinZzz/scout_simulator.git
cd ..
rosdep update
rosdep install -y --from-paths src --ignore-src --rosdistro $ROS_DISTRO
catkin build
```

## Usage

Launch the scout vehicle in different scene.

In city

```
roslaunch scout_gazebo_sim scout_city_simulation.launch
```

In warehouse

```
roslaunch scout_gazebo_sim scout_warehouse_simulation.launch
```

* ### For remote control with twist message

```
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```

* ### For navigation with autoware open planner
Install [Autoware.AI with Open Planner 2.5](https://github.com/hatem-darweesh/autoware.ai.openplanner)

## Reference

* [Robosense Simulator](https://github.com/tomlogan501/robosense_simulator)
* [Realsense Gazebo Plugin](https://github.com/pal-robotics/realsense_gazebo_plugin)
* [Realsense description](https://github.com/IntelRealSense/realsense-ros)
* [Scout Ros](https://github.com/agilexrobotics/scout_ros)
* [Citysim](https://github.com/osrf/citysim)
* [Warehouse Simulation Toolkit](https://github.com/wh200720041/warehouse_simulation_toolkit)
