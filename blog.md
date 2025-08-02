---
layout: page
title: Blog
---

<div class="container mt-5">
  <div class="row">
    <div class="col-lg-8">
      <h1 class="mb-4">Latest Posts</h1>

      {% for post in site.posts %}
        <div class="card mb-4 shadow-sm" data-aos="fade-up">
          <div class="card-body">
            <h2 class="card-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
            <p class="card-text text-muted">{{ post.date | date: "%B %d, %Y" }}</p>
            <p class="card-text">{{ post.excerpt }}</p>
            <a href="{{ post.url | relative_url }}" class="btn btn-primary">Read More &rarr;</a>
          </div>
        </div>
      {% endfor %}

    </div>
  </div>
</div>