---
layout: page
title: Projets Maker
permalink: /maker-projects/
description: Projets de fabrication, prototypage, impression 3D, mécanique et électronique.
nav: true
nav_order: 2
horizontal: false
---

<p>
  Projets personnels mêlant fabrication, mécanique, CAO, impression 3D,
  électronique et programmation.
</p>

<p>
  Une grande partie de ces réalisations part de besoins concrets rencontrés, améliorer une machine, fabriquer une pièce inexistante,
  automatiser une fonction ou simplement expérimenter une idée.
</p>

<div class="projects">

  {%- assign maker_projects = site.projects | where: "type", "maker" | sort: "importance" -%}

  {% if page.horizontal %}
    <div class="container">
      <div class="row row-cols-2">

        {%- for project in maker_projects -%}
          {%- unless project.hidden -%}
            {% include projects_horizontal.html %}
          {%- endunless -%}
        {%- endfor -%}

      </div>
    </div>

  {% else %}

    <div class="grid">

      {%- for project in maker_projects -%}
        {%- unless project.hidden -%}
          {% include projects.html %}
        {%- endunless -%}
      {%- endfor -%}

    </div>

  {% endif %}

</div>
