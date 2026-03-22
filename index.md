---
layout: default
---

{% for post in site.posts %}
  <article style="margin-bottom: 60px;">

    <p style="color: #888; font-size: 13px; margin-bottom: 5px;">
      {{ post.date | date: "%B %d, %Y" }}
    </p>

    <h2 style="margin-bottom: 10px;">
      <a href="{{ post.url }}">{{ post.title }}</a>
    </h2>

    <div>
      {{ post.content }}
    </div>

  </article>
{% endfor %}
