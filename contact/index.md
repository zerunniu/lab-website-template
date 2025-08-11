---
title: Contact
nav:
  order: 5
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact

We welcome collaboration opportunities, research inquiries, and discussions about our work in artificial intelligence, federated learning, and large language models. Whether you're interested in joining our team, exploring potential partnerships, or learning more about our research, we'd love to hear from you.

Feel free to reach out to us through any of the contact methods below.

{%
  include button.html
  type="email"
  text="dual.group@sydney.edu.au"
  link="dual.group@sydney.edu.au"
%}
{%
  include button.html
  type="address"
  tooltip="School of Computer Science, University of Sydney"
  link="https://www.google.com/maps/place/School+of+Computer+Science,+University+of+Sydney"
%}

{% include section.html %}

{% capture col1 %}

{%
  include figure.html
  image="images/lab_cropped.jpg"
  caption="Our Research Lab"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/campus_cropped.jpg"
  caption="University of Sydney Campus"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}

{% include section.html dark=true %}

{% capture col1 %}
**Office Hours**  
Monday - Friday  
9:00 AM - 5:00 PM
{% endcapture %}

{% capture col2 %}
**Location**  
School of Computer Science  
University of Sydney, NSW 2006
{% endcapture %}

{% capture col3 %}
**Research Focus**  
Federated Learning  
Large Language Models  
Edge Computing
{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}
