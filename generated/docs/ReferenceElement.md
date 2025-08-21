

# Class: ReferenceElement 


_A reference element is a data element that defines a logical reference to another element within the same or another AAS or a reference to an external object or entity._





URI: [aas:ReferenceElement](https://admin-shell.io/aas/3/0/RC02/ReferenceElement)





```mermaid
 classDiagram
    class ReferenceElement
    click ReferenceElement href "../ReferenceElement/"
      DataElement <|-- ReferenceElement
        click DataElement href "../DataElement/"
      
      ReferenceElement : category
        
      ReferenceElement : checksum
        
      ReferenceElement : description
        
      ReferenceElement : displayName
        
      ReferenceElement : embeddedDataSpecifications
        
          
    
        
        
        ReferenceElement --> "*" EmbeddedDataSpecification : embeddedDataSpecifications
        click EmbeddedDataSpecification href "../EmbeddedDataSpecification/"
    

        
      ReferenceElement : extensions
        
          
    
        
        
        ReferenceElement --> "*" Extension : extensions
        click Extension href "../Extension/"
    

        
      ReferenceElement : idShort
        
      ReferenceElement : kind
        
          
    
        
        
        ReferenceElement --> "0..1" ModelingKind : kind
        click ModelingKind href "../ModelingKind/"
    

        
      ReferenceElement : qualifiers
        
          
    
        
        
        ReferenceElement --> "*" Qualifier : qualifiers
        click Qualifier href "../Qualifier/"
    

        
      ReferenceElement : semanticId
        
          
    
        
        
        ReferenceElement --> "0..1" Reference : semanticId
        click Reference href "../Reference/"
    

        
      ReferenceElement : supplementalSemanticIds
        
          
    
        
        
        ReferenceElement --> "*" Reference : supplementalSemanticIds
        click Reference href "../Reference/"
    

        
      ReferenceElement : value
        
          
    
        
        
        ReferenceElement --> "0..1" Reference : value
        click Reference href "../Reference/"
    

        
      
```





## Inheritance
* [SubmodelElement](SubmodelElement.md) [ [Referable](Referable.md) [HasKind](HasKind.md) [HasSemantics](HasSemantics.md) [Qualifiable](Qualifiable.md) [HasDataSpecification](HasDataSpecification.md)]
    * [DataElement](DataElement.md)
        * **ReferenceElement**



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [value](value.md) | 0..1 <br/> [Reference](Reference.md) | Global reference to an external object or entity or a logical reference to an... | direct |
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
| self | aas:ReferenceElement |
| native | aas:ReferenceElement |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: ReferenceElement
description: A reference element is a data element that defines a logical reference
  to another element within the same or another AAS or a reference to an external
  object or entity.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: DataElement
attributes:
  value:
    name: value
    description: Global reference to an external object or entity or a logical reference
      to another element within the same or another AAS (i.e. a model reference to
      a Referable).
    from_schema: https://admin-shell.io/aas/3/0/RC02
    domain_of:
    - Blob
    - DataSpecificationIec61360
    - Extension
    - File
    - Key
    - MultiLanguageProperty
    - OperationVariable
    - Property
    - Qualifier
    - ReferenceElement
    - SpecificAssetId
    - SubmodelElementCollection
    - SubmodelElementList
    - ValueReferencePair
    range: Reference

```
</details>

### Induced

<details>
```yaml
name: ReferenceElement
description: A reference element is a data element that defines a logical reference
  to another element within the same or another AAS or a reference to an external
  object or entity.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: DataElement
attributes:
  value:
    name: value
    description: Global reference to an external object or entity or a logical reference
      to another element within the same or another AAS (i.e. a model reference to
      a Referable).
    from_schema: https://admin-shell.io/aas/3/0/RC02
    alias: value
    owner: ReferenceElement
    domain_of:
    - Blob
    - DataSpecificationIec61360
    - Extension
    - File
    - Key
    - MultiLanguageProperty
    - OperationVariable
    - Property
    - Qualifier
    - ReferenceElement
    - SpecificAssetId
    - SubmodelElementCollection
    - SubmodelElementList
    - ValueReferencePair
    range: Reference
  category:
    name: category
    description: The category is a value that gives further meta information w.r.t.
      to the class of the element. It affects the expected existence of attributes
      and the applicability of constraints.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: category
    owner: ReferenceElement
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
    owner: ReferenceElement
    domain_of:
    - Referable
    range: string
  description:
    name: description
    description: Description or comments on the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: description
    owner: ReferenceElement
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
    owner: ReferenceElement
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
    owner: ReferenceElement
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
    owner: ReferenceElement
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
    owner: ReferenceElement
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
    owner: ReferenceElement
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
    owner: ReferenceElement
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
    owner: ReferenceElement
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
    owner: ReferenceElement
    domain_of:
    - HasExtensions
    range: Extension
    multivalued: true

```
</details>