# summit_xls_ur5_common
Common package for the Summit XL Steel + UR5 arm for ROS Melodic.

## Depends
Clone the following into catkin workspace
- [robotnik msg][rbnk-msg]
- [robotnik sensors][rbnk-sns]
- [summit XL Common][rbnk-xl-c]

and then build them using `catkin`.




To test your installation, run 
```bash
roslaunch summit_xls_ur5_description summit_xls_ur5_omni_rviz.launch 
```




[rbnk-msg]: https://github.com/RobotnikAutomation/robotnik_msgs/tree/melodic-devel
[rbnk-sns]: https://github.com/RobotnikAutomation/robotnik_sensors
[rbnk-xl-c]: https://github.com/RobotnikAutomation/summit_xl_common