# Hardware Documentation

<div align="center">
  <img src="https://img.shields.io/badge/Status-In%20Development-yellow" alt="Status: In Development">
  <img src="https://img.shields.io/badge/Team-Robotics%20Club-blue" alt="Team: Robotics Club">
  <img src="https://img.shields.io/badge/Dimensions-60×100mm-green" alt="Dimensions: 60×100mm">
</div>

## 🔧 Hardware Specifications

- **Dimensions**: !TODO()
- **Drive System**: Differential drive 
- **Sensors**:
  - RP-LiDAR A1M8 Sensor
  - UART adapter board: STC-A0317-R03
  - BNO055 Orientation Sensor
- **Power**: 3.7V LiPo battery

## How to setup Lidar:
- mkdir -p ~/ros2_ws/src
- cd ~/ros2_ws/src
- git clone -b ros2 https://github.com/Slamtec/rplidar_ros.git
- cd ~/ros2_ws/
- source /opt/ros/humble/setup.bash
- colcon build --symlink-install
- source ./install/setup.bash
- cd ros2_ws
- sudo chmod 666 /dev/ttyUSB0
- ros2 launch rplidar_ros view_rplidar_s2e_launch.py

### Adding New CAD Files

When adding new design files, please follow these guidelines:
1. Create a new subdirectory if your design represents a major component
2. Use descriptive filenames with version numbers (e.g., `chassis_v2.ipt`)
3. Include a brief README in each directory describing the components
4. For 3D printable files, include recommended print settings

## 🔌 Electronics Design
!TODO()

### Base Configuration
- **Microcontroller**: Arduino Mega
- **Motor Driver**: JYQD-V7.3E2 brushless DC motor driver board
- **Sensor Interface**: !TODO()


## 📋 Bill of Materials
!TODO()
[Link to detailed BOM spreadsheet]

---

<div align="center">
  <i>For software documentation, please see the <a href="../CodeBase/README.md">Software README</a></i>
</div>
