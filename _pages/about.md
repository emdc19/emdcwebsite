---
permalink: /
#title: "Academic Pages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
## About Me

I am a Ph.D. candidate in Geomechanics in the Department of Civil and Environmental Engineering at Stanford University, and expect to graduate in June 2025. My research interests lie in the mechanics and failure of geomaterials across spatial scales using both mechanics-based and data-driven approaches with applications in geophysics, geomechanics, and geotechnics. In my past work, I developed a meshfree computational framework based on the smoothed particle hydrodynamics (SPH) method well-suited for modeling the deformation of fluid-saturated geomaterials over large strains. Additionally, I am interested in discontinuum modeling of granular materials and the discrete element method (DEM), which I have also used in my research. In addition to my doctoral studies, I hold a M.S. degree in Civil Engineering with specialization in Geomechanics from Stanford University and an A.B. in Geosciences from Princeton University. This webpage summarizes some of my past and current research projects (under construction), while providing links to my CV, publications (Google Scholar page), and other personal pages.

## News

{% for item in site.data.news %}
<div class="news-item">
  <h3 class="news-title"><a href="{{ item.url }}">{{ item.title }}</a></h3>
  <div class="news-date">{{ item.date }}</div>
  <p class="news-body">{{ item.body }}</p>
</div>
{% endfor %}



