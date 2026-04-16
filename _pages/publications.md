---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

{% assign math_pubs = site.publications | where: "category", "mathematics" | sort: "date" | reverse %}
{% assign other_pubs = site.publications | where: "category", "other" | sort: "date" | reverse %}

<section class="cv-section">
<h2 class="cv-section-title">Mathematics</h2>
<ol class="cv-list">
{% for post in math_pubs %}
<li class="cv-item">
  <em>{{ post.title }}</em>{% if post.coauthors and post.coauthors != "" %} ({{ post.coauthors }}){% endif %}, {{ post.citation_info }}.
</li>
{% endfor %}
</ol>
</section>

<section class="cv-section">
<h2 class="cv-section-title">Other Publications</h2>
<ol class="cv-list">
{% for post in other_pubs %}
<li class="cv-item">
  <em>{{ post.title }}</em>{% if post.coauthors and post.coauthors != "" %} ({{ post.coauthors }}){% endif %}, {{ post.citation_info }}.
</li>
{% endfor %}
</ol>
</section>
