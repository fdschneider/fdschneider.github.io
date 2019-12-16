---
layout: page
categories: blogpost
permalink: blog/2019/traitontologies/
title: Strategies for the development of community-based trait-ontologies
author: Florian D. Schneider
date: "2019-12-16 13:06:09 +0100"
teaser: '
This October, I was presenting the Ecological Trait-data Standard Vocabulary (ETS) at the Biodiversity Next conference in Leiden, Netherlands. The conference was the joint meeting of TDWG Biodiversity Standards, GBIF, DISSCO, iDigBio, CETAF and LifeWatch, and addresses issues of biodiversity data and knowledge management. The [Ecological Trait-data Standard Vocabulary (ETS)](https://besjournals.onlinelibrary.wiley.com/doi/10.1111/2041-210X.13288) and the scope of the [Open Traits Network (OTN)](https://ecoevorxiv.org/kac45/) fit in nicely.'
comments: true
disqus_identifier:
---

![](https://upload.wikimedia.org/wikipedia/commons/6/65/Naturalis_Biodiversity_Center_-_RMNH.MAM.12076.b_ven_-_Carollia_perspicillata_-_skin.jpeg)


A couple of the OTN members have been there and some are certainly more involved in the initiatives for global data standards than I am. Please read this as a rendering of my personal notes and ideas, which should be taken as very raw suggestions. The sole purpose of this draft is to spark a discussion and draft a vision for a OTN web of trait ontologies.  


During the conference, a workshop on 'Vocabularies for Values' organised by Paula Zermoglio and the TDWG Interest Group on Biodiversity Data Quality made me think about one of the tasks addressed within the OTN: facilitating the linkage of trait data to globally accessible definitions. The workshop was mostly concerned with developing controlled vocabularies of Darwin Core terms, some of which are part of the ETS. The task group on Vocabularies for Values arose from the need to facilitate the evaluation of quality of entries in DwC data, which is currently only possible after a tedious harmonization process of values. But discussions also went to the need of many participants to define vocabularies for their own project contexts.

## 0. Nomenclature

The most generic term for a list of standardised definitions of concepts is a 'terminology'. A 'controlled vocabulary', i.e. a fixed list of terms that can be used for entries in a field or as column labels.  
A 'thesaurus' is enriched by defining the relationships between terms, i.e. classes of terms or synonyms, broader or narrower terms. An 'ontology' includes a machine readable specification of the terms, concepts and relationships.
A 'standard' is a description of a best-practice, primarily in a human-readable way but if aiming for integration in data management schemes, it would also include a machine readable specification. TDWG has formulated requirements for standards in the  TDWG Standards Documentation Specification (TDWG SDS). Standards do not have to include any form of controlled vocabulary (best example is the TDGW SDS itself), but may include one or several vocabularies, thesauri or ontologies.  
The TDWG policy seems to be to speak only of a 'standard' if the document underwent a TDWG ratification process. The TDWG SDS suggests that standards should differentiate between 'normative' elements and documents and 'non-normative' elements. The prior are undergoing a ratification process for each single edit. The latter can be edited more informally, to minimize the organisational procedures for alterations that are not of any operational effect.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/0/04/Naturalis_Biodiversity_Center_-_RMNH.AVES.45518_1_-_Cotinga_cayana_%28Linnaeus%2C_1766%29_-_Cotingidae_-_bird_skin_specimen.jpeg/800px-Naturalis_Biodiversity_Center_-_RMNH.AVES.45518_1_-_Cotinga_cayana_%28Linnaeus%2C_1766%29_-_Cotingidae_-_bird_skin_specimen.jpeg)


## 1. Defining the goal for OTN

In my opinion, it is illusory to aim for a single global trait ontology, mostly for social reasons of how scientific communities work with trait data. The existing trait-based fields are communities of practice, revolving around a certain taxonomic group or functional component of ecosystems, like the soil macrofauna, grassland vegetation, or bird morphology. Also, some of these communities already have started to develop vocabularies or thesauri or more advanced semantic ontologies, like for agricultural plant traits, or vertebrate morphology, which address particular problem-centered challenges. Vocabularies could also be defined to organise data within an existing data pool, like TOP compiles trait definitions for plants based on the enormous variable input for the TRY database. Another example are initiatives that are aiming to systematically extract quantitative information on leaf dimensions from photographs.
Rather than unifying those initiatives, the OTN should aim for working towards a network of complementary but compatible controlled vocabularies, thesauri and ontologies. They can be allowed to evolve in parallel and pragmatically on the topics identified by the research communities.  The main approach here should be to work within a community of practice to develop sufficiently sharp and practical vocabularies, but with the overarching idea of trait-data within the semantic web.
These various terminologies would ideally evolve successively into a generally applicable scheme of sufficiently different, field-specific ontologies that provide terms for the particular use-cases, but also link across the domains of knowledge.

## 2. A standard for developing standards

The Open Traits Network initiative for ontologies could start with defining and publish a standard for how to define and publish trait terminologies for particular communities of practice. The aim of these field-specific terminologies would be to define unambiguous trait concepts for the given research context and problem at hand. Further the vocabularies should link, for each trait concept, the measurement and collection practice (methods of practice) with the stored values (controlled vocabularies for each trait).
The OTN standard should provide sufficient instructions to create a solid resource. It should also suggest practices of versioning of terms and the entire vocabulary, and on cross-referencing with other ontologies.

To achieve that, the standard might follow the [TDWG SDS](https://baskauf.blogspot.com/2019/03/understanding-tdwg-standards.html) and also suggest or require the vocabularies to be constructed according to the TDWG SDS. Among other things, this would define a minimum quality human readable and machine readable resources. The latter are typically written in [RDF language](https://dwc.tdwg.org/rdf/#3.7_dwc) using [SKOS schema](https://www.w3.org/2009/08/skos-reference/skos.html) and DwC or Dublin Core terms. The OTN standard could include a suggested structure for these documents.

The OTN Standard for controlled vocabularies should also classify different levels of depths of detail.
Detail may include synonyms, similar or related terms, and hierarchical relationships (broader, narrower) in the same or other ontologies. The definitions of individual terms should make use of broader  ontologies, like morphological (eg. for terms like leaf, plant, fruit, wing, egg) or units ontologies.

Finally, the Standard should provide recommendations on how to publish these trait vocabularies (these recommendations would probably be dependent on the purpose and generality of the vocabulary; see below)

![](https://upload.wikimedia.org/wikipedia/commons/8/88/Naturalis_Biodiversity_Center_-_RMNH.MOL.126642_2_-_Lambis_truncata_truncata_%28-Lightfoot-%2C_1786%29_-_Strombidae_-_Mollusc_shell.jpeg)


## 3. Quality control and ratification of vocabularies

Ratification by the TDWG for trait ontologies is unlikely, as the debated vocabularies are not of global geographic or taxonomic concern. As already discussed during the initial OTN Workshop, the OTN could implement a scheme of ratifying trait vocabularies, thesauri or ontologies.  We may differentiate between 1) simple controlled vocabularies, 2) thesauri, and 3) ontologies, and between the application level ranging from i) project specific, ii) taxon specific, and iii) global validity also define a level of maturity being in a) draft stage, b) under evaluation/testing, and c) ratified.  

