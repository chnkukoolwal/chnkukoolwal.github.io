---
layout: default
---

{% for post in site.posts %}
  <article style="margin-bottom: 60px;">
    
    <p style="color: #666; font-size: 14px;">
      {{ post.date | date: "%B %d, %Y" }}
    </p>

    <h2>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </h2>

    <div>
      {{ post.content }}
    </div>

  </article>
{% endfor %}
