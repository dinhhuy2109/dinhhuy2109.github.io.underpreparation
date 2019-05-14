---
layout: post
category: blog
title: "How to build your own smart home with customized Google Assistant"
excerpt: "Development diary of my smart home project "
tags: [learning, calibration]
comments: true
---

#### To be updated

Voice controlled assistants have quickly become commonplace. The
technology these devices run on is available—at least in part—to
everyone. Google’s Assistant SDK allows you to use the service on your
own devices. This blog covers how to set up the Google Assistant
on your Raspberry Pi or an old laptop/computer, and voice activate
electrical devices in your house.

# Hardware

{:refdef: style="text-align: center;"}
<figure>
  <img src="{{ site.url }}/images/raspberrypi.jpeg">
</figure>
{: refdef}

**You will need:**
- A Raspberry Pi with a fresh
  [Raspbian install on the SD card](https://www.raspberrypi.org/downloads/). However,
  I prefer [Ubuntu Mate](https://ubuntu-mate.org/raspberry-pi/) since
  the UI is much more familiar as I am a ubuntu user. You can also use
  an old computer as long as it has Linux based operating system.

- A microphone or a USB webcam with intergrated microphone.

- An external speaker.

- Circuit for controlling eletrical devices (optional).

Note: If you are using Rasberry Pi, make sure to check your CPU
specification. Currently, google assistant sdk only support ARMv7 and
above. So a compatible Pi is the 2 and 3. I am using the 2 model B.



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
