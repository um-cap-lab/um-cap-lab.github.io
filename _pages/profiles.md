---
layout: profiles
permalink: /people/
title: People
description: Members of our lab
nav: true
nav_order: 7

profiles:
  # if you want to include more than one profile, just replicate the following block
  # and create one content file for each profile inside _pages/
  - align: right
    image: 2024-fall.jpg
    content: about_huteng.md
    image_circular: false # crops the image to make it circular
    title: Principle Investigator
  - align: left
    image: Mulchandani_Ashana_035.jpeg
    content: about_ashna.md
    image_circular: false # crops the image to make it circular
    title: Research Assistant
---

<div style="color: gray; font-size: 1.5em; margin-top: 2em;">
  Principle Investigator
</div>

{% for profile in page.profiles %}
<div class="profile">
  {% if profile.title %}
  <h2 style="color: gray; font-weight: bold;">{{ profile.title }}</h2>
  {% endif %}
  <img src="{{ profile.image }}" alt="{{ profile.content | strip_html }}" {% if profile.image_circular %}style="border-radius: 50%;"{% endif %}>
  {% include_relative {{ profile.content }} %}
</div>
{% endfor %}

<div style="color: gray; font-size: 1.5em; margin-top: 2em;">
  Collaborators
</div>

<div>
  <p><strong>Richard Futrell</strong>, Associate Professor, Department of Language Science, University of California, Irvine,</p>
  <p><a href="https://sites.socsci.uci.edu/~rfutrell/">https://sites.socsci.uci.edu/~rfutrell/</a></p>
  <p><a href="mailto:rfutrell@uci.edu">rfutrell@uci.edu</a></p>

  <p><strong>Connor Mayer</strong>, Assistant Professor, Department of Language Science, University of California, Irvine,</p>
  <p><a href="https://www.socsci.uci.edu/~cjmayer/">https://www.socsci.uci.edu/~cjmayer/</a></p>
  <p><a href="mailto:cjmayer@uci.edu">cjmayer@uci.edu</a></p>
</div>
