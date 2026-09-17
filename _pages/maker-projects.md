---
layout: page
title: Projets Maker
permalink: /maker-projects/
nav: true
nav_order: 2
horizontal: false
---

<p>
  Je conçois principalement des objets et des systèmes destinés à répondre à
  des besoins concrets : améliorer une machine, fabriquer une pièce inexistante,
  automatiser une fonction ou expérimenter une idée.
</p>

<p>
  Ces projets me permettent de faire dialoguer
  <strong>fabrication et informatique</strong> :
  mécanique, CAO, impression 3D, travail du bois, électronique,
  microcontrôleurs et programmation. La démarche reste généralement la même :
  <strong>concevoir, fabriquer, tester, corriger et recommencer</strong>
  jusqu’à obtenir une solution fonctionnelle.
</p>

<p>
  Les projets présentés ici ne constituent qu’une sélection.
  Je documente également d’autres réalisations sous forme de pas-à-pas sur
  <strong>L’Air du Bois</strong>, je partage mes modèles destinés à l’impression 3D
  sur <strong>MakerWorld</strong>, et mes autres créations permettent de découvrir
  une facette plus large de mon travail, notamment autour du bois et du mobilier.
  Les liens vers ces contenus sont disponibles plus bas sur la page.
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
