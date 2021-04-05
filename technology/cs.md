---
layout: default
permalink: /computerscience/
title: Computer Science
h2: Technology
---

<section50short>
<h2>What is Computer Science?</h2> 
<p>Computer Science is the study of computers and computing as well as their theoretical and practical applications. The first step to learning Computer Science is "coding", which helps us communicate with computers. When you write your code, you need 3 parts:</p>
  <ul class="disc16l1" style="padding-left:100px">
  <li>An editor to write your code in</li>
  <li>A programming language</li>
  <li>The logic of the program that explains the computer what to do</li>
  </ul>
  <p>Each of these parts is explained below</p>

</section50short>

<section50>
<h2>Code Editors / IDEs</h2>
<div class="section50right">
    <iframe src="https://www.youtube.com/embed/Whps_IeaetM" scrolling="no" allowfullscreen="" width="450" height="250" frameborder="0"><br/></iframe>
</div>

<div class="section50left">
    <p>An Integraged Development Environment (IDE) is a software you install on your PC or Mac to write and debug your code easily. It's best to use an IDE that supports multiple languages, so it's one less thing to learn as you become more advanced in your programming.</p>
    <p>We highly recommend using <a href="https://code.visualstudio.com/" target="_blank">Visual Studio Code</a>, a.k.a. VSCode, because it supports many languages, is user friendly for debugging and is integrated with Git. </p>
    <p>If you prefer to use an IDE on a web browser, e.g., if you're working on a Chromebook or if you like to access your programs from multiple computers, then use <a href="https://codenvy.com/" target="_blank">Code Envy</a>.</p>
</div>
</section50>

<section50>
<h2>Programming Language</h2>
<div class="section50left">
    <iframe src="https://www.youtube.com/embed/EGQh5SZctaE" scrolling="no" allowfullscreen="" width="450" height="250" frameborder="0"><br/></iframe>
</div>

<div class="section50right">
    <p><i>"Programming is giving a set of instructions to a computer to execute."</i> </p> 
    <p>When you code, you use a <b>programming language</b> to give these instructions in a logical sequence to the computer. Once you learn how to code, it's very easy to pick up new programming languages. </p>
    <p> We recommend starting with <b>Python</b>, as it's versatile, general purpose, and easy to learn! Once you get a hang of it, you can learn <a href="https://news.codecademy.com/programming-languages/#most-popular-programming-languages" target="_blank">other languages as needed</a>.</p>
</div>
</section50>

<section50>
<h2>Program Logic / Algorithm</h2> 
<div class="section50right">
    <iframe src="https://www.youtube.com/embed/CvSOaYi89B4" scrolling="no" allowfullscreen="" width="450" height="250" frameborder="0"><br/></iframe>
</div>

<div class="section50left">
    <p>A big part of Computer Science is learning algorithms.</p>
    <p>An <b>algorithm</b> is a set of steps, or "logic", for a program to accomplish a task.  Algorithms can range from simple, like: </p>
    <p style="font-style:italic;text-align:center;">if ... then do ... else do ...</p>
    <p> to complex ones like Google's PageRank to give you the most relevant results for your search queries.</p>
    <p>An algorithm is independent of the programming language, though some languages make it easier to code certain kinds of algorithms.</p>
</div>
</section50>

<section50short>
  <div class="note">
    <p style="text-align:center; padding-top:13px">The section below delves deep into algorithmic CS. If you have an <b>artistic</b> touch, then explore the <br><a href="/techart/" target="_blank">Artistic Tech</a> page to design and create videos, websites, apps, animations, CAD and video games!</p>
  </div>
</section50short>


<br>
{% for comp in site.coding %}  
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
    <li class="li2"><b>Grades:</b> {{ comp.grades }} </li>
    {{ comp.content }} 
    </ul>
    </div>

</section50>
<br>
{% endfor %}
