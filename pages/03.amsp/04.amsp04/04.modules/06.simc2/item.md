---
title: SimC2
media_order: 'e3.jpg,simc2.png'
date: '04-06-2018 12:15'
body_classes: 'header-transparent header-dark'
visible: true
hero_classes: 'text-light parrallax title-h1h2 overlay-dark'
hero_image: e3.jpg
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

The purpose of the **Simulation-C2 Interoperability (SimC2)** component is to automate the process of interaction between C2 systems and simulations. NETN SIM-C2 relies on the Coalition Battle Management Language (C-BML) and provides a way to represent C-BML messages in a federated simulation environment without the need to implement peer-to-peer connections between C-BML services and individual simulation systems. Although, an individual simulation can use a C-BML interface to interact directly with a C-BML server the preferred NETN approach is to have a single C-BML gateway that interacts with the NETN federation regardless.

The C-BML language is a high level language representing orders, reports and requests. Some simulations can process this information directly and perform meaningful modelling of activities but most entity-level simulations are task oriented and operate on a significantly lower level. The NETN SimC2 concept does not exclude the use of simulations that can process C-BML directly but identifies the need for components that can perform both aggregation and disaggregation of orders, reports and requests into smaller elements suitable for entity-level simulations. Lower-level tasks can be used to control simulations in the NETN federation using the [Simulation Control](../lbml) component.  

![](simc2.png?resize=500)

To avoid potential mistakes, the SimC2 C-BML FOM module has been named NETN-HCBML FOM module and the Simulation Control module has been named NETN-LBML FOM module. 

The NETN HCBML FOM module focuses on transportation of C-BML messages and is basically a wrapper of C-BML messages. The C-BML Orders and Requests are represented using its C-BML XML format without modification. Some information from the message header are extracted and used for routing of the message. Reports and acknowledgements are represented as interactions with parameters based on C-BML. The following reports are supported:

* TaskReport: Progress of current task
* SituationReport: Force Tracking information
* LogReport: Logistics report
