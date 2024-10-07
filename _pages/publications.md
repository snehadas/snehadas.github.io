---
layout: archive
title: "Publications of Sneha Das"
permalink: /publications/
author_profile: true
---

{% include base_path %}
{% if author.googlescholar %}
You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

Refereed Conference/Workshop Papers
---
<ol>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'conference' %}
  <li>    {% include archive-single.html %} </li>
  {% endif %}
{% endfor %}
</ol>

Journal Articles
---
<ol>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'journal' %}
     <li> {% include archive-single.html %} </li>
  {% endif %}
{% endfor %}
</ol>


Preprints/Under Review
---
<ol>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'preprint' %}
      <li> {% include archive-single.html %} </li>
  {% endif %}
{% endfor %}
</ol>

Monographs
---
<ol>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'thesis' %}
   <li>   {% include archive-single.html %} </li>
  {% endif %}
{% endfor %}
</ol>
