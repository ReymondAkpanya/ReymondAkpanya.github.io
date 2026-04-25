---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

{% assign math_pubs = site.publications | where: "category", "mathematics" | sort: "date" | reverse %}
{% assign other_pubs = site.publications | where: "category", "other" | sort: "date" | reverse %}

<h2 class="section-label">Mathematics</h2>
<div class="card-grid">
{% for post in math_pubs %}
<div class="item-card">
  <div class="card-badges">
    {% if post.citation_info contains 'preparation' %}
      <span class="badge badge-white">In Preparation</span>
    {% elsif post.citation_info contains 'hesis' %}
      <span class="badge badge-pub">Thesis</span>
    {% elsif post.citation_info contains 'ubmit' %}
      <span class="badge badge-prep">Submitted</span>
    {% elsif post.citation_info contains 'arxiv' %}
      <span class="badge badge-prep">Arxiv</span>
    {% else %}
      <span class="badge badge-pub">{{ post.venue }}</span>
    {% endif %}
    <span class="badge badge-year">{{ post.date | date: "%Y" }}</span>
  </div>
  <p class="card-title"><span class="pub-number">{{ forloop.index }}.</span> {{ post.title }}</p>
  {% if post.coauthors and post.coauthors != "" %}
    <p class="card-authors">{{ post.coauthors }}</p>
  {% endif %}
  <p class="card-meta">{{ post.citation_info }}</p>
</div>
{% endfor %}
</div>

<h2 class="section-label" style="margin-top:2.5em;">Other Publications</h2>
<div class="card-grid">
{% for post in other_pubs %}
<div class="item-card">
  <div class="card-badges">
    {% if post.citation_info contains 'preparation' %}
      <span class="badge badge-white">In Preparation</span>
    {% elsif post.citation_info contains 'hesis' %}
      <span class="badge badge-pub">Thesis</span>
    {% elsif post.citation_info contains 'submit' %}
      <span class="badge badge-prep">Submitted</span>
    {% elsif post.citation_info contains 'arxiv' %}
      <span class="badge badge-prep">Arxiv</span>
    {% else %}
      <span class="badge badge-pub">{{ post.venue }}</span>
    {% endif %}
    <span class="badge badge-year">{{ post.date | date: "%Y" }}</span>
  </div>
  <p class="card-title"><span class="pub-number">{{ forloop.index }}.</span> {{ post.title }}</p>
  {% if post.coauthors and post.coauthors != "" %}
    <p class="card-authors">{{ post.coauthors }}</p>
  {% endif %}
  <p class="card-meta">{{ post.citation_info }}</p>
</div>
{% endfor %}
</div>
