---
layout: page
title: Publications
permalink: /publications/
---
<div class="ui raised segment">

**Inverse Kinematics for Serial Kinematic Chains via Sum of Squares Optimization**

<a class="tiny ui green button" href="https://arxiv.org/abs/1909.09318"><i class="file alternate outline icon"></i>arXiv</a>
<a class="tiny ui black button" href="https://github.com/utiasSTARS/sos-ik"><i class="github icon"></i>Github</a>

<details>
<summary>Abstract</summary>

Inverse kinematics is a fundamental challenge for articulated robots: fast and accurate algorithms are needed for translating task-related workspace constraints and goals into feasible joint configurations. In general, inverse kinematics for serial kinematic chains is a difficult nonlinear problem, for which closed form solutions cannot easily be obtained. Therefore, computationally efficient numerical methods that can be adapted to a general class of manipulators are of great importance. In this paper, we use convex optimization techniques to solve the inverse kinematics problem with joint limit constraints for highly redundant serial kinematic chains with spherical joints in two and three dimensions. This is accomplished through a novel formulation of inverse kinematics as a nearest point problem, and with a fast sum of squares solver that exploits the sparsity of kinematic constraints for serial manipulators. Our method has the advantages of post-hoc certification of global optimality and a runtime that scales polynomially with the number of degrees of freedom. Additionally, we prove that our convex relaxation leads to a globally optimal solution when certain conditions are met, and demonstrate empirically that these conditions are common and represent many practical instances. Finally, we provide an open source implementation of our algorithm.

</details>
<details>
<summary>Citation (BibTeX)</summary>
<p>

```
@inproceedings{2020_Maric_Inverse,
  address = {Paris, France},
  author = {Filip Maric and Matthew Giamou and Soroush Khoubyarian and Ivan Petrovic and Jonathan Kelly},
  booktitle = {Proceedings of the {IEEE} International Conference on Robotics and Automation {(ICRA'20})},
  date = {2020-05-31/2020-06-04},
  month = {May 31--Jun. 4},
  title = {Inverse Kinematics for Serial Kinematic Chains via Sum of Squares Optimization},
  url = {http://arxiv.org/abs/1909.09318},
  video1 = {https://www.youtube.com/watch?v=AdPze8cTUuE},
  year = {2020}
}
```

</p>
</details>
</div>

<div class="ui raised segment">

**Manipulability Maximization Using Continuous-Time Gaussian Processes**

<a class="tiny ui green button" href="https://arxiv.org/abs/1908.02963"><i class="file alternate outline icon"></i>arXiv</a>
<details>
<summary>Abstract</summary>

 A significant challenge in manipulation motion planning is to ensure agility in the face of unpredictable changes during task execution. This requires the identification and possible modification of suitable joint-space trajectories, since the joint velocities required to achieve a specific endeffector motion vary with manipulator configuration. For a given manipulator configuration, the joint space-to-task space velocity mapping is characterized by a quantity known as the manipulability index. In contrast to previous control-based approaches, we examine the maximization of manipulability during planning as a way of achieving adaptable and safe joint space-to-task space motion mappings in various scenarios. By representing the manipulator trajectory as a continuous-time Gaussian process (GP), we are able to leverage recent advances in trajectory optimization to maximize the manipulability index during trajectory generation. Moreover, the sparsity of our chosen representation reduces the typically large computational cost associated with maximizing manipulability when additional constraints exist. Results from simulation studies and experiments with a real manipulator demonstrate increases in manipulability, while maintaining smooth trajectories with more dexterous (and therefore more agile) arm configurations. 

</details>
<details>
<summary>Citation (BibTeX)</summary>
<p>

```
@inproceedings{2018_Maric_Manipulabiility,
  abstract = {A significant challenge in motion planning is to avoid being in or near singular configurations (singularities), that is, joint configurations that result in the loss of the ability to move in certain directions in task space. A robotic system's capacity for motion is reduced even in regions that are in close proximity to (i.e., neighbouring) a singularity. In this work we examine singularity avoidance in a motion planning context, finding trajectories which minimize proximity to singular regions, subject to constraints. We define a manipulability-based likelihood associated with singularity avoidance over a continuous trajectory representation, which we then maximize using a maximum a posteriori (MAP) estimator. Viewing the MAP problem as inference on a factor graph, we use gradient information from interpolated states to maximize the trajectory's overall manipulability. Both qualitative and quantitative analyses of experimental data show increases in manipulability that result in smooth trajectories with visibly more dexterous arm configurations.},
  address = {Madrid, Spain},
  author = {Filip Maric and Oliver Limoyo and Luka Petrovic and Ivan Petrovic and Jonathan Kelly},
  booktitle = {Proceedings of the IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS'18) Workshop Towards Robots that Exhibit Manipulation Intelligence},
  date = {2018-10-01},
  month = {Oct. 1},
  title = {Manipulability Maximization Using Continuous-Time Gaussian Processes},
  url = {https://arxiv.org/abs/1803.09493},
  year = {2018}
```

</p>
</details>
</div>
</br>
