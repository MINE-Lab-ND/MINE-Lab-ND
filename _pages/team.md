---
title: "MINE Lab - Team"
layout: gridlay
excerpt: "MINE Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

<div style="text-align: center; margin: 40px auto; max-width: 800px; font-family: Arial, sans-serif;">
  <!-- Title -->
  <h2 style="text-align: center; padding-top: 30px;">Principal Investigator</h2>

  <!-- Profile Image and Social Links -->
  <div style="margin-bottom: 20px;">
    <div class="image-cropper" style="display: inline-block; margin-bottom: 10px;">
      <img src="https://raw.githubusercontent.com/MINE-Lab-ND/MINE-Lab-ND.github.io/refs/heads/gh-pages/images/xzhang.jpg"
           alt="Xiangliang Zhang" 
           style="width: 200px; height: 200px; object-fit: cover; border-radius: 100%; border: 4px solid #ddd;">
    </div>
    <div style="margin-top: 10px;">
      <a href="mailto:xzhang33y@nd.edu" style="text-decoration: none;">
        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" style="margin-right: 5px; margin-left: 5px;" fill="currentColor" class="bi bi-envelope-fill" viewBox="0 0 16 16">
          <path d="M.05 3.555A2 2 0 0 1 2 2h12a2 2 0 0 1 1.95 1.555L8 8.414zM0 4.697v7.104l5.803-3.558zM6.761 8.83l-6.57 4.027A2 2 0 0 0 2 14h12a2 2 0 0 0 1.808-1.144l-6.57-4.027L8 9.586zm3.436-.586L16 11.801V4.697z"/>
        </svg>
      </a>
      <a href="https://www.linkedin.com/in/connorcoley/" style="text-decoration: none;">
        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" style="margin-right: 5px; margin-left: 5px;" fill="currentColor" class="bi bi-linkedin" viewBox="0 0 16 16">
          <path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854zm4.943 12.248V6.169H2.542v7.225zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248S2.4 3.226 2.4 3.934c0 .694.521 1.248 1.327 1.248zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016l.016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225z"/>
        </svg>
      </a>
    </div>
  </div>

  <!-- Name and Title -->
  <h4><b>Xiangliang Zhang</b></h4>
  <i>
    Associate Professor (Without Tenure) <br>
    Class of 1957 Career Development Professor <br>
    Department of Chemical Engineering <br>
    Department of Electrical Engineering and Computer Science <br>
  </i>

  <!-- Description -->
  <p style="text-align: justify; line-height: 1.6; font-size: 1em; margin-top: 20px;">
    Xiangliang Zhang is the Class of 1957 Career Development Professor and an Associate Professor without tenure at MIT 
    in the Department of Chemical Engineering and the Department of Electrical Engineering and Computer Science. 
    He received his B.S. and Ph.D. in Chemical Engineering from Caltech and MIT, respectively, and did his postdoctoral 
    training at the Broad Institute. His research group at MIT works at the interface of chemistry and data science to 
    develop models that understand how molecules behave, interact, and react and use that knowledge to engineer new ones, 
    with an emphasis on therapeutic discovery.
  </p>
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
<img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" 
     class="img-responsive" 
     style="width: 150px; height: 150px; float: left;" />
     
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
<img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" 
     class="img-responsive" 
     style="width: 150px; height: 150px; float: left;" />

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
