---
layout: page
title: Projets web
permalink: /web-projects/
description: Applications et projets réalisés en développement web.
nav: true
nav_order: 3
horizontal: false
---

<p>
  Projets réalisés lors de ma formation au Wagon et dans le cadre de mes
  expérimentations personnelles en développement web.
</p>

<p>
  Technologies principalement utilisées :
  <strong>Ruby on Rails, JavaScript, HTML/CSS, PostgreSQL, API et Git</strong>.
</p>

<div class="projects">

  {%- assign web_projects = site.projects | where: "type", "web" | sort: "importance" -%}

  {% if page.horizontal %}
    <div class="container">
      <div class="row row-cols-2">

        {%- for project in web_projects -%}
          {%- unless project.hidden -%}
            {% include projects_horizontal.html %}
          {%- endunless -%}
        {%- endfor -%}

      </div>
    </div>

  {% else %}

    <div class="grid">

      {%- for project in web_projects -%}
        {%- unless project.hidden -%}
          {% include projects.html %}
        {%- endunless -%}
      {%- endfor -%}

    </div>

  {% endif %}

</div>
