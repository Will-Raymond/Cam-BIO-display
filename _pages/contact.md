---
title: "About us"
permalink: /contact/
# People shown on this page. `role` and `bio` are optional — leave them empty to hide.
pis:
  - name: "Dr. Chris Snow"
    photo: /assets/images/chris_snow.jpg
    role: ""
    bio: ""
    link: https://www.engr.colostate.edu/bce/people/chris-snow/
  - name: "Dr. Brian Geiss"
    photo: /assets/images/brian_geiss.jpg
    role: ""
    bio: ""
    link: https://vetmedbiosci.colostate.edu/directory/member/?id=brian-geiss-3203
  - name: "Dr. Tim Stasevich"
    photo: /assets/images/tim_stasevich.png
    role: ""
    bio: ""
    link: https://stasevichlab.colostate.edu/
team:
  - name: "Dr. Will Raymond"
    photo: /assets/images/wsr_photo3.png
    role: "Project manager"
    bio: "Dr. Will Raymond is a computational biologist with a focus on RNA and machine learning. He received his PhD in 2024 from Colorado State University for work on mRNA translation modeling. He currently is the developer of the Cam-BIO environment working intently on the AI integration and protocol capabilities across the lab."
    link: https://will-raymond.github.io/will_raymond_cv/
---

<style>
  .ab-lead { font-size: 1.15rem; line-height: 1.6; margin: .5rem 0 2rem; }
  .ab-section { margin: 0 0 .25rem !important; padding-bottom: .35rem; border-bottom: 3px solid #D9782D !important; display: inline-block; }
  .ab-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(15rem, 1fr)); gap: 1.5rem; margin: 1.25rem 0 3rem; }
  .ab-card {
    display: flex; flex-direction: column; overflow: hidden;
    background: #fff; border: 1px solid #e3e3e3; border-radius: 12px;
    box-shadow: 0 2px 10px rgba(14,36,49,.06); transition: transform .25s, box-shadow .25s;
  }
  .ab-card:hover { transform: translateY(-3px); box-shadow: 0 10px 24px rgba(14,36,49,.12); }
  .ab-card img { width: 100%; aspect-ratio: 1 / 1; object-fit: cover; object-position: center top; display: block; margin: 0; }
  .ab-card__body { display: flex; flex-direction: column; flex: 1; padding: 1rem 1.15rem 1.15rem; border-top: 4px solid #7E5475; }
  .ab-card h3 { margin: 0 0 .15rem !important; font-size: 1.15rem; color: #0e2431; }
  .ab-card__role { margin: 0 0 .5rem; font-size: .85rem; font-weight: 600; color: #7E5475; }
  .ab-card__bio { margin: 0 0 .75rem; font-size: .9rem; color: #3a4650; }
  .ab-card .btn { margin-top: auto; align-self: flex-start; }
  @media (prefers-reduced-motion: reduce) { .ab-card { transition: none; } }
</style>

<p class="ab-lead">We are an interdisciplinary team of scientists with backgrounds that range from protein engineering, virology, fluorescence microscopy, machine learning, and RNA biology, aiming to bring efficient and reproducible automated laboratory experiments to Colorado State University, and to the broader scientific world!</p>

{% include contact-cta.html %}

{% assign groups = "Tag Team|pis,Cam-BIO team|team" | split: "," %}
{% for g in groups %}
{% assign parts = g | split: "|" %}
{% assign key = parts[1] %}
{% assign people = page[key] %}
<h2 class="ab-section" id="{{ parts[0] | slugify }}">{{ parts[0] }}</h2>
<div class="ab-grid">
  {% for p in people %}
  <article class="ab-card">
    <img src="{{ p.photo | relative_url }}" alt="Photo of {{ p.name }}" loading="lazy">
    <div class="ab-card__body">
      <h3>{{ p.name }}</h3>
      {% if p.role != "" %}<p class="ab-card__role">{{ p.role }}</p>{% endif %}
      {% if p.bio != "" %}<p class="ab-card__bio">{{ p.bio }}</p>{% endif %}
      {% if p.link %}<a class="btn btn--primary" href="{{ p.link }}">See more</a>{% endif %}
    </div>
  </article>
  {% endfor %}
</div>
{% endfor %}
