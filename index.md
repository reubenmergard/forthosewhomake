---
layout: default
title: Home
---

<div class="home-layout">
  <main class="home-main">

    <div class="site-bio">
      <p><a href="/" class="site-name">for those who make</a> is a somewhat open-ended writing practice where Australian artist, designer and brand consultant Reuben Mergard writes on topics intended to be relevant to professional creatives.</p>
      <p>Reuben Mergard is a designer who works primaily on branding projects, but undertakes a number of spatial deisgn and artistic projects. He thinks extensivley on creative.</p>
    </div>

    <div class="post-list">
      {% for post in site.posts limit:20 %}
      <div class="post-item">
        <div class="post-title-meta">
          <a href="{{ post.url }}">{{ post.title }}</a>
          <span class="post-meta">{{ post.date | date: "%d %b %Y" }}</span>
        </div>
      </div>
      {% endfor %}
    </div>

  </main>

  <div class="home-side">
    <div class="side-links">
      <a href="/now/">Now</a><br>
      <a href="/contact/">Contact</a>
    </div>
  </div>
</div>
