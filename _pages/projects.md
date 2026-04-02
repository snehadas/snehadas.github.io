---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

{% for post in site.projects %}
  <div class="list__item" style="margin-bottom: 2em;">
    <article class="archive__item" itemscope itemtype="https://schema.org/CreativeWork">
      <h2 class="archive__item-title" itemprop="headline">
        <a href="{{ base_path }}{{ post.url }}" rel="permalink">{{ post.title }}</a>
      </h2>

      {% if post.excerpt %}
        <p class="archive__item-excerpt" itemprop="description">{{ post.excerpt }}</p>
      {% endif %}

      {% if post.team %}
        <p style="font-size: 0.9em; color: #5a5a5a;">
          <strong>Team:</strong> <i>{{ post.team }}</i>
        </p>
      {% endif %}
    </article>
  </div>
{% endfor %}
