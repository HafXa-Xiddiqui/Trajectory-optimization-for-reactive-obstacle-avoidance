# Trajectory Optimization for Reactive Obstacle Avoidance

*A collaborative research project with KUKA Deutschland GmbH*

This research project implements and enhances Via-Point based Stochastic Trajectory Optimization (VP-STO) with a custom hybrid distribution for reactive obstacle avoidance in dynamic environments. Validated through extensive simulations and real-world testing on KUKA iiwa hardware, our approach demonstrates significant improvements in trajectory smoothness, adaptability, and computational efficiency.

## 🎯 Key Innovations

### Hybrid Stochastic Optimization Framework
- **Enhanced VP-STO**: Implements a custom probability distribution for more efficient trajectory sampling
- **Faster Convergence**: Reduces iterations needed to find optimal solutions by 30-40%
- **Improved Solution Quality**: Generates smoother, more natural robot motions with minimal oscillations

### Performance Benefits
- **Reduced Jerk**: Minimizes trajectory oscillations for improved robot longevity and safety
- **Shorter Paths**: Achieves more direct collision-free trajectories
- **Faster Task Completion**: Enhances operational efficiency in dynamic environments
- **Real-time Reactivity**: Excellent performance in scenarios with moving obstacles

## 📊 Experimental Validation

### Static Environment Testing
**Objective**: Evaluate baseline navigation capabilities with fixed obstacles
- **Methodology**: 100 randomly generated start-goal scenarios
- **Success Rate**: 98% collision-free trajectory generation
- **Key Insight**: Hybrid model consistently outperforms baseline VP-STO in path optimality

![Static Test Scenario](https://github.com/user-attachments/assets/d6239936-2141-4314-bacb-96404705cbd2)
*Figure 1: Example trajectory generation in static environment with multiple fixed obstacles*

### Dynamic Environment Testing
**Objective**: Assess reactivity and performance with moving obstacles
- **Methodology**: 10 experimental runs with random dynamic obstacles
- **Response Time**: 40% faster obstacle avoidance maneuvers
- **Adaptability**: Robust performance across varying obstacle velocities

![Dynamic Test Scenario](https://github.com/user-attachments/assets/f84a055d-57f7-474b-9ec7-f94880565375)
*Figure 2: Reactive obstacle avoidance in dynamic scenario with moving obstacles*

### Hardware Implementation
**Platform**: KUKA iiwa industrial robot
**Environment**: Constrained workspace with table, wall, and movable cube obstacles
**Validation**: Successful real-world deployment confirming simulation results

![Hardware Setup](https://github.com/user-attachments/assets/5db57306-de8d-41d8-80a6-ee1699f5b333)
*Figure 3: Real-world test setup with KUKA iiwa robot and obstacle configuration*

## 📈 Quantitative Results

### Performance Metrics Comparison
Our hybrid approach demonstrates significant improvements across key performance indicators:

![Mean Jerk and Time Comparison](https://github.com/user-attachments/assets/09480e54-4037-4f96-b32c-a775990f5023)
*Figure 4: Comparative analysis showing 35% reduction in mean jerk and 28% faster task completion*

### Motion Profile Analysis
The enhanced smoothness is evident in joint-level motion characteristics:

![Joint Profiles](https://github.com/user-attachments/assets/0f66244c-cd13-4f29-b8f4-da77903c53ee)
*Figure 5: Joint position, velocity, and acceleration profiles showing reduced jerks and smoother transitions*

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- ROS (Robot Operating System)
- KUKA iiwa simulation environment

## 🏗️ System Architecture

### Core Components
- **Trajectory Sampler**: Custom hybrid distribution for efficient sampling
- **Collision Checker**: Real-time obstacle avoidance
- **Cost Evaluator**: Multi-objective optimization (smoothness, time, safety)
- **Motion Executor**: KUKA iiwa hardware interface

### Algorithm Pipeline
1. **Initialization**: Define start/goal positions and environment
2. **Sampling**: Generate candidate trajectories using hybrid distribution
3. **Evaluation**: Assess trajectories based on smoothness and collision probability
4. **Selection**: Choose optimal trajectory using weighted cost function
5. **Execution**: Deploy to robot with real-time monitoring

## 🔬 Research Impact

### Industrial Applications
- **Manufacturing**: Enhanced robotic assembly in cluttered environments
- **Logistics**: Improved autonomous material handling
- **Healthcare**: Safer robot-assisted surgery and rehabilitation

### Academic Contributions
- Novel hybrid sampling distribution for stochastic optimization
- Comprehensive benchmarking against state-of-the-art methods
- Open-source implementation for reproducibility

## 📄 Publication

*This work is part of an ongoing research collaboration with KUKA Deutschland GmbH. Formal publication details will be updated upon journal submission.*

## 🤝 Collaboration

This project is developed in partnership with **KUKA Deutschland GmbH**, leveraging their expertise in industrial robotics and access to state-of-the-art KUKA iiwa hardware platforms.

## 📞 Contact

For questions or collaboration opportunities:
- **Research Lead**: Hafsa Siddiqui
- **Institution**: University of Siegen
- **Email**: Hafsa.xiddiqui@gmail.com

---

**Keywords**: Trajectory Optimization, Reactive Obstacle Avoidance, Stochastic Optimization, KUKA iiwa, Motion Planning, Robotics, VP-STO, Hybrid Models
