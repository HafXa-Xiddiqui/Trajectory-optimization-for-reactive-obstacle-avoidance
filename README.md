# trajectory-optimization-techniques-for-reactive-obstacle-avoidance (In collaboration with KUKA Deutschland GmBH)

This Project explores optimizing robotic trajectories in dynamic environments using Via-Point based Stochastic Trajectory Optimization (VPSTO) with a custom distribution (Hybrid model) . Simulations and real-hardware tests show that the custom distribution improves trajectory smoothness and adaptability, especially in dynamic scenarios with moving obstacles. VPSTO with the custom distribution enhances responsiveness, making it a valuable contribution to robotic motion planning.

# Improvement
The Hybrid model minimizes trajectory oscillations.
Leads to converge to a good solution (trajectory) quickly. This leads to a shorter overall path.
The approach demonstrates faster completion of tasks.
Improved time efficiency and path optimization contribute to lower overall costs.



# Experimentation:

To evaluate the proposed trajectory optimization framework, we designed two distinct test scenarios
aimed at assessing the robot’s reactive behavior. The experiments were conducted in both static and
dynamic environments, with a focus on trajectory smoothness, collision avoidance, and computational
efficiency

  Static test:
    This experiment evaluates the robot’s ability to navigate in an environment with fixed obstacles. The
robot is required to generate collision-free trajectories to reach a goal pose from a randomly generated
starting pose. To ensure robust testing, the experiment was conducted on 100 different scenarios.
Below shows the result from one of the test scenerio:

![image](https://github.com/user-attachments/assets/d6239936-2141-4314-bacb-96404705cbd2)


  Dynamic Test:
     The experiment consisted of 10 runs with randomly generated start and goal poses.
  Below shows one of the test scene
  
![image](https://github.com/user-attachments/assets/f84a055d-57f7-474b-9ec7-f94880565375)


# Hardware Experimentation:
Hardware experiments were conducted to validate the algorithms in real-world scenarios, involving static and dynamic obstacle tests. The setup included a table, a wall, and a movable cube as obstacles, simulating realistic challenges. These tests assessed the robot's ability to navigate safely and efficiently in constrained environments.

![image](https://github.com/user-attachments/assets/5db57306-de8d-41d8-80a6-ee1699f5b333)

  Mean Jerk and Time comparison:
  With the new Approach the Robot reaches the goal in sortest possible time and with minimum jerk values.
  ![image](https://github.com/user-attachments/assets/09480e54-4037-4f96-b32c-a775990f5023)

  Joint Position Velocity and Acceleration Profile:
  Profile shows that overall jerks are reduced, when KUKA iiwa is powered by the new approach.
  ![image](https://github.com/user-attachments/assets/2cc8fc92-ce5d-46aa-9ea8-75b9e8cf41d8)


  








