---
title: 'Transfer of Modelling Responsibilities'
media_order: 'arrows-box-business-533189.jpg, tmr.png'
date: '04-06-2018 12:00'
body_classes: 'header-transparent header-dark'
visible: true
hero_classes: 'text-light parrallax title-h1h2  overlay-dark'
hero_image: arrows-box-business-533189.jpg
blog_url: /netn/netn-modules
show_sidebar: false
show_breadcrumbs: true
show_pagination: true
continue_link: true
---

The **NETN Transfer of Modelling Responsibility (TMR)** component is used to control and manage the change of responsibility for modelling a set of attributes from one simulation to another. There are several reasons why a TMR can be a good solution in a federated simulation. Being able to dynamically select the most appropriate federate to model certain aspects of a simulated entity and to delegate the responsibility of updating corresponding attributes is a key feature of NETN based simulation. For example TMR can be used change modelling responsibilities from Live or Recorded entities to Constructive or Virtual simulations. It can be used for dynamic load balancing, fault handling and hand-over, delegating modelling of e.g. damage assessment and movement, etc.

TMR can be triggered either from an external source, e.g. a user, or by another federate and the pattern include both a pull (acquisition) and push (divestiture) model for responsibility transfer. The pattern combines HLA Ownership Management Services with a set of HLA Interactions used to further negotiate and control the TMR.

The TMR pattern defines five TMR interactions:
* InitiateTransferModellingResponsibility - Triggers a federate to initiate a TMR
* RequestTransferModellingResponsibility - Initiates a push or pull request of TRM
* OfferTransferModellingResponsibility - Response to a TMR Request
* Cancel Request - Abort TMR pattern
* Transfer Result - Notification of TMR result

![](tmr.png?resize=500)

> _The TMR pattern also include the following HLA Ownership Management Service calls and callbacks (†): Attribute Ownership Acquisition, Attribute Ownership Acquisition If Available, Attribute Ownership Divesture If Wanted, Cancel Attribute Ownership Acquisition, Request Attribute Ownership Release †, Attribute Ownership Acquisition Notification †, Confirm Attribute Ownership Acquisition Cancellation †, Attribute OwnershipUnavailable †_