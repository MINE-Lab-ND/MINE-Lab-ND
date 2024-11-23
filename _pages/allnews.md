---
title: "News"
layout: textlay
excerpt: "MINE Lab at University of Notre Dame."
sitemap: false
permalink: /allnews.html
---

# News

<div class="news-container">
  {% for article in site.data.news %}
    <div class="news-item">
      <span class="news-date">{{ article.date }}</span>
      <div class="news-headline">{{ article.headline | markdownify }}</div>
    </div>
  {% endfor %}
</div>
