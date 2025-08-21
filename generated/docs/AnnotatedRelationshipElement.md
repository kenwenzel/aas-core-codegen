

# Class: AnnotatedRelationshipElement 


_An annotated relationship element is a relationship element that can be annotated with additional data elements._





URI: [aas:AnnotatedRelationshipElement](https://admin-shell.io/aas/3/0/RC02/AnnotatedRelationshipElement)





```mermaid
 classDiagram
    class AnnotatedRelationshipElement
    click AnnotatedRelationshipElement href "../AnnotatedRelationshipElement/"
      RelationshipElement <|-- AnnotatedRelationshipElement
        click RelationshipElement href "../RelationshipElement/"
      
      AnnotatedRelationshipElement : annotations
        
          
    
        
        
        AnnotatedRelationshipElement --> "*" DataElement : annotations
        click DataElement href "../DataElement/"
    

        
      AnnotatedRelationshipElement : category
        
      AnnotatedRelationshipElement : checksum
        
      AnnotatedRelationshipElement : description
        
      AnnotatedRelationshipElement : displayName
        
      AnnotatedRelationshipElement : embeddedDataSpecifications
        
          
    
        
        
        AnnotatedRelationshipElement --> "*" EmbeddedDataSpecification : embeddedDataSpecifications
        click EmbeddedDataSpecification href "../EmbeddedDataSpecification/"
    

        
      AnnotatedRelationshipElement : extensions
        
          
    
        
        
        AnnotatedRelationshipElement --> "*" Extension : extensions
        click Extension href "../Extension/"
    

        
      AnnotatedRelationshipElement : first
        
          
    
        
        
        AnnotatedRelationshipElement --> "1" Reference : first
        click Reference href "../Reference/"
    

        
      AnnotatedRelationshipElement : idShort
        
      AnnotatedRelationshipElement : kind
        
          
    
        
        
        AnnotatedRelationshipElement --> "0..1" ModelingKind : kind
        click ModelingKind href "../ModelingKind/"
    

        
      AnnotatedRelationshipElement : qualifiers
        
          
    
        
        
        AnnotatedRelationshipElement --> "*" Qualifier : qualifiers
        click Qualifier href "../Qualifier/"
    

        
      AnnotatedRelationshipElement : second
        
          
    
        
        
        AnnotatedRelationshipElement --> "1" Reference : second
        click Reference href "../Reference/"
    

        
      AnnotatedRelationshipElement : semanticId
        
          
    
        
        
        AnnotatedRelationshipElement --> "0..1" Reference : semanticId
        click Reference href "../Reference/"
    

        
      AnnotatedRelationshipElement : supplementalSemanticIds
        
          
    
        
        
        AnnotatedRelationshipElement --> "*" Reference : supplementalSemanticIds
        click Reference href "../Reference/"
    

        
      
```





## Inheritance
* [SubmodelElement](SubmodelElement.md) [ [Referable](Referable.md) [HasKind](HasKind.md) [HasSemantics](HasSemantics.md) [Qualifiable](Qualifiable.md) [HasDataSpecification](HasDataSpecification.md)]
    * [RelationshipElement](RelationshipElement.md)
        * **AnnotatedRelationshipElement**



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [annotations](annotations.md) | * <br/> [DataElement](DataElement.md) | A data element that represents an annotation that holds for the relationship ... | direct |
| [first](first.md) | 1 <br/> [Reference](Reference.md) | Reference to the first element in the relationship taking the role of the sub... | [RelationshipElement](RelationshipElement.md) |
| [second](second.md) | 1 <br/> [Reference](Reference.md) | Reference to the second element in the relationship taking the role of the ob... | [RelationshipElement](RelationshipElement.md) |
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
| self | aas:AnnotatedRelationshipElement |
| native | aas:AnnotatedRelationshipElement |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: AnnotatedRelationshipElement
description: An annotated relationship element is a relationship element that can
  be annotated with additional data elements.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: RelationshipElement
attributes:
  annotations:
    name: annotations
    description: A data element that represents an annotation that holds for the relationship
      between the two elements
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - AnnotatedRelationshipElement
    range: DataElement
    multivalued: true

```
</details>

### Induced

<details>
```yaml
name: AnnotatedRelationshipElement
description: An annotated relationship element is a relationship element that can
  be annotated with additional data elements.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: RelationshipElement
attributes:
  annotations:
    name: annotations
    description: A data element that represents an annotation that holds for the relationship
      between the two elements
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: annotations
    owner: AnnotatedRelationshipElement
    domain_of:
    - AnnotatedRelationshipElement
    range: DataElement
    multivalued: true
  first:
    name: first
    description: Reference to the first element in the relationship taking the role
      of the subject.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: first
    owner: AnnotatedRelationshipElement
    domain_of:
    - RelationshipElement
    range: Reference
    required: true
  second:
    name: second
    description: Reference to the second element in the relationship taking the role
      of the object.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: second
    owner: AnnotatedRelationshipElement
    domain_of:
    - RelationshipElement
    range: Reference
    required: true
  category:
    name: category
    description: The category is a value that gives further meta information w.r.t.
      to the class of the element. It affects the expected existence of attributes
      and the applicability of constraints.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: category
    owner: AnnotatedRelationshipElement
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
    owner: AnnotatedRelationshipElement
    domain_of:
    - Referable
    range: string
  description:
    name: description
    description: Description or comments on the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: description
    owner: AnnotatedRelationshipElement
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
    owner: AnnotatedRelationshipElement
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
    owner: AnnotatedRelationshipElement
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
    owner: AnnotatedRelationshipElement
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
    owner: AnnotatedRelationshipElement
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
    owner: AnnotatedRelationshipElement
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
    owner: AnnotatedRelationshipElement
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
    owner: AnnotatedRelationshipElement
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
    owner: AnnotatedRelationshipElement
    domain_of:
    - HasExtensions
    range: Extension
    multivalued: true

```
</details>