---
layout: default
permalink: /science/
title: Science
h2: Physics, Chemistry and Biology
---

<section50short>
  <div class="note">
    <p style="text-align:center; padding-top:13px">If you enjoy Science, you're likely to love Engineering. Engineering is a natural extension of Science, <br>and includes activities like electronics and robotics. Explore <a href="/engineering/" target="_blank">our Engineering page</a> for more.</p>
  </div>
</section50short>

<section50short> 
<h2>Science in Elementary and Middle School</h2>
<p style="text-align:center"><a href="#midhigh">Jump to: Science in Middle and High School</a></p>
<p>This section has books and videos with loads of fun science topics! You can read and watch these with your child and discuss them afterwards. We also have websites that teach science through fun games and simulations, or contain science experiments you can do at home. Check them out below!</p>
</section50short>

{% for comp in site.scielem %}  
<section50> 
  <h2> <a href=" {{ comp.toplink }} " target="_blank">{{ comp.heading }} </a> </h2>

  <!-- Use capture to prevent outputting i -->
  {% capture _%}{% increment i %}{% endcapture %}
  {% assign mod = i | modulo:2 %}

  <!-- For even loop runs, put pic to left. Switch for odd -->
  {% if mod == 0 %}
    <div class="section50left">
  {% else %}
    <div class="section50right">
  {% endif %}

      {% if comp.video %}
        <iframe src="{{ comp.video }}" scrolling="no" allowfullscreen="" width="450" height="250" frameborder="0"><br/></iframe>
      {% else %}
        <a href=" {{ comp.toplink }} " target="_blank">
        <img src="{{ comp.pic }}"> </a>
      {% endif %}
    </div>

  {% if mod == 0 %}
    <div class="section50right">
  {% else %}
    <div class="section50left">
  {% endif %}
    <ul class="compl1">
    <li><b>Grades:</b> {{ comp.grades }} </li>
    <li> {{ comp.description }} </li>
    <br>
    <li>Details:
    <ul class="compl2">
      {{ comp.content }} 
    </ul> </li> </ul>
    </div>

</section50>
<br>
{% endfor %}

<hr id="midhigh">
<section50short> 
<h2>Science in Middle and High School</h2>
<p>Explore fun hands-on experiments below! To take your passion in science to the next level, compete in the <a href="#scibowl">Science Bowl</a> if you enjoy the breadth of science, or participate in the <a href="#isef">Science and Engineering Fair</a> if you want to dive deep into a research topic.</p>
</section50short>

{% for comp in site.scimid %}  
<section50> 
  <h2 id="{{ comp.hash }}"> <a href=" {{ comp.toplink }} " target="_blank">{{ comp.heading }} </a> </h2>

  <!-- Use capture to prevent outputting i -->
  {% capture _%}{% increment i %}{% endcapture %}
  {% assign mod = i | modulo:2 %}

  <!-- For even loop runs, put pic to left. Switch for odd -->
  {% if mod == 0 %}
    <div class="section50left">
  {% else %}
    <div class="section50right">
  {% endif %}

      {% if comp.video %}
        <iframe src="{{ comp.video }}" scrolling="no" allowfullscreen="" width="450" height="250" frameborder="0"><br/></iframe>
      {% else %}
        <a href=" {{ comp.toplink }} " target="_blank">
        <img src="{{ comp.pic }}"></a>
      {% endif %}
      {% if comp.piccreator %}
        <div class="license">(
        <a href="{{ comp.piclink }}" target="_blank">Image</a>
        <a href="{{ comp.piclicense }}" target="_blank">licensed</a> from {{ comp.piccreator }}
        )</div>
      {% endif %}

    </div>

  {% if mod == 0 %}
    <div class="section50right">
  {% else %}
    <div class="section50left">
  {% endif %}
    <ul class="compl1">
    <li><b>Grades:</b> {{ comp.grades }} </li>
    <li> {{ comp.description }} </li>
    <br>
    <li>Details:
    <ul class="compl2">
      {{ comp.content }} 
    </ul> </li> </ul>
    </div>

</section50>
<br>
{% endfor %}
