---
name: Obstacle detection car
tools: [ESP32, Micropython, Circuits, Class Project]
image: https://f001.backblazeb2.com/file/BIT-Magazine-Images/image-1270-news.jpg
description: Feb. 2024 - May 2024 This project is an RC car showcasing a concept in car obstacle detection to reduce blind spots. The prototype also provides user information about location of object.
---

# Obstacle Detection Car
###### **Collaborator/s:** Jacob Feingold, Panithan Lertsuntivit
###### February 2024 - May 2024
___
![Preview](https://raw.githubusercontent.com/rhkhuggay/Projects/refs/heads/main/ME100%20Project/ME100_project.png)

**Figure 1:** RC car and controller

The goal of this project is to build a Remote Controlled (RC) car that detects and alerts the user of surrounding obstacles. It showcases a concept for blindspot monitoring system in cars to increase driver awareness through the use of an ultrasonic sensor or Lidar. This is useful especially in non-ideal condition (e.g. fog, rain, night) that reduces visibility when driving. 

![Preview](https://raw.githubusercontent.com/rhkhuggay/Projects/refs/heads/main/ME100%20Project/diagram.png)

**Figure 2:** Communication diagram of the our system

The control system of the device is shown figure 2. There are two ESP32 that connected together via ESPnow. One microcontroller is connected to 2 dc motor, a servo motor, and ultrasonic sensor. This ESP32 then sends information about the distance between an object relative to the car to the other ESP32. Once received, the object's position is revealed to the user through LED lights indicating whether the object is North/Northeast /Northwest /East/West of the car. A demo of our project is shown below.

{% include elements/video.html id="DEBuqSdDbdw" %}

## Contribution

My main responsibilities include creating the circuit and code for the 2 DC motor, and managing battery supply. For better control of the car, I decided to use two joysticks where one controls the left motor and the other controls the right. This makes it easier to maneuver the car in tight spaces. One challenge that I had was efficiently distributing power between all the components. My first solution was powering the ESP32 and servo moor with a 5V Lipo battery and the the 2DC motor with a 9V battery. This ensures that our components receive required voltage input. However, given the physical model of our car, the Lipo battery were overcrowding the components on top of the car. Therefore, I decided to connect a 5V voltage regulator between the motor driver and the ESP32. This then allows the ESP32 and servo motor to be powered by thesame 9V battery while ensuring required voltage inputs are met for each component. Motor code is shown [here](https://github.com/rhkhuggay/Projects/blob/main/ME100%20Project/Motor_with_receiver_V2.py)

In addition, I collaborated with my team in creating code for connecting the two ESP32s via ESPnow and helped with overall integration of all our components. I also did the demo and presented our project on google slide with the team. Click "Learn more" to access our code.

<p class="text-center">
{% include elements/button.html link="https://github.com/rhkhuggay/Projects/tree/main/ME100%20Project" text="Learn More" %}
</p>