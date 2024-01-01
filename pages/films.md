---
layout: page
title: "Films"
permalink: /films/
---

  <ul>
    {% assign sorted = site.films | sort: 'date' | reverse %}
    {% for item in sorted %}
      <a href="{{ item.url }}">
        {% if item.image %}
        <img class="filmCover" src="{{ site.url }}/assets/img/films/{{ item.slug }}.jpg" alt="{{ item.slug }}">
        {% else %}
        <img class="filmCover" src="{{ site.url }}/assets/img/missingCover.jpg">
        {% endif %}
      </a>
    {% endfor %}
  </ul>
  
