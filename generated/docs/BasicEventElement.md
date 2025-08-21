

# Class: BasicEventElement 


_A basic event element._





URI: [aas:BasicEventElement](https://admin-shell.io/aas/3/0/RC02/BasicEventElement)





```mermaid
 classDiagram
    class BasicEventElement
    click BasicEventElement href "../BasicEventElement/"
      EventElement <|-- BasicEventElement
        click EventElement href "../EventElement/"
      
      BasicEventElement : category
        
      BasicEventElement : checksum
        
      BasicEventElement : description
        
      BasicEventElement : direction
        
          
    
        
        
        BasicEventElement --> "1" Direction : direction
        click Direction href "../Direction/"
    

        
      BasicEventElement : displayName
        
      BasicEventElement : embeddedDataSpecifications
        
          
    
        
        
        BasicEventElement --> "*" EmbeddedDataSpecification : embeddedDataSpecifications
        click EmbeddedDataSpecification href "../EmbeddedDataSpecification/"
    

        
      BasicEventElement : extensions
        
          
    
        
        
        BasicEventElement --> "*" Extension : extensions
        click Extension href "../Extension/"
    

        
      BasicEventElement : idShort
        
      BasicEventElement : kind
        
          
    
        
        
        BasicEventElement --> "0..1" ModelingKind : kind
        click ModelingKind href "../ModelingKind/"
    

        
      BasicEventElement : lastUpdate
        
      BasicEventElement : maxInterval
        
      BasicEventElement : messageBroker
        
          
    
        
        
        BasicEventElement --> "0..1" Reference : messageBroker
        click Reference href "../Reference/"
    

        
      BasicEventElement : messageTopic
        
      BasicEventElement : minInterval
        
      BasicEventElement : observed
        
          
    
        
        
        BasicEventElement --> "1" Reference : observed
        click Reference href "../Reference/"
    

        
      BasicEventElement : qualifiers
        
          
    
        
        
        BasicEventElement --> "*" Qualifier : qualifiers
        click Qualifier href "../Qualifier/"
    

        
      BasicEventElement : semanticId
        
          
    
        
        
        BasicEventElement --> "0..1" Reference : semanticId
        click Reference href "../Reference/"
    

        
      BasicEventElement : state
        
          
    
        
        
        BasicEventElement --> "1" StateOfEvent : state
        click StateOfEvent href "../StateOfEvent/"
    

        
      BasicEventElement : supplementalSemanticIds
        
          
    
        
        
        BasicEventElement --> "*" Reference : supplementalSemanticIds
        click Reference href "../Reference/"
    

        
      
```





## Inheritance
* [SubmodelElement](SubmodelElement.md) [ [Referable](Referable.md) [HasKind](HasKind.md) [HasSemantics](HasSemantics.md) [Qualifiable](Qualifiable.md) [HasDataSpecification](HasDataSpecification.md)]
    * [EventElement](EventElement.md)
        * **BasicEventElement**



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [direction](direction.md) | 1 <br/> [Direction](Direction.md) | Direction of event | direct |
| [lastUpdate](lastUpdate.md) | 0..1 <br/> [String](String.md) | Timestamp in UTC, when the last event was received (input direction) or sent ... | direct |
| [maxInterval](maxInterval.md) | 0..1 <br/> [String](String.md) | For input direction: not applicable | direct |
| [messageBroker](messageBroker.md) | 0..1 <br/> [Reference](Reference.md) | Information, which outer message infrastructure shall handle messages for the... | direct |
| [messageTopic](messageTopic.md) | 0..1 <br/> [String](String.md) | Information for the outer message infrastructure for scheduling the event to ... | direct |
| [minInterval](minInterval.md) | 0..1 <br/> [String](String.md) | For input direction, reports on the maximum frequency, the software entity be... | direct |
| [observed](observed.md) | 1 <br/> [Reference](Reference.md) | Reference to the 'Referable', which defines the scope of the event | direct |
| [state](state.md) | 1 <br/> [StateOfEvent](StateOfEvent.md) | State of event | direct |
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
| self | aas:BasicEventElement |
| native | aas:BasicEventElement |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: BasicEventElement
description: A basic event element.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: EventElement
attributes:
  direction:
    name: direction
    description: Direction of event.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - BasicEventElement
    range: Direction
    required: true
  lastUpdate:
    name: lastUpdate
    description: Timestamp in UTC, when the last event was received (input direction)
      or sent (output direction).
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - BasicEventElement
    range: string
    pattern: ^-?(([1-9][0-9][0-9][0-9]+)|(0[0-9][0-9][0-9]))-((0[1-9])|(1[0-2]))-((0[1-9])|([12][0-9])|(3[01]))T(((([01][0-9])|(2[0-3])):[0-5][0-9]:([0-5][0-9])(\.[0-9]+)?)|24:00:00(\.0+)?)Z$
  maxInterval:
    name: maxInterval
    description: 'For input direction: not applicable.'
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - BasicEventElement
    range: string
    pattern: ^-?(([1-9][0-9][0-9][0-9]+)|(0[0-9][0-9][0-9]))-((0[1-9])|(1[0-2]))-((0[1-9])|([12][0-9])|(3[01]))T(((([01][0-9])|(2[0-3])):[0-5][0-9]:([0-5][0-9])(\.[0-9]+)?)|24:00:00(\.0+)?)Z$
  messageBroker:
    name: messageBroker
    description: Information, which outer message infrastructure shall handle messages
      for the 'EventElement'. Refers to a 'Submodel', 'SubmodelElementList', 'SubmodelElementCollection'
      or 'Entity', which contains 'DataElement''s describing the proprietary specification
      for the message broker.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - BasicEventElement
    range: Reference
  messageTopic:
    name: messageTopic
    description: Information for the outer message infrastructure for scheduling the
      event to the respective communication channel.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - BasicEventElement
    range: string
  minInterval:
    name: minInterval
    description: For input direction, reports on the maximum frequency, the software
      entity behind the respective Referable can handle input events.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - BasicEventElement
    range: string
    pattern: ^-?(([1-9][0-9][0-9][0-9]+)|(0[0-9][0-9][0-9]))-((0[1-9])|(1[0-2]))-((0[1-9])|([12][0-9])|(3[01]))T(((([01][0-9])|(2[0-3])):[0-5][0-9]:([0-5][0-9])(\.[0-9]+)?)|24:00:00(\.0+)?)Z$
  observed:
    name: observed
    description: Reference to the 'Referable', which defines the scope of the event.
      Can be 'AssetAdministrationShell', 'Submodel', or 'SubmodelElement'.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - BasicEventElement
    range: Reference
    required: true
  state:
    name: state
    description: State of event.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    domain_of:
    - BasicEventElement
    range: StateOfEvent
    required: true

```
</details>

### Induced

<details>
```yaml
name: BasicEventElement
description: A basic event element.
from_schema: https://admin-shell.io/aas/3/0/RC02
is_a: EventElement
attributes:
  direction:
    name: direction
    description: Direction of event.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: direction
    owner: BasicEventElement
    domain_of:
    - BasicEventElement
    range: Direction
    required: true
  lastUpdate:
    name: lastUpdate
    description: Timestamp in UTC, when the last event was received (input direction)
      or sent (output direction).
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: lastUpdate
    owner: BasicEventElement
    domain_of:
    - BasicEventElement
    range: string
    pattern: ^-?(([1-9][0-9][0-9][0-9]+)|(0[0-9][0-9][0-9]))-((0[1-9])|(1[0-2]))-((0[1-9])|([12][0-9])|(3[01]))T(((([01][0-9])|(2[0-3])):[0-5][0-9]:([0-5][0-9])(\.[0-9]+)?)|24:00:00(\.0+)?)Z$
  maxInterval:
    name: maxInterval
    description: 'For input direction: not applicable.'
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: maxInterval
    owner: BasicEventElement
    domain_of:
    - BasicEventElement
    range: string
    pattern: ^-?(([1-9][0-9][0-9][0-9]+)|(0[0-9][0-9][0-9]))-((0[1-9])|(1[0-2]))-((0[1-9])|([12][0-9])|(3[01]))T(((([01][0-9])|(2[0-3])):[0-5][0-9]:([0-5][0-9])(\.[0-9]+)?)|24:00:00(\.0+)?)Z$
  messageBroker:
    name: messageBroker
    description: Information, which outer message infrastructure shall handle messages
      for the 'EventElement'. Refers to a 'Submodel', 'SubmodelElementList', 'SubmodelElementCollection'
      or 'Entity', which contains 'DataElement''s describing the proprietary specification
      for the message broker.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: messageBroker
    owner: BasicEventElement
    domain_of:
    - BasicEventElement
    range: Reference
  messageTopic:
    name: messageTopic
    description: Information for the outer message infrastructure for scheduling the
      event to the respective communication channel.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: messageTopic
    owner: BasicEventElement
    domain_of:
    - BasicEventElement
    range: string
  minInterval:
    name: minInterval
    description: For input direction, reports on the maximum frequency, the software
      entity behind the respective Referable can handle input events.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: minInterval
    owner: BasicEventElement
    domain_of:
    - BasicEventElement
    range: string
    pattern: ^-?(([1-9][0-9][0-9][0-9]+)|(0[0-9][0-9][0-9]))-((0[1-9])|(1[0-2]))-((0[1-9])|([12][0-9])|(3[01]))T(((([01][0-9])|(2[0-3])):[0-5][0-9]:([0-5][0-9])(\.[0-9]+)?)|24:00:00(\.0+)?)Z$
  observed:
    name: observed
    description: Reference to the 'Referable', which defines the scope of the event.
      Can be 'AssetAdministrationShell', 'Submodel', or 'SubmodelElement'.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: observed
    owner: BasicEventElement
    domain_of:
    - BasicEventElement
    range: Reference
    required: true
  state:
    name: state
    description: State of event.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: state
    owner: BasicEventElement
    domain_of:
    - BasicEventElement
    range: StateOfEvent
    required: true
  category:
    name: category
    description: The category is a value that gives further meta information w.r.t.
      to the class of the element. It affects the expected existence of attributes
      and the applicability of constraints.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: category
    owner: BasicEventElement
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
    owner: BasicEventElement
    domain_of:
    - Referable
    range: string
  description:
    name: description
    description: Description or comments on the element.
    from_schema: https://admin-shell.io/aas/3/0/RC02
    rank: 1000
    alias: description
    owner: BasicEventElement
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
    owner: BasicEventElement
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
    owner: BasicEventElement
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
    owner: BasicEventElement
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
    owner: BasicEventElement
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
    owner: BasicEventElement
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
    owner: BasicEventElement
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
    owner: BasicEventElement
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
    owner: BasicEventElement
    domain_of:
    - HasExtensions
    range: Extension
    multivalued: true

```
</details>