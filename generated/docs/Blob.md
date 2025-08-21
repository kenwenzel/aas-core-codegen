

# Class: Blob 


_A 'Blob' is a data element that represents a file that is contained with its source code in the value attribute._





URI: [aas:Blob](https://admin-shell.io/aas/3/0/RC02/Blob)





```mermaid
 classDiagram
    class Blob
    click Blob href "../Blob/"
      DataElement <|-- Blob
        click DataElement href "../DataElement/"
      
      Blob : category
        
      Blob : checksum
        
      Blob : contentType
        
      Blob : description
        
      Blob : displayName
        
      Blob : embeddedDataSpecifications
        
          
    
        
        
        Blob --> "*" EmbeddedDataSpecification : embeddedDataSpecifications
        click EmbeddedDataSpecification href "../EmbeddedDataSpecification/"
    

        
      Blob : extensions
        
          
    
        
        
        Blob --> "*" Extension : extensions
        click Extension href "../Extension/"
    

        
      Blob : idShort
        
      Blob : kind
        
          
    
        
        
        Blob --> "0..1" ModelingKind : kind
        click ModelingKind href "../ModelingKind/"
    

        
      Blob : qualifiers
        
          
    
        
        
        Blob --> "*" Qualifier : qualifiers
        click Qualifier href "../Qualifier/"
    

        
      Blob : semanticId
        
          
    
        
        
        Blob --> "0..1" Reference : semanticId
        click Reference href "../Reference/"
    

        
      Blob : supplementalSemanticIds
        
          
    
        
        
        Blob --> "*" Reference : supplementalSemanticIds
        click Reference href "../Reference/"
    

        
      Blob : value
        
      
```





## Inheritance
* [SubmodelElement](SubmodelElement.md) [ [Referable](Referable.md) [HasKind](HasKind.md) [HasSemantics](HasSemantics.md) [Qualifiable](Qualifiable.md) [HasDataSpecification](HasDataSpecification.md)]
    * [DataElement](DataElement.md)
        * **Blob**



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [contentType](contentType.md) | 1 <br/> [String](String.md) | Content type of the content of the 'Blob' | direct |
| [value](value.md) | 0..1 <br/> [Base64Binary](Base64Binary.md) | The value of the 'Blob' instance of a blob data element | direct |
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
| self | aas:Blob |
| native | aas:Blob |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: Blob
description: A 'Blob' is a data element that represents a file that is contained with
  its source code in the value attribute.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: DataElement
attributes:
  contentType:
    name: contentType
    description: Content type of the content of the 'Blob'.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - Blob
    - File
    - Resource
    range: string
    required: true
    pattern: ^([!#$%&'*+\-.^_`|~0-9a-zA-Z])+/([!#$%&'*+\-.^_`|~0-9a-zA-Z])+([ \t]*;[
      \t]*([!#$%&'*+\-.^_`|~0-9a-zA-Z])+=(([!#$%&'*+\-.^_`|~0-9a-zA-Z])+|"(([\t !#-\[\]-~]|[\x80-\xff])|\\([\t
      !-~]|[\x80-\xff]))*"))*$
  value:
    name: value
    description: The value of the 'Blob' instance of a blob data element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
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
    range: Base64Binary

```
</details>

### Induced

<details>
```yaml
name: Blob
description: A 'Blob' is a data element that represents a file that is contained with
  its source code in the value attribute.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: DataElement
attributes:
  contentType:
    name: contentType
    description: Content type of the content of the 'Blob'.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: contentType
    owner: Blob
    domain_of:
    - Blob
    - File
    - Resource
    range: string
    required: true
    pattern: ^([!#$%&'*+\-.^_`|~0-9a-zA-Z])+/([!#$%&'*+\-.^_`|~0-9a-zA-Z])+([ \t]*;[
      \t]*([!#$%&'*+\-.^_`|~0-9a-zA-Z])+=(([!#$%&'*+\-.^_`|~0-9a-zA-Z])+|"(([\t !#-\[\]-~]|[\x80-\xff])|\\([\t
      !-~]|[\x80-\xff]))*"))*$
  value:
    name: value
    description: The value of the 'Blob' instance of a blob data element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: value
    owner: Blob
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
    range: Base64Binary
  category:
    name: category
    description: The category is a value that gives further meta information w.r.t.
      to the class of the element. It affects the expected existence of attributes
      and the applicability of constraints.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: category
    owner: Blob
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
    owner: Blob
    domain_of:
    - Referable
    range: string
  description:
    name: description
    description: Description or comments on the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: description
    owner: Blob
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
    owner: Blob
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
    owner: Blob
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
    owner: Blob
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
    owner: Blob
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
    owner: Blob
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
    owner: Blob
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
    owner: Blob
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
    owner: Blob
    domain_of:
    - HasExtensions
    range: Extension
    multivalued: true

```
</details>