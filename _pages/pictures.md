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

(Right-click *'view image'* to see a larger image.)
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>