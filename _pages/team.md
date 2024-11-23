---
title: "MINE Lab - Team"
layout: gridlay
excerpt: "MINE Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

<!-- Jump to [staff](#staff), [master and bachelor students](#master-and-bachelor-students), [alumni](#alumni), [administrative support](#administrative-support), [lab visitors](#lab-visitors). -->

<div style="text-align: center; margin: 40px auto; max-width: 800px; font-family: Arial, sans-serif;">
  <!-- Title -->
  <h1 style="font-size: 2em; font-weight: bold; margin-bottom: 20px;">Principal Investigator</h1>

  <!-- Profile Image -->
  <div style="margin-bottom: 20px;">
    <img src="path/to/image.jpg" alt="Xiangliang Zhang" style="width: 150px; height: 150px; object-fit: cover; border-radius: 50%; border: 4px solid #ddd;">
  </div>

  <!-- Name and Title -->
  <h2 style="font-size: 1.8em; font-weight: bold; margin-bottom: 10px;">Xiangliang Zhang</h2>
  <p style="font-size: 1.1em; margin: 5px 0;"> Leonard C. Bettex Collegiate Professor</p>
  <p style="font-size: 1.1em; margin: 5px 0;">Department of Computer Science and Engineering</p>

  <!-- Social Links -->
  <div style="margin: 20px 0;">
    <a href="mailto:example@domain.com" style="text-decoration: none; margin-right: 15px;">
      <img src="path/to/email-icon.png" alt="Email" style="width: 24px; height: 24px;">
    </a>
    <a href="https://linkedin.com/in/connorwcoley" style="text-decoration: none;">
      <img src="path/to/linkedin-icon.png" alt="LinkedIn" style="width: 24px; height: 24px;">
    </a>
  </div>

  <!-- Description -->
  <div style="text-align: justify; line-height: 1.6; font-size: 1em; margin-top: 20px;">
    <p>
      Connor W. Coley is the Class of 1957 Career Development Professor and an Associate Professor without tenure at MIT 
      in the Department of Chemical Engineering and the Department of Electrical Engineering and Computer Science. 
      He received his B.S. and Ph.D. in Chemical Engineering from Caltech and MIT, respectively, and did his postdoctoral 
      training at the Broad Institute. His research group at MIT works at the interface of chemistry and data science to 
      develop models that understand how molecules behave, interact, and react and use that knowledge to engineer new ones, 
      with an emphasis on therapeutic discovery.
    </p>
    <p>
      Connor is a recipient of C&EN’s “Talented Twelve” award, Forbes Magazine’s “30 Under 30” for Healthcare, Technology Review’s 
      35 Innovators Under 35, the NSF CAREER award, the ACS COMP OpenEye Outstanding Junior Faculty Award, the Bayer Early 
      Excellence in Science Award, the 3M NTFA, and was named a Schmidt AI2050 Early Career Fellow, a 2023 Samsung AI Researcher 
      of the Year, and a Scialog Fellow (Automating Chemical Laboratories). Connor has been recognized for his teaching and 
      mentorship by MIT’s inaugural Common Ground Award for Excellence in Teaching, the 2024 Outstanding UROP Mentor Award, 
      and the 2024 James W. Swan Outstanding Faculty Award for Graduate Teaching in Chemical Engineering.
    </p>
  </div>
</div>


<p>
  We invite open research collaborations! Undergraduate and Master's students are encouraged to send their CVs via <a href="mailto:minelab.nd.cs@gmail.com">email</a>. 
</p>


## PhD Student
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" class="img-responsive" width="50%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!-- <br>email: <{{ member.email }}></i> -->
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


## Alumni
{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


## Pets Scholars


{% assign number_printed = 0 %}
{% for member in site.data.alumni_pets %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" class="img-responsive" width="50%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!-- <br>email: <{{ member.email }}></i> -->
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}



## Former visitors, BSc/ MSc students

<div class="col-sm-4 clearfix">
<h4>Master students</h4>
{% for member in site.data.alumni_msc %}
{{ member.name }}
{% endfor %}
</div>

<div class="col-sm-4 clearfix">
<h4>Bachelor Students</h4>
{% for member in site.data.alumni_bsc %}
{{ member.name }}
{% endfor %}
</div>


<!-- ## Administrative Support
<a href="mailto:Rijsewijk@Physics.LeidenUniv.nl">Ellie van Rijsewijk</a> is helping us (and other groups) with administration. -->
