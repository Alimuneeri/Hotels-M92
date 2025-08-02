---
layout: page
title: Special Offers & Packages
---

Take advantage of our exclusive packages to make your stay even more memorable.

<div class="row row-cols-1 row-cols-md-2 g-4 mt-4">
{% for offer in site.offers %}
<div class="col" data-aos="fade-up" data-aos-delay="{{ forloop.index0 | times: 100 }}">
<div class="card h-100 card-hover">
<!--
== IMAGE REPLACEMENT ==
- The image source is set in the front matter of each offer's Markdown file (e.g., _offers/sample-offer.md).
- It uses offer.image to get the path.
- Recommended Size: 800x600 pixels
- Image Type: An attractive image representing the offer.
-->
<img src="{{ offer.image }}" class="card-img-top" alt="{{ offer.title }}">
<div class="card-body d-flex flex-column">
<h5 class="card-title">{{ offer.title }}</h5>
<p class="card-text">{{ offer.excerpt }}</p>
<a href="{{ offer.url }}" class="btn btn-primary mt-auto">View Offer Details</a>
</div>
</div>
</div>
{% endfor %}
</div>