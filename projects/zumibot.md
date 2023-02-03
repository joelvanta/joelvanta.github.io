---
layout: project
type: project
image: img/vacay/Screenshot 2023-02-02 at 7.00.16 PM.png
title: "Zumibot"
date: 2022
published: true
labels:
  - Python
  - Machine Learning
  - Artificial Intelligence
  
summary: "A miniature robotic car for DiscoverAI program Fall 2022"
---


During the Fall 2022 semester, I joined the DiscoverAI program in the University of Hawaii of Manoa. 


Here is an example code to used to operate the Zumi bot:

```cpp
zumi.mpu.calibrate_MPU() // calibrates the zumi's position
camera.start_camera() // starts zumi camera
   while 1 == 1:
      ir_readings = zumi.get_all_IR_data() // object detection sensors
      back_right_ir = ir_readings[2]
      back_left_ir = ir_readings[4]
      
      front_right_ir = ir_readings[0]
      front_left_ir = ir_readings[5]
      
      if front_left_ir < 100: 
        zumi.reverse()
      if back_right_ir < 50:
        zumi.forward()

```
 
Source: <a href="https://github.com/theVacay/vacay">theVacay/vacay</a>
