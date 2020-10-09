---
layout: default
title: Block Programming
permalink: /technology/blockprogram/
h1: Block Programming
h2: Technology
---
<section50> 
<h1>Coding for Beginners</h1>
<p> Google's Blockly and MIT's Scratch
are both great block-based programming languages to learn coding. Both provide visual interlocking blocks to represent code concepts like variables, logical expressions, loops, and more.</p>

<div class="section50left">
<h2>Blockly</h2>
<p>Blockly is used by a variety of coding platforms like code.org, MIT App Inventor and popular robots like Dash. <br> It allows you to create computer games and apps. </p> </div>

<div class="section50right">
<h2><a href="https://scratch.mit.edu/" target="_blank">Scratch</a></h2>
<p>MIT's Scratch is a popular language for beginners. All you have to do is make an account <a href="https://scratch.mit.edu/" target="_blank">here</a>, and you can create games, animations, and interactive stories.</p>
</div>
</section50> 

<section50short>
<div>We recommend Blockly because of it's wider usage. Once you’re comfortable with Blockly or Scratch, check out our other pages to learn Python, Java, C++, and HTML, which allow you to create programs that can do even cooler things!</div>
</section50short>
<br>

{% for comp in site.block %}  
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
    </div>

    <div class="section50right">
    <ul class="compl1">
    <li> {{ comp.description }} </li>
    <br>
    <li><b>Grades:</b> {{ comp.grades }} </li>
    </ul>
    <ul class="compl2">
      {{ comp.content }} 
    </ul>

    </div>

  {% else %}

    <div class="section50left">
    <ul class="compl1">
    <li> {{ comp.description }} </li>
    <br>
    <li><b>Grades:</b> {{ comp.grades }} </li>
    </ul>
    <ul class="compl2">
      {{ comp.content }} 
    </ul>

    </div>
 
    <div class="section50right">

    {% if comp.picsmall %}
      <img style="width:350px" src="{{ comp.pic }}">
    {% else %}
      <img src="{{ comp.pic }}">
    {% endif %}

    </div>

  {% endif %}

</section50>
<br>
{% endfor %}