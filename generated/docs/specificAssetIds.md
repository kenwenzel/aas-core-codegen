

# Slot: specificAssetIds 


_Additional domain-specific, typically proprietary identifier for the asset like e.g., serial number etc._





URI: [aas:specificAssetIds](https://admin-shell.io/aas/3/0/RC02/specificAssetIds)
Alias: specificAssetIds

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [AssetInformation](AssetInformation.md) | In 'AssetInformation' identifying meta data of the asset that is represented ... |  no  |






## Properties

* Range: [SpecificAssetId](SpecificAssetId.md)

* Multivalued: True




## Identifier and Mapping Information






### Schema Source


* from schema: https://admin-shell.io/aas/3/0/RC02




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | aas:specificAssetIds |
| native | aas:specificAssetIds |




## LinkML Source

<details>
```yaml
name: specificAssetIds
description: Additional domain-specific, typically proprietary identifier for the
  asset like e.g., serial number etc.
from_schema: https://admin-shell.io/aas/3/0/RC02
rank: 1000
alias: specificAssetIds
owner: AssetInformation
domain_of:
- AssetInformation
range: SpecificAssetId
multivalued: true

```
</details>