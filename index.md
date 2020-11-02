---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page
---
<div class="ui basic segment">
  <img class="ui small left floated rounded image" src="/assets/filip_275.jpg">

  My name is Filip Marić and I am a Ph.D. student with the [STARS](www.starslab.ca) lab at the University of Toronto, directed by Prof. [Jonathan Kelly](http://stars.utias.utoronto.ca/~jkelly/). 
  I am also jointly affiliated with [LAMOR](https://lamor.fer.hr/lamor) at the University of Zagreb, directed by Prof. Ivan Petrović.
  
  I'm exploring how methods based on computational [differential](https://en.wikipedia.org/wiki/Differential_geometry) and [algebraic](https://en.wikipedia.org/wiki/Algebraic_geometry) geometry can be used in motion planning, analysis and control for robotic manipulators. 
  If you're interested in my work, check out the [publications](/publications) page for a list of papers and related resources.
  
</div>

### Recent Publications

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
</div>

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
**[ submitted ]** Robotics and Autonomous Systems 
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


</br>
