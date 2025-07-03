# Robotic-ARM
Projects on Robotic arm
# Robotic Arm Pick-and-Place using ROS Simulation

**Objective**: Simulate a 6-DOF robotic arm that performs autonomous pick-and-place tasks using ROS, showcasing integration of motion planning, perception, and control in a simulated environment.

---

## Tools & Frameworks

- **ROS**: [ROS1 Noetic / ROS2 Humble]
- **Simulation**: Gazebo / CoppeliaSim / MoveIt
- **Programming**: Python, C++
- **Planner**: MoveIt! (RRTConnect / OMPL)
- **Gripper**: Vacuum gripper / 2F Parallel gripper (URDF model)

---

##  Key Features

-  Inverse Kinematics-based motion execution  
-  Object detection using simulated camera or predefined coordinates  
-  Motion planning with obstacle avoidance  
-  Pick and place logic using joint trajectory controllers  
-  Fully simulated environment with spawnable objects  

---

##  How it Works

1. **Initialization**: Launch simulation with robot, table, and multiple objects.
2. **Perception**: Either fixed coordinates or simulated RGB-D camera for object location.
3. **Planning**:
   - Use MoveIt or custom planner for computing pick/place trajectories.
   - Perform IK solution to move to pick pose.
4. **Control**:
   - Close gripper → lift object → move to drop location → release.
5. **Loop**: Repeat for multiple objects or random positions.
