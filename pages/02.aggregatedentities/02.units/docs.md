---
title: 'Aggregate Units'
taxonomy:
    category:
        - docs
child_type: docs
visible: true
---

Aggregate Units are represented in an NETN Federation as an instance of the HLA object class *HLAobjectRoot.Unit* with the follwing attributes.

Identifiers
- Name, AggregateMarking
- UUID, UniqueID, EntityIdentifier
- Callsign

Organizational Attributes
- SuperiorUnit, HigherHeadquarters
- SubUnits, EmbeddedUnitList, SilentAggregates, SubAggregateIdentifiers, EntityIdentifiers, EntityList
- Force, ForceIdentifier
- Echelon

Resources
- Holdings
- UnitPersonnel
- UnitSupplies
- UnitEquipment
- ArrayOfResourceStatus

Type Classification
- EntityType
- CategoryCode
- ArmCategoryCode
- SizeCode
- TypeServiceCode
- CommandFunctionIndicatorCode

- SymbolIdentifier, Symbol
- SymbolIdentifierEchelon
- SymbolIdentifierDesignation

State Attributes
- Location, Spatial, RelativeSpatial
- Footprint, Dimensions
- Mounted, IsPartOf

Capabilities
- CombatValue
- CaptureStatus

Modelling Attributes
- Federate
- IsSimulationEntity

Activity
- Mission
- Activity
- SourceUnit
- SupportUnit
- WeaponsControlOrder
- Formation

Signatures
- VisualSignature
- HUMINTSignature
- ElectronicSignature
- CoverStatus



- Status

- AggregateState
- NumberOfSilentEntities
- NumberOfVariableDatums


