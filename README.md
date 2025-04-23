# Maze Solving Robot

This project demonstrates a minimal setup for autonomous navigation of a TurtleBot3 Burger robot in a maze using **ROS2 Humble**, **Gazebo**, and the **Navigation2** stack. The `maze_solver.py` script sends the robot to two predefined goal poses within a maze, utilizing the `nav2_simple_commander` library to interface with Navigation2.

---

## 🚀 Features

- **Gazebo Simulation**  
  Renders a maze (`maze.pgm`, `maze.yaml`) and the TurtleBot3 Burger robot in Gazebo.

- **Navigation2 Integration**  
  Implements localization using AMCL and autonomous path planning using Navigation2.

- **Maze Solver Script**  
  The `maze_solver.py` script:
  - Sets the initial robot pose to `(-5.18, -6.58)`
  - Sends navigation goals to:
    - `(-1.23, -2.1)`
    - `(-7.4, -1.17)`

---

## 📦 Prerequisites

- **OS**: Ubuntu 22.04  
- **ROS2**: Humble Hawksbill

### Dependencies

Install the following ROS2 packages:

```bash
sudo apt install \
  ros-humble-turtlebot3 \
  ros-humble-turtlebot3-simulations \
  ros-humble-nav2-simple-commander \
  ros-humble-navigation2 \
  ros-humble-gazebo-ros-pkgs
