## Robot Package Template

This is a GitHub template. You can make your own copy by clicking the green "Use this template" button.

It is recommended that you keep the repo/package name the same, but if you do change it, ensure you do a "Find all" using your IDE (or the built-in GitHub IDE by hitting the `.` key) and rename all instances of `ros_bot` to whatever your project's name is.

Note that each directory currently has at least one file in it to ensure that git tracks the files (and, consequently, that a fresh clone has direcctories present for CMake to find). These example files can be removed if required (and the directories can be removed if `CMakeLists.txt` is adjusted accordingly).


## HOW TO

Terminal1
source /ros_entrypoint.sh
cd ros2_ws
source install/setup.bash
colcon --smylink-install
ros2 launch ros_bot rsp.lanch.py

Terminal2
rviz2 -d ROS_BOT/config/robot.rviz

Terminal3
ros2 run joint_state_publisher_gui joint_state_publisher_gui