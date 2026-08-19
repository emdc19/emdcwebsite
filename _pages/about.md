---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
{% include base_path %}

<img src="{{ base_path }}/images/lablogoTrans" alt="del Castillo Research Group logo" class="homepage-logo">

Welcome to the **del Castillo Research Group** at **Northeastern University**, led by Dr. Enrique M. del Castillo. Our objective as a research group is to further
fundamental understanding of the mechanics and physics governing **complex materials** and **geosystems**, and harnessing this knowledge for solving engineering and geophysical challenges in relation to the built environment. 

From a methodology standpoint, in addition to developing computational methods, we use simulation and experimentation to probe and
improve mechanistic theory, and to create **computational digital twins** of geomaterials and earth structures. We utilize the computational resources from Northeastern's **Explorer cluster**, located in the Massachusetts Green High Performance Computing Center (MGHPCC) and also steward the new **Geotechnical and Sustainable Materials Laboratory** space at Northeastern University, which will include modern material testing and geotechnical equipment, as well as high-velocity optical imaging for DIC analysis.

By **complex materials** we refer to both natural and engineered materials which exhibit heterogeneity, evolving microstructures, multiple phases, internal interfaces, nonlinear/inelastic behavior, localized failure and fracture, and coupled physical processes. This includes most geomaterials, porous materials, and granular media, which are the second most abundant type of material on Earth.

By **geosystems** we tackle problems spanning geomechanics, structural geology, geotechnical engineering, geotechnical engineering, geophysics, and geohazards, where the mechanics of Earth materials governs processes across scales—from grain-scale interactions and localized deformation to faults, landslides, subsurface systems, and other large-scale geological and engineered systems.

**We are currently recruiting two fully-funded PhD students to join our group**. For more information please see the Opportunities tab. We also welcome inquiries from prospective postdoctoral researchers and other opportunities for collaboration. If our research interests overlap with yours, please feel free to reach out.

---

### Overview of Research

The del Castillo Research Group focuses on four main interconnected research thrusts:

### 1. 🌍 Post-Failure Modeling of Natural Hazards and Engineered Structures

Failure initiation is often only the beginning - the subsequent large-deformation response ultimately governs the severity and extent of natural hazards. We develop meshfree computational frameworks, including smoothed particle hydrodynamics (SPH), that can handle the relevant large-deformation, as well as multiphysics or coupled hydromechanical conditions.

### 2. 🌋 Large-Deformation Structural Geology, Tectonics, and Volcanology

Understanding how deformation accumulates and reorganizes geological systems is central to explaining the emergence and evolution of large-scale tectonic and volcanic structures. Our research uses mechanics-based computational models to investigate these large-deformation processes and uncover the physical mechanisms that govern the evolution of geological systems

### 3. ⚡ Geomaterials & Geomechanics for Sustainable Energy Infrastructure

We study the mechanics of geomaterials relevant to energy storage, resource extraction, and sustainable energy infrastructure, with particular emphasis on the formation and evolution of compaction bands and faults, their influence on permeability and fluid transport, and their implications for subsurface applications such as carbon sequestration.

### 4. 💥 Nonlinear Mechanics and Physics of Dynamic Fracture

We study dynamic fracture, with particular emphasis on crack initiation, propagation, branching, crack interaction, and friction, as well as how stress waves and energy transport govern the evolution of rapidly propagating fractures. We use both experimental and computational approaches, with particular emphasis on developing and improving phase field fracture formulations and consider applications in engineered materials and structures as well as earthquake processes.

Put together, these areas of study help us understand the performance and, critically, the failure of materials as a dynamically evolving process—spanning the initiation and localization of deformation, the propagation and interaction of discrete fractures, and ultimately catastrophic collapse and large-deformation behavior.

<div class="research-framework-crop">
  <img src="{{ base_path }}/images/stages2.png" alt="Failure across stages diagram">
</div>

Likewise, we seek to understand and ultimately reliably predict material behavior and failure as an interconnected process across spatial scales, linking micromechanical processes at the grain scale to specimen-scale behavior, localization and fracture at the mesoscale, and lastly system-scale geotechnical, geological, and geophysical processes.

<div class="research-framework-crop">
  <img src="{{ base_path }}/images/scale2.png" alt="Failure across stages diagram">
</div>

For more details, please check the Research Projects tab.



---

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
