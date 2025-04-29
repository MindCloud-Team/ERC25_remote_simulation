# ERC25_remote_simulation
## Mind Cloud Adaptation for GZ Sim Harmonic and ERC25 Remote Extension

This repository provides a customized and simplified Mars Yard environment adapted for use with **Gazebo Sim Harmonic** and **ROS 2 Jazzy**. It is based on the original model provided [here](https://drive.google.com/drive/folders/1kvJ4vRcukgJdDpJXkft8xSptM3QwUmzl), which we cleaned and reduced from **over 3 million** faces to approximately **300,000** to improve performance. *(Note: We are not 3D modeling experts, but this is the best optimization we could achieve.)*

### Key Contributions

- ✅ Created a usable version of the Mars Yard simulation model  
- ✅ Added a **ZED X camera** to the rover model *(camera positions may not be accurate)*  
- ✅ Included **landmarks** for use in localization and navigation tasks  

---

### Installation & Setup

1. **First**, follow the instructions and install the base package from:  
   👉 https://github.com/husarion/husarion_ugv_ros

2. **Then**, download the customized Mars Yard simulation files from:  
   👉 https://drive.google.com/drive/folders/146GUOfDKCR5hZu9cTbaz5I9Dk50ku7-T?usp=drive_link

3. Move the downloaded folder to your `src` directory inside your ROS 2 workspace and merge it with the existing packages.

---

### How to Launch the Simulation

```bash
ros2 launch husarion_ugv_gazebo simulation.launch.py gz_world:=`ros2 pkg prefix husarion_gz_worlds`/share/husarion_gz_worlds/worlds/mars_yard.sdf
```

---
