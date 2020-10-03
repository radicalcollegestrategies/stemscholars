---
layout: default
title: Logic Puzzles and Games
permalink: /technology/logic/
h1: Logic Puzzles and Games
h2: Technology / Mathematics
---

<section50short> 
<h2>Why Logic Puzzles and Games?</h2>
<div>
Logic is the bridge between Math and Programming. Logic puzzles and games teach you to:
<ul class="yes">
 <li>Think step-by-step to arrive at your solution</li>  
 <li>Work forward from the starting point and backwards from the end point to find the right path to reach the solution.</li>
 <li> Critical Thinking, Problem Solving and Reasoning. 
 <ul class="aboutl2"><li>All these are the same ingredients that you need to learn coding / programming! </li></ul>
 </li>
 <li>These puzzles provide you with hours of fun!
 <ul class="aboutl2"><li>If you enjoy math, you will surely enjoy solving Logic Puzzles and playing Logic Games.</li></ul>
 </li>
</ul>
<h2>Great Logic Puzzles and Games</h2>
<p> <a href="https://www.amazon.com/s?k=maze+books+for+kids&ref=nb_sb_noss_2" target="_blank">Mazes</a> and <a href="https://www.amazon.com/s?k=jigsaw+puzzles&ref=nb_sb_noss_2" target="_blank">Jigsaws</a> are great puzzles to start in pre-school. Some popular puzzles designed for school-aged kids and adults are listed below. Many puzzles here point to a website where you can play the puzzle, but you can easily substitute that with another website, or an app or a puzzle book! Use whatever medium works for you. </p>
</div>
<br>
</section50short>

{% for comp in site.logic %}  
<section50> 
  <h2> <a href=" {{ comp.toplink }} " target="_blank">{{ comp.heading }} </a> </h2>

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
        <a href="{{ comp.piclicense }} target="_blank"">licensed</a> from {{ comp.piccreator }}
        )</div>
    {% endif %}

    <h3> {{ comp.piccaption }} </h3>
    </div>

    <div class="section50right">
    <ul class="compl1">
    <li> {{ comp.description }} </li>
    <li><b>Ages:</b> {{ comp.ages }} </li>
    <li><b>Number of players:</b> {{ comp.num }} </li>   

    <br>
    <li>Puzzle Setup:
    <ul class="compl2">
      {{ comp.content }} 
    </ul> </li> </ul>
    </div>

  {% else %}

    <div class="section50left">
    <ul class="compl1">
    <li> {{ comp.description }} </li>
    <li><b>Ages:</b> {{ comp.ages }} </li>
    <li><b>Number of players:</b> {{ comp.num }} </li>
 
    <br>
    <li>Puzzle Setup:
    <ul class="compl2">
      {{ comp.content }} 
    </ul> </li> </ul>
    </div>
 
    <div class="section50right">

    {% if comp.picsmall %}
      <img style="width:350px" src="{{ comp.pic }}">
    {% else %}
      <img src="{{ comp.pic }}">
    {% endif %}

    {% if comp.piccreator %}
      <div class="license">(
        <a href="{{ comp.piclink }} target="_blank"">Image</a>
        <a href="{{ comp.piclicense }} target="_blank"">licensed</a> from {{ comp.piccreator }}
        )</div>
    {% endif %}

    <h3> {{ comp.piccaption }} </h3>
    </div>

  {% endif %}

</section50>
<br>
{% endfor %}
