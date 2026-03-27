---
layout: index
title: Home
description: ""
navorder: 1
---

<div class="container px-5 py-3 bg-gray-2 rounded">

<p>Robotics and AI are transformative tools for scientific discovery and integral components of future laboratories. The primary goal of the summer school is to engage students in materials science in the era of automation and AI/ML. Through lectures, coding tutorials, hands-on robotic hardware integration and robotic synthesis experiments, participants will explore closed-loop experiment design, machine learning, data handling and visualization, as well as hands-on lab work to create thin film and nanocrystal semiconductors using different robotic platforms.</p>

<p>We aim to foster the development of the future workforce in materials science, engineering, computer science, physics, and related fields, anticipating that science and research will increasingly integrate artificial intelligence and machine learning (AI/ML).</p>

<hr class="my-4">

<div class="text-center">

<h2>Who is eligible to register?</h2>

<ul class="list-unstyled">
<li>Professionals, postdocs, graduate students, undergraduate students.</li>
<li>All coding activities will have ChatGPT-assisted coding — no Python or coding experience required.</li>
</ul>

<ul class="list-unstyled mt-2">
<li> Bring your own laptop.</li>
<li> Long pants and close-toed shoes required to enter labs.</li>
</ul>

<a href="#" class="btn btn-primary mb-4">Register</a>

</div>

<hr class="my-4">

<h2>Invited Speakers</h2>

{% for speaker in site.data.home.invited_speakers %}
<div class="row mb-4 align-items-center">
<div class="col-auto">
<img src="{{ '/assets/images/' | append: speaker.photo | relative_url }}"
     class="rounded-circle" style="width:175px;height:175px;object-fit:cover;object-position:top center;" alt="{{ speaker.name }}">
</div>
<div class="col">
<strong>{{ speaker.name }}</strong><br>
<span class="text-muted">{{ speaker.affiliation }}</span>
<p class="mt-1 mb-0">{{ speaker.bio }}</p>
</div>
</div>
{% endfor %}

</div>

<div class="container my-5">

<h2>Organizers</h2>

{% include people_grid.html people=site.data.home.organizers %}

<h2>Experimental Instructors</h2>

{% include people_grid.html people=site.data.home.experimental_instructors %}

<h2>Data Science Instructors</h2>

{% include people_grid.html people=site.data.home.data_instructors %}

<div class="d-flex flex-wrap gap-2 mb-2">
<a href="https://camsunlab.com/papers" class="btn btn-outline-primary btn-sm">Read More @ SunLab@Cambridge</a>
<a href="https://sutterfellalab.lbl.gov/publications/" class="btn btn-outline-primary btn-sm">Read More @ Carolin M. Sutter-Fella Lab</a>
<a href="https://www.alvinyzhou.com/" class="btn btn-outline-primary btn-sm">Read More @ Yuanyuan Zhou Lab</a>
<a href="https://people.llnl.gov/gongora1" class="btn btn-outline-primary btn-sm">Read More @ Aldair Ernesto Gongora</a>
</div>

</div>
