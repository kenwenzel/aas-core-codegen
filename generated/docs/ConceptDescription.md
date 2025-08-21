

# Class: ConceptDescription 


_The semantics of a property or other elements that may have a semantic description is defined by a concept description._





URI: [aas:ConceptDescription](https://admin-shell.io/aas/3/0/RC02/ConceptDescription)





```mermaid
 classDiagram
    class ConceptDescription
    click ConceptDescription href "../ConceptDescription/"
      Identifiable <|-- ConceptDescription
        click Identifiable href "../Identifiable/"
      HasDataSpecification <|-- ConceptDescription
        click HasDataSpecification href "../HasDataSpecification/"
      
      ConceptDescription : administration
        
          
    
        
        
        ConceptDescription --> "0..1" AdministrativeInformation : administration
        click AdministrativeInformation href "../AdministrativeInformation/"
    

        
      ConceptDescription : category
        
      ConceptDescription : checksum
        
      ConceptDescription : description
        
      ConceptDescription : displayName
        
      ConceptDescription : embeddedDataSpecifications
        
          
    
        
        
        ConceptDescription --> "*" EmbeddedDataSpecification : embeddedDataSpecifications
        click EmbeddedDataSpecification href "../EmbeddedDataSpecification/"
    

        
      ConceptDescription : extensions
        
          
    
        
        
        ConceptDescription --> "*" Extension : extensions
        click Extension href "../Extension/"
    

        
      ConceptDescription : id
        
      ConceptDescription : idShort
        
      ConceptDescription : isCaseOf
        
          
    
        
        
        ConceptDescription --> "*" Reference : isCaseOf
        click Reference href "../Reference/"
    

        
      
```





## Inheritance
* **ConceptDescription** [ [Identifiable](Identifiable.md) [HasDataSpecification](HasDataSpecification.md)]



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [isCaseOf](isCaseOf.md) | * <br/> [Reference](Reference.md) | Reference to an external definition the concept is compatible to or was deriv... | direct |
| [administration](administration.md) | 0..1 <br/> [AdministrativeInformation](AdministrativeInformation.md) | Administrative information of an identifiable element | [Identifiable](Identifiable.md) |
| [id](id.md) | 1 <br/> [String](String.md) | The globally unique identification of the element | [Identifiable](Identifiable.md) |
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
| [Environment](Environment.md) | [conceptDescriptions](conceptDescriptions.md) | range | [ConceptDescription](ConceptDescription.md) |







## Identifier and Mapping Information






### Schema Source


* from schema: https://admin-shell.io/aas/3/0/RC02




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | aas:ConceptDescription |
| native | aas:ConceptDescription |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: ConceptDescription
description: The semantics of a property or other elements that may have a semantic
  description is defined by a concept description.
from_schema: https://admin-shell.io/aas/3/0/RC02
mixins:
- Identifiable
- HasDataSpecification
attributes:
  isCaseOf:
    name: isCaseOf
    description: Reference to an external definition the concept is compatible to
      or was derived from.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - ConceptDescription
    range: Reference
    multivalued: true

```
</details>

### Induced

<details>
```yaml
name: ConceptDescription
description: The semantics of a property or other elements that may have a semantic
  description is defined by a concept description.
from_schema: https://admin-shell.io/aas/3/0/RC02
mixins:
- Identifiable
- HasDataSpecification
attributes:
  isCaseOf:
    name: isCaseOf
    description: Reference to an external definition the concept is compatible to
      or was derived from.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: isCaseOf
    owner: ConceptDescription
    domain_of:
    - ConceptDescription
    range: Reference
    multivalued: true
  administration:
    name: administration
    description: Administrative information of an identifiable element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: administration
    owner: ConceptDescription
    domain_of:
    - Identifiable
    range: AdministrativeInformation
  id:
    name: id
    description: The globally unique identification of the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: id
    owner: ConceptDescription
    domain_of:
    - Identifiable
    range: string
    required: true
  embeddedDataSpecifications:
    name: embeddedDataSpecifications
    description: Embedded data specification.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: embeddedDataSpecifications
    owner: ConceptDescription
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
    owner: ConceptDescription
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
    owner: ConceptDescription
    domain_of:
    - Referable
    range: string
  description:
    name: description
    description: Description or comments on the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: description
    owner: ConceptDescription
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
    owner: ConceptDescription
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
    owner: ConceptDescription
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
    owner: ConceptDescription
    domain_of:
    - HasExtensions
    range: Extension
    multivalued: true

```
</details>