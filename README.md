# Gusman
---
layout: default
---

<div class="home">
  <div class="hero">
    <div class="avatar">
      <img src="{{ site.avatar }}" alt="Avatar de {{ site.author }}">
    </div>
    <div class="description">
      <h1>{{ site.title }}</h1>
      <p>{{ site.description }}</p>
    </div>
  </div>

  <div class="recent-posts">
    <h2>Entradas recientes</h2>
    <ul>
      {% for post in site.posts limit: 5 %}
        <li>
          <a href="{{ post.url }}">{{ post.title }}</a>
          <span class="post-date">{{ post.date | date_to_string }}</span>
        </li>
      {% endfor %}
    </ul>
  </div>
</div>
