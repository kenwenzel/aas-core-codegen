

# Class: Range 


_A range data element is a data element that defines a range with min and max._





URI: [aas:Range](https://admin-shell.io/aas/3/0/RC02/Range)





```mermaid
 classDiagram
    class Range
    click Range href "../Range/"
      DataElement <|-- Range
        click DataElement href "../DataElement/"
      
      Range : category
        
      Range : checksum
        
      Range : description
        
      Range : displayName
        
      Range : embeddedDataSpecifications
        
          
    
        
        
        Range --> "*" EmbeddedDataSpecification : embeddedDataSpecifications
        click EmbeddedDataSpecification href "../EmbeddedDataSpecification/"
    

        
      Range : extensions
        
          
    
        
        
        Range --> "*" Extension : extensions
        click Extension href "../Extension/"
    

        
      Range : idShort
        
      Range : kind
        
          
    
        
        
        Range --> "0..1" ModelingKind : kind
        click ModelingKind href "../ModelingKind/"
    

        
      Range : max
        
      Range : min
        
      Range : qualifiers
        
          
    
        
        
        Range --> "*" Qualifier : qualifiers
        click Qualifier href "../Qualifier/"
    

        
      Range : semanticId
        
          
    
        
        
        Range --> "0..1" Reference : semanticId
        click Reference href "../Reference/"
    

        
      Range : supplementalSemanticIds
        
          
    
        
        
        Range --> "*" Reference : supplementalSemanticIds
        click Reference href "../Reference/"
    

        
      Range : valueType
        
          
    
        
        
        Range --> "1" DataTypeDefXsd : valueType
        click DataTypeDefXsd href "../DataTypeDefXsd/"
    

        
      
```





## Inheritance
* [SubmodelElement](SubmodelElement.md) [ [Referable](Referable.md) [HasKind](HasKind.md) [HasSemantics](HasSemantics.md) [Qualifiable](Qualifiable.md) [HasDataSpecification](HasDataSpecification.md)]
    * [DataElement](DataElement.md)
        * **Range**



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [max](max.md) | 0..1 <br/> [String](String.md) | The maximum value of the range | direct |
| [min](min.md) | 0..1 <br/> [String](String.md) | The minimum value of the range | direct |
| [valueType](valueType.md) | 1 <br/> [DataTypeDefXsd](DataTypeDefXsd.md) | Data type of the min und max | direct |
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
| self | aas:Range |
| native | aas:Range |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: Range
description: A range data element is a data element that defines a range with min
  and max.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: DataElement
attributes:
  max:
    name: max
    description: The maximum value of the range.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - Range
    range: string
  min:
    name: min
    description: The minimum value of the range.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - Range
    range: string
  valueType:
    name: valueType
    description: Data type of the min und max
    from_schema: https://admin-shell.io/aas/3/0/RC02
    domain_of:
    - Extension
    - Property
    - Qualifier
    - Range
    range: DataTypeDefXsd
    required: true

```
</details>

### Induced

<details>
```yaml
name: Range
description: A range data element is a data element that defines a range with min
  and max.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: DataElement
attributes:
  max:
    name: max
    description: The maximum value of the range.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: max
    owner: Range
    domain_of:
    - Range
    range: string
  min:
    name: min
    description: The minimum value of the range.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: min
    owner: Range
    domain_of:
    - Range
    range: string
  valueType:
    name: valueType
    description: Data type of the min und max
    from_schema: https://admin-shell.io/aas/3/0/RC02
    alias: valueType
    owner: Range
    domain_of:
    - Extension
    - Property
    - Qualifier
    - Range
    range: DataTypeDefXsd
    required: true
  category:
    name: category
    description: The category is a value that gives further meta information w.r.t.
      to the class of the element. It affects the expected existence of attributes
      and the applicability of constraints.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: category
    owner: Range
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
    owner: Range
    domain_of:
    - Referable
    range: string
  description:
    name: description
    description: Description or comments on the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: description
    owner: Range
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
    owner: Range
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
    owner: Range
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
    owner: Range
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
    owner: Range
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
    owner: Range
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
    owner: Range
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
    owner: Range
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
    owner: Range
    domain_of:
    - HasExtensions
    range: Extension
    multivalued: true

```
</details>