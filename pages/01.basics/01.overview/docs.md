---
title: Basics
taxonomy:
    category:
        - docs
visible: true
---

The NATO Education and Training Network (NETN) Federation Architecture and FOM Design (FAFD)
document is a reference document intended to provide architecture and design guidance for developing distributed simulation and training systems. 

The NETN FAFD maintained and published by NATO as an Allied Modelling and Simulation Publication (AMSP-04) and is covered by NATO STANREC 4800. The document and associated data files are publically available for download.

In this tutorial the focus is the use of the NETN FAFD when designing, implementing and executing distributed federated simulations using IEEE 1516 High-Level Architecture (HLA) as the core technical interoperability standard and with the NETN FAFD Federation Object Model (FOM) Modules as the information exchange object model. 

! NETN FAFD is based on the RPR-FOM v2.0 and any RPR-FOM based Federate is per definition NETN compliant. 
! But that definitely does not meen fully compliant as you will discover later in this documentation.

### Quick Intro to the Lingo

An HLA **Federation** is a loosely coupled simulation system of systems where the system elements (**Federates**) interact using communication services provided by an runtime infrastructure component (**RTI**) through open well defined and standardized services (**HLA**) and interfaces (HLA APIs). A **Federation Object Model (FOM)** specifies the type of data exchanged in the federation and is separate from the services used for sending the data making the RTI and HLA simulation domain agnostic. A **Federation Agreement** is a specification of federates' modelling responsibilities and how the HLA Services and a FOM should be applied to create a **Synthetic Environment** that is valid with respect to the overall purpose of the federation.

![](federation.jpg)

For details on HLA we recommend the following free [HLA Tutorial](http://www.pitchtechnologies.com/hlatutorial/).


