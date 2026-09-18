---
layout: page
title: Projets Maker
permalink: /maker-projects/
nav: true
nav_order: 2
horizontal: false
---

<p>
Sélection de projets mêlant mécanique, CAO, impression 3D, électronique et programmation. La plupart sont nés d’un besoin d’atelier ou d’une envie d’expérimenter.
</p>

<p>
  Les projets présentés ici ne constituent qu’une sélection.
  Je documente également d’autres réalisations sous forme de pas-à-pas sur
  <a href="https://www.lairdubois.fr/@bingods/pas-a-pas" target="_blank" rel="noopener noreferrer">
    <strong>L’Air du Bois</strong>
  </a>,
  je partage mes modèles destinés à l’impression 3D sur
  <a href="https://makerworld.com/fr/@BingoDS/upload" target="_blank" rel="noopener noreferrer">
    <strong>MakerWorld</strong>
  </a>,
  et mes autres créations permettent de découvrir une facette plus large de mon travail,
  notamment autour du bois et du mobilier.
  <strong> Les liens vers ces contenus sont disponibles plus bas sur la page. </strong>
</p>

---

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

---

## Pour aller plus loin

<div class="maker-platforms">

  <a
    class="maker-platform"
    href="https://www.lairdubois.fr/@bingods/pas-a-pas"
    target="_blank"
    rel="noopener noreferrer"
  >
    <span class="maker-platform-title">L’Air du Bois</span>
    <span class="maker-platform-description">
      Pas-à-pas, restaurations et documentation de projets
    </span>
    <span class="maker-platform-arrow">↗</span>
  </a>

  <a
    class="maker-platform"
    href="https://makerworld.com/fr/@BingoDS/upload"
    target="_blank"
    rel="noopener noreferrer"
  >
    <span class="maker-platform-title">MakerWorld</span>
    <span class="maker-platform-description">
      Modèles et pièces fonctionnelles pour l’impression 3D
    </span>
    <span class="maker-platform-arrow">↗</span>
  </a>

  <a
    class="maker-platform"
    href="https://www.lairdubois.fr/@bingods/creations"
    target="_blank"
    rel="noopener noreferrer"
  >
    <span class="maker-platform-title">Créations</span>
    <span class="maker-platform-description">
      Mobilier, travail du bois et autres réalisations
    </span>
    <span class="maker-platform-arrow">↗</span>
  </a>

</div>
