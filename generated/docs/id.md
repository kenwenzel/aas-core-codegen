

# Slot: id 


_The globally unique identification of the element._





URI: [aas:id](https://admin-shell.io/aas/3/0/RC02/id)
Alias: id

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [AssetAdministrationShell](AssetAdministrationShell.md) | An asset administration shell |  no  |
| [Submodel](Submodel.md) | A submodel defines a specific aspect of the asset represented by the AAS |  no  |
| [ConceptDescription](ConceptDescription.md) | The semantics of a property or other elements that may have a semantic descri... |  no  |
| [Identifiable](Identifiable.md) | An element that has a globally unique identifier |  no  |






## Properties

* Range: [String](String.md)

* Required: True




## Identifier and Mapping Information






### Schema Source


* from schema: https://admin-shell.io/aas/3/0/RC02




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | aas:id |
| native | aas:id |




## LinkML Source

<details>
```yaml
name: id
description: The globally unique identification of the element.
from_schema: https://admin-shell.io/aas/3/0/RC02
rank: 1000
alias: id
owner: Identifiable
domain_of:
- Identifiable
range: string
required: true

```
</details>