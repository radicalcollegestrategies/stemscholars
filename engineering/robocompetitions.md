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
You don’t have to shoot to win 1st place. Just enjoy the experience. </p>
 </div>
</section50>
<br>

<section50>
<h2>Robotics Competition Format</h2>

<div class="section50left">
<p>For any robotics competition, you will need a team. You can form a robotics team with your friends, or join a team and make new friends. What can be more fun than spending hours with them every week doing robotics together? </p>

<p>In the months prior to the competition date, teams build a robot and some attachments, then use the accompanying software to program it to complete a series of missions. During the competition, every team runs their robot, and the team with most points from the missions wins. </p>

<p>There are a wide variety of robotics competitions out there. We’ve compiled the most fun and prestigious ones below. </p>
</div>

<img class="section50right" src="/images/engg/EmanueleTeam.jpg">

</section50>

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

<section50>
  <h2>Our Recommendations</h2>

  <div class="section50left">
  <img style="width:300px" src="/images/stem/Maze.png">
  <div class="license">
   <a href="https://www.wannapik.com/vectors/5479" target="_blank">Image</a>
      <a href="https://creativecommons.org/licenses/by/3.0/" target="_blank">licensed</a> from Wannapik Studio
  </div>
  </div>
  <div class="section50right">
    <ul class="disc" style="padding-left:40px"> 
    <li>Lost in a maze of choices?</li>
    <li>No worries! We'll help you navigate</li>
    <li>Try the recommendations below to decide which competitions are right for <i>you</i></li>
    </ul>
  </div>
</section50>

<section50short> 
<h3>Elementary School</h3>
<p>For elementary school students, we recommend the <b>Dash</b> robot by Wonder Workshop. You can get started with it very quickly, with no prior technical expertise. And remember to get together a team of your friends because it’s a lot more fun that way! </p>

<h3>Middle School</h3>
<p> Once you outgrow the Dash robot, you have a choice to make. If you have a parent or another mentor who is an expert in tech <i>and</i> can spend about 3 hrs every week coaching your team, then go ahead and buy the Lego EV3 robot. If you have no mentors to guide you, then get the Wonder Workshop Cue Robot to continue your robotics journey. </p>

<p>If you buy the EV3 robot, then you need to decide which competition to prepare for. Robofest is purely a robotics competition with easy setup where you can participate in one or more challenges. FLL is an intense competition with a lot of missions, along with a science project on the side. So the time commitment is equivalent to that of a competitive soccer team. It’s also a lot of fun because the mat is very colorful and the LEGO missions are kinda … cute. </p>
<p> If your team is willing to commit to FLL being their only extracurricular activity during August-November (and beyond, if you qualify for the next level), which means spending 10-15 hrs on it per week, then go for it! If you want enjoy robotics with lesser commitment, say about 5 hrs/week, then stick with Robofest, where you can decide how many challenges to participate in, depending on your interest level and other activities.</p>

<h3>High School</h3>
<p>The recommendation for high school is similar to middle school. All the FIRST competitions like FTC and FRC are intense and require a lot of time commitment. For example, during the build season for FRC, you may be working on your robot for about 15-20 hours a week during a 2-3 month period. Another issue is that there are very few FTC and FRC teams out there, so you may have to look for a team outside your school, sometimes even ~10 miles away! </p>
<p>If you are able to find a team, and are willing to commit to FTC or FRC being their only extracurricular activity during their season, then go for it! If you want enjoy robotics with lesser commitment, say about 10 hrs/week, then stick with Robofest, where you can decide how many challenges to participate in, depending on your interest level and other activities.</p>
<br>
</section50short>