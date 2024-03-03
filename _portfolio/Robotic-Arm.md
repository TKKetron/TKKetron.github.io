---
title: "Robotic Arm (WIP)"
excerpt: "A robotic arm a team and I are implementing computer vision to identify and pick up boxes"
collection: portfolio
---

This is a project I am currently working on as my capstone for the University of Louisville. One of the professors here at the university has a robotic arm that was build by a previous mechanical engineering team as their capstone. My team and I are tasked with aiding computer vision to the robotic arm to allow it to maneuver and grab boxes autonomously.

Here is what the arm currently Looks like:
![Robotic arm](/images/Robotic%20arm/robotic-arm.jpg)

We are going to be using a Raspberry pi, and an HDR camera to perform the vision processing. From there the PI will perform the math required to calculated the position of each motor needs to be turned to in order for the head to be above the box. These positions will be sent to a motor controller separate form the PI. Once the arm is in place we have a simple relay to turn on the vacuum to grab the box. From there we can then move it to the desired drop off location.

Currently we are still in the early stages and are also working with a mechanical team for a redesign of the arm. The primary goal as of now if figure out the kinematics to calculate the motors positions. The mechanical team is also working to change from stepper motors to encoded DC motors. this will alow for more precision because we will have a closed loop from the encoder and we cant miss steps.

As for the vision, it was a fairly simple problem and we already have the box detection on a uniform background:
![box detection](/images/Robotic%20arm/box-detection.png)