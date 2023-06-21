---
title: Opportunities
nav:
  order: 4
  tooltip: Positions we need filled
---

# {% include icon.html icon="fa-regular fa-user" %}Opportunities

The ReZoom team is currently seeking University of Maryland students skilled in 
mechanical engineering, electrical engineering, and business.


Email us below if you feel you meet these requirements!

{%
  include button.html
  type="email"
  text="dpaley@umd.edu"
  link="dpaley@umd.edu"
%}


{% include section.html %}
Examples of what we need:
{% capture col1 %}

{%
  include figure.html
  image="images/opportunity_pics/arduino.jpg"
  caption=" Flimsy Arduino mount"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/opportunity_pics/jetson.jpeg"
  caption="Insecure Jetson Computer mount"
%}

{% endcapture %}


{% capture col3 %}

{%
  include figure.html
  image="images/opportunity_pics/ODrive.jpeg"
  caption="No way to mount ODrive to scooter base "
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3%}

{% include section.html dark=true %}

