---
layout: default
permalink: /stem/science/
title: Science
h2: Physics, Chemistry and Biology
---

<section50short> 
<h2>Explore Science in Elementary School</h2>
<p>Several book sets and video series cover a variety of fascinating topics in Science. The child and their parent should ideally read and watch these together and discuss them afterwards.</p>
</section50short>

{% for comp in site.elemsci %}  
<section50> 
  <h2> <a href=" {{ comp.toplink }} " target="_blank">{{ comp.heading }} </a> </h2>

  <!-- Use capture to prevent outputting i -->
  {% capture _%}{% increment i %}{% endcapture %}
  {% assign mod = i | modulo:2 %}

  <!-- For even loop runs, put pic to left. Switch for odd -->
  {% if mod == 0 %}

    <div class="section50left">
      {% if comp.video %}
        <iframe src="{{ comp.video }}" scrolling="no" allowfullscreen="" width="450" height="250" frameborder="0"><br/></iframe>
      {% else %}
        <img src="{{ comp.pic }}">
      {% endif %}
    </div>

    <div class="section50right">
    <ul class="compl1">
    <li><b>Grades:</b> {{ comp.grades }} </li>
    <li> {{ comp.description }} </li>
    <br>
    <li>Details:
    <ul class="compl2">
      {{ comp.content }} 
    </ul> </li> </ul>
    </div>

  {% else %}

    <div class="section50left">
    <ul class="compl1">
    <li><b>Grades:</b> {{ comp.grades }} </li>
    <li> {{ comp.description }} </li>
    <br>
    <li>Details:
    <ul class="compl2">
      {{ comp.content }} 
    </ul> </li> </ul>
    </div>

    <div class="section50right">
      {% if comp.video %}
        <iframe src="{{ comp.video }}" scrolling="no" allowfullscreen="" width="450" height="250" frameborder="0"><br/></iframe>
      {% else %}
        <img src="{{ comp.pic }}">
      {% endif %}
    </div>

  {% endif %}

</section50>
<br>
{% endfor %}

<section50short>
<h2>More Science in Middle and High School</h2>
<img class="center" src="/images/ComingSoon.png" style="width:600px; padding-bottom:50px;">
</section50short>
