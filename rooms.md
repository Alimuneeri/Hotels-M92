---
layout: page
title: Our Rooms & Suites
---

Here is a list of our beautifully appointed rooms. Choose the perfect space for your stay.

<div class="row row-cols-1 row-cols-md-2 g-4 mt-4">
{% for room in site.rooms %}
<div class="col" data-aos="fade-up" data-aos-delay="{{ forloop.index0 | times: 100 }}">
<div class="card h-100 card-hover">
<!--
== IMAGE REPLACEMENT ==
- The image source is set in the front matter of each room's Markdown file (e.g., _rooms/sample-room.md).
- It uses room.image to get the path.
- Recommended Size: 800x600 pixels
- Image Type: A clear, attractive photo of the specific room.
-->
<img src="{{ room.image }}" class="card-img-top" alt="{{ room.title }}">
<div class="card-body d-flex flex-column">
<h5 class="card-title">{{ room.title }}</h5>
<p class="card-text">{{ room.excerpt }}</p>
<a href="{{ room.url }}" class="btn btn-primary mt-auto">View Details</a>
</div>
</div>
</div>
{% endfor %}
</div>