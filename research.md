---
permalink: /research/
layout: page
title: Current Research
---

## Biodiversity and society

In my current work projects, I am interpreting biodiversity from a systemic point of view that assumes that individual organisms form populations and communities in complex interactions and by doing so, produce ecosystem functions and services that are of interest to human wellbeing. Vice versa, anthropogenic pressures such as land use change and climate change are going to affect ecosystem functions only via affecting individual interactions in the first place.
I am involved in projects within the framework of the Biodiversity Exploratories, which investigate trait composition at the community level.

The role that science takes in the process of negotiating biodiversity values are key. In my collaboration with ISOE, Frankfurt, and the linguistics department at TU Darmstadt, I am looking into the ways of knowledge transfer from scientific communities into the public.

### Collaborators

[Markus Fischer](http://www.botany.unibe.ch/planteco/index.php), [Pete Manning](http://www.bik-f.de/root/index.php?page_id=1051), [Nico Blüthgen](https://www.econetlab.net/prof-dr-nico-bluethgen),
[Nina Janich](https://www.linglit.tu-darmstadt.de/index.php?id=janich), [Alexandra Lux](http://www.isoe.de/das-isoe/team/mitarbeitende/alexandra-lux/)

### Relevant publications

<div class = "publist">
  <ul>
  {% for publication in site.pages %}
    {% if publication.categories contains 'article' and publication.tag contains 'biodiversity'%}
     <li>{% include publication.html %} </li>
    {% endif %} 			
  {% endfor %}

  {% for project in site.pages %}
    {% if project.categories contains 'project' and project.tag contains 'biodiversity'%}
    <li> {% include project.html %} </li>
    {% endif %} 			
  {% endfor %}
  </ul>
</div>

## Catastrophic Shifts in Drylands

The [CASCADE project](http://www.cascade-project.eu/)[^1] investigates sudden regime shifts in dryland ecosystems, particularly in the Mediterranean. Arid ecosystems are suffering from climatic and anthropogenic pressures. Those combined stressors can lead to the permanent loss of vegetation. My PostDoc in Montpellier was dedicated to the development of models that reproduce these shifts. Such models serve the evaluation of indicators of early warning as well as the development of sustainable land use strategies.

Many landscapes in the mediterranean are intensely grazed by sheep or goats. We developed a model to estimate how grazing in addition to abiotic effects changes the face of a landscape in terms of vegetation cover and patch structure. The cellular automata model is based on a model of local facilitation developed by Sonia Kéfi[^2].
Previous landscape approaches on the effect of grazing used a rather abstract conception. Grazing intensity was defined to increase individual plant mortality linearly. In nature, the grazing pressure on an individual plant depends on the vegetation cover non-linearly (functional response). The precise shape of this non-linear function depends on many things, like the foraging behaviour and body mass of the grazers, but in rangelands, also on the management decisions of the shepperd and the governance regime of the region. We are aiming at a conceptional framework that allows a meaningful translation between model and metrics of land use management.

[^1]:CASCADE is funded by the Framework Programme 7 of the European Comission.

[^2]:Kéfi, S., M. Rietkerk, M. van Baalen & M. Loreau. 2007. [Local facilitation, bistability and transitions in arid ecosystems](http://www.sciencedirect.com/science/article/pii/S0040580906001250). *Theoretical Population Biology*. 71(3): 267-400.


### Collaborators

[Sonia Kéfi](http://sonia.kefi.fr), [Alain Danet](http://www.biodicee.univ-montp2.fr/index.php/alain-danet), [Mara Baudena](http://www.uu.nl/staff/MBaudena), [Max Rietkerk](http://www.uu.nl/staff/MGRietkerk), [Susanna Bautista](http://imem.ua.es/en/about-us/susana-bautista-aguilar.html), [Luuk Fleskens](https://www.wageningenur.nl/en/Persons/Fleskens.htm), [Diana Sietz](https://www.wageningenur.nl/en/Persons/D-Diana-Sietz.htm)

### Relevant publications

<div class = "publist">
  <ul>
  {% for publication in site.pages %}
    {% if publication.categories contains 'article' and publication.tag contains 'cascade'%}
     <li>{% include publication.html %} </li>
    {% endif %} 			
  {% endfor %}

  {% for project in site.pages %}
    {% if project.categories contains 'project' and project.tag contains 'cascade'%}
    <li> {% include project.html %} </li>
    {% endif %} 			
  {% endfor %}
  </ul>
</div>


## Predator diversity and ecosystem function

Many aspects of predation can be estimated from the species' average individual body mass. This allows the prediction of quality and quantity of interaction strengths in natural food webs. The network approach bridges the physiological properties of individuals and dynamic interactions within complex, multi-predator communities and provides a mechanistic view on ecosystems.

This simplification is quite radical but incredibly useful.
Since body mass is quite easy to measure in the field or in experiments, this allows us to interpolate known physiological or ecological properties for any species. For instance, we can estimate a species' food uptake, it's movement speed or guess it's role in the food chain.
By making these rough assumptions, we can even project the dynamic development of an entire community over time or estimate the importance of particular species or their risk of extinction. Of course not to the point and not with absolute certainty, but more universal and with less effort than with any other method.

### Collaborators

[Ulrich Brose](https://www.idiv.de/de/das_zentrum/mitarbeiterinnen/mitarbeiterdetails/eshow/brose-ulrich.html), [Christian Guill](https://www.uni-potsdam.de/ibb/arbeitsgruppen/ordentliche-professuren/oekologie/mitarbeit/guill.html), [Gregor Kalinkat](http://www.igb-berlin.de/staff-igb.html?per_page=0&search=lastname&for=kalinkat&show=662), [Björn C. Rall](https://www.idiv.de/de/das_zentrum/mitarbeiterinnen/mitarbeiterdetails/eshow/rall-bjoern.html)

### Relevant publications

<div class = "publist">
  <ul>
  {% for publication in site.pages %}
    {% if publication.categories contains 'article' and publication.tag contains 'allometry'%}

     <li>{% include publication.html %}  </li>

    {% endif %} 			
  {% endfor %}

  {% for project in site.pages %}
    {% if project.categories contains 'project' and project.tag contains 'allometry'%}
    <li>{% include project.html %}    </li>
    {% endif %} 			
  {% endfor %}
  </ul>
</div>

---
