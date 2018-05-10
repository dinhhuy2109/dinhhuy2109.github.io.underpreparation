---
layout: post
category: blog
title: "Hand-eye calibration"
excerpt: "A short introduction to hand-eye calibration (camera-robot calibration)."
tags: [learning, calibration]
comments: true
---

#### To be updated

To relate the object pose
estimation to the robot base frame, the problem of determining the
transformation between the sensor and the end-effector is
crucial. This problem is usually referred as hand-eye calibration
problem and has long been an interesting topic which draws an
extensive attention from many robotic researchers. Here we
will show you how to formulate the hand-eye calibration problem as
well as suggest some relevant approaches to solve it.


<!-- In this Chapter, we consider one of the most fundamental tasks of -->
<!-- robot vision: *determining the position of the object relative to the -->
<!-- robot*. -->

{:refdef: style="text-align: center;"}
<figure>
  <img src="{{ site.url }}/images/denso-ensenso-object.png">
  <figcaption>"Fig.1 : A robot system with a camera mounted on the end-effector."</figcaption>
</figure>
{: refdef}

<!-- To have a better visualization of the problem, let us briefly consider -->
<!-- a robotics system as depicted in Fig. 1. The relative -->
<!-- transformation $_{b} T^{o}$ between the object -->
<!-- and the robot base is determined as follows: -->

<!-- Approaches and Implementations -->
<!-- ============================================ -->
<!-- As :math:`\bfX`, :math:`\bfA` and :math:`\bfB` represent rigid-body trans- formations, they live in -->
<!-- :math:`\bfS \bfE(3)`, a subset of the space of 4×4 matrices endowed with a -->
<!-- non-trivial Lie group structure, solving for :math:`\bfX` a difficult -->
<!-- problem. As it will requires many advanced mathematics theories to solve -->
<!-- this problem, we only list out some well-known articles for your reference. -->

<!-- - Using the Euclidean Group: -->
  
<!--   Park F. & Martin B., *Robot Sensor Calibration: Solving AX = XB -->
<!--   on the Euclidean Group*,  IEEE Transactions on Robotics and -->
<!--   Automation, (10) 1994, p. 717–721, available at `robotics.snu.ac.kr <http://robotics.snu.ac.kr/fcp/files/_pdf_files_publications/7_c/robot_sensor_calibration.pdf>`_ -->

<!-- - Using dual quaternions: -->
  
<!--   Daniilidis K., *Hand-eye calibration using dual quaternions* -->
<!--   Int. Journ. Robotics Res, 18: 286-298, 1999, available at -->
<!--   `citeseerx.ist.psu.edu <http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.18.366&rep=rep1&type=pdf>`_ -->

<!-- - Others: -->
  
<!--   Strobl, K. H., & Hirzinger, G. (2006, October), *Optimal hand-eye -->
<!--   calibration*, In Intelligent Robots and Systems, 2006 IEEE/RSJ -->
<!--   International Conference on (pp. 4647-4653),  available at -->
<!--   `here <http://ai2-s2-pdfs.s3.amazonaws.com/0646/aaa662a8e0b2a0a2bbcad938d68cd45102f7.pdf>`_ -->
  

<!-- Our open-source python implementation of F. Park, B. Martin's paper is available at . -->


> Exercises
> ===========================================
> **Note that:** Sometimes the camera may not be mounted on the end-effector
> but on a fixed stand (the system in fig. 2 is a prime
> example). In this case the relative transformation between the camera
> and the robot base is required to relate the object pose estimation to
> the robot base frame. This problem can also be formulated as the :math:`\bfA\bfX = \bfX\bfB`
> problem by commanding the robot moving a pattern mounted on its end
> effector while observing this pattern from the camera. (We let you do
> this as an exercise.)

<!-- .. admonition:: Exercise -->
		
<!--    Consider the system in fig. 2, formulate the problem of finding the -->
<!--    relative transformation between the camera and the robot base as -->
<!--    the :math:`\bfA\bfX = \bfX\bfB` problem. -->

<!--    .. figure:: ../figures/robot_vision/ensenso-denso-fixed.png -->
<!--       :width: 80% -->
<!--       :alt: denso -->
<!--       :align: center -->

<!--       ..    -->

<!-- 	 Fig. 2: A robot system where the camera is not mounted on the -->
<!-- 	 end-effector but on a fixed stand. -->
