# OSS-Overview
# Robotics Projects

---

## Project 1
## Build a 6 DoF Robotic Arm to catch a TT Ball randomly tossed at it.

This would involve using Object Tracking using Image Analysis tools (We will use OpenCV)

Then we will suitably scale the image such that the distance of the ball can be analysed.

We will train a NN to recognize the ball and depending on its size, find its distance from the arm. Then it will compare it with previous images to determine the trajectory of the ball.

Once the trajectory it determined, a separate NN will parallely solve the **Inverse Kinematics** problem of orienting the arm by manipulating the 6 Degrees of Freedom.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=M413lLWvrbI
" target="_blank"><img src="http://img.youtube.com/vi/M413lLWvrbI/0.jpg" 
alt="EPFL Project using KUKA Robot" width="640" height="480" border="10" /></a>

---

## Project 2
## Have group of robots (drones) to explore a region in co-ordinated manner for Simultaneous Localization and Mappin (SLAM) implementation.

A couple of drones would fly from designated starting points and fly around in a seemingly random manner while covering the whole space.
They will avoid all the obstacles they encounter all the while capturing local images helping build a map of their surroundings.

*We will add additional tasks to perform for the drones after all the region is fully explored*

<a href="http://www.youtube.com/watch?feature=player_embedded&v=EMNNSEwX1tE
" target="_blank"><img src="http://img.youtube.com/vi/EMNNSEwX1tE/0.jpg" 
alt="University of Pennsylvania Project" width="640" height="480" border="10" /></a>

---
