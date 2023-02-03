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


During the Fall 2022 semester, I joined the DiscoverAI program in the University of Hawaii of Manoa. We had online synchronous meetings every Friday. The topics that were discussed dealt with Artificial Intelligence, Machine Learning, and coding using Python. We were assigned groups and tasked to come up with a final project related to AI.

As a member of the group, I participated with group discussion and threw in ideas about our final project. We came up with the topic about computer vision in cars. We come up with the idea of the Zumi bot, which is a miniature programmable robotic car. We used Python to code the actions of the robotic car. It can do forward, backward, left, and right motion. It can also detect objects and colors.

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

Overall, the project was successful. There are some minor improvements that should be done such as proper object recognition since it needs a lot of pictures to store in its memory to identify a certain object as well as the color.

Source: <a href="https://github.com/theVacay/vacay](https://www.robolink.com/products/zumi">Information about Zumi</a>
