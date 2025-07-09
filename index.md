---
layout: page
title: "Home"
class: home
mathjax: true
---

# Hi, I'm Shelby Cox.

<div class="columns" markdown="1">

<div class="intro" markdown="1">
  I am a postdoc in the <a href="https://www.mis.mpg.de/nonlinear-algebra">Non-Linear Algebra Group at the Max Planck Institute for Mathematics in the Sciences</a>. 
  I work in algebraic statistics and use tools from tropical geometry, algebraic geometry, commutative algebra, and combinatorics. I am particularly interested in problems in phylogenetics.
  
  I completed my Ph.D. at the University of Michigan with <a href="https://websites.umich.edu/~speyer">David Speyer</a> in May 2024. I received my B.S. in mathematics and B.A. in linguistics from UMass Amherst, where I was advised by <a href="https://people.umass.edu/~tevelev">Jenia Tevelev</a>.

  Here is my <a href="/assets/cox_cv.pdf">CV</a>.

  I am organizing a mini-symposium on Phylogenetic Networks at SIAM-AG 2025 together with Max Hill, Annachiara Korchmaros, and Danai Deligeorgaki. See <a href="https://meetings.siam.org/sess/dsp_programsess.cfm?SESSIONCODE=84216">here</a> for more details.
</div>

<div class="me" markdown="1">
<picture>
  <source srcset='/images/shelby-photo.jpeg' type='image/webp' />
  <img
    src='/shelby-photo.jpeg'
    alt='photo of Shelby'>
</picture>

{:.no-list}
* <a href="mailto:{{ site.email }}">{{ site.email }}</a>
* F3 04
</div>

</div>

## Recent <a href="{{ "/publications/" | relative_url }}">Papers</a>
<a href="https://arxiv.org/a/cox_s_1.html"><i class="fab fa-scroll" aria-hidden="true"></i> ArXiv</a>
<a href="https://scholar.google.com/citations?user=dFznJ9gAAAAJ&hl=en&oi=ao"><i class="fab fa-google" aria-hidden="true"></i> Google Scholar</a>

<div class="featured-publications">
  {% assign sorted_publications = site.publications | sort: 'year' | reverse %}
  {% for pub in sorted_publications %}
    {% if pub.highlight %}
      <a href="{{ pub.pdf }}" class="publication">
        <strong>{{ pub.title }}</strong>
        <span class="authors">{% for author in pub.authors %}{{ author }}{% unless forloop.last %}, {% endunless %}{% endfor %}</span>.
        <br>
        <i>{% if pub.status %}({{ pub.status }}){% endif %} {% if pub.venue %}{{ pub.venue }}, {% endif %}{{ pub.year }}</i>.
        {% for award in pub.awards %}<br/><span class="award"><i class="fas fa-{% if award == "Best Paper Award" %}trophy{% else %}award{% endif %}" aria-hidden="true"></i> {{ award }}</span>{% endfor %}
      </a>
    {% endif %}
  {% endfor %}
</div>

<a href="{{ "/publications/" | relative_url }}" class="button">
  <i class="fas fa-chevron-circle-right"></i>
  Show All Papers
</a>

## Featured <a href="{{ "/projects/" | relative_url }}">Projects</a>

<div class="featured-projects">
  {% assign sorted_projects = site.data.projects | sort: 'highlight' %}
  {% for project in sorted_projects %}
    {% if project.highlight %}
      {% include project.html project=project %}
    {% endif %}
  {% endfor %}
</div>
<a href="{{ "/projects/" | relative_url }}" class="button">
  <i class="fas fa-chevron-circle-right"></i>
  Show More Projects
</a>

