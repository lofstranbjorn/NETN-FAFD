---
title: CBRN
media_order: danger-daylight-dry-340926.jpg
date: '04-06-2018 12:15'
body_classes: 'header-transparent header-dark'
visible: true
hero_classes: 'text-light parrallax title-h1h2 overlay-dark'
hero_image: danger-daylight-dry-340926.jpg
blog_url: /blog
show_sidebar: false
show_breadcrumbs: false
show_pagination: false
continue_link: true
content:
    items: '@self.children'
    limit: '5'
    order:
        by: date
        dir: desc
    pagination: '1'
    url_taxonomy_filters: '1'
---

The **Chemical, Biological, Radiological and Nuclear (CBRN)** component to perform CBRN dispersion calculations and the dissemination of information about the dispersion effects on entities and the environment. The component specifies the use of a CBRN Federate to manage some of the CBRN related modelling.

The CBRN component consists of five parts:

1. **Source Release:**  A _CBRN Release_ interaction is published in the federation to trigger the CBRN Federate to start simulation of the release. The interaction defines all of the information required to model a CBRN source release.
2. **Detectors:** Detector properties is represented as a _CBRN Detector_ objects and detections are published as _CBRN Detector Alarm_ interactions. Sensor concentration readings is published using the _CBRN Sensor_ object and _CBRN Sensor Update_ interactions. 
3. **CBRN Effects:** The _CBRN Human_ object class extends the representation of humans to include casualty state attributes. _TriageLevel_ uses the NATO representation of triage category scores and _IPE Type_ denotes the level of Individual Protective Equipment (IPE) that the unit is wearing according to Nuclear, Biological and Chemical (NBC) dress states. A _CBRN Casualty_ interaction is also used to send notifications of casualty state change. Extensions to NETN Platform classes are also included to represent contaminated materials.
4. **Protective Measures:** This part include both modelling of CBRN treatments and the modelling the level of  individual (IPE) and collective CBRN protection equipment (COLPRO). 
5. **Hazard Area:** Representation of a contamination area used by simulation to model CBRN effects. It can be the output from a hazard prediction algorithm (a warning area defined in Allied Tactical Publication (ATP-45) or output from a dispersion model (contours).
 
 
> Note that meteorological information and CBRN material properties are not part of the current NETN FAFD specification.