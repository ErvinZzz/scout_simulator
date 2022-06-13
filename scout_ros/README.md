# Simulation Packages for Scout Mobile Robot

├── scout_ros
│   ├── scout_controller
│   ├── scout_description
│   └── scout_gazebo_sim
└── README.md

## scout_controller

Include a node for converting the /twist_cmd TwistStamped Message from Autoware Twist Filter node to /cmd_vel Twist Message used for controlling the mobile base.

## scout_description

Simulation of scout mobile base with realsense d435 camera and robosense rs-16 Lidar.

## scout_gazebo_sim

Scout low-level control simulation.
