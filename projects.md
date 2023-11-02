---
layout: page
permalink: /projects/
title: Projects
class: projects
---

{:.hidden}
# Projects

{:.lead}

<div class="grid">
  {% for project in site.data.projects %}
    {% include project.html project=project %}
  {% endfor %}
</div>

<div class="columns" markdown="1">

{% for project in site.data.projects %}
  <h2><a class="anchor" id="{{project.title}}"> {{ project.title }} </a></h2>
  <p>{{ project.description-extended }}</p>
  {% include project-extended.html project=project %}
{% endfor %}

</div>