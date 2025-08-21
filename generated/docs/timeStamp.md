

# Slot: timeStamp 


_Timestamp in UTC, when this event was triggered._





URI: [aas:timeStamp](https://admin-shell.io/aas/3/0/RC02/timeStamp)
Alias: timeStamp

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [EventPayload](EventPayload.md) | Defines the necessary information of an event instance sent out or received |  no  |






## Properties

* Range: [String](String.md)

* Required: True

* Regex pattern: `^-?(([1-9][0-9][0-9][0-9]+)|(0[0-9][0-9][0-9]))-((0[1-9])|(1[0-2]))-((0[1-9])|([12][0-9])|(3[01]))T(((([01][0-9])|(2[0-3])):[0-5][0-9]:([0-5][0-9])(\.[0-9]+)?)|24:00:00(\.0+)?)Z$`




## Identifier and Mapping Information






### Schema Source


* from schema: https://admin-shell.io/aas/3/0/RC02




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | aas:timeStamp |
| native | aas:timeStamp |




## LinkML Source

<details>
```yaml
name: timeStamp
description: Timestamp in UTC, when this event was triggered.
from_schema: https://admin-shell.io/aas/3/0/RC02
rank: 1000
alias: timeStamp
owner: EventPayload
domain_of:
- EventPayload
range: string
required: true
pattern: ^-?(([1-9][0-9][0-9][0-9]+)|(0[0-9][0-9][0-9]))-((0[1-9])|(1[0-2]))-((0[1-9])|([12][0-9])|(3[01]))T(((([01][0-9])|(2[0-3])):[0-5][0-9]:([0-5][0-9])(\.[0-9]+)?)|24:00:00(\.0+)?)Z$

```
</details>