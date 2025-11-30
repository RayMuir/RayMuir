---
permalink: /
title: "Rachel Muir"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a PhD student at the University of Kent, supervised by [Prof. Mark Batty](https://www.kent.ac.uk/school-of-computing/people/3126/batty-mark) and [Dr. Michael Vollmer](https://recurial.com/). My research focuses on type systems, operational semantics, theorem proving and mechanisation of proofs in Rocq.

My other interests include electronics, model making (planes, cars and motorbikes), working on my car (often not by choice, thanks car) and gaming. You can read more about some of my projects in my blog!

{% include base_path %}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.posts limit:3 %}
{% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
{% if year != written_year %}
<h2 id="{{ year | slugify }}" class="archive__subtitle">{{ year }}</h2>
{% capture written_year %}{{ year }}{% endcapture %}
{% endif %}
{% include archive-single.html %}
{% endfor %}