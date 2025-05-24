---
layout: about
title: My Poetry
permalink: /my-poetry/
published: false
---

# My Poetry

This page is under construction.

<div class="poetry-table-container">
  <div class="poem-list">
    {% assign sorted_poems = site.poems | sort: 'date' %}
    {% for poem in sorted_poems %}
      <div class="poem-item">
        <span class="poem-title"><a href="{{ poem.url }}">{{ poem.title }}</a></span>
        <span class="poem-date">{{ poem.date | date: "%B %d, %Y" }}</span>
      </div>
    {% endfor %}
  </div>
</div>

