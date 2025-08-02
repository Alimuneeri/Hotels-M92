---
layout: default
title: Home
---
<!-- 1. HERO CAROUSEL & BOOKING WIDGET -->

<div class="hero-carousel-container">
<!-- Bootstrap Carousel -->
<div id="heroCarousel" class="carousel slide" data-bs-ride="carousel">
<div class="carousel-indicators">
<button type="button" data-bs-target="#heroCarousel" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
<button type="button" data-bs-target="#heroCarousel" data-bs-slide-to="1" aria-label="Slide 2"></button>
<button type="button" data-bs-target="#heroCarousel" data-bs-slide-to="2" aria-label="Slide 3"></button>
</div>
<div class="carousel-inner">
<div class="carousel-item active" style="background-image: url('/assets/images/hero-background1.jpg');">
<!-- == IMAGE REPLACEMENT ==
- Replace with a high-quality image of your lobby or exterior.
- Recommended Size: 1920x1080 pixels
-->
<div class="carousel-caption d-none d-md-block">
<h2>Unmatched Luxury & Service</h2>
<p>Experience a stay unlike any other.</p>
</div>
</div>
<div class="carousel-item" style="background-image: url('/assets/images/hero-background2.jpg');">
<!-- == IMAGE REPLACEMENT ==
- Replace with a high-quality image of a room with a view.
- Recommended Size: 1920x1080 pixels
-->
<div class="carousel-caption d-none d-md-block">
<h2>Rooms with Breathtaking Views</h2>
<p>Wake up to the beauty of the city.</p>
</div>
</div>
<div class="carousel-item" style="background-image: url('/assets/images/hero-background3.jpg');">
<!-- == IMAGE REPLACEMENT ==
- Replace with a high-quality image of your pool or another key amenity.
- Recommended Size: 1920x1080 pixels
-->
<div class="carousel-caption d-none d-md-block">
<h2>Relax and Unwind in Style</h2>
<p>Your perfect urban oasis awaits.</p>
</div>
</div>
</div>
<button class="carousel-control-prev" type="button" data-bs-target="#heroCarousel" data-bs-slide="prev">
<span class="carousel-control-prev-icon" aria-hidden="true"></span>
<span class="visually-hidden">Previous</span>
</button>
<button class="carousel-control-next" type="button" data-bs-target="#heroCarousel" data-bs-slide="next">
<span class="carousel-control-next-icon" aria-hidden="true"></span>
<span class="visually-hidden">Next</span>
</button>
</div>
</div>

<!-- Booking Widget -->

<div class="booking-widget">
<form class="row g-3 align-items-end">
<div class="col-md">
<label for="checkin" class="form-label">Check-in</label>
<input type="date" class="form-control" id="checkin">
</div>
<div class="col-md">
<label for="checkout" class="form-label">Check-out</label>
<input type="date" class="form-control" id="checkout">
</div>
<div class="col-md">
<label for="guests" class="form-label">Guests</label>
<select id="guests" class="form-select">
<option selected>1 Guest</option>
<option>2 Guests</option>
<option>3 Guests</option>
<option>4 Guests</option>
</select>
</div>
<div class="col-md-auto">
<button type="submit" class="btn btn-primary w-100">Check Availability</button>
</div>
</form>
</div>
</div>

<div class="container my-5">
<!-- 2. AMENITIES SECTION -->
<section id="amenities" class="text-center my-5 py-5" data-aos="fade-up">
<h2>Our Amenities</h2>
<p class="lead">We offer a wide range of amenities to make your stay exceptional.</p>
<div class="row mt-5">
{% for amenity in site.data.amenities %}
<div class="col-md-4 col-lg-2 mb-4">
<div class="amenity-item">
<div class="amenity-icon">
<i class="{{ amenity.icon }}"></i>
</div>
<h6>{{ amenity.name }}</h6>
</div>
</div>
{% endfor %}
</div>
</section>

<!-- 3. TESTIMONIALS SECTION -->

<section id="testimonials" class="testimonials-section bg-light my-5 py-5" data-aos="fade-up">
<div class="container">
<h2 class="text-center">What Our Guests Say</h2>
<div id="testimonialCarousel" class="carousel slide" data-bs-ride="carousel">
<div class="carousel-inner">
{% for testimonial in site.data.testimonials %}
<div class="carousel-item {% if forloop.first %}active{% endif %}">
<div class="testimonial-content">
<p class="testimonial-quote">"{{ testimonial.quote }}"</p>
<h5 class="testimonial-author">- {{ testimonial.author }}, {{ testimonial.location }}</h5>
</div>
</div>
{% endfor %}
</div>
<button class="carousel-control-prev" type="button" data-bs-target="#testimonialCarousel" data-bs-slide="prev">
<span class="carousel-control-prev-icon" aria-hidden="true"></span>
<span class="visually-hidden">Previous</span>
</button>
<button class="carousel-control-next" type="button" data-bs-target="#testimonialCarousel" data-bs-slide="next">
<span class="carousel-control-next-icon" aria-hidden="true"></span>
<span class="visually-hidden">Next</span>
</button>
</div>
</div>
</section>

<!-- 4. MEMBER BENEFITS SECTION -->

<section id="member-benefits" class="text-center my-5 py-5" data-aos="fade-up">
<div class="container">
<div class="row justify-content-center">
<div class="col-lg-8">
<div class="member-benefit-icon">
<i class="fas fa-crown"></i>
</div>
<h2>Become a Member</h2>
<p class="lead">Join our loyalty program to unlock exclusive benefits, including special rates, room upgrades, and members-only offers. Your loyalty deserves to be rewarded.</p>
<a href="#" class="btn btn-outline-primary btn-lg mt-3">Join Now & Save</a>
</div>
</div>
</div>
</section>
</div>