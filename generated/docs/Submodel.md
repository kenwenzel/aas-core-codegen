

# Class: Submodel 


_A submodel defines a specific aspect of the asset represented by the AAS._





URI: [aas:Submodel](https://admin-shell.io/aas/3/0/RC02/Submodel)





```mermaid
 classDiagram
    class Submodel
    click Submodel href "../Submodel/"
      Identifiable <|-- Submodel
        click Identifiable href "../Identifiable/"
      HasKind <|-- Submodel
        click HasKind href "../HasKind/"
      HasSemantics <|-- Submodel
        click HasSemantics href "../HasSemantics/"
      Qualifiable <|-- Submodel
        click Qualifiable href "../Qualifiable/"
      HasDataSpecification <|-- Submodel
        click HasDataSpecification href "../HasDataSpecification/"
      
      Submodel : administration
        
          
    
        
        
        Submodel --> "0..1" AdministrativeInformation : administration
        click AdministrativeInformation href "../AdministrativeInformation/"
    

        
      Submodel : category
        
      Submodel : checksum
        
      Submodel : description
        
      Submodel : displayName
        
      Submodel : embeddedDataSpecifications
        
          
    
        
        
        Submodel --> "*" EmbeddedDataSpecification : embeddedDataSpecifications
        click EmbeddedDataSpecification href "../EmbeddedDataSpecification/"
    

        
      Submodel : extensions
        
          
    
        
        
        Submodel --> "*" Extension : extensions
        click Extension href "../Extension/"
    

        
      Submodel : id
        
      Submodel : idShort
        
      Submodel : kind
        
          
    
        
        
        Submodel --> "0..1" ModelingKind : kind
        click ModelingKind href "../ModelingKind/"
    

        
      Submodel : qualifiers
        
          
    
        
        
        Submodel --> "*" Qualifier : qualifiers
        click Qualifier href "../Qualifier/"
    

        
      Submodel : semanticId
        
          
    
        
        
        Submodel --> "0..1" Reference : semanticId
        click Reference href "../Reference/"
    

        
      Submodel : submodelElements
        
          
    
        
        
        Submodel --> "*" SubmodelElement : submodelElements
        click SubmodelElement href "../SubmodelElement/"
    

        
      Submodel : supplementalSemanticIds
        
          
    
        
        
        Submodel --> "*" Reference : supplementalSemanticIds
        click Reference href "../Reference/"
    

        
      
```





## Inheritance
* **Submodel** [ [Identifiable](Identifiable.md) [HasKind](HasKind.md) [HasSemantics](HasSemantics.md) [Qualifiable](Qualifiable.md) [HasDataSpecification](HasDataSpecification.md)]



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [submodelElements](submodelElements.md) | * <br/> [SubmodelElement](SubmodelElement.md) | A submodel consists of zero or more submodel elements | direct |
| [administration](administration.md) | 0..1 <br/> [AdministrativeInformation](AdministrativeInformation.md) | Administrative information of an identifiable element | [Identifiable](Identifiable.md) |
| [id](id.md) | 1 <br/> [String](String.md) | The globally unique identification of the element | [Identifiable](Identifiable.md) |
| [kind](kind.md) | 0..1 <br/> [ModelingKind](ModelingKind.md) | Kind of the element: either type or instance | [HasKind](HasKind.md) |
| [semanticId](semanticId.md) | 0..1 <br/> [Reference](Reference.md) | Identifier of the semantic definition of the element | [HasSemantics](HasSemantics.md) |
| [supplementalSemanticIds](supplementalSemanticIds.md) | * <br/> [Reference](Reference.md) | Identifier of a supplemental semantic definition of the element | [HasSemantics](HasSemantics.md) |
| [qualifiers](qualifiers.md) | * <br/> [Qualifier](Qualifier.md) | Additional qualification of a qualifiable element | [Qualifiable](Qualifiable.md) |
| [embeddedDataSpecifications](embeddedDataSpecifications.md) | * <br/> [EmbeddedDataSpecification](EmbeddedDataSpecification.md) | Embedded data specification | [HasDataSpecification](HasDataSpecification.md) |
| [category](category.md) | 0..1 <br/> [String](String.md) | The category is a value that gives further meta information w | [Referable](Referable.md) |
| [checksum](checksum.md) | 0..1 <br/> [String](String.md) | Checksum to be used to determine if an Referable (including its aggregated ch... | [Referable](Referable.md) |
| [description](description.md) | * <br/> [LangString](LangString.md) | Description or comments on the element | [Referable](Referable.md) |
| [displayName](displayName.md) | * <br/> [LangString](LangString.md) | Display name | [Referable](Referable.md) |
| [idShort](idShort.md) | 0..1 <br/> [String](String.md) | In case of identifiables this attribute is a short name of the element | [Referable](Referable.md) |
| [extensions](extensions.md) | * <br/> [Extension](Extension.md) | An extension of the element | [HasExtensions](HasExtensions.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [Environment](Environment.md) | [submodels](submodels.md) | range | [Submodel](Submodel.md) |







## Identifier and Mapping Information






### Schema Source


* from schema: https://admin-shell.io/aas/3/0/RC02




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | aas:Submodel |
| native | aas:Submodel |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: Submodel
description: A submodel defines a specific aspect of the asset represented by the
  AAS.
from_schema: https://admin-shell.io/aas/3/0/RC02
mixins:
- Identifiable
- HasKind
- HasSemantics
- Qualifiable
- HasDataSpecification
attributes:
  submodelElements:
    name: submodelElements
    description: A submodel consists of zero or more submodel elements.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - Submodel
    range: SubmodelElement
    multivalued: true

```
</details>

### Induced

<details>
```yaml
name: Submodel
description: A submodel defines a specific aspect of the asset represented by the
  AAS.
from_schema: https://admin-shell.io/aas/3/0/RC02
mixins:
- Identifiable
- HasKind
- HasSemantics
- Qualifiable
- HasDataSpecification
attributes:
  submodelElements:
    name: submodelElements
    description: A submodel consists of zero or more submodel elements.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: submodelElements
    owner: Submodel
    domain_of:
    - Submodel
    range: SubmodelElement
    multivalued: true
  administration:
    name: administration
    description: Administrative information of an identifiable element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: administration
    owner: Submodel
    domain_of:
    - Identifiable
    range: AdministrativeInformation
  id:
    name: id
    description: The globally unique identification of the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: id
    owner: Submodel
    domain_of:
    - Identifiable
    range: string
    required: true
  kind:
    name: kind
    description: 'Kind of the element: either type or instance.'
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: kind
    owner: Submodel
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
    owner: Submodel
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
    owner: Submodel
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
    owner: Submodel
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
    owner: Submodel
    domain_of:
    - HasDataSpecification
    range: EmbeddedDataSpecification
    multivalued: true
  category:
    name: category
    description: The category is a value that gives further meta information w.r.t.
      to the class of the element. It affects the expected existence of attributes
      and the applicability of constraints.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: category
    owner: Submodel
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
    owner: Submodel
    domain_of:
    - Referable
    range: string
  description:
    name: description
    description: Description or comments on the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: description
    owner: Submodel
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
    owner: Submodel
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
    owner: Submodel
    domain_of:
    - Referable
    range: string
    pattern: ^[a-zA-Z][a-zA-Z0-9_]+$
  extensions:
    name: extensions
    description: An extension of the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: extensions
    owner: Submodel
    domain_of:
    - HasExtensions
    range: Extension
    multivalued: true

```
</details>