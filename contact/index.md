---
title: Contact
nav:
  order: 5
  tooltip: How to reach us!
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact

Please feel free to reach out to us with inquiries about joining the team!

{%
  include button.html
  type="email"
  text="dpaley@umd.edu"
  link="dpaley@umd.edu"
%}
{%
  include button.html
  type="address"
  tooltip="Our location on Google Maps for easy navigation"
  link="https://goo.gl/maps/mQDBj1beFYWfvSLg9"
%}

{% include section.html %}

{% capture col1 %}

{%
  include figure.html
  image="images/derek_paley.jpg"
  caption="Dr. Derek Paley, Principal Investigator"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/idea_factory.jpg"
  caption="We are situated at the E.A. Fernandez IDEA Factory Building"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}

{% include section.html dark=true %}

