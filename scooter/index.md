---
title: Scooter
description: Technical research details. Read what our project is about.
nav:
  order: 0
  tooltip: Details on what we do
  
---
# {% include icon.html icon="fa-solid fa-book" %} Our Research
Our goal is to make e-scooters more convenient to access and less annoying when 
left behind. We set out to design an inexpensive addition for e-scooters that
allows them to park themselves after a rider is done so that they do not get 
in the way. To that end, we have designed an autonomous electric scooter that 
can sense the  environment, develop a path plan, and execute it. The scooter has
been shown to autonomously navigate paths up to 400 meters, and we have
plans to extend that range. 

{% include figure.html image="images/scooter_in_motion.png" width="50%" %}

# {% include icon.html icon="fa-solid fa-users" %} Meet the Scooters
{% include figure.html image="images/all_3_scooters.jpg" width="75%" %}
From left to right, we have Ben Parker, Richard Parker, and Peter Parker!

__Ben__ is the oldest. It was our first foray into self-navigating scooters. 
Please excuse it's small size—it was meant to be a proof of concept, not a fully-fledged vehicle for riding!

__Richard__ has received the most development. After Richard, we knew we were 
serious about this project.
Richard can navigate, avoid obstacles, and park itself completely autonomously 
(without a remote control!). However, Richard can't be controlled by human riders.
It is due to this reason that, with great sadness, we put Richard to rest and began working
on the newest iteration.

__Peter__ is the youngest. We are still bringing Peter up to speed with Richard. 
Our goal is for Peter to be ridable by humans while retaining it's ability to 
move autonomously like Richard. Peter is rough around the edges right now, but,
with time, Peter will grow up to be just like Richard!

__All__ are Parker's. All "park" themselves. Their name follows from their function!



# {% include icon.html icon="fa-solid fa-wrench" %} How We Did It

Our approach is to customize commercial off-the-shelf electric scooters with the hardware
and sensors required to achieve micro-scale re-positioning up to several hundred meters. This project
was originally funded as a seed grant from the Maryland Transportation Institute entitled “Research in Electric Scooter Urban Mobility (RESUME)”, which we have renamed ReZoom. Our
ongoing efforts have led to three iterations, an example of which can be seen in the above picture.
The ReZoom electronic stack includes a single board computer that performs all onboard
computing and runs the Robot Operating System (ROS) on Ubuntu Linux. Additionally, we have
a stereo camera for depth sensing, Inertial Measurement Units (IMUs) and GPS modules for
localization, a motor driver and accompanying power circuitry for navigation.

Creating a self-driving electric scooter poses novel challenges in autonomous vehicle research. By comparison, self-driving cars are equipped with sensors and computation capabilities
that are too large and expensive for e-scooters. Therefore, our approach towards these challenges
is to leverage advances in mobile robotics, while keeping in mind the physical, technical, and
financial constraints of a shared e-scooter system including the unit cost. Our efforts focus on
developing hardware and software specific to this system to help achieve the goal of building a
sustainable, accessible, and equitable micromobility platform for shared rental operators.

We seek to develop a hardware and software stack capable of achieving autonomous micro-scale re-positioning of the scooter; planning a path through roads, trails, and sidewalks; navigating while avoiding cars and pedestrians; and being sufficiently low-cost to be deployed on a large
scale. Historical rental scooter ride data will allow the scooter to take advantage of previous rides
performed by humans and learn the optimal paths to navigate through the urban landscape. In addition, we will develop onboard perception and state estimation algorithms to enable the scooter
to perceive its environment and navigate relative to its goal, up to hundreds of meters away.


{% include tags.html tags="publication, resource, website" %}

{% include search-info.html %}

{% include section.html %}

{% include figure.html image="images/electronic_stack.png" width="50%" %}

The electronic stack (pictured above) includes an Nvidia Jetson Orin single board computer, which performs all on-board computing, that runs the Robot Operating System (ROS) and Ubuntu 20. Additionally, we have a stereo camera (pictured below) for depth sensing, inertial measurement units (IMUs) and GPS modules for localization, a motor driver, and an accompanying power circuit for navigation. Motion planning for the scooter follows an Ackermann (car-like) drive model, implemented with the TEB Local Planner in ROS.


{% capture col1 %}

{%
  include figure.html
  image="images/stereo_camera.png"
  caption="Camera on the scooter"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/historical_scooter_data.png"
  caption="Historical scooter data"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}


Another aspect of this work is to use historical scooter data from Veo for global path planning. This data consists of GPS locations from scooter rides taken in and around campus during 2019 and 2020, and with it, we have been able to construct a graph of scooter paths, where lower edge weights correspond to more frequently taken paths. This allows us to not only create the heatmap as shown in the picture above, but also allows for efficient path planning.


Check out our scooter in action:
<iframe width="800" height="450" src="https://www.youtube.com/embed/videoseries?list=PLEhNI36DhkD_JkXSu9XVa--v94nfLigpu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<!-- 
<iframe width="800" height="450" src="https://www.youtube.com/embed/Z1cvNpJkJLY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe> -->


{% include section.html dark=true %}

<center>Please feel free to contact us with any questions!</center>
{%
  include button.html
  type="contact-page"
  text="Contact Us"
  link="contact"
%}
