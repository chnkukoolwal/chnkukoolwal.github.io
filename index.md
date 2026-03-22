---
layout: default
---

<div style="display: flex; justify-content: space-between; align-items: flex-start; margin-bottom: 40px; border-bottom: 1px solid #e0e0e0; padding-bottom: 25px; gap: 20px; flex-wrap: wrap;">

  <!-- Left side: name, social icons, handle -->
  <div style="flex: 1; min-width: 250px;">
    <h1 style="margin: 0; font-size: 32px; font-weight: 600; line-height: 1.2;">
      Chinku Koolwal
    </h1>

    <p style="margin: 5px 0 10px 0; font-size: 16px; color: #555; font-weight: 400;">
      Startup Advisor & Venture Scout
    </p>

    <!-- Social icons -->
    <p style="margin: 5px 0 5px 0; font-size: 0;"> 
      <a href="https://www.linkedin.com/in/chnkukoolwal/" style="margin-right: 10px; display: inline-block; color: #0A66C2; text-decoration: none;" aria-label="LinkedIn">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M19 0h-14c-2.76 0-5 2.24-5 5v14c0 2.76 2.24 5 5 5h14c2.76 0 5-2.24 5-5v-14c0-2.76-2.24-5-5-5zm-11 19h-3v-9h3v9zm-1.5-10.29c-.97 0-1.75-.79-1.75-1.75s.78-1.75 1.75-1.75 1.75.78 1.75 1.75-.78 1.75-1.75 1.75zm13.5 10.29h-3v-4.5c0-1.07-.02-2.44-1.49-2.44-1.49 0-1.72 1.16-1.72 2.36v4.58h-3v-9h2.88v1.23h.04c.4-.75 1.37-1.54 2.82-1.54 3.02 0 3.58 1.99 3.58 4.58v5.73z"/></svg>
      </a>

      <a href="https://x.com/chnkukoolwal" style="margin-right: 10px; display: inline-block; color: #1DA1F2; text-decoration: none;" aria-label="X">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M23 3a10.9 10.9 0 01-3.14 0.86A4.48 4.48 0 0022.4.36a9.04 9.04 0 01-2.88 1.1A4.52 4.52 0 0016.88 0c-2.5 0-4.52 2.02-4.52 4.5 0 .35.04.69.12 1.02C7.72 5.41 4.07 3.48 1.64.38a4.5 4.5 0 00-.61 2.27c0 1.56.8 2.94 2 3.74a4.51 4.51 0 01-2.05-.57v.06c0 2.18 1.55 4 3.6 4.42a4.5 4.5 0 01-2.04.08c.58 1.8 2.28 3.12 4.28 3.15A9.03 9.03 0 010 19.54a12.74 12.74 0 006.92 2.03c8.3 0 12.84-6.87 12.84-12.84 0-.2 0-.39-.01-.58A9.18 9.18 0 0024 4.56a9.06 9.06 0 01-2.6.71A4.5 4.5 0 0023 3z"/></svg>
      </a>

      <a href="https://chnkukoolwal.medium.com/" style="margin-right: 10px; display: inline-block; color: #000000; text-decoration: none;" aria-label="Medium">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M2 4h3v16H2V4zm5 0h2.6l4.6 16H12L7 4zm7.1 0h4.9c.7 0 1.3.5 1.3 1.2v13.5c0 .7-.6 1.3-1.3 1.3h-4.9V4z"/></svg>
      </a>

      <a href="https://substack.com/@chnkukoolwal" style="display: inline-block; color: #FF6719; text-decoration: none;" aria-label="Substack">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M0 3v18h24V3H0zm3 3h18v12H3V6z"/></svg>
      </a>
    </p>

    <p style="margin: 5px 0 0 0; font-size: 14px; color: #888;">
      <a href="https://linktr.ee/chnkukoolwal" style="color: inherit; text-decoration: none;">@chnkukoolwal</a>
    </p>
  </div>

  <!-- Right side: subscribe box -->
  <div id="subscribe" style="flex-shrink: 0; max-width: 300px; border: 1px solid #e0e0e0; border-radius: 6px; padding: 20px; background: #fafafa;">
    <h3 style="margin-bottom: 10px; font-weight: 600;">Subscribe to my updates</h3>
    <p style="margin-bottom: 15px; color: #555; font-size: 14px;">
      Get weekly updates on startups, venture capital, and ecosystem insights directly to your inbox.
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
