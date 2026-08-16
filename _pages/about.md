---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
{% include base_path %}

![Lab logo]({{ base_path }}/images/lablogoTrans.png)

Welcome to the **del Castillo Research Group** at **Northeastern University**, led by Dr. Enrique M. del Castillo. Our objective as a research group is to further
fundamental understanding of the mechanics and physics governing **complex materials**, **geosystems**, and harnessing this knowledge for solving engineering and geophysical challenges in relation to the built environment. 

From a methodology standpoint, in addition to developing computational methods, we use simulation and experimentation to probe and
improve mechanistic theory, and to create **computational digital twins** of geomaterials and earth structures. We utilize the computational resources from Northeastern's **Explorer cluster**, located in the Massachusetts Green High Performance Computing Center (MGHPCC) and also steward the new **Geotechnical and Sustainable Materials Laboratory** space at Northeastern University, which will include modern material testing and geotechnical equipment, as well as high-velocity optical imaging for DIC analysis.

By **complex materials** we refer to both natural and engineered materials which exhibit heterogeneity, evolving microstructures, multiple phases, internal interfaces, nonlinear/inelastic behavior, localized failure and fracture, and coupled physical processes. This includes most geomaterials, porous materials, and granular media, which are the second most abundant type of material on Earth.

By **geosystems** we tackle problems spanning geomechanics, structural geology, geotechnical engineering, geotechnical engineering, geophysics, and geohazards, where the mechanics of Earth materials governs processes across scales—from grain-scale interactions and localized deformation to faults, landslides, subsurface systems, and other large-scale geological and engineered systems.

---

### Overview of Research

The del Castillo Research Group focuses on four interconnected areas:

![Research framework1]({{ base_path }}/images/stages2.png)

![Research framework2]({{ base_path }}/images/scale2.png)



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
