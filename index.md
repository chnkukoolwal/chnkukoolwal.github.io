---
layout: default
---

<div style="margin-bottom: 50px;">

  <h1 style="margin-bottom: 5px;">Chinku Koolwal</h1>

  <p style="margin: 0; font-size: 16px; color: #444;">
    Startup Advisor & Venture Scout
  </p>

  <p style="margin: 5px 0 0 0; font-size: 14px; color: #777;">
    @chnkukoolwal
  </p>

</div>

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
