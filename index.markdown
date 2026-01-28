---
layout: default
---

<div class="home-hero">
  <h1>Engineering Excellence.</h1>
  <p>Leveled is an elite boutique firm dedicated to crafting high-quality, high-performance software solutions. We specialize in building robust platforms like <a href="https://medicalscribe.app">medicalscribe.app</a> that redefine industries.</p>

  <img src="{{ '/assets/app-screenshot.png' | relative_url }}" alt="Medical Scribe App Interface" style="width: 100%; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1); margin-top: 20px;">
</div>

<div class="latest-news" style="margin-top: 60px; border-top: 1px solid #eee; padding-top: 20px;">
  <h3>Latest News</h3>
  <ul class="post-list">
    {% for post in site.posts limit:3 %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h3>
      </li>
    {% endfor %}
  </ul>
</div>
