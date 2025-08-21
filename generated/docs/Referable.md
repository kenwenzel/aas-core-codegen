

# Class: Referable 


_An element that is referable by its 'idShort'._




* __NOTE__: this is an abstract class and should not be instantiated directly


URI: [aas:Referable](https://admin-shell.io/aas/3/0/RC02/Referable)





```mermaid
 classDiagram
    class Referable
    click Referable href "../Referable/"
      HasExtensions <|-- Referable
        click HasExtensions href "../HasExtensions/"
      

      Referable <|-- Identifiable
        click Identifiable href "../Identifiable/"
      Referable <|-- SubmodelElement
        click SubmodelElement href "../SubmodelElement/"
      

      Referable : category
        
      Referable : checksum
        
      Referable : description
        
      Referable : displayName
        
      Referable : extensions
        
          
    
        
        
        Referable --> "*" Extension : extensions
        click Extension href "../Extension/"
    

        
      Referable : idShort
        
      
```





## Inheritance
* [HasExtensions](HasExtensions.md)
    * **Referable**
        * [Identifiable](Identifiable.md)



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [category](category.md) | 0..1 <br/> [String](String.md) | The category is a value that gives further meta information w | direct |
| [checksum](checksum.md) | 0..1 <br/> [String](String.md) | Checksum to be used to determine if an Referable (including its aggregated ch... | direct |
| [description](description.md) | * <br/> [LangString](LangString.md) | Description or comments on the element | direct |
| [displayName](displayName.md) | * <br/> [LangString](LangString.md) | Display name | direct |
| [idShort](idShort.md) | 0..1 <br/> [String](String.md) | In case of identifiables this attribute is a short name of the element | direct |
| [extensions](extensions.md) | * <br/> [Extension](Extension.md) | An extension of the element | [HasExtensions](HasExtensions.md) |










## Identifier and Mapping Information






### Schema Source


* from schema: https://admin-shell.io/aas/3/0/RC02




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | aas:Referable |
| native | aas:Referable |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: Referable
description: An element that is referable by its 'idShort'.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: HasExtensions
abstract: true
attributes:
  category:
    name: category
    description: The category is a value that gives further meta information w.r.t.
      to the class of the element. It affects the expected existence of attributes
      and the applicability of constraints.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - Referable
    range: string
  checksum:
    name: checksum
    description: Checksum to be used to determine if an Referable (including its aggregated
      child elements) has changed.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - Referable
    range: string
  description:
    name: description
    description: Description or comments on the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - Referable
    range: LangString
    multivalued: true
  displayName:
    name: displayName
    description: Display name. Can be provided in several languages.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
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
    domain_of:
    - Referable
    range: string
    pattern: ^[a-zA-Z][a-zA-Z0-9_]+$

```
</details>

### Induced

<details>
```yaml
name: Referable
description: An element that is referable by its 'idShort'.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: HasExtensions
abstract: true
attributes:
  category:
    name: category
    description: The category is a value that gives further meta information w.r.t.
      to the class of the element. It affects the expected existence of attributes
      and the applicability of constraints.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: category
    owner: Referable
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
    owner: Referable
    domain_of:
    - Referable
    range: string
  description:
    name: description
    description: Description or comments on the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: description
    owner: Referable
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
    owner: Referable
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
    owner: Referable
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
    owner: Referable
    domain_of:
    - HasExtensions
    range: Extension
    multivalued: true

```
</details>