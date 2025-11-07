# Handycar

This project was developed for the **Workshop on Robotics and Intelligent Systems**, hosted by the **RIoT Research Centre (Independent University, Bangladesh)** and **TEXON**. And this project got 2nd position.

**Project Visualization:** [*Link*](https://youtu.be/77_cAe_exHk)


## About the Project

This project is a **URDF (Unified Robot Description Format)** file, which is a standard ROS (Robot Operating System) file for describing a robot's physical structure.

The "handycar" is a simple **mobile manipulator** model featuring:
* **A Mobile Base:** A chassis with three wheels.
* **A Manipulator Arm:** A 2-Degree-of-Freedom (DOF) arm mounted on the base.

## Technologies Used

* **URDF (Unified Robot Description Format):** To define the robot's physical structure, links, and joints.
* **XML:** The markup language used to write the `.urdf` file.
* **ROS 2 (Humble):** The core robotics framework used for visualization and simulation.
* **Rviz2:** The primary 3D visualization tool in ROS 2, used to view and test the model.
* **Linux (Ubuntu):** The operating system used for ROS 2 development.

## How to Run (ROS 2 Visualization)

You can visualize this robot model using ROS 2 and Rviz2.

### 1. Prerequisites

You must have ROS 2 installed (e.g., Humble, Foxy, Jazzy). You also need the necessary visualization packages.

If you don't have them, install them by replacing `<distro>` with your ROS 2 version:

```bash
# Install the core desktop and visualization tools
sudo apt install ros-humble-desktop-full

# Install the tutorial package that provides the easy launch file
sudo apt install ros-humble-urdf-tutorial
```

```bash
source /opt/ros/humble/setup.bash
```

```bash
ros2 launch urdf_tutorial display.launch.py model:=[path of the file]/handycar.urdf
```