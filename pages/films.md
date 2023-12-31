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
        <img class="filmCover" src="/assets/img/missingCover.jpg">
        {% else %}
        <img class="filmCover" src="/assets/img/thumb/{{ item.slug }}.jpg" alt="{{ item.film }}">
        {% endif %}
      </a>
    {% endfor %}
  </ul>
  
