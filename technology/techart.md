---
layout: default
permalink: /techart/
title: Artistic Technology
h2: Technology
---

<section50>
<h2>Unleash your Creativity</h2> 
<div class="section50right">
<iframe src="https://www.youtube.com/embed/CwDAv_ihml0" scrolling="no" allowfullscreen="" width="450" height="250" frameborder="0"><br/></iframe>
</div>

<div class="section50left">
<p>Do you have an artistic bone and admire the aesthetics of 
  <ul class="disc16l1" style="padding-left:50px">
  <li>an app/website</li>
  <li>a logo</li>
  <li>a great animation</li>
  <li>the scenery of a virtual reality game</li>
  <li>the smooth curves on a car</li>
  </ul>
  
  There are many exciting trends in the tech industry which let you express your creativity at a whole different level! </p>

</div>
</section50>

<br>
{% for comp in site.techart %}  
<section50> 
  <h2 id="{{ comp.hash }}"> {{ comp.heading }} </h2>

  <!-- Use capture to prevent outputting i -->
  {% capture _%}{% increment i %}{% endcapture %}
  {% assign mod = i | modulo:2 %}

  <!-- For even loop runs, put pic to left. Switch for odd -->
  {% if mod == 0 %}
  <div class="section50right">
  {% else %}
  <div class="section50left">
  {% endif %}

  <a href="{{ comp.link }}" target="_blank">
    {% if comp.picsmall %}
      <img style="width:350px" src="{{ comp.pic }}">
    {% else %}
      <img src="{{ comp.pic }}">
    {% endif %}
  </a>

    {% if comp.piccreator %}
      <div class="license">(
        <a href="{{ comp.piclink }}" target="_blank">Image</a>
        <a href="{{ comp.piclicense }}" target="_blank">licensed</a> from {{ comp.piccreator }}
        )</div>
    {% endif %}

    <h3> {{ comp.piccaption }} </h3>
  </div>

  {% if mod == 0 %}
  <!--div class="section50left" style="padding-left:20px"-->
  <div class="section50left">
  {% else %}
  <div class="section50right">
  {% endif %}
    <ul class="compl1">
    <li class="li2" ><b>Grades:</b> {{ comp.grades }} </li>
    <li>
    <ul class="disc16l1">
    {{ comp.content }} 
    </ul> </li>
    </ul>
    </div>

</section50>
<br>
{% endfor %}

<section50>
<h2>More coming soon</h2>
<img class="center" src="/images/ComingSoon.png" style="width:600px; padding-top:50px;">
</section50>
