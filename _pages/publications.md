---
layout: page
permalink: /publications/
title: Publications
description: Publications in reversed chronological order.
nav: true
nav_order: 2
---
 
<!-- _pages/publications.md -->
<div class="publications">

<h1>preprints</h1>

{% bibliography -f preprints %}

<h1>conference &amp; journal articles</h1>

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h1>technical reports &amp; short papers</h1>

{% bibliography -f reports %}

</div>

## Other contributions

@article{rincon2023quien,
  title={Who would bear a reduction of the corporate income tax?},
  author={{Rincon Castro}, Hernan and {Angel Mojica}, Juan Pablo},
  journal={Borradores de Econom{\'\i}a; No. 1260},
  year={2023},
  publisher={Banco de la Rep{\'u}blica de Colombia},
  doi = {10.32468/be.1260},
  abstract = {The objective of the study is to model and determine the tax incidence of a reduction in the corporate income tax in Colombia. To meet this objective, a dynamic and stochastic general equilibrium model DSGE of a closed economy with heterogeneous households and two types of capital is used. These make it possible to easily include the skill-premium and the complementarity of capital with labor skills (capital-skill complementarity), variables that are determinants of changes in the distribution of income and the welfare of the different types of households. The results indicate that a reduction in the corporate income tax increases economic growth but generates unwanted redistributive effects and is not optimal in the Pareto sense, since, depending on the type of fiscal consolidation instrument used, it can enlarge the distribution income gap and negatively affect the welfare of those households with financial constraints and less qualified. To achieve at the same time a lower tax burden on companies and greater economic growth, but with more equity and welfare for all households, alternative instruments are required},
  html= {https://doi.org/10.32468/be.1260},
  bibtex_show={true},
  preview={banrep.png}
}
