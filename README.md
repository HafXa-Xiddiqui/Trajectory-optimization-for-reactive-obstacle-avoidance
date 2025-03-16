# trajectory-optimization-techniques-for-reactive-obstacle-avoidance (In collaboration with KUKA Deutschland GmBH)

This Project explores optimizing robotic trajectories in dynamic environments using Via-Point based Stochastic Trajectory Optimization (VPSTO) with a custom distribution. Simulations and real-hardware tests show that the custom distribution improves trajectory smoothness and adaptability, especially in dynamic scenarios with moving obstacles. VPSTO with the custom distribution enhances responsiveness, making it a valuable contribution to robotic motion planning.


# Overall Architecture:
![image](https://github.com/user-attachments/assets/37203b54-6cc8-459b-8020-5eff8529dc30)

![image](https://github.com/user-attachments/assets/9ed18590-716f-43a6-b31a-a4a629e481f2)

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
![image](https://github.com/user-attachments/assets/c13767cd-53bb-4a24-8627-8b9a4b4b57a3)

  Dynamic Test:
     The experiment consisted of 10 runs with randomly generated start and goal poses.
  Below shows one of the test scene
  ![image](https://github.com/user-attachments/assets/c070aa45-9cef-4353-af9c-bf318f029e25)

  






