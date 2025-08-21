

# Slot: minInterval 


_For input direction, reports on the maximum frequency, the software entity behind the respective Referable can handle input events._





URI: [aas:minInterval](https://admin-shell.io/aas/3/0/RC02/minInterval)
Alias: minInterval

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [BasicEventElement](BasicEventElement.md) | A basic event element |  no  |






## Properties

* Range: [String](String.md)

* Regex pattern: `^-?(([1-9][0-9][0-9][0-9]+)|(0[0-9][0-9][0-9]))-((0[1-9])|(1[0-2]))-((0[1-9])|([12][0-9])|(3[01]))T(((([01][0-9])|(2[0-3])):[0-5][0-9]:([0-5][0-9])(\.[0-9]+)?)|24:00:00(\.0+)?)Z$`




## Identifier and Mapping Information






### Schema Source


* from schema: https://admin-shell.io/aas/3/0/RC02




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | aas:minInterval |
| native | aas:minInterval |




## LinkML Source

<details>
```yaml
name: minInterval
description: For input direction, reports on the maximum frequency, the software entity
  behind the respective Referable can handle input events.
from_schema: https://admin-shell.io/aas/3/0/RC02
rank: 1000
alias: minInterval
owner: BasicEventElement
domain_of:
- BasicEventElement
range: string
pattern: ^-?(([1-9][0-9][0-9][0-9]+)|(0[0-9][0-9][0-9]))-((0[1-9])|(1[0-2]))-((0[1-9])|([12][0-9])|(3[01]))T(((([01][0-9])|(2[0-3])):[0-5][0-9]:([0-5][0-9])(\.[0-9]+)?)|24:00:00(\.0+)?)Z$

```
</details>