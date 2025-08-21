

# Slot: supplementalSemanticIds 


_Identifier of a supplemental semantic definition of the element. It is called supplemental semantic ID of the element._





URI: [aas:supplementalSemanticIds](https://admin-shell.io/aas/3/0/RC02/supplementalSemanticIds)
Alias: supplementalSemanticIds

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [Capability](Capability.md) | A capability is the implementation-independent description of the potential o... |  no  |
| [Extension](Extension.md) | Single extension of an element |  no  |
| [ReferenceElement](ReferenceElement.md) | A reference element is a data element that defines a logical reference to ano... |  no  |
| [Property](Property.md) | A property is a data element that has a single value |  no  |
| [SubmodelElementList](SubmodelElementList.md) | A submodel element list is an ordered list of submodel elements |  no  |
| [RelationshipElement](RelationshipElement.md) | A relationship element is used to define a relationship between two elements ... |  no  |
| [BasicEventElement](BasicEventElement.md) | A basic event element |  no  |
| [SubmodelElement](SubmodelElement.md) | A submodel element is an element suitable for the description and differentia... |  no  |
| [File](File.md) | A File is a data element that represents an address to a file (a locator) |  no  |
| [Submodel](Submodel.md) | A submodel defines a specific aspect of the asset represented by the AAS |  no  |
| [Qualifier](Qualifier.md) | A qualifier is a type-value-pair that makes additional statements w |  no  |
| [AnnotatedRelationshipElement](AnnotatedRelationshipElement.md) | An annotated relationship element is a relationship element that can be annot... |  no  |
| [EventElement](EventElement.md) | An event element |  no  |
| [Operation](Operation.md) | An operation is a submodel element with input and output variables |  no  |
| [Range](Range.md) | A range data element is a data element that defines a range with min and max |  no  |
| [SubmodelElementCollection](SubmodelElementCollection.md) | A submodel element collection is a kind of struct, i |  no  |
| [Entity](Entity.md) | An entity is a submodel element that is used to model entities |  no  |
| [MultiLanguageProperty](MultiLanguageProperty.md) | A property is a data element that has a multi-language value |  no  |
| [DataElement](DataElement.md) | A data element is a submodel element that is not further composed out of othe... |  no  |
| [SpecificAssetId](SpecificAssetId.md) | A specific asset ID describes a generic supplementary identifying attribute o... |  no  |
| [HasSemantics](HasSemantics.md) | Element that can have a semantic definition plus some supplemental semantic d... |  no  |
| [Blob](Blob.md) | A 'Blob' is a data element that represents a file that is contained with its ... |  no  |






## Properties

* Range: [Reference](Reference.md)

* Multivalued: True




## Identifier and Mapping Information






### Schema Source


* from schema: https://admin-shell.io/aas/3/0/RC02




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | aas:supplementalSemanticIds |
| native | aas:supplementalSemanticIds |




## LinkML Source

<details>
```yaml
name: supplementalSemanticIds
description: Identifier of a supplemental semantic definition of the element. It is
  called supplemental semantic ID of the element.
from_schema: https://admin-shell.io/aas/3/0/RC02
rank: 1000
alias: supplementalSemanticIds
owner: HasSemantics
domain_of:
- HasSemantics
range: Reference
multivalued: true

```
</details>