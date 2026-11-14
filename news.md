---
layout: default
permalink: /news/
title: "News & updates"
description: "News and updates from the AS²ERT Lab at UT Dallas."
---

{% include page-head.html eyebrow="AS²ERT Lab" title="News &amp; updates" %}

<div class="wrap">
  <div class="page-body news-page">
    {% assign groups = site.data.news | group_by: "year" %}
    {% for group in groups %}
    <section class="year-block" id="{{ group.name }}">
      <h2 class="year-label">{{ group.name }}</h2>
      <ul class="news-list">
        {% for item in group.items %}
        <li class="news-item">
          <span class="news-date">{{ item.date }}</span>
          <span class="news-text">{{ item.text }}</span>
        </li>
        {% endfor %}
      </ul>
    </section>
    {% endfor %}
  </div>
</div>
