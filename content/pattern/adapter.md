---
title: "Adapter"
date: 2021-03-15T13:24:44+01:00
draft: false
pattern_types: ["GOF", "Structural"]
wikipedia: ""
diagramtype: "class"
---

The adapter aims to be a converter between two specific interfaces: one belonging to "our" side of the application, the other to the library or other tool we need to interact with. This is very important, because it enables us to delay decisions, as the choice of a spcific implementation of the adapter becomes less important due to the fact that we are at that point using the adapter itself as our communication contract.
## Usage
Often used in combo with other patterns, such as [Inversion of Control]({{< ref "/pattern/inversion_of_control" >}}) and several [Factories]({{< ref "/pattern_types/factory" >}})

## Examples
Typical example of this pattern in a "pure" form is the Driver. Whether it is for printing or for database access, the API exposed by the common development systems just require the connection to the adapter and, with some kind of [Factory]({{< ref "/pattern_types/factory" >}}) or repository we get the specific implementation of what we need at the moment, based on the configuration of the system we have.