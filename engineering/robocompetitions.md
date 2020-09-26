---
layout: default
title: Robotics Competitions
permalink: /engineering/robocompetitions/
h1: Robotics Competitions
h2: Engineering
---
<section50short style="height: 75px; padding-bottom:10px">
  <div class="tabinactive">
    <h2><a class="h2link" href="/engineering/robotics">Robotics</a></h2>
  </div>
  <div class="tabactive">
    <h2>Robotics Competitions</h2>
  </div>
</section50short>

<section50short> 
<h2>What are Robotics Competitions?</h2>
<div>There are several robotics competitions for all age levels. Why should you participate in them? Robotics competitions give you a goal to work towards while learning robotics. Without a competition, you will buy a robot, and maybe play with it for a few days or weeks, and then it becomes another “toy” lying around the house. A competition, on the other hand, gives you a framework that defines what size team to collect, what kind of robot to build, what missions to program the robot for, and what timeframe to shoot for. It makes robotics a lot more fun!
You don’t have to shoot to win 1st place. Just enjoy the experience.
 </div>

<h2>Robotics Competition Format</h2>
<section50>
    <img class="section50left" src="/images/engg/Emanuele1.jpg">
<div class="sectionpdright">
For any competition, you will need a team. At least in elementary and middle schools,
you can form a robotics team with your friends, or join a team and make new friends. 
What can be more fun than spending hours with them every week doing robotics together? 

<br> <br>

Most robotics competitions follow the same format: Teams build a robot and some attachments, then use the accompanying software to program it to complete a series of missions. During the competition, every team runs their robot, and the team with most points from the missions wins.
<br> <br>
There are a wide variety of robotics competitions out there. We’ve compiled the most fun and prestigious ones below. 
 </div>
</section50>

{% for comp in site.robocomp %}  
<section50> 
  <h2> <a class="h2link" href=" {{ comp.toplink }} ">{{ comp.heading }} </a> </h2>

  <!-- Use capture to prevent outputting i -->
  {% capture _%}{% increment i %}{% endcapture %}
  {% assign mod = i | modulo:2 %}

  <!-- For even loop runs, put pic to left. Switch for odd -->
  {% if mod == 0 %}

    <img class="section50left" src="{{ comp.pic }}">
    <div class="section50right">
    <ul class="compl1">
    <li><b>Grades:</b> {{ comp.grades }} </li>
    <li><b>Team Size:</b> {{ comp.teamsize }} </li>
    <li><a href=" {{ comp.video }} ">Video Demo</a> </li>
    <li>You need:
    <ul class="compl2">
      {{ comp.content }} 
    </ul> </li> </ul>
    </div>

  {% else %}

    <div class="section50left">
    <ul class="compl1">
    <li><b>Grades:</b> {{ comp.grades }} </li>
    <li><b>Team Size:</b> {{ comp.teamsize }} </li>
    <li><a href=" {{ comp.video }} ">Video Link</a> </li>
    <li>What you need
    <ul class="compl2">
      {{ comp.content }} 
    </ul> </li> </ul>
    </div>
    <img class="section50right" src="{{ comp.pic }}">

  {% endif %}

</section50>
<br>
{% endfor %}

<section50short> 
<h2>Our recommendations</h2>
<img class="center" src="/images/ComingSoon.png" style="width:600px;">
</section50short>

<br>