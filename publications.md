---
layout: page
title: Publications
permalink: /publications/
---
This list contains selected publications and various additional materials (code, media, pdfs).
For a more detailed listing please check out my profile on [google scholar](https://scholar.google.com/citations?hl=en&user=o_cwgrkAAAAJ). 
### 2020

<div class="ui raised segment">

#### Riemannian Optimization for Distance Geometric Inverse Kinematics  
F. Marić, M. Giamou, A. Hall, S. Khoubyarian, I. Petrović, and J. Kelly\
**[ submitted ]** IEEE Transactions on Robotics 
<details>
<summary>Abstract</summary>
<div class="ui secondary segment">
Solving the inverse kinematics problem is a fundamental challenge in motion planning, control, and calibration for articulated robots. Kinematic models for these robots are typically param- eterized by joint angles, generating a complicated trigonometric mapping between a robot's configuration and end-effector pose. Alternatively, the kinematic model and task constraints can be represented using invariant distances between points attached to the robot. In this paper, we prove the equivalence of distance-based inverse kinematics formulations and the distance geometry problem for a large class of robots comprised of revolute joints. Unlike previous approaches, we use the connection between distance geometry and low-rank matrix completion to find inverse kinematics solutions by completing a partial Euclidean distance matrix using local optimization. Further, we parameterize the space of Euclidean distance matrices with the Riemannian manifold of fixed-rank Gram matrices, allowing us to leverage a variety of mature Riemannian optimization methods. Finally, we show that bound smoothing can be used to generate informed initializations without significant computational overhead, improving convergence. We demonstrate that our novel inverse kinematics solver achieves higher success rates compared to traditional approaches, and significantly outperforms them in many cases where multiple end-effectors are present.
</div>
</details>

<details>
<summary>Citation (BibTeX)</summary>
<p>

```
@article{2020_Marić_Riemannian,
  abstract = {Solving the inverse kinematics problem is a fundamental challenge in motion planning, control, and calibration for articulated robots. Kinematic models for these robots are typically param- eterized by joint angles, generating a complicated trigonometric mapping between a robot's configuration and end-effector pose. Alternatively, the kinematic model and task constraints can be represented using invariant distances between points attached to the robot. In this paper, we prove the equivalence of distance-based inverse kinematics formulations and the distance geometry problem for a large class of robots comprised of revolute joints. Unlike previous approaches, we use the connection between distance geometry and low-rank matrix completion to find inverse kinematics solutions by completing a partial Euclidean distance matrix using local optimization. Further, we parameterize the space of Euclidean distance matrices with the Riemannian manifold of fixed-rank Gram matrices, allowing us to leverage a variety of mature Riemannian optimization methods. Finally, we show that bound smoothing can be used to generate informed initializations without significant computational overhead, improving convergence. We demonstrate that our novel inverse kinematics solver achieves higher success rates compared to traditional approaches, and significantly outperforms them in many cases where multiple end-effectors are present.},
  author = {Filip Marić and Matthew Giamou and Adam Hall and Soroush Khoubyarian and Ivan Petrović and Jonathan Kelly},
  journal = {IEEE Transactions on Robotics},
  note = {Submitted},
  title = {Riemannian Optimization for Distance Geometric Inverse Kinematics},
  year = {2020}
}
```

</p>
</details>
</div>

<div class="ui raised segment">

#### Geometry-Aware Singularity Avoidance for Articulated Robots Using a Riemannian Metric 
F. Marić, L. Petrović, M. Guberina, J. Kelly, and I. Petrović\
Robotics and Autonomous Systems 
<details>
<summary>Abstract</summary>
<div class="ui secondary segment">
Articulated robots such as manipulators are increasingly being used for tasks that involve interaction (with humans, for example), where a capacity to adapt to unexpected changes in operational space constraints is essential. 
In certain configurations, known as singularities, a manipulator loses one or more degrees of freedom (DoF) and is unable to move in certain operational space directions.
The inability to move in arbitrary directions in operational space compromises adaptivity and, potentially, safety. 
In this paper, we introduce a geometry-aware singularity index that uses a Riemannian metric to provide a measure of proximity to singular configurations and that avoids some failure modes of other common indices. 
We show that this index can be elegantly differentiated using a connection with Frećhet derivatives, making it compatible with popular local optimization approaches used for operational space control. 
Our experimental results show that a singularity avoidance method based on our index outperforms a
common manipulability maximizing method in reaching and path following tasks optimized for singularity-robust and safe motion.
</div>
</details>

<details>
<summary>Citation (BibTeX)</summary>
<p>

```
@article{2020_Marić_Geometry-Aware,
  author = {Filip Marić and Luka Petrović and Marko Guberina and Jonathan Kelly and Ivan Petrović},
  journal = {Robotics and Autonomous Systems},
  note = {Submitted},
  title = {Geometry-Aware Singularity Avoidance for Articulated Robots Using a Riemannian Metric},
  year = {2020}
}
```

</p>
</details>
</div>


<div class="ui raised segment">

#### Inverse Kinematics as Low-Rank Euclidean Distance Matrix Completion
F. Marić, M. Giamou, S. Khoubyarian, I. Petrović, J. Kelly\
<a class="ui red left horizontal label">Best Paper</a>
IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS’20) Workshop on Bringing Geometric Methods to Robot Learning, Optimization and Control, Las Vegas, Nevada, USA 
<details>
<summary>Abstract</summary>
<div class="ui secondary segment">
The majority of inverse kinematics (IK) algorithms search for solutions in a configuration space defined by joint angles. However, the kinematics of many robots can also be described in terms of distances between rigidly-attached points, which collectively form a Euclidean distance matrix. This alternative geometric description of the kinematics reveals an elegant equivalence between IK and the problem of low-rank matrix completion. We use this connection to implement a novel Riemannian optimization-based solution to IK for various articulated robots with symmetric joint angle constraints.nverse kinematics is a fundamental challenge for articulated robots: fast and accurate algorithms are needed for translating task-related workspace constraints and goals into feasible joint configurations. In general, inverse kinematics for serial kinematic chains is a difficult nonlinear problem, for which closed form solutions cannot easily be obtained. Therefore, computationally efficient numerical methods that can be adapted to a general class of manipulators are of great importance. In this paper, we use convex optimization techniques to solve the inverse kinematics problem with joint limit constraints for highly redundant serial kinematic chains with spherical joints in two and three dimensions. This is accomplished through a novel formulation of inverse kinematics as a nearest point problem, and with a fast sum of squares solver that exploits the sparsity of kinematic constraints for serial manipulators. Our method has the advantages of post-hoc certification of global optimality and a runtime that scales polynomially with the number of degrees of freedom. Additionally, we prove that our convex relaxation leads to a globally optimal solution when certain conditions are met, and demonstrate empirically that these conditions are common and represent many practical instances. Finally, we provide an open source implementation of our algorithm.
</div>
</details>

