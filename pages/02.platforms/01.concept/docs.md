---
title: Concepts
child_type: docs
visible: true
---

Physical Entities are objects in the synthetic environment that models real-world physical objects. Each entity has a set of attributes that characterizes the object and defines its ground-truth state.

The NETN FOM specifies a **NETN_PhysicalEntity** FOM module to define extensions to the corresponding **RPR2-PhysicalEntity** FOM module object classes.

Common to all Physical Entities is a set of base attributes defining the object spatial state and entity type according to the RPR-FOM standard and associated EntityType enumeration standard.

Some physical entities are self-propelled movable objects such as vehicles, some are movable or transportable and some are on fixed locations and not movable at all. Some physical entities are attached or thethered to other physical objects and have relative positions with respect to the object to which it is attached.

Some physical entities may exist at the start of a simulation, some are introduced dynamically during execution of the simulation and some may be removed from simulation during simulation.

Some physical entities are known at the start of a simulation and some may be unknwon from the start and created dynamically by a model during simulation execution.