The OTN could organise a database or repository to publish vocabularies (thereby also considering the use of OBO foundry), as well as a mode to assess and validate (with badges or labels), and continuously revise these ontologies (this should be minimally prescriptive about the frequency and involvement and openness of a community). Here, on the overarching level, we would also work on strengthening the cross-referencing of ontologies, e.g. by suggesting synonyms or related terms, and paths of trait inference (e.g. a statement on digits allows to infer the presence of limbs, and an assignment to vertebrata) during the ratification process.  

OTN could also think about practicality of ontologies: When is writing a new ontology justified, when is it filling an own niche, and when is it redundant because widely overlapping or included in another ontology? Also, co-existence of ontologies might be problematic if they are contradictory in their definitions of relationships between apparently compatible terms.  

![](https://upload.wikimedia.org/wikipedia/commons/thumb/7/70/Naturalis_Biodiversity_Center_-_RMNH.MAM.1068.a_lat_-_Martes_foina_foina_-_skull.jpeg/529px-Naturalis_Biodiversity_Center_-_RMNH.MAM.1068.a_lat_-_Martes_foina_foina_-_skull.jpeg)

## 4. Meta-Evaluation and utilization

At the level of OTN, we could continuously evaluate the coverage of the trait ontologies for all domains of life, for fields of research, quantify their overlap and redundancy or possible conflicts. We could also keep record of their application in published data.
With web technology existing in initiatives of the biodiversity informatics community, the network of ontologies can be patched into a meta-ontology that enables the reading of all trait datasets that have been created with one of the ontologies. However, this would require to deal with the coexistence of conflicting or incompletely overlapping terms.  
This toolchain would then potentially feed into the Essential Biodiversity Variables (EBV) initiative, which aims to link more or less systematic field survey data  with the required indicators and reports required on the policy side through an expansive system of data management. A suite of functional traits have been defined in the EBV Framework that promise key insights into the state and functioning of ecosystems ([Kissling et al. 2018 Nature Ecology & Evolution 2: 1531–1540.](https://doi.org/10.1038/s41559-018-0667-3)).
With an ontology network for traits, the trait-data cosmos would be made available to these analyses and functional indicators could be more easily derived from field data on community assemblages and systematic monitoring data.





<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">Strategies for the development of community-based trait-ontologies</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://fdschneider.de/blog/2019/traitontologies/" property="cc:attributionName" rel="cc:attributionURL">Florian D. Schneider</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

All of these ideas should be taken as suggestions. The sole purpose of this draft is to provide a first  vision  and spark a discussion for the OTN strategy towards trait ontologies.

---


Florian D. Schneider is working at ISOE Institute for Social-ecological Research, Frankfurt am Main, Germany. He investigates knowledge integration in cross-disciplinary cooperations, particularly on topics of biodiversity and insect decline due to human land use.   

Researchgate: [Florian Schneider](https://www.researchgate.net/profile/Florian_Schneider12)  

Twitter: [f_d_schneider](https://twitter.com/f_d_schneider)

Instagram: [fdschn](https://www.instagram.com/fdschn/)

---

*all photographs are public domain released by Naturalis Biodiversity Center*
