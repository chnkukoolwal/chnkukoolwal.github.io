---
layout: default
---

<div style="margin-bottom: 60px; border-bottom: 1px solid #e0e0e0; padding-bottom: 25px;">

  <h1 style="margin: 0; font-size: 32px; font-weight: 600; line-height: 1.2;">
    Chinku Koolwal
  </h1>

  <p style="margin: 5px 0 0 0; font-size: 16px; color: #555; font-weight: 400;">
    Startup Advisor & Venture Scout
  </p>

  <p style="margin: 5px 0 0 0; font-size: 14px; color: #888;">
    <a href="https://linktr.ee/chnkukoolwal" style="color: inherit; text-decoration: none;">
      @chnkukoolwal
    </a>
  </p>

</div>

{% for post in site.posts %}
  <article style="margin-bottom: 90px;">

    <p style="color: #888; font-size: 13px; margin-bottom: 8px;">
      {{ post.date | date: "%B %d, %Y" }}
    </p>

    <h2 style="margin-bottom: 15px;">
      <a href="{{ post.url }}" style="color: #111; text-decoration: none;">
        {{ post.title }}
      </a>
    </h2>

    <div style="line-height: 1.75; font-size: 16px; color: #111;">
      {{ post.content }}
    </div>

  </article>
{% endfor %}
