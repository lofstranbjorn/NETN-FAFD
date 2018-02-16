---
title: Overview
taxonomy:
    category:
        - docs
visible: true
---

The NATO Education and Training Network (NETN) Federation Architecture and FOM Design (FAFD)
document is a reference document intended to provide architecture and design guidance for developing
distributed simulation and training systems. 

Current version of the NETN FAFD is published by NATO as STANREC 4800 and is publically available. 

In this documentation the main focus is use of the NETN FAFD when designing, implementing and executing distributed 
federated simulations using the IEEE 1516 **High-Level Architecture** (HLA) as the core technical interoperability standard and the NETN 
FAFD **Federation Object Model** (FOM) Modules as the associated information exchange object model. 

For details on HLA we recommend the following free [HLA Tutorial](http://www.pitchtechnologies.com/hlatutorial/).

## Quick Intro to the Lingo

An HLA **Federation** is a loosely coupled simulation system of systems where the system elements (**Federates**) interact using communication services provided by an runtime infrastructure component (**RTI**) through open well defined and standardized interfaces (**HLA**) and APIs. A **Federation Object Model (FOM)** specifies the type of data exchanged in the federation and is separate from the services used for sending the data making the RTI and HLA simulation domain agnostic. A **Federation Agreement** is a specification of federates' modelling responsibilities and how the HLA Services and a FOM should be applied to create a **Synthetic Environment** that is valid with respect to the overall purpose of the federation.

PICS
