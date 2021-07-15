---
layout: page
title:  "Caja de herramientas"
permalink: /caja-de-herramientas/
---

<div class="posts">
  {% for post in site.posts %}
  {% if post.visible== 1 %}

  <div class="post">
    <h1>
      <a href="{{ post.url }}">
        {{ post.title }}      </a>
    </h1>
  <span class="post-date">{{ post.date | date_to_string }}</span>
        <a class="subtitle" href="{{ post.url }}"></a>
  {%- if post.author -%}
    • <span class="post.author"> {{ post.author }}
  </span>
    {% endif %}
      
  </div>
  {% endif %}
  {% endfor %}
</div>