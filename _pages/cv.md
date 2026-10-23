---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* **Ph.D.**, Institute of Automation, Chinese Academy of Sciences (CASIA), 2026 – present
* **B.Eng.**, Electronic Engineering, College of Information and Electrical Engineering, China Agricultural University, 2022 – 2026

Experience
======
* **Research Intern**, SenseNova, SenseTime, Sep. 2026 – present

Research Interests
======
* Unified multimodal models for understanding and generation
* Efficient foundation-model architectures
* Representation learning

Publications
======
{% for category in site.publication_category %}
  {% assign shown = false %}
  {% for post in site.publications reversed %}
    {% if post.category != category[0] %}{% continue %}{% endif %}
    {% unless shown %}<h3>{{ category[1].title }}</h3><ul>{% assign shown = true %}{% endunless %}
    {% include archive-single-cv.html %}
  {% endfor %}
  {% if shown %}</ul>{% endif %}
{% endfor %}