<details>
<summary>Citation (BibTeX)</summary>
<p>

```
@inproceedings{2020_Marić_Inverse_B,
  abstract = {The majority of inverse kinematics (IK) algorithms search for solutions in a configuration space defined by joint angles. However, the kinematics of many robots can also be described in terms of distances between rigidly-attached points, which collectively form a Euclidean distance matrix. This alternative geometric description of the kinematics reveals an elegant equivalence between IK and the problem of low-rank matrix completion. We use this connection to implement a novel Riemannian optimization-based solution to IK for various articulated robots with symmetric joint angle constraints.},
  address = {Las Vegas, Nevada, USA},
  author = {Filip Marić and Matthew Giamou and Ivan Petrović and Jonathan Kelly},
  booktitle = {Proceedings of the {IEEE/RSJ} International Conference on Intelligent Robots and Systems {(IROS'20)} Workshop on Bringing Geometric Methods to Robot Learning, Optimization and Control},
  date = {2020-10-29},
  month = {Oct. 29},
  note = {Bosch Center for Artificial Intelligence Best Workshop Contribution Award},
  title = {Inverse Kinematics as Low-Rank Euclidean Distance Matrix Completion},
  year = {2020}
}
```

</p>
</details>

[<span style="color:red">**[ video ]**</span>](https://youtu.be/wO0_w2Gw5jk)
<!-- <a class="tiny ui red button" href="https://youtu.be/wO0_w2Gw5jk"><i class="youtube icon"></i>Video</a> -->
</div>

<div class="ui raised segment">

#### Inverse Kinematics for Serial Kinematic Chains via Sum of Squares Optimization
F. Marić, M. Giamou, S. Khoubyarian, I. Petrović, J. Kelly\
IEEE International Conference on Robotics and Automation (ICRA’20), Paris, France
<details>
<summary>Abstract</summary>
<div class="ui secondary segment">
Inverse kinematics is a fundamental challenge for articulated robots: fast and accurate algorithms are needed for translating task-related workspace constraints and goals into feasible joint configurations. In general, inverse kinematics for serial kinematic chains is a difficult nonlinear problem, for which closed form solutions cannot easily be obtained. Therefore, computationally efficient numerical methods that can be adapted to a general class of manipulators are of great importance. In this paper, we use convex optimization techniques to solve the inverse kinematics problem with joint limit constraints for highly redundant serial kinematic chains with spherical joints in two and three dimensions. This is accomplished through a novel formulation of inverse kinematics as a nearest point problem, and with a fast sum of squares solver that exploits the sparsity of kinematic constraints for serial manipulators. Our method has the advantages of post-hoc certification of global optimality and a runtime that scales polynomially with the number of degrees of freedom. Additionally, we prove that our convex relaxation leads to a globally optimal solution when certain conditions are met, and demonstrate empirically that these conditions are common and represent many practical instances. Finally, we provide an open source implementation of our algorithm.
</div>
</details>

<details>
<summary>Citation (BibTeX)</summary>
<p>

```
@inproceedings{2020_Marić_Inverse,
  address = {Paris, France},
  author = {Filip Marić and Matthew Giamou and Soroush Khoubyarian and Ivan Petrović and Jonathan Kelly},
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

[<span style="color:green">**[ preprint ]**</span>](https://arxiv.org/abs/1909.09318) 
[<span style="color:black">**[ code ]**</span>](https://github.com/utiasSTARS/sos-ik) 
[<span style="color:red">**[ video ]**</span>](https://www.youtube.com/watch?v=AdPze8cTUuE)
<!-- <a class="tiny ui green button" href="https://arxiv.org/abs/1909.09318"><i class="file alternate outline icon"></i>Preprint</a> -->
<!-- <a class="tiny ui black button" href="https://github.com/utiasSTARS/sos-ik"><i class="github icon"></i>Code</a> -->
<!-- <a class="tiny ui red button" href="https://www.youtube.com/watch?v=AdPze8cTUuE"><i class="youtube icon"></i>Video</a> -->
</div>

### 2019
<div class="ui raised segment">

#### Manipulability Maximization Using Continuous-Time Gaussian Processes
F. Marić and O. Limoyo and L. Petrović and I. Petrović and J. Kelly\
IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS’19), Macau, China
<details>
<summary>Abstract</summary>
<div class="ui secondary segment">
 A significant challenge in manipulation motion planning is to ensure agility in the face of unpredictable changes during task execution. This requires the identification and possible modification of suitable joint-space trajectories, since the joint velocities required to achieve a specific end-effector motion vary with manipulator configuration. For a given manipulator configuration, the joint space-to-task space velocity mapping is characterized by a quantity known as the manipulability index. In contrast to previous control-based approaches, we examine the maximization of manipulability during planning as a way of achieving adaptable and safe joint space-to-task space motion mappings in various scenarios. By representing the manipulator trajectory as a continuous-time Gaussian process (GP), we are able to leverage recent advances in trajectory optimization to maximize the manipulability index during trajectory generation. Moreover, the sparsity of our chosen representation reduces the typically large computational cost associated with maximizing manipulability when additional constraints exist. Results from simulation studies and experiments with a real manipulator demonstrate increases in manipulability, while maintaining smooth trajectories with more dexterous (and therefore more agile) arm configurations. 
</div>
</details>
<details>
<summary>Citation (BibTeX)</summary>
<p>

```
@inproceedings{2018_Marić_Manipulabiility,
  abstract = {A significant challenge in motion planning is to avoid being in or near singular configurations (singularities), that is, joint configurations that result in the loss of the ability to move in certain directions in task space. A robotic system's capacity for motion is reduced even in regions that are in close proximity to (i.e., neighbouring) a singularity. In this work we examine singularity avoidance in a motion planning context, finding trajectories which minimize proximity to singular regions, subject to constraints. We define a manipulability-based likelihood associated with singularity avoidance over a continuous trajectory representation, which we then maximize using a maximum a posteriori (MAP) estimator. Viewing the MAP problem as inference on a factor graph, we use gradient information from interpolated states to maximize the trajectory's overall manipulability. Both qualitative and quantitative analyses of experimental data show increases in manipulability that result in smooth trajectories with visibly more dexterous arm configurations.},
  address = {Madrid, Spain},
  author = {Filip Marić and Oliver Limoyo and Luka Petrović and Ivan Petrović and Jonathan Kelly},
  booktitle = {Proceedings of the IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS'18) Workshop Towards Robots that Exhibit Manipulation Intelligence},
  date = {2018-10-01},
  month = {Oct. 1},
  title = {Manipulability Maximization Using Continuous-Time Gaussian Processes},
  url = {https://arxiv.org/abs/1803.09493},
  year = {2018}
```

</p>
</details>

[<span style="color:green">**[ preprint ]**</span>](https://arxiv.org/abs/1908.02963) 
[<span style="color:red">**[ video ]**</span>](https://youtu.be/tB34VfDrF84)
<!-- <a class="tiny ui green button" href="https://arxiv.org/abs/1908.02963"><i class="file alternate outline icon"></i>Preprint</a> -->
<!-- <a class="tiny ui red button" href="https://youtu.be/tB34VfDrF84"><i class="youtube icon"></i>Video</a> -->
</div>
</br>
