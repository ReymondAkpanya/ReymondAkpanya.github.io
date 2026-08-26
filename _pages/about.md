---
permalink: /
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<p style="text-align: center;">
    <img src="/images/MagmaLogoOfficial.png" alt="Magma" style="max-width: 30%; height: auto;">
</p>

<div class="news-box">
  <p class="news-box-header">News</p>
  {% assign nl = "
" %}
  {% capture talk_lines %}{% for t in site.talks %}{{ t.date | date: "%Y-%m-%d" }}|talk|{{ t.title }}|{{ t.venue }}|{{ t.location }}{{ nl }}{% endfor %}{% endcapture %}
  {% capture data_lines %}{% for n in site.data.news %}{{ n.date | date: "%Y-%m-%d" }}|news|{{ n.text }}{{ nl }}{% endfor %}{% endcapture %}
  {% assign all_lines = talk_lines | append: data_lines | split: nl | sort | reverse %}
  {% assign shown = 0 %}
  {% for line in all_lines %}
    {% if line != "" and shown < 3 %}
      {% assign parts = line | split: "|" %}
      {% assign shown = shown | plus: 1 %}
      <div class="news-item">
        <span class="news-date">{{ parts[0] | date: "%b %Y" }}</span>
        <span class="news-text">{% if parts[1] == "talk" %}Talk at <strong>{{ parts[2] }}</strong>{% if parts[3] != "" and parts[3] != "Remote" %}, {{ parts[3] }}{% endif %}, {{ parts[4] }}{% else %}{{ parts[2] }}{% endif %}</span>
      </div>
    {% endif %}
  {% endfor %}
</div>

I am a Magma Research Associate at the [Magma Group](https://magma.maths.usyd.edu.au/magma/), within the School of Mathematics and Statistics at the [University of Sydney](https://www.sydney.edu.au/), working with John Voight.

My research lies in combinatorics, computational algebra, and their applications, with a particular focus on the interplay between combinatorial structures and their geometric realisations as polyhedra. I combine theoretical methods with extensive use of computer algebra systems, in particular Magma, as well as GAP and related tools.

Previously I completed my [PhD thesis](https://www.art.rwth-aachen.de/cms/mathb/forschung/publikationen/~rekk/details/?file=1016413&lidx=1) at RWTH Aachen University under the supervision of
Alice C. Niemeyer and Wilhelm Plesken.


<h2 class="section-label" style="margin-top:2em;">Research</h2>
<div class="card-grid card-grid-2col" style="margin-top:1em;">

  <div class="item-card research-card">
    <img src="/images/C23.png" alt="Algebraic Graph Theory" class="research-card-img">
    <p class="card-title" style="margin-top:0.7em;">Algebraic Graph Theory</p>
  </div>

  <div class="item-card research-card">
    <img src="/images/platonic_solids.png" alt="Simplicial Surfaces" class="research-card-img">
    <p class="card-title" style="margin-top:0.7em;">Simplicial Surfaces</p>
  </div>

  <div class="item-card research-card">
    <img src="/images/helix5_torus1.png" alt="Group Actions on Discrete Structures" class="research-card-img">
    <p class="card-title" style="margin-top:0.7em;">Group Actions on Discrete Structures</p>
  </div>

  <div class="item-card research-card">
    <img src="/images/aperiodicinterlocking.png" alt="Topological Interlockings" class="research-card-img">
    <p class="card-title" style="margin-top:0.7em;">Topological Interlockings</p>
  </div>

</div>
