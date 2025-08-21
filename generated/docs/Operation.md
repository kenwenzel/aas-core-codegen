

# Class: Operation 


_An operation is a submodel element with input and output variables._





URI: [aas:Operation](https://admin-shell.io/aas/3/0/RC02/Operation)





```mermaid
 classDiagram
    class Operation
    click Operation href "../Operation/"
      SubmodelElement <|-- Operation
        click SubmodelElement href "../SubmodelElement/"
      
      Operation : category
        
      Operation : checksum
        
      Operation : description
        
      Operation : displayName
        
      Operation : embeddedDataSpecifications
        
          
    
        
        
        Operation --> "*" EmbeddedDataSpecification : embeddedDataSpecifications
        click EmbeddedDataSpecification href "../EmbeddedDataSpecification/"
    

        
      Operation : extensions
        
          
    
        
        
        Operation --> "*" Extension : extensions
        click Extension href "../Extension/"
    

        
      Operation : idShort
        
      Operation : inoutputVariables
        
          
    
        
        
        Operation --> "*" OperationVariable : inoutputVariables
        click OperationVariable href "../OperationVariable/"
    

        
      Operation : inputVariables
        
          
    
        
        
        Operation --> "*" OperationVariable : inputVariables
        click OperationVariable href "../OperationVariable/"
    

        
      Operation : kind
        
          
    
        
        
        Operation --> "0..1" ModelingKind : kind
        click ModelingKind href "../ModelingKind/"
    

        
      Operation : outputVariables
        
          
    
        
        
        Operation --> "*" OperationVariable : outputVariables
        click OperationVariable href "../OperationVariable/"
    

        
      Operation : qualifiers
        
          
    
        
        
        Operation --> "*" Qualifier : qualifiers
        click Qualifier href "../Qualifier/"
    

        
      Operation : semanticId
        
          
    
        
        
        Operation --> "0..1" Reference : semanticId
        click Reference href "../Reference/"
    

        
      Operation : supplementalSemanticIds
        
          
    
        
        
        Operation --> "*" Reference : supplementalSemanticIds
        click Reference href "../Reference/"
    

        
      
```





## Inheritance
* [SubmodelElement](SubmodelElement.md) [ [Referable](Referable.md) [HasKind](HasKind.md) [HasSemantics](HasSemantics.md) [Qualifiable](Qualifiable.md) [HasDataSpecification](HasDataSpecification.md)]
    * **Operation**



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [inoutputVariables](inoutputVariables.md) | * <br/> [OperationVariable](OperationVariable.md) | Parameter that is input and output of the operation | direct |
| [inputVariables](inputVariables.md) | * <br/> [OperationVariable](OperationVariable.md) | Input parameter of the operation | direct |
| [outputVariables](outputVariables.md) | * <br/> [OperationVariable](OperationVariable.md) | Output parameter of the operation | direct |
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
| self | aas:Operation |
| native | aas:Operation |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: Operation
description: An operation is a submodel element with input and output variables.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: SubmodelElement
attributes:
  inoutputVariables:
    name: inoutputVariables
    description: Parameter that is input and output of the operation.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - Operation
    range: OperationVariable
    multivalued: true
  inputVariables:
    name: inputVariables
    description: Input parameter of the operation.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - Operation
    range: OperationVariable
    multivalued: true
  outputVariables:
    name: outputVariables
    description: Output parameter of the operation.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - Operation
    range: OperationVariable
    multivalued: true

```
</details>

### Induced

<details>
```yaml
name: Operation
description: An operation is a submodel element with input and output variables.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: SubmodelElement
attributes:
  inoutputVariables:
    name: inoutputVariables
    description: Parameter that is input and output of the operation.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: inoutputVariables
    owner: Operation
    domain_of:
    - Operation
    range: OperationVariable
    multivalued: true
  inputVariables:
    name: inputVariables
    description: Input parameter of the operation.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: inputVariables
    owner: Operation
    domain_of:
    - Operation
    range: OperationVariable
    multivalued: true
  outputVariables:
    name: outputVariables
    description: Output parameter of the operation.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: outputVariables
    owner: Operation
    domain_of:
    - Operation
    range: OperationVariable
    multivalued: true
  category:
    name: category
    description: The category is a value that gives further meta information w.r.t.
      to the class of the element. It affects the expected existence of attributes
      and the applicability of constraints.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: category
    owner: Operation
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
    owner: Operation
    domain_of:
    - Referable
    range: string
  description:
    name: description
    description: Description or comments on the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: description
    owner: Operation
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
    owner: Operation
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
    owner: Operation
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
    owner: Operation
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
    owner: Operation
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
    owner: Operation
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
    owner: Operation
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
    owner: Operation
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
    owner: Operation
    domain_of:
    - HasExtensions
    range: Extension
    multivalued: true

```
</details>