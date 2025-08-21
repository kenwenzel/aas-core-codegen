

# Class: Entity 


_An entity is a submodel element that is used to model entities._





URI: [aas:Entity](https://admin-shell.io/aas/3/0/RC02/Entity)





```mermaid
 classDiagram
    class Entity
    click Entity href "../Entity/"
      SubmodelElement <|-- Entity
        click SubmodelElement href "../SubmodelElement/"
      
      Entity : category
        
      Entity : checksum
        
      Entity : description
        
      Entity : displayName
        
      Entity : embeddedDataSpecifications
        
          
    
        
        
        Entity --> "*" EmbeddedDataSpecification : embeddedDataSpecifications
        click EmbeddedDataSpecification href "../EmbeddedDataSpecification/"
    

        
      Entity : entityType
        
          
    
        
        
        Entity --> "1" EntityType : entityType
        click EntityType href "../EntityType/"
    

        
      Entity : extensions
        
          
    
        
        
        Entity --> "*" Extension : extensions
        click Extension href "../Extension/"
    

        
      Entity : globalAssetId
        
          
    
        
        
        Entity --> "0..1" Reference : globalAssetId
        click Reference href "../Reference/"
    

        
      Entity : idShort
        
      Entity : kind
        
          
    
        
        
        Entity --> "0..1" ModelingKind : kind
        click ModelingKind href "../ModelingKind/"
    

        
      Entity : qualifiers
        
          
    
        
        
        Entity --> "*" Qualifier : qualifiers
        click Qualifier href "../Qualifier/"
    

        
      Entity : semanticId
        
          
    
        
        
        Entity --> "0..1" Reference : semanticId
        click Reference href "../Reference/"
    

        
      Entity : specificAssetId
        
          
    
        
        
        Entity --> "0..1" SpecificAssetId : specificAssetId
        click SpecificAssetId href "../SpecificAssetId/"
    

        
      Entity : statements
        
          
    
        
        
        Entity --> "*" SubmodelElement : statements
        click SubmodelElement href "../SubmodelElement/"
    

        
      Entity : supplementalSemanticIds
        
          
    
        
        
        Entity --> "*" Reference : supplementalSemanticIds
        click Reference href "../Reference/"
    

        
      
```





## Inheritance
* [SubmodelElement](SubmodelElement.md) [ [Referable](Referable.md) [HasKind](HasKind.md) [HasSemantics](HasSemantics.md) [Qualifiable](Qualifiable.md) [HasDataSpecification](HasDataSpecification.md)]
    * **Entity**



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [entityType](entityType.md) | 1 <br/> [EntityType](EntityType.md) | Describes whether the entity is a co-managed entity or a self-managed entity | direct |
| [globalAssetId](globalAssetId.md) | 0..1 <br/> [Reference](Reference.md) | Global identifier of the asset the entity is representing | direct |
| [specificAssetId](specificAssetId.md) | 0..1 <br/> [SpecificAssetId](SpecificAssetId.md) | Reference to a specific asset ID representing a supplementary identifier of t... | direct |
| [statements](statements.md) | * <br/> [SubmodelElement](SubmodelElement.md) | Describes statements applicable to the entity by a set of submodel elements, ... | direct |
| [category](category.md) | 0..1 <br/> [String](String.md) | The category is a value that gives further meta information w | [Referable](Referable.md) |
| [checksum](checksum.md) | 0..1 <br/> [String](String.md) | Checksum to be used to determine if an Referable (including its aggregated ch... | [Referable](Referable.md) |
| [description](description.md) | * <br/> [LangString](LangString.md) | Description or comments on the element | [Referable](Referable.md) |
| [displayName](displayName.md) | * <br/> [LangString](LangString.md) | Display name | [Referable](Referable.md) |
| [idShort](idShort.md) | 0..1 <br/> [String](String.md) | In case of identifiables this attribute is a short name of the element | [Referable](Referable.md) |
| [kind](kind.md) | 0..1 <br/> [ModelingKind](ModelingKind.md) | Kind of the element: either type or instance | [HasKind](HasKind.md) |
| [semanticId](semanticId.md) | 0..1 <br/> [Reference](Reference.md) | Identifier of the semantic definition of the element | [HasSemantics](HasSemantics.md) |
| [supplementalSemanticIds](supplementalSemanticIds.md) | * <br/> [Reference](Reference.md) | Identifier of a supplemental semantic definition of the element | [HasSemantics](HasSemantics.md) |
| [qualifiers](qualifiers.md) | * <br/> [Qualifier](Qualifier.md) | Additional qualification of a qualifiable element | [Qualifiable](Qualifiable.md) |
| [embeddedDataSpecifications](embeddedDataSpecifications.md) | * <br/> [EmbeddedDataSpecification](EmbeddedDataSpecification.md) | Embedded data specification | [HasDataSpecification](HasDataSpecification.md) |
| [extensions](extensions.md) | * <br/> [Extension](Extension.md) | An extension of the element | [HasExtensions](HasExtensions.md) |










## Identifier and Mapping Information






### Schema Source


* from schema: https://admin-shell.io/aas/3/0/RC02




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | aas:Entity |
| native | aas:Entity |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: Entity
description: An entity is a submodel element that is used to model entities.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: SubmodelElement
attributes:
  entityType:
    name: entityType
    description: Describes whether the entity is a co-managed entity or a self-managed
      entity.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - Entity
    range: EntityType
    required: true
  globalAssetId:
    name: globalAssetId
    description: Global identifier of the asset the entity is representing.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    domain_of:
    - AssetInformation
    - Entity
    range: Reference
  specificAssetId:
    name: specificAssetId
    description: Reference to a specific asset ID representing a supplementary identifier
      of the asset represented by the Asset Administration Shell.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - Entity
    range: SpecificAssetId
  statements:
    name: statements
    description: Describes statements applicable to the entity by a set of submodel
      elements, typically with a qualified value.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - Entity
    range: SubmodelElement
    multivalued: true

```
</details>

### Induced

<details>
```yaml
name: Entity
description: An entity is a submodel element that is used to model entities.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: SubmodelElement
attributes:
  entityType:
    name: entityType
    description: Describes whether the entity is a co-managed entity or a self-managed
      entity.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: entityType
    owner: Entity
    domain_of:
    - Entity
    range: EntityType
    required: true
  globalAssetId:
    name: globalAssetId
    description: Global identifier of the asset the entity is representing.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    alias: globalAssetId
    owner: Entity
    domain_of:
    - AssetInformation
    - Entity
    range: Reference
  specificAssetId:
    name: specificAssetId
    description: Reference to a specific asset ID representing a supplementary identifier
      of the asset represented by the Asset Administration Shell.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: specificAssetId
    owner: Entity
    domain_of:
    - Entity
    range: SpecificAssetId
  statements:
    name: statements
    description: Describes statements applicable to the entity by a set of submodel
      elements, typically with a qualified value.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: statements
    owner: Entity
    domain_of:
    - Entity
    range: SubmodelElement
    multivalued: true
  category:
    name: category
    description: The category is a value that gives further meta information w.r.t.
      to the class of the element. It affects the expected existence of attributes
      and the applicability of constraints.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: category
    owner: Entity
    domain_of:
    - Referable
    range: string
  checksum:
    name: checksum
    description: Checksum to be used to determine if an Referable (including its aggregated
      child elements) has changed.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: checksum
    owner: Entity
    domain_of:
    - Referable
    range: string
  description:
    name: description
    description: Description or comments on the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: description
    owner: Entity
    domain_of:
    - Referable
    range: LangString
    multivalued: true
  displayName:
    name: displayName
    description: Display name. Can be provided in several languages.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: displayName
    owner: Entity
    domain_of:
    - Referable
    range: LangString
    multivalued: true
  idShort:
    name: idShort
    description: In case of identifiables this attribute is a short name of the element.
      In case of referable this ID is an identifying string of the element within
      its name space.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: idShort
    owner: Entity
    domain_of:
    - Referable
    range: string
    pattern: ^[a-zA-Z][a-zA-Z0-9_]+$
  kind:
    name: kind
    description: 'Kind of the element: either type or instance.'
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: kind
    owner: Entity
    domain_of:
    - HasKind
    - Qualifier
    range: ModelingKind
  semanticId:
    name: semanticId
    description: Identifier of the semantic definition of the element. It is called
      semantic ID of the element or also main semantic ID of the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: semanticId
    owner: Entity
    domain_of:
    - HasSemantics
    range: Reference
  supplementalSemanticIds:
    name: supplementalSemanticIds
    description: Identifier of a supplemental semantic definition of the element.
      It is called supplemental semantic ID of the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: supplementalSemanticIds
    owner: Entity
    domain_of:
    - HasSemantics
    range: Reference
    multivalued: true
  qualifiers:
    name: qualifiers
    description: Additional qualification of a qualifiable element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: qualifiers
    owner: Entity
    domain_of:
    - Qualifiable
    range: Qualifier
    multivalued: true
  embeddedDataSpecifications:
    name: embeddedDataSpecifications
    description: Embedded data specification.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: embeddedDataSpecifications
    owner: Entity
    domain_of:
    - HasDataSpecification
    range: EmbeddedDataSpecification
    multivalued: true
  extensions:
    name: extensions
    description: An extension of the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: extensions
    owner: Entity
    domain_of:
    - HasExtensions
    range: Extension
    multivalued: true

```
</details>