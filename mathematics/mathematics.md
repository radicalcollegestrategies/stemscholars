---
layout: default
permalink: /mathematics/
title: Mathematics
h2: Problem Solving
---
<section50>
<h2>Math Beyond School : Problem Solving</h2>

  <div class="section50right">
    <img style="width:350px" src="/images/math/Rubix.png">
  </div>

  <div class="section50left">

    <p>If you love Math in school, and are reasonably good at it, then go deeper to hone your Problem Solving, Logical Reasoning and Critical Thinking skills. <i>Do not</i> waste your time doing busy work like pages and pages of long division! Do just enough practice problems in school math to make sure you don't make silly mistakes, and spend the rest of your time solving more fun and engaging problems! </p>

    <p>Problem Solving involves understanding the problem and finding a strategy to solve it. When you grow up, you may not use a lot of the actual math you learn in school in your daily lives or your career. However, the problem solving skills that you build while doing hard math problems will help you excel in many different fields.</p>

  </div>

</section50>
<section50short>
<p style="text-align:center">Build your problem solving skills in a variety of ways listed below.</p>
</section50short>

{% for comp in site.math %}  
<section50> 
  <h2>{{ comp.heading }}</h2>

  <!-- Use capture to prevent outputting i -->
  {% capture _%}{% increment i %}{% endcapture %}
  {% assign mod = i | modulo:2 %}

  <!-- For even loop runs, put pic to left. Switch for odd -->
  {% if mod == 0 %}
  <div class="section50right">
  {% else %}
  <div class="section50left">
  {% endif %}

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

  {% if mod == 0 %}
  <div class="section50left">
  {% else %}
  <div class="section50right">
  {% endif %}
    <ul class="compl1">
    <li> {{ comp.description }} </li>
    <br>
    <li><b>Grades:</b> {{ comp.grades }} </li>
    <li>Resources:
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
    <p style="text-align:center; ">You can present your original math research at your local <a href="/science/#isef" target="_blank">Science and Engineering Fair</a>.
    </p>
  </div>
</section50short>

<br>

<!--section50>
<h2>Accelerating in school curriculum</h2>
<p>If you are fantastic at math, you can accelerate through the Math Curriculum to cover: </p>
    <ul class="disc16l1" style="padding-left:40px"> 
    <li>Middle School: Algebra, Geometry and maybe Algebra-2</li>
    <li>High School: Pre-Calculus, AP Calculus BC, AP Statistics, and even Multivariable Calculus or Linear Algebra (if your school offers them)</li>
    </ul>
 <p>We do not recommend accelerating any more than the roadmap laid out above because:</p>
    <ul class="disc16l1" style="padding-left:40px"> 
    <li>Many colleges only ask for classes/GPA for Grades 10 and up, so don't "waste" an AP class by taking it in 9th grade</li>
    <li>The roadmap outlined above is sufficient for most popular math competitions</li>
    <li>If you are hungry for more math, we recommend that you go into the depth by exploring the Competition / Research aspect of it, instead of going through the subject faster.</li>
    </ul>

<p> Work with your school counselor on how to take online classes if you want to accelerate through your Math Curriculum at school. Several schools recognize courses offered by <a href="https://www.byu.edu/" target="_blank">BYU</a>, <a href="https://svhs.co/" target="_blank">SVHS</a> or <a href="https://www.ucscout.org/" target="_blank">UC Scout</a>, but each school may be different.</p>
<p>Remember, if your school won't accept an online course, then it's a waste of time because you'll just have to repeat the whole subject in school. For that reason, while Khan Academy is great for reviewing any topics that were not covered (well) in school, it's probably not the best way to do complete courses that are already offered in school.</p> 
</section50-->
<br>