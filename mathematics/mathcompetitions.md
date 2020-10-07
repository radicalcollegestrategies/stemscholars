---
layout: default
title: Mathematics
permalink: /mathematics/mathcompetitions
h1: Mathematics
h2: Competitions
---

<section50short style="height: 75px; padding-bottom:10px">
  <div class="tabactive">
    <h2><a href="/stem/mathematics">Mathematics</a></h2>
  </div>
  <div class="tabinactive">
    <h2>Math Competitions</h2>
  </div>
</section50short>

<section50> 
<h2>Why should you participate in Math Competitions?</h2>
<!--img class="section50left" src="/images/engg/EmanueleRobot.jpg"-->
<div class="section50left"><br><br><br><h3>TODO: Add Pic</h3></div>

<div class="section50right">
  <ul class="yes">
    <li>Math Competitions give you a syllabus of fun new math concepts to learn in a given timeframe</li>
    <li>The competitions help you build your thinking and problem-solving skills</li>
    <li>Some competition topics like combinatorics are not covered in depth in school, but are needed for a good Math foundation</li>
    <li>As a bonus, if you do well, you get to brag about it to your friends and in your college applications!</li>
  </ul>
 </div>
</section50>

<section50short> 
<h2>Registering for the competitions</h2>
<div style="text-align:left">
  <ul class="disc16l1"> Different Math Competitions follow different formats:
    <li>Some let you register as an individual, e.g. Math Kangaroo. All you have to do is find a Test Center that is holding the competition. This is useful if your school doesn't have a Math Club or Team. </li>
    <li>Some require that you register through the school, but are flexible about the location or proctoring, e.g. MOEMS. So if your school doesn't have a Math Club, you can form a team with some friends, and convince one of the parents to be the proctor.</li>
    <li>Some have strict requirements that the school should register the team and the school teacher should proctor, e.g., Math League. For such competitions, you will need to convince a school teacher to hold the competition.</li>
    <li>Some competitions allow private institutions to register a team, e.g, HMMT. If your school doesn't have a Math Team, you can join a local Math Circle (e.g., Stanford Math Circle) or a private Math institute, and participate in a team through them.</li>
  </ul>
</div>
</section50short>

{% for comp in site.mathcomp %}  
<section50short> 
  <h2> <a href=" {{ comp.toplink }} " target="_blank">{{ comp.heading }} </a> </h2>

  <div class="section50left">
    <ul class="compl1">
    <li><b>Grades:</b> {{ comp.grades }} </li>
    <li><b>Enrollment:</b> {{ comp.enrollment }} </li>
    <li><b>Format:</b> {{ comp.format }} </li>
    <li><b>Approx Cost:</b> {{ comp.cost }} </li>
    <li><b><a href=" {{ comp.details }} " target="_blank">Important details</a>:</b> Dates, grades, etc</li>
    <li><b><a href=" {{ comp.prep }} " target="_blank">How to prepare</a></b></li>
    </ul>
  </div>

  <div class="section50right">
    <ul class="compl1">
    <li><b>Good to know:</b>
    <ul class="compl2">
      {{ comp.content }} 
    </ul> </li>
    </ul>
  </div>

</section50short>
<br><br>
{% endfor %}

<section50short>
<h2>More competitions for Middle and High Schools</h2>
<img class="center" src="/images/ComingSoon.png" style="width:600px; padding-bottom:50px;">
</section50short>

<section50>
  <h2>Our Recommendations</h2>
  <img class="center" src="/images/ComingSoon.png" style="width:600px; padding-top:50px;">

</section50>