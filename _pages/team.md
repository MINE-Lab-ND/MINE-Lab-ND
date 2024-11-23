---
title: "MINE Lab - Team"
layout: gridlay
excerpt: "MINE Lab: Team members"
sitemap: false
permalink: /team/
---

<div style="position: absolute; top: 5px; left: 5px; max-width: 400px;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logo.png" alt="MINE Lab" style="width: 100%;">
</div>


   <pre style="white-space: pre-wrap;">
    
    

   </pre>



<div style="text-align: center; margin: 40px auto; max-width: 800px; font-family: Arial, sans-serif;">
  <h2 style="text-align: center; padding-top: 30px; font-family: Arial, sans-serif;">Principal Investigator</h2>

  <div class="image-cropper,style=margin-bottom: 20px; display: flex; justify-content: center; align-items: center;">
  <img class="person-pic" src="{{ site.url }}{{ site.baseurl }}/images/xzhang.jpg" alt="xiangliang zhang"/>
  </div>


  <!-- Name and Title -->
  <h4><b>Xiangliang Zhang</b></h4>
  <i>
    Leonard C. Bettex Collegiate Professor <br>
    Department of Computer Science and Engineering <br>
  </i>

  <!-- Description -->
  <p style="text-align: justify; line-height: 1.6; font-size: 1em; margin-top: 20px;">
    Dr. Zhang is a Leonard C. Bettex Collegiate Professor of Computer Science at University of Notre Dame, where she is leading a Machine Intelligence and kNowledge Engineering (MINE) group.
    Her research broadly addresses ways that enable ​computer machines to​ learn by the use of diverse types of data. Specifically, she is interested in designing machine learning algorithms for learning from complex and large-scale streaming data and graph data, with applications to recommendation systems, knowledge discovery, and natural language understanding. Her recent research notably advances the application of AI in scientific disciplines such as Chemistry, Biology, and Physics. More information can be found in the publications grouped by research problems, or the full list of over 200 peer-reviewed papers.
    She was invited to deliver an Early Career Spotlight talk at IJCAI-ECAI 2018. In 2009, she was awarded the European Research Consortium for Informatics and Mathematics (ERCIM) Alain Bensoussan Fellowship. She regularly serves on the Program Committee for premier conferences like SIGKDD (Area Chair, Senior PC), AAAI (Area Chair, Senior PC), IJCAI (Area Chair, Senior PC), etc. She also serves as Editor-in-Chief of ACM SIGKDD Explorations, associate editor for IEEE Transactions on Dependable and Secure Computing (TDSC), and Information Sciences.
    Prior to joining the University of Notre Dame, she was an Associate Professor in Computer Science at KAUST, Saudi Arabia. She completed her Ph.D. degree in computer science from INRIA-University Paris-Sud, France, in July 2010. She received her master and bachelor degrees from Xi’an Jiaotong University, China.
  </p>
</div>


<p>
  We invite open research collaborations! Check out our opening [here](https://mine-lab-nd.github.io/vacancies). 
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
