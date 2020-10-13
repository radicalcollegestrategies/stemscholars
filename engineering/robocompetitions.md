---
layout: default
title: Robotics Competitions
permalink: /engineering/robocompetitions/
h1: Robotics Competitions
h2: Engineering
---
<section50short style="height: 75px; padding-bottom:10px">
  <div class="tabinactive">
    <h2><a href="/engineering/robotics">Robotics</a></h2>
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
<section50short>
<p>There are a wide variety of robotics competitions out there. We’ve compiled the most fun and prestigious ones below. </p>
</section50short>

<br>

{% for comp in site.robocomp %}  
<section50> 
  <h2> <a href=" {{ comp.toplink }} " target="_blank">{{ comp.heading }} </a> </h2>

  <!-- Use capture to prevent outputting i -->
  {% capture _%}{% increment i %}{% endcapture %}
  {% assign mod = i | modulo:2 %}

  <!-- For even loop runs, put pic to left. Switch for odd -->
  {% if mod == 0 %}

    <div class="section50left">
        <iframe src="{{ comp.video }}" scrolling="no" allowfullscreen="" width="450" height="250" frameborder="0"><br/></iframe>
    <h3>Video Demo</h3>
    </div>

    <div class="section50right">
    <ul class="compl1">
    <li><b>Grades:</b> {{ comp.grades }} </li>
    <li><b>Team Size:</b> {{ comp.teamsize }} </li>
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
    <li>You need
    <ul class="compl2">
      {{ comp.content }} 
    </ul> </li> </ul>
    </div>

    <div class="section50right">
        <iframe src="{{ comp.video }}" scrolling="no" allowfullscreen="" width="450" height="250" frameborder="0"><br/></iframe>
    <h3>Video Demo</h3>
    </div>

  {% endif %}

</section50>
<br>
{% endfor %}

<section50 style="min-height: 200px;">
  <h2>Our Recommendations</h2>

  <div class="section50left">
  <img style="width:200px" src="/images/stem/Maze.png">
  <div class="license">
   <a href="https://www.wannapik.com/vectors/5479" target="_blank">Image</a>
      <a href="https://creativecommons.org/licenses/by/3.0/" target="_blank">licensed</a> from Wannapik Studio
  </div>
  </div>
  <div class="section50right">
    <ul class="disc" style="padding-left:40px"> 
    <li>Are you lost in a maze of choices?</li>
    <li>No worries! We'll help you navigate</li>
    <li>Try the recommendations below to decide which competitions are right for <i>you</i></li>
    </ul>
  </div>
</section50>

<section50short> 
<h3>Step 1: Elementary School</h3>
<p><b><a href="https://wwww.amazon.com/Wonder-Workshop-Dash-Activated-Programming/dp/B00SKURVKY" target="_blank">Buy Dash Robot:</a></b> For elementary school students, we recommend the Dash robot by Wonder Workshop. You can get started with it very quickly, with no prior technical expertise. And remember to get together a team of your friends to participate in the <a href="https://www.makewonder.com/classroom/robotics-competition/" target="_blank">Wonder League Robotics Competition</a> because it’s a lot more fun that way! </p>

<h3>Step 2: Around Grades 4-6</h3>
<p> Once you outgrow the Dash robot, or if you skipped it altogether, you have a choice to make. </p>
<p><b>Deciding question:</b> Do you have a parent or another mentor who is an expert in tech <i>and</i> can spend at least 3 hrs every week for several months coaching your team? </p>

<div class="section50left"> 
<h4>I have a mentor</h4>
<p> Buy the <a href="https://education.lego.com/en-us/products/lego-mindstorms-education-ev3-homeschool-combo-pack/5003480" target="_blank">Lego EV3 robot</a> and move onto Step 3</p>
</div>

<div class="section50right"> 
<h4> I do not have a mentor </h4>
<p> Continue your robotics journey with <a href="https://www.amazon.com/Wonder-Workshop-QU01-13-Cue-Robot/dp/B078XXPDVV/" target="_blank">Cue Robot</a>, and participate in the <a href="https://www.makewonder.com/classroom/robotics-competition/" target="_blank">Wonder League Robotics Competition</a> </p>
</div>
</section50short> 

<section50 style="padding-top:125px"> 
<h3>Step 3: You are in grades 4-8 with the Lego EV3 robot</h3>
<p>First collect a team of your friends who will participate in a robotics competition with you. Now you need to decide which competition to prepare for. </p>
<p><b>Deciding question:</b> How many hours a week are you and your team willing to commit to robotics?</p>

<div class="section50left"> 
<h4> 10 or more hours/week </h4>
<p> <b>Do FLL:</b> FLL is an intense competition with a lot of missions, along with a science project on the side. So the time commitment is equivalent to that of a competitive soccer team. It’s also a lot of fun because the mat is very colorful and the LEGO missions are kinda … cute.</p>
<p>Your team should be willing to commit to FLL being their only (or main) extracurricular activity during August-November (and beyond, if you qualify for the next level). </p>
</div>

<div class="section50right"> 
<h4> About 3-8 hours/week </h4>
<p> <b>Do robofest:</b> Robofest is purely a robotics competition with easy setup where you can participate in one or more challenges.</p>
<p>You can decide how many challenges to participate in, depending on your interest level and other activities.</p>
</div>
</section50>
<br>

<section50short>
<h3>High School</h3>
<p>All the FIRST competitions like FTC and FRC are intense and require a lot of time commitment. For example, during the build season for FRC, you may be working on your robot for about 15-20 hours a week during a 2-3 month period. Another issue is that there are very few FTC and FRC teams out there, so you may have to look for a team outside your school and your immediate community. </p>
<p><b>Deciding questions:</b></p>
<ul class="disc16l1">
<li>Are you willing to commit to FTC or FRC as your only extracurricular activity during their season, spending about 15-20 hrs/week?</li>
<li>Are you able to find an FTC or FRC team to join?</li>
</ul>

<div class="section50left"> 
<h4> Yes to both </h4>
<p><b>Definitely go for FTC or FRC:</b> These are intense but very rewarding experiences. You will thoroughly enjoy them, learn a lot along the way and make lasting friendships.</p>
</div>
<div class="section50right"> 
<h4>Ummm... not sure</h4>
<p><b>Do Robofest:</b> Robofest will let you enjoy robotics with lesser commitment, say about 5-15 hrs/week. You can decide how many challenges to participate in, depending on your interest level and other activities.</p>
</div>
<br>
</section50short>