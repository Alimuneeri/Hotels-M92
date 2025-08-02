---
layout: page
title: Our Location
---
We are centrally located, providing easy access to the city's top attractions.

<div class="row">
<div class="col-lg-8" data-aos="fade-up">
<!-- Google Maps Embed -->
<div class="ratio ratio-16x9 mb-4">
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3022.62954512527!2d-73.98235!3d40.74844!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89c259a6f3b7ac8d%3A0x6b6a5a4a4b0c4e8!2s123%20Park%20Ave%2C%20New%20York%2C%20NY%2010001%2C%20USA!5e0!3m2!1sen!2sin!4v1620201655322!5m2!1sen!2sin" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
</div>
</div>
<div class="col-lg-4" data-aos="fade-up" data-aos-delay="100">
<div class="location-details">
<h3>The Central Park Hotel</h3>
<p>123 Park Avenue<br>New York, NY 10001</p>
</div>
</div>
</div>

<div class="row mt-5">
<div class="col-12" data-aos="fade-up">
<!-- "What's Nearby" Feature -->
<div class="nearby-container">
<ul class="nav nav-tabs" id="locationTab" role="tablist">
<li class="nav-item" role="presentation">
<button class="nav-link active" id="nearby-tab" data-bs-toggle="tab" data-bs-target="#nearby" type="button" role="tab" aria-controls="nearby" aria-selected="true">What's nearby</button>
</li>
<li class="nav-item" role="presentation">
<button class="nav-link" id="airports-tab" data-bs-toggle="tab" data-bs-target="#airports" type="button" role="tab" aria-controls="airports" aria-selected="false">Airports</button>
</li>
</ul>
<div class="tab-content" id="locationTabContent">
<div class="tab-pane fade show active" id="nearby" role="tabpanel" aria-labelledby="nearby-tab">
<ul class="list-group list-group-flush">
{% for item in site.data.nearby %}
<li class="list-group-item d-flex justify-content-between align-items-center">
<span><i class="fas fa-map-marker-alt me-2"></i>{{ item.name }}</span>
<span class="text-muted">{{ item.distance }}</span>
</li>
{% endfor %}
</ul>
</div>
<div class="tab-pane fade" id="airports" role="tabpanel" aria-labelledby="airports-tab">
<ul class="list-group list-group-flush">
<li class="list-group-item d-flex justify-content-between align-items-center">
<span><i class="fas fa-plane-departure me-2"></i>LaGuardia Airport (LGA)</span>
<span class="text-muted">8 miles</span>
</li>
<li class="list-group-item d-flex justify-content-between align-items-center">
<span><i class="fas fa-plane-departure me-2"></i>John F. Kennedy Airport (JFK)</span>
<span class="text-muted">15 miles</span>
</li>
</ul>
</div>
</div>
</div>
</div>
</div>