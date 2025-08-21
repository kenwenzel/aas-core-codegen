# aas



URI: https://admin-shell.io/aas/3/0/RC02

Name: aas



## Classes

| Class | Description |
| --- | --- |
| [AssetAdministrationShell](AssetAdministrationShell.md) | An asset administration shell |
| [AssetInformation](AssetInformation.md) | In 'AssetInformation' identifying meta data of the asset that is represented ... |
| [ConceptDescription](ConceptDescription.md) | The semantics of a property or other elements that may have a semantic descri... |
| [DataSpecificationContent](DataSpecificationContent.md) | Data specification content is part of a data specification template and defin... |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[DataSpecificationIec61360](DataSpecificationIec61360.md) | Content of data specification template for concept descriptions for propertie... |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[DataSpecificationPhysicalUnit](DataSpecificationPhysicalUnit.md) |  |
| [EmbeddedDataSpecification](EmbeddedDataSpecification.md) | Embed the content of a data specification |
| [Environment](Environment.md) | Container for the sets of different identifiables |
| [EventPayload](EventPayload.md) | Defines the necessary information of an event instance sent out or received |
| [HasDataSpecification](HasDataSpecification.md) | Element that can be extended by using data specification templates |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[AdministrativeInformation](AdministrativeInformation.md) | Administrative meta-information for an element like version information |
| [HasExtensions](HasExtensions.md) | Element that can be extended by proprietary extensions |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Referable](Referable.md) | An element that is referable by its 'idShort' |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Identifiable](Identifiable.md) | An element that has a globally unique identifier |
| [HasKind](HasKind.md) | An element with a kind is an element that can either represent a template or ... |
| [HasSemantics](HasSemantics.md) | Element that can have a semantic definition plus some supplemental semantic d... |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Extension](Extension.md) | Single extension of an element |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Qualifier](Qualifier.md) | A qualifier is a type-value-pair that makes additional statements w |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[SpecificAssetId](SpecificAssetId.md) | A specific asset ID describes a generic supplementary identifying attribute o... |
| [Key](Key.md) | A key is a reference to an element by its ID |
| [OperationVariable](OperationVariable.md) | The value of an operation variable is a submodel element that is used as inpu... |
| [Qualifiable](Qualifiable.md) | The value of a qualifiable element may be further qualified by one or more qu... |
| [Reference](Reference.md) | Reference to either a model element of the same or another AAS or to an exter... |
| [Resource](Resource.md) | Resource represents an address to a file (a locator) |
| [Submodel](Submodel.md) | A submodel defines a specific aspect of the asset represented by the AAS |
| [SubmodelElement](SubmodelElement.md) | A submodel element is an element suitable for the description and differentia... |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Capability](Capability.md) | A capability is the implementation-independent description of the potential o... |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[DataElement](DataElement.md) | A data element is a submodel element that is not further composed out of othe... |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Blob](Blob.md) | A 'Blob' is a data element that represents a file that is contained with its ... |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[File](File.md) | A File is a data element that represents an address to a file (a locator) |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[MultiLanguageProperty](MultiLanguageProperty.md) | A property is a data element that has a multi-language value |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Property](Property.md) | A property is a data element that has a single value |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Range](Range.md) | A range data element is a data element that defines a range with min and max |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[ReferenceElement](ReferenceElement.md) | A reference element is a data element that defines a logical reference to ano... |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Entity](Entity.md) | An entity is a submodel element that is used to model entities |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[EventElement](EventElement.md) | An event element |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[BasicEventElement](BasicEventElement.md) | A basic event element |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Operation](Operation.md) | An operation is a submodel element with input and output variables |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[RelationshipElement](RelationshipElement.md) | A relationship element is used to define a relationship between two elements ... |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[AnnotatedRelationshipElement](AnnotatedRelationshipElement.md) | An annotated relationship element is a relationship element that can be annot... |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[SubmodelElementCollection](SubmodelElementCollection.md) | A submodel element collection is a kind of struct, i |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[SubmodelElementList](SubmodelElementList.md) | A submodel element list is an ordered list of submodel elements |
| [ValueList](ValueList.md) | A set of value reference pairs |
| [ValueReferencePair](ValueReferencePair.md) | A value reference pair within a value list |



## Slots

