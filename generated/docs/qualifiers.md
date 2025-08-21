

# Slot: qualifiers 


_Additional qualification of a qualifiable element._





URI: [aas:qualifiers](https://admin-shell.io/aas/3/0/RC02/qualifiers)
Alias: qualifiers

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [Capability](Capability.md) | A capability is the implementation-independent description of the potential o... |  no  |
| [ReferenceElement](ReferenceElement.md) | A reference element is a data element that defines a logical reference to ano... |  no  |
| [Property](Property.md) | A property is a data element that has a single value |  no  |
| [SubmodelElementList](SubmodelElementList.md) | A submodel element list is an ordered list of submodel elements |  no  |
| [RelationshipElement](RelationshipElement.md) | A relationship element is used to define a relationship between two elements ... |  no  |
| [BasicEventElement](BasicEventElement.md) | A basic event element |  no  |
| [SubmodelElement](SubmodelElement.md) | A submodel element is an element suitable for the description and differentia... |  no  |
| [File](File.md) | A File is a data element that represents an address to a file (a locator) |  no  |
| [Submodel](Submodel.md) | A submodel defines a specific aspect of the asset represented by the AAS |  no  |
| [AnnotatedRelationshipElement](AnnotatedRelationshipElement.md) | An annotated relationship element is a relationship element that can be annot... |  no  |
| [EventElement](EventElement.md) | An event element |  no  |
| [Operation](Operation.md) | An operation is a submodel element with input and output variables |  no  |
| [Range](Range.md) | A range data element is a data element that defines a range with min and max |  no  |
| [Qualifiable](Qualifiable.md) | The value of a qualifiable element may be further qualified by one or more qu... |  no  |
| [SubmodelElementCollection](SubmodelElementCollection.md) | A submodel element collection is a kind of struct, i |  no  |
| [Entity](Entity.md) | An entity is a submodel element that is used to model entities |  no  |
| [MultiLanguageProperty](MultiLanguageProperty.md) | A property is a data element that has a multi-language value |  no  |
| [DataElement](DataElement.md) | A data element is a submodel element that is not further composed out of othe... |  no  |
| [Blob](Blob.md) | A 'Blob' is a data element that represents a file that is contained with its ... |  no  |






## Properties

* Range: [Qualifier](Qualifier.md)

* Multivalued: True




## Identifier and Mapping Information






### Schema Source


* from schema: https://admin-shell.io/aas/3/0/RC02




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | aas:qualifiers |
| native | aas:qualifiers |




## LinkML Source

<details>
```yaml
name: qualifiers
description: Additional qualification of a qualifiable element.
from_schema: https://admin-shell.io/aas/3/0/RC02
rank: 1000
alias: qualifiers
owner: Qualifiable
domain_of:
- Qualifiable
range: Qualifier
multivalued: true

```
</details>