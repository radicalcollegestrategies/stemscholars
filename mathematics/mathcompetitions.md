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
    <li>Some have strict requirements that the school should register the team and the school teacher should proctor, e.g., Math League. This works great by providing you a ready-made team if your school has an after-school Math program. If it doesn't, then you will need to convince a school teacher to hold the competition.</li>
    <li>Some competitions allow private institutions to register a team, e.g, HMMT. If your school doesn't have a Math Team, you can join a <a href="https://mathcircles.org/find-a-math-circle/" target="_blank">local Math Circle</a> or a private Math institute, and participate in a team through them.</li>
  </ul>
</div>
</section50short>

<section50short> 
<h2>Preparing for the competitions</h2>
<div style="text-align:left">
<p>If you just show up for any Math Competition without much preparation, quite likely you won't perform well. It takes months of preparation to do well in elementary school competitions, and sometimes years of preparation to do well in middle and high school competition. The secret to success is to make this a designated extra-curricular activity where you dedicate some time every week to prepare. If it's hard to motivate yourself to study, form a study-group of like-minded friends and meet regularly.
</p>
<p>More tips:</p>
  <ul class="disc16l1">
    <li>Several competitions in the same age group will typically have similar syllabus. The textbooks we mention for each competition will typically prepare you for many competitions simultaneously.</li>
    <li>Try to find a local middle school student to coach an elementary school team, and a local high school student to coach a middle school team. This is a win-win because the coach develops leadership skills and/or earns volunteer hours while the students benefit from the coach's expertise. Ask neighbors or try nextdoor.com for finding interested coaches.</li>
    <li>High school students can self-prepare using the material listed. If you are serious about the competitions, then it may be a good idea to join a <a href="https://mathcircles.org/find-a-math-circle/" target="_blank">local Math Circle</a> or a private Math institute. This will put you in touch with like-minded people, boost up your motivation level, and you will be able to register for team-competitions through the institute. Specifically, <a href="https://artofproblemsolving.com/" target="_blank">Art of Problem Solving</a> has several classes for all levels of Math Competitions.</li>
    <li> There are YouTube channels targetting various competitions. This may work well for you especially if you don't have a coach.</li>
    <li>In the weeks leading up to the competition, do several practice problems/exams for that specific competition.</li>
  </ul>
<p>There are a wide variety of Math competitions out there. We’ve compiled the most fun and prestigious ones below. </p>
</div>
</section50short>

{% for comp in site.mathcomp %}  
<section50 style="min-height: 150px;"> 
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

</section50>
<br><br>
{% endfor %}

<section50short>
<h2>More competitions for Middle and High Schools</h2>
<img class="center" src="/images/ComingSoon.png" style="width:400px; padding-bottom:50px;">
</section50short>

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

<section50> 
<h3>Upper Elementary School: Grades 4-6</h3>
<p>The idea of Math Competitions in Elementary School is to develop a love and habit for the deep thinking that goes into Math competitions. The goal is not to go win an international prize! Also little kids can only understand short timeframes, so it'as hard for them to practice for a competition that's 4 months away! For this reason, we recommend competitions that hold multiple contests in a year. This keep the kids engaged in the competition and keeps their motivation level high.</p>

<p><b>Deciding question:</b> Does your school offer MOEMS? (<u>or</u>) Can you <a href="#moems">persuade a school teacher to be the official PICO</a> for MOEMS?</p>

<div class="section50left"> 
<h4>Yes!</h4>
<p><b>Participate in MOEMS.</b> It is a prestigious competition, and is fun and challenging at the same time.</p>
<p>Optional: In addition to MOEMS, you can consider participate in Math Kangaroo, which has a single contest. The "syllabus" is the same, and it's a prestigious international competition.</p>
</div>

<div class="section50right"> 
<h4>No, I'm on my own</h4>
<p><b>Participate in CML</b> as a "Home School". It is a good alternative to MOEMS.</p>
<p>Optional: In addition to CML, you can consider participating in Math Kangaroo, which has a single contest. It is a prestigious international competition, and is slightly more challenging than CML, so may need extra preparation.</p>
</div>

</section50>

<section50>
<h3>Recommendations for for Middle and High Schools</h3>
  <img class="center" src="/images/ComingSoon.png" style="width:400px; padding-top:50px;">

</section50>