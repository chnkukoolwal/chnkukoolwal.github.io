---
layout: default
---

<div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 40px; border-bottom: 1px solid #e0e0e0; padding-bottom: 25px; gap: 20px; flex-wrap: wrap;">

  <!-- Left side: name, social links, handle -->
  <div style="flex: 1; min-width: 250px;">
    <h1 style="margin: 0 0 10px 0; font-size: 32px; font-weight: 600; line-height: 1.4;">
      Chinku Koolwal
    </h1>

    <p style="margin: 0 0 10px 0; font-size: 16px; color: #555; font-weight: 400; line-height: 1.4; font-style: italic;">
      Startup Advisor & Venture Scout
    </p>

    <!-- Social links -->
    <p style="margin: 0 0 10px 0; font-size: 14px; color: #555; line-height: 1.4;">
      <a href="https://www.linkedin.com/in/chnkukoolwal/" style="color: inherit; text-decoration: none;">LinkedIn</a> •
      <a href="https://x.com/chnkukoolwal" style="color: inherit; text-decoration: none;">X</a> •
      <a href="https://chnkukoolwal.medium.com/" style="color: inherit; text-decoration: none;">Medium</a> •
      <a href="https://substack.com/@chnkukoolwal" style="color: inherit; text-decoration: none;">Substack</a>
    </p>

    <p style="margin: 0; font-size: 14px; color: #888; line-height: 1.4;">
      <a href="https://linktr.ee/chnkukoolwal" style="color: inherit; text-decoration: none;">@chnkukoolwal</a>
    </p>
  </div>

  <!-- Right side: subscribe box -->
  <div id="subscribe" style="flex-shrink: 0; max-width: 300px; border: 1px solid #e0e0e0; border-radius: 6px; padding: 20px; background: #fafafa;">
    <h3 style="margin-bottom: 10px; font-weight: 600;">Subscribe to my updates</h3>
    <p style="margin-bottom: 15px; color: #555; font-size: 14px;">
      Get weekly updates on startups, fundraising, and the venture ecosystem directly to your inbox.
    </p>

    <form action="YOUR_EMAIL_PROVIDER_FORM_URL" method="post" style="display: flex; flex-wrap: wrap; gap: 10px;">
      <input type="email" name="email" placeholder="Your email" required
        style="flex: 1; padding: 8px 10px; font-size: 14px; border: 1px solid #ccc; border-radius: 4px;">
      <button type="submit"
        style="padding: 8px 15px; font-size: 14px; background: #111; color: #fff; border: none; border-radius: 4px; cursor: pointer;">
        Subscribe
      </button>
    </form>
  </div>

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
