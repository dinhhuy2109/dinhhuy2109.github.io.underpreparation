---
layout: post
category: projects
title: "We won 2nd place at Airbus Shopfloor Challenge @ICRA2016"
excerpt: "Competing teams designed and built robotic systems that are able to perform accurate drilling compliant with aeronautic standards. "
tags: [ICRA2016, Airbus, Challenge]
comments: true
---

### May 2016

Our research group participated in Airbus Shopfloor Challenge which was held at IEEE International Conference on Robotics and Automation (ICRA) 15-21 May 2016 in Stockholm, Sweden.

Many tasks in an aircraft assembly line involve drilling. At Airbus, million of holes are needed to be drilled every year, by human operators. This motivates the company to look for automated solutions for drilling process. A competing team needed to build a light-weighted robot system (weighing less than 100 kg.) able to perform drilling tasks with a stringent accuracy requirement. In particular, a competing robot needed to drill a given pattern of 255 holes on a 70 cm. x 70 cm. aluminium plate.

Our solution consisted of a 6-DOF Denso VS-060 arm equipped with an industrial ENSENSO camera and a drill at the end-effector. Simulations in a virtual environment were done using OpenRAVE. We used ROS for system integration and real-time communication with the robot.

I was in charge of sensor, robot calibrations and perception for the system. The calibration tasks includes the tool (drill bit) calibration, camera calibration and hand-eye calibration. The perception tasks were to locate the aluminium plate (with respect to 3 small reference holes on the plate). Following the aircaft manufacturing standard, this challenge has a very high accuracy requirement; therefore, calibration and perception are really crucial. We developed new tool-base calibration method that allows us to perform quickly the calibration with high accuracy. During this time, we also came up with the new approach for hand-eye calibration [paper]. The perception solution is a combination of 3D (pointcloud) an 2D (image) processing.
 
Our team finished at second! You can find the coverage on the [Airbus website](http://company.airbus.com/careers/Working-for-Airbus/Airbus-Shopfloor-Challenge-2016.html), [Robohub](http://robohub.org/airbus-shopfloor-challenge-overview-with-video/), [NTU MAE website](http://www.mae.ntu.edu.sg/NewsnEvents/Pages/Detailed-Page.aspx?news=9719917d-4ffb-40ac-aaf6-897f5ed58a93).

Bonus: We had 3 months to build up our system (since we decided to join the challenge). We did work really hard. And we did learn a lot from the challenge! Such a great experience!

{:refdef: style="text-align: center"}
<figure>
  <img src="{{ site.url }}/images/airbus_challenge.jpg">
  <figcaption>Fig.1: Our team with the robot. We drilled the group name onto the plate to showcase our abilies to airbus for the first round.</figcaption>
</figure>
{: refdef}

<iframe width="560" height="315" src="https://www.youtube.com/embed/FUmx7c8P-gs?start=179" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
{:refdef: style="text-align: center"}
<figcaption>Vid.1: Interview at the live competition</figcaption>
{: refdef}
