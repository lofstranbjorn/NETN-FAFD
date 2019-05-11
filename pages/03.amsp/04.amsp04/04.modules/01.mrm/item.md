---
title: 'Multi-Resolution Modelling'
media_order: 'army-blur-figurines-231014.jpg,mrm.png'
date: '04-06-2018 12:15'
body_classes: 'header-transparent header-dark'
menu: MRM
hero_classes: 'text-light parrallax title-h1h2 overlay-dark'
hero_image: army-blur-figurines-231014.jpg
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

The **NETN Multi-Resolution Modelling (MRM)** component provides a way to manage aggregation and disaggregation of simulated units and physical entities. MRM can also use the [NETN TMR](../tmr) component for transferring modelling responsibilities between federates that simulate the entity at different levels of resolution. 

* **Resolution** is defined as _the degree of detail used to represent aspects of the real world by a model_.
* **Aggregate Unit** is a model of an organizational unit with an hierarchical relationships to other units in the same organization, aggregated state information and **holdings** representing the unit's supplies, equipment and personnel.

A federate implementing a MRM Service (MRM Service Provider) use information about the unit organizational hierarchy and holdings to manage and control MRM, e.g. registering entity instances based on holdings when disaggregating an Aggregate Unit. The MRM Service Provider also manages any Transfer of Modelling Responsibilities (TMR) required as part of aggregation and disaggregation.

![](mrm.png?resize=500)

**Disaggregation** is the process changing the level of modelling of an Aggregate Unit to instead model its constituent parts as either sub-units and/or physical entities such as ground vehicles, aircraft, surface vessels etc. The disaggregation of an Aggregate Unit requires the transfer of modelling responsibility of all (non static) attributes to the MRM Service Provider. During a disaggregated state the MRM Service Provider will be responsible for updating all the aggregate unit (non static) attributes (a fully disaggregated unit is considered inactive). The MRM Service Provider registers disaggregated units and/or entities resolution entities and transfers responsibility using NETN TRM to federates with the capability of modelling at the required level of resolution.

**Aggregation** is the process of changing the level of modelling by combining constituent parts into the Aggregate Unit itself, i.e. the opposite of disaggregation. The aggregation of an Aggregate Unit involves transferring modelling responsibilities of attributes of multiple simulated entities potentially modelled by different federates. The MRM Service Provider acquires the required modelling responsibility and on completion the disaggregated entities are either deleted or inactivated. The MRM Service Provider creates/activates the Aggregate Unit and transfers the modelling responsibility to a federate capable of modelling the unit at the required level of resolution.

> **Accuracy** is defined as _the maximum allowed difference between a simulated aspect of a model and the corresponding real-world value_.
> 
> **Fidelity** is _the combination of resolution and accuracy concepts_. Higher-Fidelity means higher resolution and/or higher accuracy. Lower-fidelity less resolution and/or less accuracy.