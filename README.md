# 🤖 mobile_arm_robot

A ROS 2 simulation project that brings together a **robotic arm** and a **mobile base** in Gazebo, fully integrated with URDF, TF2, RViz, and ROS 2 launch workflows. Designed for learning robot modeling, simulation, and system integration in a clean, modular way.

---

## 🚀 Features

- 🦾 Modular **robotic arm** designed using URDF + Xacro
- 📡 Real-time **TF2 transforms** for all joints and links
- 🖥️ Full **RViz2** visualization (joints, frames, model)
- 🌍 **Gazebo** simulation support with physics
- 🔄 ROS-Gazebo communication via **`ros_gz_bridge`**
- 🧠 Custom **launch files** to start the system easily

---

## 🛠️ Requirements

- ✅ ROS 2 (tested on **Jazzy** )
- 🛠️ Gazebo Fortress or newer
- 🐍 Python 3
- 🔗 `ros_gz_bridge` (ROS-Gazebo bridge)
- 📦 `xacro`, `robot_state_publisher`, `joint_state_broadcaster`

---

## 📁 Project Structure (with descriptions)

```bash
$ tree mobile_arm_robot

mobile_arm_robot
├── my_robot_description      # URDF and Xacro robot model files
├── my_robot_bringup          # ROS 2 launch files and Gazebo bridge setup
├── config                    # YAML config files for RViz and bridge topics
└── README.md                 # Project documentation
```


---

## ▶️ How to Launch

1. **Source ROS 2 environment**
   ```bash
   source /opt/ros/jazzy/setup.bash
   ```

2. **Clone and build the workspace**
   ```bash
   git clone https://github.com/Sohrab999/mobile_arm_robot.git src/mobile_arm_robot
   cd ..
   colcon build
   source install/setup.bash
   ```

3. **Launch the robot with Gazebo bridge**
   ```bash
   ros2 launch my_robot_bringup display.launch.xml
   ```


## 📸 Preview

This project visualizes a robotic arm in RViz using a URDF model with color and joint configurations. The robot's transforms are correctly published via TF, and you can also bridge topics between Gazebo and ROS 2 to simulate real-time motion and state feedback.

You can run the RViz visualization using the launch file provided in `my_robot_bringup`.


## 📚 What I Learned

- 🧱 Building robots with URDF & Xacro  
- 🔗 Broadcasting and listening to TF2 frames  
- 🌉 Bridging data between Gazebo & ROS 2  
- 🛠️ Creating modular launch files with `launch.py`  
- 🧪 Debugging topics, transforms, and simulation behaviors  

---

## 🧠 Future Plans

- 🔧 Add real mobile base plugin (differential drive)  
- 📷 Mount sensors like camera/LiDAR  
- 📡 Integrate Bluetooth control for hardware version  
- 🎯 Add MoveIt2 integration for motion planning  
- 🛤️ Implement navigation and obstacle avoidance  

---

## 👨‍💻 Author

**Sohrab Vimadalal**  
Robotics | ROS 2 | Simulation <br>
📫 [GitHub Profile](https://github.com/Sohrab999)





