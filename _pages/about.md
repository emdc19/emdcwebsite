---
permalink: /
title: "The del Castillo Research Group"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
{% include base_path %}

**Welcome to our lab website!!** 👋😊

![Lab logo]({{ base_path }}/images/lablogo.png)

Welcome to the del Castillo Research Group at Northeastern University, led by Dr. Enrique M. del Castillo. Our research explores the mechanics and physics of granular and porous media—soil, rock, ice, and snow—using computational and experimental methods, with a focus on natural hazards, geotechnics, and geomechanics across spatial scales.

Since granular materials are the second most abundant type of material on Earth, understanding how they deform, localize, and fail has broad societal benefit—from earthquake hazard mitigation to the design of resilient infrastructure. Our work bridges continuum, discrete, and data-driven computational methods with field and experimental data to advance this understanding.

---

### Overview of Research

The del Castillo Research Group focuses on four interconnected areas:

![Research framework]({{ site.baseurl }}/images/research-framework.png)



### 1. 🌍 Meshfree Computational Modeling of Geomaterials

We develop meshfree computational frameworks, including smoothed particle hydrodynamics (SPH), to model large-deformation, coupled hydromechanical problems in geotechnics and geomechanics.

### 2. 🌋 Structural Geology, Tectonics, and Volcanology

We model large-deformation tectonic and volcanic processes, including fault rupture, accretionary wedge formation, and compaction band propagation in porous rock.

### 3. ⚡ Geomaterials & Geomechanics for Sustainable Energy Infrastructure

We study the mechanics of geomaterials relevant to energy storage, extraction, and critical infrastructure resilience.

### 4. 💥 Nonlinear Mechanics and Physics of Dynamic Fracture

We investigate the fundamental mechanics of fracture and friction in geomaterials, coupling simulation with experimentation to test mechanistic theory.

If you share our vision for advancing resilient, sustainable infrastructure through geomechanics, we would love to hear from you — check out the Research Projects page for more detail, and stay tuned for opportunities to join the group.

## News

{% for item in site.data.news %}
<div class="news-item">
  {% if item.image %}
  <div class="news-item__image">
    <img src="{{ item.image.src }}" alt="{{ item.image.alt }}">
  </div>
  {% endif %}
  <div class="news-item__content">
    <h3 class="news-title">{{ item.title }}</h3>
    <div class="news-date">{{ item.date }}</div>
    <p class="news-body">{{ item.body }}</p>
    {% if item.url %}
    <a class="news-readmore" href="{{ item.url }}">Click to see more</a>
    {% endif %}
  </div>
</div>
{% endfor %}
