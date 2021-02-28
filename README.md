# Sawyer-IRL

This repo is for inverse reinforcement learning algortihm demonstration on the actual Rethink Sawyer robot using MoveIt.

## Packages

```
rethink packages
sawyer_moveit
```

## Instruction

1. Connect with Sawyer through Ethernet
2. Ping 10.42.0.2 or ```sawyer.local``` to confirm connection
3. Set environment variables
  ```
  export ROS_MASTER_URI=http://10.42.0.2:11311
  export ROS_IP=10.42.0.1
  unset ROS_HOSTNAME
  ```
4. source rethink workspace
5. Enable the robot ```rosrun intera_interface enable_robot.py -e```
6. Run the joint_server ```rosrun intera_interface joint_trajectory_action_server.py```
7. ```roslaunch sawyer_irl sawyer_irl.launch```
