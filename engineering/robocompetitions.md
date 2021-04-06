---
layout: default
permalink: /robocompetitions/
title: Robotics Competitions
h2: Engineering
---
<section50short style="height: 75px; padding-bottom:10px">
  <div class="tabinactive">
    <h2><a href="/robotics">Robotics</a></h2>
  </div>
  <div class="tabactive">
    <h2>Robotics Competitions</h2>
  </div>
</section50short>

<section50> 
<h2>Why should you participate in Robotics Competitions?</h2>
<img class="section50left" src="/images/engg/EmanueleRobot.jpg">

<div class="section50right">
<p>There are several robotics competitions for all age levels. These competitions give you a goal to work towards while learning robotics. </p>
<p>Without a competition, you will buy a robot, and maybe play with it for a few days or weeks, and then it becomes another “toy” lying around the house.</p> 
<p>A competition, on the other hand, gives you a framework that defines what size team to collect, what kind of robot to build, what missions to program, and what timeframe to shoot for. It makes robotics a lot more fun!
Don't worry about winning - just enjoy the experience. </p>
 </div>
</section50>
<br>

<section50>
<h2>Robotics Competition Format</h2>

<div class="section50left">
<p>For any robotics competition, you will need a team. You can form a robotics team with your friends, or join a team and make new friends. What can be more fun than spending hours with them every week doing robotics together? </p>

<p>In the months prior to the competition date, teams build a robot and some attachments, then use the accompanying software to program it to complete a series of missions. An attachment is like an arm to push any levers or hold any parts to be dropped off or picked up during the challenge. </p>
<p>During the competition, every team runs their robot, and the team with most points from the missions wins. </p>

</div>

<img class="section50right" src="/images/engg/EmanueleTeam.jpg">

</section50>
<br>
<section50short>
<h2>Which competition should I participate in?</h2>
<p>Browse our <mark><a href="#list">complete list of popular robotics competitions</a></mark>, or follow the guidelines here to find the competition that's right for you!</p>
</section50short>

<section50short> 
<h3>Lower Elementary School: Grades K-3</h3>
<p><b><a href="/robotics#WhichRobot" target="_blank">Buy Dash Robot:</a></b> For elementary school students, we recommend the Dash robot by Wonder Workshop. You can get started with it very quickly, with no prior technical expertise. And remember to get together a team of your friends to participate in the <a href="#wonder">Wonder League Robotics Competition</a> because it’s a lot more fun that way! </p>

<h3>Upper Elementary / Middle School: Grades 4-8</h3>
<p> Once you outgrow the Dash robot, or if you skipped it altogether, you need to decide which robot to buy and which competition to participate in. First collect a team of your friends who will participate in a robotics competition with you, so you can make the decision togehter.</p>
<p><b>Deciding question 1:</b> Do you have a parent or another mentor who is an expert in tech <i>and</i> can spend at least 3 hrs every week for several months coaching your team? </p>

<div class="section50left"> 
<h4>I have a mentor</h4>
<p> Buy the <a href="/robotics#WhichRobot" target="_blank">Lego EV3 robot</a> and move onto "Deciding question 2"</p>
</div>

<div class="section50right"> 
<h4> I do not have a mentor </h4>
<p> Continue your robotics journey with <a href="/robotics#WhichRobot" target="_blank">Cue Robot</a>, and participate in the <a href="#wonder">Wonder League Robotics Competition</a> </p>
</div>

</section50short>
<section50short>

<p><b>Deciding question 2:</b> You decided to buy the EV3 robot, and now you need to decide which competition to prepare for. How many hours a week are you and your team willing to commit to robotics?</p>

<div class="section50left"> 
<h4> 10 or more hours/week </h4>
<p> <b><a href="#fll">Do FLL:</a></b> FLL is an intense competition with a lot of missions and a science project. The time commitment is equivalent to that of a competitive soccer team. It’s also a lot of fun because the mat is colorful and the LEGO missions are cute.</p>
<p>Your team should be willing to commit to FLL being their only (or main) extracurricular activity during August-November (and beyond, if you qualify for the next level). </p>
</div>

<div class="section50right"> 
<h4> About 3-8 hours/week </h4>
<p> <b><a href="#robofest">Do Robofest:</a></b> Robofest is purely a robotics competition with easy setup where you can participate in one or more challenges.</p>
<p>You can decide how many challenges to participate in, depending on your interest level and other activities.</p>
</div>
</section50short>

<section50short>
<h3>High School: Grades 9-12</h3>
<p>You can participate in a traditional robotics competition (below) or build your own engineering device and present it at your local <a href="/science/#isef" target="_blank">Science and Engineering Fair</a>.</p>
<p>All the FIRST competitions like FTC and FRC are intense and require a lot of time commitment. For example, during the build season for FRC, you may be working on your robot for about 15-20 hours a week during a 2-3 month period. Another issue is that there are very few FTC and FRC teams out there, so you may have to look for a team outside your school and your immediate community. </p>
<p><b>Deciding questions:</b></p>
<ul class="disc16l1">
<li>Are you willing to commit to FTC or FRC as your only extracurricular activity during their season, spending about 15-20 hrs/week?</li>
<li>Are you able to find an FTC or FRC team to join?</li>
</ul>

<div class="section50left"> 
<h4> Yes to both </h4>
<p><b>Definitely go for <a href="#ftc">FTC</a> or <a href="#frc">FRC:</a></b> These are intense but very rewarding experiences. You will thoroughly enjoy them, learn a lot along the way and make lasting friendships.</p>
</div>
<div class="section50right"> 
<h4>Ummm... not sure</h4>
<p><b><a href="#robofest">Do Robofest:</a></b> Robofest will let you enjoy robotics with lesser commitment, say about 5-15 hrs/week. You can decide how many challenges to participate in, depending on your interest level and other activities.</p>
</div>
</section50short>
<br>

<div id="list"></div>
<section50short> 
<div class="tabcenter">
  <h2>Popular Robotics Competitions</h2>
</div>
<br>
<p>There are a wide variety of Robotics competitions out there. We’ve compiled the most fun and prestigious ones below.</p>
</section50short>

{% for comp in site.robocomp %}  
<section50> 
  <h2 id="{{ comp.hash }}"> <a href=" {{ comp.toplink }} " target="_blank">{{ comp.heading }} </a> </h2>

  <!-- Use capture to prevent outputting i -->
  {% capture _%}{% increment i %}{% endcapture %}
  {% assign mod = i | modulo:2 %}

  <!-- For even loop runs, put pic to left. Switch for odd -->
  {% if mod == 0 %}
  <div class="section50right">
  {% else %}
  <div class="section50left">
  {% endif %}

        <iframe src="{{ comp.video }}" scrolling="no" allowfullscreen="" width="450" height="250" frameborder="0"><br/></iframe>
  </div>

  {% if mod == 0 %}
  <div class="section50left">
  {% else %}
  <div class="section50right">
  {% endif %}
    <ul class="compl1">
    <li><b>Grades:</b> {{ comp.grades }} </li>
    <li><b>Team Size:</b> {{ comp.teamsize }} </li>
    <li>You need:
    <ul class="compl2">
      {{ comp.content }} 
    </ul> </li> </ul>
  </div>

</section50>
<br>
{% endfor %}

<section50short>
  <div class="note" style="height:70px;">
    <h3 style="line-height:1; ">Science and Engineering Fair</h3>
    <p style="text-align:center; ">You can present your original robotics or engineering device at your local <a href="/science/#isef" target="_blank">Science and Engineering Fair</a>.
    </p>
  </div>
</section50short>

<br>