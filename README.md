# summit_xls_ur5_common
Common package for the Summit XL Steel + UR5 arm for ROS Melodic.

## Depends
Clone the following into catkin workspace and switch to the melodic branches in al
- [robotnik msg][rbnk-msg]
- [robotnik sensors][rbnk-sns]
- [summit XL Common][rbnk-xl-c]
- [ur description][ur-desc]

Find any other missing ROS dependencies using `rosdep`
```bash
rosdep install --from-paths src --ignore-src --rosdistro melodic -y
```


And then build them using `catkin`.



### Test RVIZ
To test your installation, run 
```bash
roslaunch summit_xls_ur5_description summit_xls_ur5_omni_rviz.launch 
```


### Test Gazebo RVIZ
```bash
roslaunch summit_xls_ur5_sim summit_xls_ur5_gazebo.launch
```
Launch RVIZ separately
```bash
roslaunch summit_xls_ur5_moveit_config_new moveit_rviz.launch
```
Then run this to control the arm
```bash
ROS_NAMESPACE=summit_xls rosrun rqt_joint_trajectory_controller rqt_joint_trajectory_controller
```


[rbnk-msg]: https://github.com/RobotnikAutomation/robotnik_msgs/tree/melodic-devel
[rbnk-sns]: https://github.com/RobotnikAutomation/robotnik_sensors
[rbnk-xl-c]: https://github.com/RobotnikAutomation/summit_xl_common
[ur-desc]: http://wiki.ros.org/ur_description