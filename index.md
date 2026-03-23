---
layout: default
---

<div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 40px; border-bottom: 1px solid #e0e0e0; padding-bottom: 25px; gap: 20px; flex-wrap: wrap;">

  <!-- Left side: profile image, name, social links, handle, intake forms -->
  <div style="flex: 1; min-width: 250px; display: flex; flex-direction: column; align-items: flex-start;">

    <!-- Profile image -->
    <img src="https://github.com/chnkukoolwal/chnkukoolwal.github.io/blob/main/IMG_9253%20copy.png?raw=true" 
         alt="Chinku Koolwal" 
         style="width: 260px; height: auto; object-fit: cover; margin-bottom: 10px;">

    <h1 style="margin: 0 0 5px 0; font-size: 28px; font-weight: 600; line-height: 1.2;">
      Chinku Koolwal
    </h1>

    <p style="margin: 0 0 5px 0; font-size: 16px; color: #555; font-weight: 400; line-height: 1.2; font-style: italic;">
      Startup Advisor & Venture Scout
    </p>

    <!-- Social links -->
    <p style="margin: 0 0 5px 0; font-size: 14px; color: #555; line-height: 1.2;">
      <a href="https://www.linkedin.com/in/chnkukoolwal/" style="color: inherit; text-decoration: underline;">LinkedIn</a> •
      <a href="https://x.com/chnkukoolwal" style="color: inherit; text-decoration: underline;">X</a> •
      <a href="https://chnkukoolwal.medium.com/" style="color: inherit; text-decoration: underline;">Medium</a> •
      <a href="https://substack.com/@chnkukoolwal" style="color: inherit; text-decoration: underline;">Substack</a>
    </p>

    <!-- Handle -->
    <p style="margin: 0 0 10px 0; font-size: 14px; color: #888; line-height: 1.2;">
      <a href="https://linktr.ee/chnkukoolwal" style="color: inherit; text-decoration: underline;">@chnkukoolwal</a>
    </p>

    <!-- Intake form links (Investor first) -->
    <p style="margin: 5px 0 2px 0; font-size: 14px; color: #555; line-height: 1.2;">
      Join the fund: <a href="https://jazzy-yttrium-143.notion.site/327cd7e0672c814eb9a1e77dcf94e955?pvs=105" style="color: #111; text-decoration: underline;">Investor Intake Form</a>
    </p>
    <p style="margin: 2px 0 0 0; font-size: 14px; color: #555; line-height: 1.2;">
      Join the portfolio: <a href="https://jazzy-yttrium-143.notion.site/326cd7e0672c810385dfc3251f95ae38?pvs=105" style="color: #111; text-decoration: underline;">Founder Intake Form</a>
    </p>

  </div>

  <!-- Right side: subscribe box -->
  <div id="subscribe" style="flex-shrink: 0; max-width: 300px; border: 1px solid #e0e0e0; border-radius: 6px; padding: 20px; background: #fafafa;">
    
    <!-- Description above subscribe input -->
    <p style="margin-bottom: 15px; color: #555; font-size: 14px;">
      Get weekly updates on startups and venture capital directly to your inbox.
    </p>

    <!-- Minimal Substack subscribe iframe -->
    <iframe src="https://chnkukoolwal.substack.com/embed?type=subscribe_only" 
            width="100%" height="60" 
            style="border: 1px solid #EEE; background: white;" 
            frameborder="0" scrolling="no">
    </iframe>
    
  </div>

</div>

{% for post in site.posts %}
  <article style="margin-bottom: 90px;">

    <p style="color: #888; font-size: 13px; margin-bottom: 8px;">
      {{ post.date | date: "%B %d, %Y" }}
    </p>

    <h2 style="margin-bottom: 15px;">
      <a href="{{ post.url }}" style="color: #111; text-decoration: underline;">
        {{ post.title }}
      </a>
    </h2>

    <div style="line-height: 1.75; font-size: 16px; color: #111;">
      {{ post.content }}
    </div>

  </article>
{% endfor %}