| Slot | Description |
| --- | --- |
| [administration](administration.md) | Administrative information of an identifiable element |
| [annotations](annotations.md) | A data element that represents an annotation that holds for the relationship ... |
| [assetAdministrationShells](assetAdministrationShells.md) | Asset administration shell |
| [assetInformation](assetInformation.md) | Meta-information about the asset the AAS is representing |
| [assetKind](assetKind.md) | Denotes whether the Asset is of kind 'Type' or 'Instance' |
| [category](category.md) | The category is a value that gives further meta information w |
| [checksum](checksum.md) | Checksum to be used to determine if an Referable (including its aggregated ch... |
| [conceptDescriptions](conceptDescriptions.md) | Concept description |
| [contentType](contentType.md) | Content type of the content of the 'Blob' |
| [conversionFactor](conversionFactor.md) | Conversion factor |
| [dataSpecification](dataSpecification.md) | Reference to the data specification |
| [dataSpecificationContent](dataSpecificationContent.md) | Actual content of the data specification |
| [dataType](dataType.md) | Data Type |
| [defaultThumbnail](defaultThumbnail.md) | Thumbnail of the asset represented by the Asset Administration Shell |
| [definition](definition.md) | Definition in different languages |
| [derivedFrom](derivedFrom.md) | The reference to the AAS the AAS was derived from |
| [description](description.md) | Description or comments on the element |
| [dinNotation](dinNotation.md) | Notation of physical unit conformant to DIN |
| [direction](direction.md) | Direction of event |
| [displayName](displayName.md) | Display name |
| [eceCode](eceCode.md) | Code of physical unit conformant to ECE |
| [eceName](eceName.md) | Name of physical unit conformant to ECE |
| [embeddedDataSpecifications](embeddedDataSpecifications.md) | Embedded data specification |
| [entityType](entityType.md) | Describes whether the entity is a co-managed entity or a self-managed entity |
| [extensions](extensions.md) | An extension of the element |
| [externalSubjectId](externalSubjectId.md) | The (external) subject the key belongs to or has meaning to |
| [first](first.md) | Reference to the first element in the relationship taking the role of the sub... |
| [globalAssetId](globalAssetId.md) | Global identifier of the asset the AAS is representing |
| [id](id.md) | The globally unique identification of the element |
| [idShort](idShort.md) | In case of identifiables this attribute is a short name of the element |
| [inoutputVariables](inoutputVariables.md) | Parameter that is input and output of the operation |
| [inputVariables](inputVariables.md) | Input parameter of the operation |
| [isCaseOf](isCaseOf.md) | Reference to an external definition the concept is compatible to or was deriv... |
| [keys](keys.md) | Unique references in their name space |
| [kind](kind.md) | Kind of the element: either type or instance |
| [lastUpdate](lastUpdate.md) | Timestamp in UTC, when the last event was received (input direction) or sent ... |
| [levelType](levelType.md) | Set of levels |
| [max](max.md) | The maximum value of the range |
| [maxInterval](maxInterval.md) | For input direction: not applicable |
| [messageBroker](messageBroker.md) | Information, which outer message infrastructure shall handle messages for the... |
| [messageTopic](messageTopic.md) | Information for the outer message infrastructure for scheduling the event to ... |
| [min](min.md) | The minimum value of the range |
| [minInterval](minInterval.md) | For input direction, reports on the maximum frequency, the software entity be... |
| [name](name.md) | Name of the extension |
| [nistName](nistName.md) | Name of NIST physical unit |
| [observableReference](observableReference.md) | Reference to the referable, which defines the scope of the event |
| [observableSemanticId](observableSemanticId.md) | 'semanticId' of the referable which defines the scope of the event, if availa... |
| [observed](observed.md) | Reference to the 'Referable', which defines the scope of the event |
| [orderRelevant](orderRelevant.md) | Defines whether order in list is relevant |
| [outputVariables](outputVariables.md) | Output parameter of the operation |
| [path](path.md) | Path and name of the resource (with file extension) |
| [payload](payload.md) | Event specific payload |
| [preferredName](preferredName.md) | Preferred name |
| [qualifiers](qualifiers.md) | Additional qualification of a qualifiable element |
| [referredSemanticId](referredSemanticId.md) | 'semanticId' of the referenced model element ('type' = 'ModelReference') |
| [refersTo](refersTo.md) | Reference to an element the extension refers to |
| [registrationAuthorityId](registrationAuthorityId.md) | Registration authority ID |
| [revision](revision.md) | Revision of the element |
| [second](second.md) | Reference to the second element in the relationship taking the role of the ob... |
| [semanticId](semanticId.md) | Identifier of the semantic definition of the element |
| [semanticIdListElement](semanticIdListElement.md) | Semantic ID the submodel elements contained in the list match to |
| [shortName](shortName.md) | Short name |
| [siName](siName.md) | Name of SI physical unit |
| [siNotation](siNotation.md) | Notation of SI physical unit |
| [source](source.md) | Reference to the source event element, including identification of 'AssetAdmi... |
| [sourceOfDefinition](sourceOfDefinition.md) | Source of definition |
| [sourceSemanticId](sourceSemanticId.md) | 'semanticId' of the source event element, if available |
| [specificAssetId](specificAssetId.md) | Reference to a specific asset ID representing a supplementary identifier of t... |
| [specificAssetIds](specificAssetIds.md) | Additional domain-specific, typically proprietary identifier for the asset li... |
| [state](state.md) | State of event |
| [statements](statements.md) | Describes statements applicable to the entity by a set of submodel elements, ... |
| [subjectId](subjectId.md) | Subject, who/which initiated the creation |
| [submodelElements](submodelElements.md) | A submodel consists of zero or more submodel elements |
| [submodels](submodels.md) | References to submodels of the AAS |
| [supplementalSemanticIds](supplementalSemanticIds.md) | Identifier of a supplemental semantic definition of the element |
| [supplier](supplier.md) | Supplier |
| [symbol](symbol.md) | Symbol |
| [timeStamp](timeStamp.md) | Timestamp in UTC, when this event was triggered |
| [topic](topic.md) | Information for the outer message infrastructure for scheduling the event to ... |
| [type](type.md) | Denotes which kind of entity is referenced |
| [typeValueListElement](typeValueListElement.md) | The submodel element type of the submodel elements contained in the list |
| [unit](unit.md) | Unit |
| [unitId](unitId.md) | Unique unit id |
| [unitName](unitName.md) | Name of the physical unit |
| [unitSymbol](unitSymbol.md) | Symbol for the physical unit |
| [value](value.md) | The value of the 'Blob' instance of a blob data element |
| [valueFormat](valueFormat.md) | Value Format |
| [valueId](valueId.md) | Reference to the global unique ID of a coded value |
| [valueList](valueList.md) | List of allowed values |
| [valueReferencePairs](valueReferencePairs.md) | A pair of a value together with its global unique id |
| [valueType](valueType.md) | Type of the value of the extension |
| [valueTypeListElement](valueTypeListElement.md) | The value type of the submodel element contained in the list |
| [version](version.md) | Version of the element |


## Enumerations

| Enumeration | Description |
| --- | --- |
| [AasSubmodelElements](AasSubmodelElements.md) |  |
| [AssetKind](AssetKind.md) |  |
| [DataTypeDefXsd](DataTypeDefXsd.md) |  |
| [DataTypeIec61360](DataTypeIec61360.md) |  |
| [Direction](Direction.md) |  |
| [EntityType](EntityType.md) |  |
| [KeyTypes](KeyTypes.md) |  |
| [LevelType](LevelType.md) |  |
| [ModelingKind](ModelingKind.md) |  |
| [QualifierKind](QualifierKind.md) |  |
| [ReferenceTypes](ReferenceTypes.md) |  |
| [StateOfEvent](StateOfEvent.md) |  |


## Types

| Type | Description |
| --- | --- |
| [Base64Binary](Base64Binary.md) | Base64-encoded binary data |
| [Boolean](Boolean.md) | A binary (true or false) value |
| [Curie](Curie.md) | a compact URI |
| [Date](Date.md) | a date (year, month and day) in an idealized calendar |
| [DateOrDatetime](DateOrDatetime.md) | Either a date or a datetime |
| [Datetime](Datetime.md) | The combination of a date and time |
| [Decimal](Decimal.md) | A real number with arbitrary precision that conforms to the xsd:decimal speci... |
| [Double](Double.md) | A real number that conforms to the xsd:double specification |
| [Float](Float.md) | A real number that conforms to the xsd:float specification |
| [Integer](Integer.md) | An integer |
| [Jsonpath](Jsonpath.md) | A string encoding a JSON Path |
| [Jsonpointer](Jsonpointer.md) | A string encoding a JSON Pointer |
| [LangString](LangString.md) | String with a language tag |
| [Ncname](Ncname.md) | Prefix part of CURIE |
| [Nodeidentifier](Nodeidentifier.md) | A URI, CURIE or BNODE that represents a node in a model |
| [Objectidentifier](Objectidentifier.md) | A URI or CURIE that represents an object in the model |
| [Sparqlpath](Sparqlpath.md) | A string encoding a SPARQL Property Path |
| [String](String.md) | A character string |
| [Time](Time.md) | A time object represents a (local) time of day, independent of any particular... |
| [Uri](Uri.md) | a complete URI |
| [Uriorcurie](Uriorcurie.md) | a URI or a CURIE |


## Subsets

| Subset | Description |
| --- | --- |
