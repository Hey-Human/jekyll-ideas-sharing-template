---
layout: default
title: "Inicio"
---

<main class="page-content" aria-label="Content">
    <div class="wrapper">
      <div class="home">
        <h2 class="post-list-heading">Publicaciones</h2>
        <ul class="post-list">
        {% for post in site.posts %}
          <li>
            <span class="post-meta">{{ post.date | date: "%d de %B, %Y" }}</span>
            <h3>
              <a class="post-link" href="{{ post.url | relative_url }}">
                {{ post.title }}
              </a>
            </h3>
          </li>
        {% endfor %}
        </ul>
        <p class="rss-subscribe">Suscríbete <a href="{{ "/feed.xml" | relative_url }}">vía RSS</a></p>
      </div>
    </div>
  </main>
