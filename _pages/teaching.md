---
layout: archive
title: "Teaching"
permalink: /teaching/
author_profile: true
---
I am not currently leading undergraduate classes at the University of Kent. 

However, I occasionally lead and assist in teaching classes at the [Tinker Society](https://www.tinkersoc.org). This is a free [maker society](https://ksu.co.uk/activities/tinkersoc) for both students and external participants to learn, share and create new things. If that sounds good to you, and you're in the Kent area, come along for an evening! (Externals can do a free trial - just come along).

My classes often consist of electronics and microcontrollers, but we also offer classes on 3D modelling/printing and PCB design. In the future, we aim to offer lessons on metalworking, including the use of our lathe and mill.

{% include base_path %}

{% for post in site.teaching reversed %}
  {% include archive-single.html %}
{% endfor %}
