---
title: Initialization
media_order: adult-army-battle-171944.jpg
date: '04-06-2018 12:15'
body_classes: 'header-transparent header-dark'
visible: true
hero_classes: 'text-light parrallax title-h1h2 overlay-dark'
hero_image: adult-army-battle-171944.jpg
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

The **NETN Initialization** component provides a standard way of documenting and providing key data related to the initial states and relationships among units represented in a scenario. Preparation of a distributed CAX environment includes the distribution and initialization of common data including but not limited to Order of Battle (ORBAT), environment datasets and other initial scenario settings. The **Military Scenario Definition Language (MSDL)** [SISO-STD-007](https://www.sisostds.org/ProductsPublications/Standards/SISOStandards.aspx) is the core standard used by NETN to represent ORBAT and initial scenario data. 

NETN also defines the following MSDL extensions:
* Initial allocation of modelling responsibilities as additional deployment information
* Extended unit and equipment type identification based on [SISO-REF-010](https://www.sisostds.org/ProductsPublications/ReferenceDocuments.aspx) enumerations
* Representation of a unit's holdings of platform, equipment, human and other resources
* Extended description of humans to capture rank and category codes
* Embarkment added as new type status for a unit's support role to indicate that a unit or equipment is embarked on another unit.

The representation of Aggregate Units and Physical Object in NETN is based on the RPR-FOM representation with extensions to better reference data captured in MSDL. In particular a Universally Unique IDentifier (UUID) is added to all Aggregate and Physical Entities in the federation. The UUID use the same format as in MSDL and is used to provide a unique identifier of simulated objects to its corresponding scenario description in MSDL format. The RPR-FOM has been extended with subclasses for all platforms and the AggregateEntity object class to add the UUID attribute and additional information.

> The MSDL standard is currently undergoing revision and new versions of this standard will impact how initialization data is represented in future versions of NETN FAFD.
> Representation of task organization, internal organizational relationships and relationships between different organizations may in some situations need to change dynamically during execution of a federation. Future versions of the NETN Initialization module will provide standards for both initialization and dynamic update of this type of  information.

