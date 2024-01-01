---
layout: page
title: "Films"
permalink: /films/
---

  <ul>
    {% assign sorted = site.films | sort: 'date' | reverse %}
    {% for item in sorted %}
      <a href="{{ item.url }}">
        <img class="filmCover" src="{{ site.url }}/assets/img/films/{{ item.slug }}.jpg" alt="{{ item.slug }}">
      </a>
    {% endfor %}
  </ul>
  
