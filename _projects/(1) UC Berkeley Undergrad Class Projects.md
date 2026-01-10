---
name: Undergraduate Class Projects (UC Berkeley)
tools: [DOE, Micropython, Circuits, Rapid Prototyping]
image: ..\images\UCBerkeley_undergrad\UCBerkeley_Eng.png
description: Courses ME127, ME100, ME103, ME130
---

<div class="text-center mb-4">
  <h1><strong>Undergraduate Class Projects</strong></h1>
</div>

{% capture list_items %}
Saddle Height Optimization
Multimaterial Deployable Thick Origami Structure
Analysis and Characterization of Househoold Duct Tape Brands
Obstacle Detection Car
{% endcapture %}
{% include elements/list.html title="Table of Contents" type="toc" %}

## Saddle Height Optimization 
###### **MECENG 130:** Design of Planar Machineries
###### **Team:** Rhonin Huggay
<h6 class="date mb-0">January 2025 - May 2025</h6>
___

<p class="lead" style="font-size: 1rem; line-height: 1.6; text-indent: 40px;">
For my MECENG 130 (Design of Planar Machineries) final project, I developed a MATLAB simulation using kinetostatic analysis on a 4-bar linkage model of a single-leg pedaling system. The project successfully determined the optimal bicycle saddle height that minimizes knee-joint load, providing a theoretical validation for popular, experimentally-derived fitting methods (e.g., Hamley, LeMond).
</p>

{% include elements/figure.html image="..\images\ME130_diagram.png" %}

<p class="text-center">
{% include elements/button.html link="https://drive.google.com/file/d/191gWbL7SsXyeodLGF1TsKzNfSvwPpLN0/view?usp=sharing" text="Learn More" %}
</p>

## Multimaterial Deployable Thick Origami Structure
###### **MECENG 127:** Introduction to Composite Materials
###### **Team:** Rhonin Huggay, Jason Wang
<h6 class="date mb-0">January 2025 - May 2025</h6>
___
<p class="lead" style="font-size: 1rem; line-height: 1.6; text-indent: 40px;">
Led research to experimentally optimized TPU hinge size in 3D printable and deployable origami materials. As well as validate the reliability of a low-cost fatigue testing machine for 3D printed elastomeric materials.
</p>


{% include elements/figure.html image="..\images\UCBerkeley_undergrad\OrigamiProject_cover_page.png" %}

{% include elements/video.html id="XRCKx74p40I" %}

<p class="text-center">
{% include elements/button.html link="https://drive.google.com/file/d/1k56PbLyQcEGEvgtSzirEbqEmIXiwhN9k/view?usp=drive_link" text="Learn More" %}
</p>

# Analysis and Characterization of Househoold Duct Tape Brands
###### **MECENG 103:** Experimentations and Measurements
###### **Team:** Rhonin Huggay, Akshat Kumar, Edwin Lopez, Siddhart, Ken Chen, Aashray
###### October 2024 - December 2024
___
<p class="lead" style="font-size: 1rem; line-height: 1.6; text-indent: 40px;">
The goal of this research is to analyze the strength per cost of common Duct Tape Brands (i.e. Scotch, 3M, Duck, Gorilla) and determine the the cost-effective brand in terms of tensile strength. Through this work, I gain experience in utilizing an Instron for tensile testing, plotting stress-strain graphs, and statistical error analysis.  
</p>
{% include elements/figure.html image="..\images\UCBerkeley_undergrad/ME103_diagram.png" %}

<p class="text-center">
{% include elements/button.html link="https://drive.google.com/file/d/1_Hy9LuYH-EkjDJz6zdFN6-1K1aMcR9n_/view?usp=sharing" text="Learn More" %}
</p>

# Obstacle Detection Car
###### **MECENG 100:** Internet of Things (IoT)
###### **Team:** Rhonin Huggay, Jacob Feingold, Panithan Lertsuntivit
###### February 2024 - May 2024
___

{% include elements/video.html id="DEBuqSdDbdw" %}

![Preview](https://raw.githubusercontent.com/rhkhuggay/Projects/refs/heads/main/ME100%20Project/ME100_project.png)

**Figure 1:** RC car and controller

The goal of this project is to build a Remote Controlled (RC) car that detects and alerts the user of surrounding obstacles. It showcases a concept for blindspot monitoring system in cars to increase driver awareness through the use of an ultrasonic sensor or Lidar. This is useful especially in non-ideal condition (e.g. fog, rain, night) that reduces visibility when driving. 

![Preview](https://raw.githubusercontent.com/rhkhuggay/Projects/refs/heads/main/ME100%20Project/diagram.png)

**Figure 2:** Communication diagram of the our system

The control system of the device is shown figure 2. There are two ESP32 that connected together via ESPnow. One microcontroller is connected to 2 dc motor, a servo motor, and ultrasonic sensor. This ESP32 then sends information about the distance between an object relative to the car to the other ESP32. Once received, the object's position is revealed to the user through LED lights indicating whether the object is North/Northeast /Northwest /East/West of the car. A demo of our project is shown below.



## Contribution

My main responsibilities include creating the circuit and code for the 2 DC motor, and managing battery supply. For better control of the car, I decided to use two joysticks where one controls the left motor and the other controls the right. This makes it easier to maneuver the car in tight spaces. One challenge that I had was efficiently distributing power between all the components. My first solution was powering the ESP32 and servo moor with a 5V Lipo battery and the the 2DC motor with a 9V battery. This ensures that our components receive required voltage input. However, given the physical model of our car, the Lipo battery were overcrowding the components on top of the car. Therefore, I decided to connect a 5V voltage regulator between the motor driver and the ESP32. This then allows the ESP32 and servo motor to be powered by thesame 9V battery while ensuring required voltage inputs are met for each component. Motor code is shown [here](https://github.com/rhkhuggay/Projects/blob/main/ME100%20Project/Motor_with_receiver_V2.py)

In addition, I collaborated with my team in creating code for connecting the two ESP32s via ESPnow and helped with overall integration of all our components. I also did the demo and presented our project on google slide with the team. Click "Learn more" to access our code.

<p class="text-center">
{% include elements/button.html link="https://github.com/rhkhuggay/Projects/tree/main/ME100%20Project" text="Learn More" %}
</p>