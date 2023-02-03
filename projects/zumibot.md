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
  
summary: "A responsive web application for travel planning that my team developed in ICS 415."
---

<img class="ui left medium float image" width="250"src="..img/vacay/Screenshot 2023-02-02 at 7.00.16 PM.png">

Vacay is a web application that I helped create as a team project in ICS 415, Spring 2015. The project helped me learn how to design and implement a responsive web site.

Vacay is implemented using [Meteor](http://meteor.com), a JavaScript application platform. Within two weeks, we created a website that implements several types of reservations including flights, hotels, and car rentals.

In this project I gained experience with full-stack web application design and associated technologies, including [MongoDB](http://mongodb.com) for database storage, the [Twitter Bootstrap](http://getbootstrap.com/) CSS Framework for the user interface, and Javascript for both client and server-side programming. 

Here is some example code to illustrate Simple Schema use:

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
