---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<h2 class="section-label">Education</h2>
<div class="card-grid">

  <div class="item-card">
    <div class="card-badges">
      <span class="badge badge-pub">Postdoc</span>
      <span class="badge badge-year">2025 – present</span>
    </div>
    <p class="card-title">Postdoctoral Research Associate</p>
    <p class="card-venue">University of Sydney &mdash; School of Mathematics and Statistics</p>
    <p class="card-meta">Working with Prof. John Voight</p>
  </div>

  <div class="item-card">
    <div class="card-badges">
      <span class="badge badge-talk">PhD</span>
      <span class="badge badge-year">2021 – 2025</span>
    </div>
    <p class="card-title">Doctor of Philosophy in Mathematics</p>
    <p class="card-venue">RWTH Aachen University</p>
    <p class="card-meta">Supervisors: Prof. Dr. Alice C. Niemeyer, Prof. Dr. Wilhelm Plesken &middot; Thesis: <em>Simplicial surfaces and their applications to topological interlocking</em></p>
  </div>

  <div class="item-card">
    <div class="card-badges">
      <span class="badge badge-thesis">MSc</span>
      <span class="badge badge-year">2021</span>
    </div>
    <p class="card-title">Master of Science in Mathematics</p>
    <p class="card-venue">RWTH Aachen University</p>
    <p class="card-meta">Minor: Business Studies &middot; Supervisors: Prof. Dr. Alice C. Niemeyer, Prof. Dr. Wilhelm Plesken</p>
  </div>

  <div class="item-card">
    <div class="card-badges">
      <span class="badge badge-thesis">BSc</span>
      <span class="badge badge-year">2018</span>
    </div>
    <p class="card-title">Bachelor of Science in Mathematics</p>
    <p class="card-venue">RWTH Aachen University</p>
    <p class="card-meta">Minor: Business Studies &middot; Supervisors: Prof. Dr. Alice C. Niemeyer, Prof. Dr. Wilhelm Plesken</p>
  </div>

</div>

<h2 class="section-label" style="margin-top:2.5em;">Experience Abroad</h2>
<div class="card-grid">

  <div class="item-card">
    <div class="card-badges">
      <span class="badge badge-workshop">Research Visit</span>
      <span class="badge badge-year">Sep 2023</span>
    </div>
    <p class="card-title">RMIT University &mdash; 3 weeks</p>
    <p class="card-venue">Melbourne, Australia</p>
    <p class="card-meta">Host: Prof. Yi Min Xie &middot; Project: Construction of Tubular Topological Interlocking Assemblies</p>
  </div>

  <div class="item-card">
    <div class="card-badges">
      <span class="badge badge-workshop">Research Visit</span>
      <span class="badge badge-year">Jul 2023</span>
    </div>
    <p class="card-title">RMIT University &mdash; 2 weeks</p>
    <p class="card-venue">Melbourne, Australia</p>
    <p class="card-meta">Host: Prof. Yi Min Xie &middot; Project: Topological Interlocking Assemblies with prescribed boundary conditions</p>
  </div>

  <div class="item-card">
    <div class="card-badges">
      <span class="badge badge-workshop">Research Visit</span>
      <span class="badge badge-year">Apr – Oct 2023</span>
    </div>
    <p class="card-title">University of Sydney &mdash; 6 months</p>
    <p class="card-venue">Sydney, Australia</p>
    <p class="card-meta">Collaboration with Jonathan Spreer &middot; Classification of face-transitive surfaces; 2-transitive simplicial surfaces</p>
  </div>

  <div class="item-card">
    <div class="card-badges">
      <span class="badge badge-workshop">Erasmus</span>
      <span class="badge badge-year">Sep 2019 – May 2020</span>
    </div>
    <p class="card-title">Queen Mary University of London &mdash; 9 months</p>
    <p class="card-venue">London, United Kingdom</p>
  </div>

</div>

<h2 class="section-label" style="margin-top:2.5em;">Skills</h2>
<ul class="simple-list">
  <li><span class="list-item-title">GAP</span><span class="list-item-meta"> &mdash; Advanced &middot; Maintainer of <em>SimplicialSurfaces</em> and <em>GaPic</em></span></li>
  <li><span class="list-item-title">Julia</span><span class="list-item-meta"> &mdash; Basic &middot; Maintainer of <em>GeoCombSurfX</em></span></li>
  <li><span class="list-item-title">LaTeX</span><span class="list-item-meta"> &mdash; Advanced</span></li>
  <li><span class="list-item-title">3D-printing</span><span class="list-item-meta"> &mdash; Advanced</span></li>
  <li><span class="list-item-title">Python, C++, Java, Maple, Matlab</span><span class="list-item-meta"> &mdash; Basic</span></li>
  <li><span class="list-item-title">Languages</span><span class="list-item-meta"> &mdash; German (native), English (fluent)</span></li>
</ul>

<h2 class="section-label" style="margin-top:2em;">Software</h2>
<ul class="simple-list">
  <li><span class="list-item-title">GeoCombSurfX</span><span class="list-item-meta"> &mdash; Julia package, 2023 (with Sascha Stüttgen)</span></li>
  <li><span class="list-item-title">Honeycomb</span><span class="list-item-meta"> &mdash; Rhino plugin, 2023 (with Tom Goertzen, Samuel Losi)</span></li>
  <li><span class="list-item-title">GaPic</span><span class="list-item-meta"> &mdash; GAP package, 2022 (with Alice C. Niemeyer, Tom Goertzen, Meike Weiss, Lukas Schnelle)</span></li>
  <li><span class="list-item-title">SimplicialSurfaces</span><span class="list-item-meta"> &mdash; GAP package, 2022 (with Markus Baumeister, Tom Goertzen, Alice C. Niemeyer, Meike Weiss)</span></li>
</ul>

<h2 class="section-label" style="margin-top:2em;">Teaching</h2>
<ul class="simple-list">
  {% assign sorted_teaching = site.teaching | sort: "date" | reverse %}
  {% for post in sorted_teaching %}
  <li>
    <span class="list-item-title">{{ post.title }}</span>
    <span class="list-item-meta"> &mdash; {{ post.venue }}, {{ post.date | date: "%Y" }}</span>
  </li>
  {% endfor %}
</ul>

<h2 class="section-label" style="margin-top:2em;">Social Involvement</h2>
<ul class="simple-list">
  <li><span class="list-item-title">Chairman</span><span class="list-item-meta"> &mdash; <em>We Won't Be Quiet</em> association (since 2019)</span></li>
  <li><span class="list-item-title">Member</span><span class="list-item-meta"> &mdash; <em>Monada</em> association (since 2022)</span></li>
</ul>

<h2 class="section-label" style="margin-top:2em;">Personal Interests</h2>
<ul class="simple-list">
  <li><span class="list-item-title">Photography</span></li>
  <li><span class="list-item-title">Dancing</span></li>
  <li><span class="list-item-title">Volleyball &amp; Basketball</span></li>
  <li><span class="list-item-title">Exercising</span></li>
</ul>
