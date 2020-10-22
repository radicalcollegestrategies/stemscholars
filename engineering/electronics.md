---
layout: default
permalink: /engineering/electronics/
title: Electronics
h2: Engineering
---
{% for comp in site.electronics %}  
<section50> 
  <h2><a href="{{ comp.toplink }}" target="_blank">{{ comp.heading }}</a></h2>

  <!-- Use capture to prevent outputting i -->
  {% capture _%}{% increment i %}{% endcapture %}
  {% assign mod = i | modulo:2 %}

  <!-- For even loop runs, put pic to left. Switch for odd -->
  {% if mod == 0 %}

    <div class="section50left">
    {% if comp.picsmall %}
      <img style="width:350px" src="{{ comp.pic }}">
    {% else %}
      <img src="{{ comp.pic }}">
    {% endif %}

    {% if comp.piccreator %}
      <div class="license">(
        <a href="{{ comp.piclink }}" target="_blank">Image</a>
        <a href="{{ comp.piclicense }}" target="_blank">licensed</a> from {{ comp.piccreator }}
        )</div>
    {% endif %}

    <h3> {{ comp.piccaption }} </h3>
    </div>

    <div class="section50right">
    <p style="font-size:18px"> {{ comp.description }} <br>
    <b>Grades:</b> {{ comp.grades }} </p>
    <ul class="compl2" style="line-height:1.75;">
      {{ comp.content }} 
    </ul>
    </div>

  {% else %}

    <div class="section50left">
    <p style="font-size:18px"> {{ comp.description }} <br>
    <b>Grades:</b> {{ comp.grades }} </p>
    <ul class="compl2" style="line-height:1.75;">
      {{ comp.content }} 
    </ul>
    </div>
 
    <div class="section50right">

    {% if comp.picsmall %}
      <img style="width:350px" src="{{ comp.pic }}">
    {% else %}
      <img src="{{ comp.pic }}">
    {% endif %}

    {% if comp.piccreator %}
      <div class="license">(
        <a href="{{ comp.piclink }}" target="_blank">Image</a>
        <a href="{{ comp.piclicense }}" target="_blank">licensed</a> from {{ comp.piccreator }}
        )</div>
    {% endif %}

    <h3> {{ comp.piccaption }} </h3>
    </div>

  {% endif %}

</section50>
<br>
{% endfor %}

