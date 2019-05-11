---
title: 'Logistics Module'
media_order: 'aeroplane-aircraft-airplane-54098.jpg,log.png'
date: '04-06-2018 12:15'
body_classes: 'header-transparent header-dark'
visible: true
hero_classes: 'text-light parrallax title-h1h2 overlay-dark'
hero_image: aeroplane-aircraft-airplane-54098.jpg
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

The **Logistics** module defines patterns used by federates to negotiate and deliver logistics simulation as a service during runtime. All the NETN logistics patterns use the concept of a service provider and a service consumer that are modelled in two different federates. The federates use the NETN logistics pattern to manage the service negotiation and delivery using HLA interactions and in some cases other NETN patterns such as NETN TMR.

The Logistics services include:

* **Supply** service provided by a facility, a unit or entity with consumable materials supply capability. Resources are transferred from the federate modelling the service provider to the federate modelling the service consumer.
* **Storage** service provided by a facility, a unit or entity with consumable materials storage capability. Resources are transferred from the federate modelling the service consumer to the federate modelling the service provider.
* **Repair** service can be performed on equipment (i.e. non-consumables items such as platforms) by facilities or units capable of performing the requested repairs. Modelling responsibility is by default not transferred from federate modelling the service consumer (e.g. a damaged platform) to the application with modelling responsibility for the service provider (i.e. repairing facility). However, modelling responsibility can be transferred with the inclusion of the Transfer of Modelling Responsibility (TMR) pattern.
* **Transport** service is provided by a facility, a unit or entity with transportation capability of non-consumable materials, e.g. units and platforms. Transported units are embarked, transported and disembarked. Modelling responsibility is by default not transferred from the federate modelling the service consumer (transported unit) to the federate modelling the service provider (transporter). However, modelling responsibility can be transferred with the inclusion of the Transfer of Modelling Responsibility (TMR) pattern. Units or platforms being transported are modelled as inactive during transportation.

![](log.png?resize=500)

> Examples of uses:
> 
> * Supply of fixed wing aircraft in airports or during aerial refueling.
> * Supply of helicopters in assembly areas.
> * Repair of damaged platforms by a maintenance unit without changing platform's location.
> * Maintenance of damaged platforms previously deposited in a facility.
> * Transport of units, platforms, and humans by train, ship, or aircraft.
> * Embarkment and disembarkment of units.
> 