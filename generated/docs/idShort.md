

# Slot: idShort 


_In case of identifiables this attribute is a short name of the element. In case of referable this ID is an identifying string of the element within its name space._





URI: [aas:idShort](https://admin-shell.io/aas/3/0/RC02/idShort)
Alias: idShort

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [Capability](Capability.md) | A capability is the implementation-independent description of the potential o... |  no  |
| [ReferenceElement](ReferenceElement.md) | A reference element is a data element that defines a logical reference to ano... |  no  |
| [Referable](Referable.md) | An element that is referable by its 'idShort' |  no  |
| [Property](Property.md) | A property is a data element that has a single value |  no  |
| [SubmodelElementList](SubmodelElementList.md) | A submodel element list is an ordered list of submodel elements |  no  |
| [RelationshipElement](RelationshipElement.md) | A relationship element is used to define a relationship between two elements ... |  no  |
| [Blob](Blob.md) | A 'Blob' is a data element that represents a file that is contained with its ... |  no  |
| [BasicEventElement](BasicEventElement.md) | A basic event element |  no  |
| [Identifiable](Identifiable.md) | An element that has a globally unique identifier |  no  |
| [SubmodelElement](SubmodelElement.md) | A submodel element is an element suitable for the description and differentia... |  no  |
| [File](File.md) | A File is a data element that represents an address to a file (a locator) |  no  |
| [Submodel](Submodel.md) | A submodel defines a specific aspect of the asset represented by the AAS |  no  |
| [AnnotatedRelationshipElement](AnnotatedRelationshipElement.md) | An annotated relationship element is a relationship element that can be annot... |  no  |
| [EventElement](EventElement.md) | An event element |  no  |
| [Operation](Operation.md) | An operation is a submodel element with input and output variables |  no  |
| [Range](Range.md) | A range data element is a data element that defines a range with min and max |  no  |
| [SubmodelElementCollection](SubmodelElementCollection.md) | A submodel element collection is a kind of struct, i |  no  |
| [Entity](Entity.md) | An entity is a submodel element that is used to model entities |  no  |
| [MultiLanguageProperty](MultiLanguageProperty.md) | A property is a data element that has a multi-language value |  no  |
| [DataElement](DataElement.md) | A data element is a submodel element that is not further composed out of othe... |  no  |
| [AssetAdministrationShell](AssetAdministrationShell.md) | An asset administration shell |  no  |
| [ConceptDescription](ConceptDescription.md) | The semantics of a property or other elements that may have a semantic descri... |  no  |






## Properties

* Range: [String](String.md)

* Regex pattern: `^[a-zA-Z][a-zA-Z0-9_]+$`




## Identifier and Mapping Information






### Schema Source


* from schema: https://admin-shell.io/aas/3/0/RC02




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | aas:idShort |
| native | aas:idShort |




## LinkML Source

<details>
```yaml
name: idShort
description: In case of identifiables this attribute is a short name of the element.
  In case of referable this ID is an identifying string of the element within its
  name space.
from_schema: https://admin-shell.io/aas/3/0/RC02
rank: 1000
alias: idShort
owner: Referable
domain_of:
- Referable
range: string
pattern: ^[a-zA-Z][a-zA-Z0-9_]+$

```
</details>