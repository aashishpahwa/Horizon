---
layout: default
title: Home
---

<section id="archive" class="k-archive">
  <div class="k-section-head">
    <p class="k-eyebrow"><span class="k-eyebrow-n">02</span><span class="k-eyebrow-rule"></span>Archive</p>
    <h2 class="h-section">Every briefing<br><span class="k-italic">so far.</span></h2>
  </div>

  {% assign en_posts = site.posts | where: "lang", "en" %}
  {% assign en_by_month = en_posts | group_by_exp: "post", "post.date | date: '%B %Y'" %}
  {% for month in en_by_month %}
  <div class="k-month">
    <h3 class="k-month-name"><span class="k-month-n">/{{ forloop.index | prepend: "0" | slice: -2, 2 }}</span>{{ month.name }}</h3>
    <ul class="k-days">
      {% for post in month.items %}
      <li><a href="{{ post.url | relative_url }}">
        <span class="k-day-num">{{ post.date | date: "%d" }}</span>
        <span class="k-day-name">{{ post.date | date: "%A" }}</span>
        <span class="k-day-arrow" aria-hidden="true">→</span>
      </a></li>
      {% endfor %}
    </ul>
  </div>
  {% else %}
  <p class="k-muted">No briefings yet.</p>
  {% endfor %}
</section>
