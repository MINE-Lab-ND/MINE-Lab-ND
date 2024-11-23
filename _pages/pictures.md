---
title: "MINE Lab - Pictures"
layout: textlay
excerpt: "MINE Lab -- Pictures"
permalink: /pictures/
---
<!-- Logo Section -->
<div class="logo-container" style="text-align: center; margin-top: 20px;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logo.png" 
       alt="MINE Lab" 
       style="max-width: 50%; height: auto; border: none;">
</div>

<!-- Spacer to Add Room Below the Logo -->
<div style="margin-top: 50px;"></div>

# Group Photos

{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 3 %} 

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/{{ pic.image }}" 
       class="img-responsive" 
       style="width: 100%; max-width: 100%; border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 3 %}
{% if even_odd == 1 %}
</div>
{% endif %}
{% if even_odd == 2 %}
</div>
{% endif %}

<p> &nbsp; </p>
