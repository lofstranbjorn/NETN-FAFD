---
title: Concepts
taxonomy:
    category:
        - docs
visible: true
---

In our use-case we will represent organizational units such as a Brigate or Battalion. A Unit is an aggregate concept consisting of resources and have aggregate capabilties to perform certain activities. A unit can also be part of an organizational structure with relationships to superior and subordinate units. Furthermore, the organization to which the unit belong can have some relationship with other organizations.

The unit resources are of different kind and the available amount of resources and the units ability to utilize sub-units capabilities will affect the unit's aggregated ability to perform activities. 

There are basically two (2) approaches to simulate an aggregate unit.
1. Model and Simulate the unit's individual resources and sub-units and then represent the unit by combining the result
2. Model and Simulate on an aggregate level and do not explicitly represent individual resources and sub-units

However, in many cases the most common approach is to allow a combination if the two approaches where some individual resources and some sub-units are simulated while others are modelled at an aggregate level. Furthermore, the selection of which resources or sub-units to model individually may change  dynamically during the execution of an exercise. This behaviour is called Multi-Resolution Modelling (MRM), Aggregation/Disaggregation, or unit divide/join and will be explored later in this tutorial.

