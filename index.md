---
layout: default
---

{% for post in site.posts %}
  <article style="margin-bottom: 60px;">
    <h2>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </h2>
    <div>
      {{ post.content }}
    </div>
  </article>
{% endfor %}
