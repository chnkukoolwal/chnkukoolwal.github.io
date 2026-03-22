---
layout: default
---

<h1 style="margin-bottom: 40px;">Chinku Koolwal</h1>

{% for post in site.posts %}
  <article style="margin-bottom: 80px;">

    <p style="color: #888; font-size: 13px; margin-bottom: 8px;">
      {{ post.date | date: "%B %d, %Y" }}
    </p>

    <h2 style="margin-bottom: 15px;">
      <a href="{{ post.url }}">{{ post.title }}</a>
    </h2>

    <div style="line-height: 1.7;">
      {{ post.content }}
    </div>

  </article>
{% endfor %}
