---
---

# a Self-Driving E-scooter

The long-term goal of this research is to develop self-driving e-scooter technology to increase sustainability, accessibility, and equity in urban mobility. Toward this goal, in this work we design and implement a self-driving e-scooter with the ability to safely travel along a pre-planned route using automated, onboard control without a rider. We also construct an autonomous driving framework by synthesizing open-source robotics software libraries with custom-designed modules specific to an e-scooter, including path planning and state estimation. The hardware and software development steps along with design choices and pitfalls are documented. Results of real-world autonomous navigation of our retrofitted e-scooter, along with the effectiveness of our localization methods are presented. Please feel free to reach out to us with inquiries!

{% include figure.html image="images/scooter_in_motion.png" width="50%" %}

{% include section.html %}



## Highlights

{% capture text %}

Learn more about our project!

{%
  include button.html
  link="scooter"
  text="Check out how it works"
  icon="fa-solid fa-arrow-right"
  flip=false
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/scooter_wide.jpg"
  link="scooter"
  title="Our Scooter"
  style="bare"
  text=text
%}

{% capture text %}

Check out our research papers!

{%
  include button.html
  link="publications"
  text="See what we've published"
  icon="fa-solid fa-arrow-right"
  flip = true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/book_icon.jpg"
  link="publications"
  title="Our Publications"
  flip = true
  text=text
%}


{% capture text %}

Look at who keeps ReZoom driving!

{%
  include button.html
  link="team"
  text="Meet our team"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/idea_factory.jpg"
  link="team"
  title="Our Team"
  text=text
%}
